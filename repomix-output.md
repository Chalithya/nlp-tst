This file is a merged representation of the entire codebase, combined into a single document by Repomix.

# File Summary

## Purpose
This file contains a packed representation of the entire repository's contents.
It is designed to be easily consumable by AI systems for analysis, code review,
or other automated processes.

## File Format
The content is organized as follows:
1. This summary section
2. Repository information
3. Directory structure
4. Multiple file entries, each consisting of:
  a. A header with the file path (## File: path/to/file)
  b. The full contents of the file in a code block

## Usage Guidelines
- This file should be treated as read-only. Any changes should be made to the
  original repository files, not this packed version.
- When processing this file, use the file path to distinguish
  between different files in the repository.
- Be aware that this file may contain sensitive information. Handle it with
  the same level of security as you would the original repository.

## Notes
- Some files may have been excluded based on .gitignore rules and Repomix's configuration
- Binary files are not included in this packed representation. Please refer to the Repository Structure section for a complete list of file paths, including binary files
- Files matching patterns in .gitignore are excluded
- Files matching default ignore patterns are excluded
- Files are sorted by Git change count (files with more changes are at the bottom)

## Additional Info

# Directory Structure
```
.gitignore
.repomixignore
app.json
App.tsx
index.ts
local_test_server.js
package.json
raspberry_pi_server.py
README.md
repomix-output.xml
repomix.config.json
test_server.py
tsconfig.json
```

# Files

## File: .repomixignore
````
# Add patterns to ignore here, one per line
# Example:
# *.log
# tmp/

# dependencies
node_modules/
````

## File: local_test_server.js
````javascript
#!/usr/bin/env node

/**
 * Local Test Server for IoT Sensor Data Collection
 * A simple Node.js server to test the React Native app locally
 * 
 * Usage:
 * 1. Install dependencies: npm install express cors
 * 2. Run server: node local_test_server.js
 * 3. Use your local IP address in the app (e.g., 192.168.1.XXX)
 * 
 * To find your local IP:
 * - Windows: ipconfig
 * - Mac/Linux: ifconfig or ip addr show
 */

const express = require('express');
const cors = require('cors');
const app = express();
const port = 5000;

// Middleware
app.use(cors());
app.use(express.json());

// Store recent sensor data in memory
let sensorDataHistory = [];
const MAX_HISTORY = 100;

// Health check endpoint
app.get('/health', (req, res) => {
  res.json({ 
    status: 'healthy', 
    timestamp: new Date().toISOString(),
    message: 'IoT Test Server is running!'
  });
});

// Main sensor data endpoint
app.post('/sensor_data', (req, res) => {
  const sensorData = req.body;
  
  console.log('\n📱 Received sensor data:', {
    timestamp: sensorData.timestamp,
    deviceId: sensorData.deviceId,
    accelerometer: sensorData.accelerometer,
    gyroscope: sensorData.gyroscope,
    location: sensorData.location
  });
  
  // Add to history
  sensorDataHistory.unshift({
    ...sensorData,
    receivedAt: new Date().toISOString()
  });
  
  // Keep only recent data
  if (sensorDataHistory.length > MAX_HISTORY) {
    sensorDataHistory = sensorDataHistory.slice(0, MAX_HISTORY);
  }
  
  // Send success response
  res.json({ 
    status: 'success',
    message: 'Sensor data received',
    timestamp: new Date().toISOString(),
    dataCount: sensorDataHistory.length
  });
});

// Get recent sensor data
app.get('/recent_data', (req, res) => {
  const limit = parseInt(req.query.limit) || 10;
  res.json({
    data: sensorDataHistory.slice(0, limit),
    total: sensorDataHistory.length
  });
});

// Statistics endpoint
app.get('/stats', (req, res) => {
  if (sensorDataHistory.length === 0) {
    return res.json({ message: 'No data received yet' });
  }
  
  const latestData = sensorDataHistory[0];
  const dataCount = sensorDataHistory.length;
  
  res.json({
    totalDataPoints: dataCount,
    latestTimestamp: latestData.timestamp,
    latestDevice: latestData.deviceId,
    latestLocation: latestData.location,
    serverUptime: process.uptime(),
    message: `Received ${dataCount} data points`
  });
});

// Start server
app.listen(port, '0.0.0.0', () => {
  console.log('\n🚀 IoT Test Server Started!');
  console.log(`📡 Server running on port ${port}`);
  console.log('\n📱 To use with the React Native app:');
  console.log('1. Find your computer\'s IP address:');
  console.log('   - Windows: Run "ipconfig" in cmd');
  console.log('   - Mac: Run "ifconfig" in terminal');
  console.log('   - Look for your local network IP (usually 192.168.x.x)');
  console.log('\n2. Enter that IP address in the app');
  console.log('3. Start data collection');
  console.log('\n🔍 Available endpoints:');
  console.log(`   - POST http://YOUR_IP:${port}/sensor_data (main endpoint)`);
  console.log(`   - GET  http://YOUR_IP:${port}/health (health check)`);
  console.log(`   - GET  http://YOUR_IP:${port}/recent_data (view recent data)`);
  console.log(`   - GET  http://YOUR_IP:${port}/stats (statistics)`);
  console.log('\n✅ Ready to receive sensor data!');
});

// Graceful shutdown
process.on('SIGINT', () => {
  console.log('\n👋 Shutting down server...');
  process.exit(0);
});
````

## File: raspberry_pi_server.py
````python
#!/usr/bin/env python3
"""
Raspberry Pi Server for IoT Sensor Data Collection
This Flask server receives sensor data from the React Native app
and stores it in JSON format with timestamps.

Requirements:
- Flask
- Python 3.6+

Installation:
pip3 install flask

Usage:
python3 raspberry_pi_server.py

The server will run on http://0.0.0.0:5000
"""

from flask import Flask, request, jsonify
import json
import os
from datetime import datetime
import logging

# Configure logging
logging.basicConfig(level=logging.INFO)
logger = logging.getLogger(__name__)

app = Flask(__name__)

# Data storage directory
DATA_DIR = "sensor_data"
if not os.path.exists(DATA_DIR):
    os.makedirs(DATA_DIR)

# In-memory storage for recent data (last 100 readings)
recent_data = []
MAX_RECENT_DATA = 100

@app.route('/sensor_data', methods=['POST'])
def receive_sensor_data():
    """
    Endpoint to receive sensor data from the React Native app
    Expected JSON format:
    {
        "timestamp": "2025-06-04T10:30:00.000Z",
        "accelerometer": {"x": 0.1, "y": 0.2, "z": 9.8},
        "gyroscope": {"x": 0.01, "y": 0.02, "z": 0.03},
        "location": {"latitude": 40.7128, "longitude": -74.0060, "altitude": 10, "speed": 0},
        "deviceId": "iPhone_12345"
    }
    """
    try:
        # Get JSON data from request
        data = request.get_json()
        
        if not data:
            return jsonify({"error": "No JSON data received"}), 400
        
        # Validate required fields
        required_fields = ["timestamp", "accelerometer", "gyroscope", "location", "deviceId"]
        for field in required_fields:
            if field not in data:
                return jsonify({"error": f"Missing required field: {field}"}), 400
        
        # Add server receive timestamp
        data["server_timestamp"] = datetime.now().isoformat()
        
        # Store in recent data (in memory)
        recent_data.append(data)
        if len(recent_data) > MAX_RECENT_DATA:
            recent_data.pop(0)
        
        # Save to file (one file per day)
        today = datetime.now().strftime("%Y-%m-%d")
        filename = f"{DATA_DIR}/sensor_data_{today}.json"
        
        # Append to daily file
        with open(filename, "a") as f:
            f.write(json.dumps(data) + "\n")
        
        # Log the received data
        logger.info(f"Received data from {data['deviceId']} at {data['timestamp']}")
        logger.info(f"Accelerometer: {data['accelerometer']}")
        logger.info(f"Gyroscope: {data['gyroscope']}")
        logger.info(f"Location: {data['location']}")
        
        return jsonify({
            "status": "success",
            "message": "Data received successfully",
            "timestamp": data["server_timestamp"]
        }), 200
        
    except Exception as e:
        logger.error(f"Error processing sensor data: {str(e)}")
        return jsonify({"error": "Internal server error"}), 500

@app.route('/health', methods=['GET'])
def health_check():
    """Health check endpoint"""
    return jsonify({
        "status": "healthy",
        "timestamp": datetime.now().isoformat(),
        "total_readings": len(recent_data)
    }), 200

@app.route('/recent_data', methods=['GET'])
def get_recent_data():
    """Get recent sensor data (last 100 readings)"""
    limit = request.args.get('limit', 10, type=int)
    limited_data = recent_data[-limit:] if limit < len(recent_data) else recent_data
    
    return jsonify({
        "data": limited_data,
        "total_count": len(recent_data),
        "returned_count": len(limited_data)
    }), 200

@app.route('/stats', methods=['GET'])
def get_stats():
    """Get statistics about received data"""
    if not recent_data:
        return jsonify({
            "total_readings": 0,
            "devices": [],
            "latest_timestamp": None
        }), 200
    
    # Get unique device IDs
    devices = list(set(data["deviceId"] for data in recent_data))
    
    # Get latest timestamp
    latest_timestamp = max(data["timestamp"] for data in recent_data)
    
    return jsonify({
        "total_readings": len(recent_data),
        "devices": devices,
        "latest_timestamp": latest_timestamp,
        "server_time": datetime.now().isoformat()
    }), 200

@app.route('/', methods=['GET'])
def index():
    """Simple index page"""
    return """
    <html>
    <head><title>IoT Sensor Data Server</title></head>
    <body>
        <h1>IoT Sensor Data Server</h1>
        <p>Server is running and ready to receive sensor data.</p>
        <h2>Available Endpoints:</h2>
        <ul>
            <li><a href="/health">GET /health</a> - Health check</li>
            <li><a href="/recent_data">GET /recent_data</a> - Recent sensor data</li>
            <li><a href="/stats">GET /stats</a> - Data statistics</li>
            <li>POST /sensor_data - Receive sensor data (from app)</li>
        </ul>
        <h2>Current Stats:</h2>
        <p>Total readings received: {}</p>
        <p>Server time: {}</p>
    </body>
    </html>
    """.format(len(recent_data), datetime.now().isoformat())

if __name__ == '__main__':
    logger.info("Starting IoT Sensor Data Server...")
    logger.info("Endpoints available:")
    logger.info("  POST /sensor_data - Receive sensor data")
    logger.info("  GET /health - Health check")
    logger.info("  GET /recent_data - Get recent readings")
    logger.info("  GET /stats - Get statistics")
    logger.info("  GET / - Index page")
    
    # Run the server
    # Use 0.0.0.0 to accept connections from any IP address
    app.run(host='0.0.0.0', port=5000, debug=True)
````

## File: README.md
````markdown
# IoT Sensor Data Collection App

A React Native Expo app that collects sensor data from iOS devices and transmits it to a Raspberry Pi server. This project is designed for IoT assignments and demonstrates real-time sensor data collection, processing, and wireless transmission.

## 📱 Features

### Sensor Data Collection
- **Accelerometer**: X, Y, Z acceleration values (updated every 100ms)
- **Gyroscope**: X, Y, Z rotation rates (updated every 100ms)
- **GPS Location**: Latitude, longitude, altitude, speed (updated every 2-3 seconds)
- **Device Information**: Unique device ID and orientation
- **Activity Detection**: Automatically detects walking, running, stationary, or driving

### User Interface
- Clean, modern design with real-time sensor displays
- IP address input with validation for Raspberry Pi connection
- Large START/STOP collection buttons
- Connection status indicator (green/red dot)
- Data transmission counter
- Last successful transmission timestamp
- Current activity display

### Data Transmission
- Batches sensor readings every 1-2 seconds
- HTTP POST requests to Raspberry Pi
- Graceful network error handling
- Real-time connection status updates

## 🛠️ Requirements

### Mobile App Requirements
- **iOS Device** (iPhone/iPad) - Physical device required for sensor access
- **Expo SDK 50+**
- **Node.js 18+**
- **npm or yarn**

### Raspberry Pi Server Requirements
- **Raspberry Pi** (any model with WiFi)
- **Python 3.6+**
- **Flask** web framework
- **Network connectivity** (same WiFi network as mobile device)

## 📦 Dependencies

### React Native App
```json
{
  "expo-sensors": "^14.1.4",
  "expo-location": "^18.1.5", 
  "expo-device": "^7.1.4",
  "axios": "^1.9.0"
}
```

### Python Server
```
Flask>=2.0.0
```

## 🚀 Setup Instructions

### 1. Mobile App Setup

```bash
# Clone or navigate to project directory
cd IoTSensorApp

# Install dependencies (already done if following the creation steps)
npm install

# Start the Expo development server
npm start
# or
npx expo start
```

#### Running on iOS Device
1. Install **Expo Go** app from the App Store
2. Scan the QR code displayed in terminal/browser
3. The app will load on your device

**Note**: Physical device is required - iOS Simulator cannot access device sensors.

### 2. Raspberry Pi Server Setup

#### Option A: Direct Setup on Raspberry Pi
```bash
# Copy the server file to your Raspberry Pi
scp raspberry_pi_server.py pi@[PI_IP_ADDRESS]:~/

# SSH into Raspberry Pi
ssh pi@[PI_IP_ADDRESS]

# Install Flask
pip3 install flask

# Run the server
python3 raspberry_pi_server.py
```

#### Option B: Setup from the Project Directory
```bash
# If you have the Raspberry Pi accessible locally
python3 raspberry_pi_server.py
```

The server will start on `http://0.0.0.0:5000` and display available endpoints.

## 📊 Data Format

The app sends JSON data in the following format:

```json
{
  "timestamp": "2025-06-04T10:30:00.000Z",
  "accelerometer": {
    "x": 0.1,
    "y": 0.2, 
    "z": 9.8
  },
  "gyroscope": {
    "x": 0.01,
    "y": 0.02,
    "z": 0.03
  },
  "location": {
    "latitude": 40.7128,
    "longitude": -74.0060,
    "altitude": 10,
    "speed": 0
  },
  "deviceId": "iPhone_12345"
}
```

## 🔧 Usage Instructions

### 1. Start the Raspberry Pi Server
```bash
python3 raspberry_pi_server.py
```
- Server runs on port 5000
- Note the Pi's IP address (displayed in terminal or use `hostname -I`)

### 2. Configure the Mobile App
1. Open the app on your iOS device
2. Enter the Raspberry Pi IP address (e.g., `192.168.1.100`)
3. Tap **START COLLECTION**

### 3. Monitor Data Collection
- Watch real-time sensor values update on screen
- Monitor connection status (green dot = connected)
- Check transmission counter
- Observe activity detection (stationary/walking/running/driving)

### 4. View Collected Data
Access the Raspberry Pi server endpoints:
- `http://[PI_IP]:5000/` - Web interface
- `http://[PI_IP]:5000/health` - Server health check
- `http://[PI_IP]:5000/recent_data` - Recent sensor readings
- `http://[PI_IP]:5000/stats` - Collection statistics

## 📁 Data Storage

The Raspberry Pi server stores data in two ways:

1. **In-Memory**: Last 100 readings for quick access
2. **File Storage**: Daily JSON files in `sensor_data/` directory
   - Format: `sensor_data_YYYY-MM-DD.json`
   - Each line contains one sensor reading

## 🔍 Troubleshooting

### Common Issues

**App won't connect to Pi:**
- Verify both devices are on the same WiFi network
- Check IP address is correct (use `hostname -I` on Pi)
- Ensure Pi server is running on port 5000
- Check firewall settings on Pi

**Sensors not working:**
- Use physical iOS device (not simulator)
- Grant location permissions when prompted
- Ensure app has sensor access permissions

**No GPS data:**
- Enable location services in iOS Settings
- Grant location permission to Expo Go app
- Test outdoors for better GPS signal

**Connection errors:**
- Check network connectivity
- Verify IP address format (e.g., 192.168.1.100)
- Restart both app and server

### Network Setup
Ensure both devices are on the same network:
```bash
# On Raspberry Pi, check IP
hostname -I

# Test connectivity from another device
ping [PI_IP_ADDRESS]
```

## 🎯 Activity Detection Logic

The app automatically detects user activity based on sensor data:

- **Stationary**: Low acceleration and gyroscope values
- **Walking**: Moderate movement, speed < 2 m/s
- **Running**: Higher movement, speed 2-10 m/s  
- **Driving**: High speed > 10 m/s

## 📈 Performance

- **Sensor Update Rate**: 100ms for accelerometer/gyroscope
- **GPS Update Rate**: 2-3 seconds
- **Data Transmission**: Every 1.5 seconds
- **Network Timeout**: 5 seconds
- **Data Buffer**: Latest reading per transmission

## 🔒 Security Notes

- Server accepts connections from any IP (0.0.0.0)
- No authentication implemented (suitable for local networks)
- Data transmitted in plain HTTP (not HTTPS)
- For production use, implement proper security measures

## 📝 Assignment Notes

This project demonstrates:
- **IoT Sensor Integration**: Multiple sensor types with real-time data
- **Wireless Communication**: HTTP-based data transmission
- **Data Processing**: Activity detection and sensor fusion
- **User Interface**: Clean, functional mobile app design
- **Server-Side Handling**: Data reception, validation, and storage
- **Error Handling**: Network failures and graceful degradation

## 🤝 Contributing

For educational use and IoT assignments. Feel free to extend with additional features:
- HTTPS support
- Database integration
- Data visualization
- Additional sensors
- Authentication
- Real-time charting

## 📄 License

Educational use for IoT assignments at Loyalist College.
````

## File: repomix-output.xml
````xml
This file is a merged representation of the entire codebase, combined into a single document by Repomix.

<file_summary>
This section contains a summary of this file.

<purpose>
This file contains a packed representation of the entire repository's contents.
It is designed to be easily consumable by AI systems for analysis, code review,
or other automated processes.
</purpose>

<file_format>
The content is organized as follows:
1. This summary section
2. Repository information
3. Directory structure
4. Repository files, each consisting of:
  - File path as an attribute
  - Full contents of the file
</file_format>

<usage_guidelines>
- This file should be treated as read-only. Any changes should be made to the
  original repository files, not this packed version.
- When processing this file, use the file path to distinguish
  between different files in the repository.
- Be aware that this file may contain sensitive information. Handle it with
  the same level of security as you would the original repository.
</usage_guidelines>

<notes>
- Some files may have been excluded based on .gitignore rules and Repomix's configuration
- Binary files are not included in this packed representation. Please refer to the Repository Structure section for a complete list of file paths, including binary files
- Files matching patterns in .gitignore are excluded
- Files matching default ignore patterns are excluded
- Files are sorted by Git change count (files with more changes are at the bottom)
</notes>

<additional_info>

</additional_info>

</file_summary>

<directory_structure>
.gitignore
app.json
App.tsx
index.ts
local_test_server.js
package.json
raspberry_pi_server.py
README.md
test_server.py
tsconfig.json
</directory_structure>

<files>
This section contains the contents of the repository's files.

<file path="local_test_server.js">
#!/usr/bin/env node

/**
 * Local Test Server for IoT Sensor Data Collection
 * A simple Node.js server to test the React Native app locally
 * 
 * Usage:
 * 1. Install dependencies: npm install express cors
 * 2. Run server: node local_test_server.js
 * 3. Use your local IP address in the app (e.g., 192.168.1.XXX)
 * 
 * To find your local IP:
 * - Windows: ipconfig
 * - Mac/Linux: ifconfig or ip addr show
 */

const express = require('express');
const cors = require('cors');
const app = express();
const port = 5000;

// Middleware
app.use(cors());
app.use(express.json());

// Store recent sensor data in memory
let sensorDataHistory = [];
const MAX_HISTORY = 100;

// Health check endpoint
app.get('/health', (req, res) => {
  res.json({ 
    status: 'healthy', 
    timestamp: new Date().toISOString(),
    message: 'IoT Test Server is running!'
  });
});

// Main sensor data endpoint
app.post('/sensor_data', (req, res) => {
  const sensorData = req.body;
  
  console.log('\n📱 Received sensor data:', {
    timestamp: sensorData.timestamp,
    deviceId: sensorData.deviceId,
    accelerometer: sensorData.accelerometer,
    gyroscope: sensorData.gyroscope,
    location: sensorData.location
  });
  
  // Add to history
  sensorDataHistory.unshift({
    ...sensorData,
    receivedAt: new Date().toISOString()
  });
  
  // Keep only recent data
  if (sensorDataHistory.length > MAX_HISTORY) {
    sensorDataHistory = sensorDataHistory.slice(0, MAX_HISTORY);
  }
  
  // Send success response
  res.json({ 
    status: 'success',
    message: 'Sensor data received',
    timestamp: new Date().toISOString(),
    dataCount: sensorDataHistory.length
  });
});

// Get recent sensor data
app.get('/recent_data', (req, res) => {
  const limit = parseInt(req.query.limit) || 10;
  res.json({
    data: sensorDataHistory.slice(0, limit),
    total: sensorDataHistory.length
  });
});

// Statistics endpoint
app.get('/stats', (req, res) => {
  if (sensorDataHistory.length === 0) {
    return res.json({ message: 'No data received yet' });
  }
  
  const latestData = sensorDataHistory[0];
  const dataCount = sensorDataHistory.length;
  
  res.json({
    totalDataPoints: dataCount,
    latestTimestamp: latestData.timestamp,
    latestDevice: latestData.deviceId,
    latestLocation: latestData.location,
    serverUptime: process.uptime(),
    message: `Received ${dataCount} data points`
  });
});

// Start server
app.listen(port, '0.0.0.0', () => {
  console.log('\n🚀 IoT Test Server Started!');
  console.log(`📡 Server running on port ${port}`);
  console.log('\n📱 To use with the React Native app:');
  console.log('1. Find your computer\'s IP address:');
  console.log('   - Windows: Run "ipconfig" in cmd');
  console.log('   - Mac: Run "ifconfig" in terminal');
  console.log('   - Look for your local network IP (usually 192.168.x.x)');
  console.log('\n2. Enter that IP address in the app');
  console.log('3. Start data collection');
  console.log('\n🔍 Available endpoints:');
  console.log(`   - POST http://YOUR_IP:${port}/sensor_data (main endpoint)`);
  console.log(`   - GET  http://YOUR_IP:${port}/health (health check)`);
  console.log(`   - GET  http://YOUR_IP:${port}/recent_data (view recent data)`);
  console.log(`   - GET  http://YOUR_IP:${port}/stats (statistics)`);
  console.log('\n✅ Ready to receive sensor data!');
});

// Graceful shutdown
process.on('SIGINT', () => {
  console.log('\n👋 Shutting down server...');
  process.exit(0);
});
</file>

<file path="raspberry_pi_server.py">
#!/usr/bin/env python3
"""
Raspberry Pi Server for IoT Sensor Data Collection
This Flask server receives sensor data from the React Native app
and stores it in JSON format with timestamps.

Requirements:
- Flask
- Python 3.6+

Installation:
pip3 install flask

Usage:
python3 raspberry_pi_server.py

The server will run on http://0.0.0.0:5000
"""

from flask import Flask, request, jsonify
import json
import os
from datetime import datetime
import logging

# Configure logging
logging.basicConfig(level=logging.INFO)
logger = logging.getLogger(__name__)

app = Flask(__name__)

# Data storage directory
DATA_DIR = "sensor_data"
if not os.path.exists(DATA_DIR):
    os.makedirs(DATA_DIR)

# In-memory storage for recent data (last 100 readings)
recent_data = []
MAX_RECENT_DATA = 100

@app.route('/sensor_data', methods=['POST'])
def receive_sensor_data():
    """
    Endpoint to receive sensor data from the React Native app
    Expected JSON format:
    {
        "timestamp": "2025-06-04T10:30:00.000Z",
        "accelerometer": {"x": 0.1, "y": 0.2, "z": 9.8},
        "gyroscope": {"x": 0.01, "y": 0.02, "z": 0.03},
        "location": {"latitude": 40.7128, "longitude": -74.0060, "altitude": 10, "speed": 0},
        "deviceId": "iPhone_12345"
    }
    """
    try:
        # Get JSON data from request
        data = request.get_json()
        
        if not data:
            return jsonify({"error": "No JSON data received"}), 400
        
        # Validate required fields
        required_fields = ["timestamp", "accelerometer", "gyroscope", "location", "deviceId"]
        for field in required_fields:
            if field not in data:
                return jsonify({"error": f"Missing required field: {field}"}), 400
        
        # Add server receive timestamp
        data["server_timestamp"] = datetime.now().isoformat()
        
        # Store in recent data (in memory)
        recent_data.append(data)
        if len(recent_data) > MAX_RECENT_DATA:
            recent_data.pop(0)
        
        # Save to file (one file per day)
        today = datetime.now().strftime("%Y-%m-%d")
        filename = f"{DATA_DIR}/sensor_data_{today}.json"
        
        # Append to daily file
        with open(filename, "a") as f:
            f.write(json.dumps(data) + "\n")
        
        # Log the received data
        logger.info(f"Received data from {data['deviceId']} at {data['timestamp']}")
        logger.info(f"Accelerometer: {data['accelerometer']}")
        logger.info(f"Gyroscope: {data['gyroscope']}")
        logger.info(f"Location: {data['location']}")
        
        return jsonify({
            "status": "success",
            "message": "Data received successfully",
            "timestamp": data["server_timestamp"]
        }), 200
        
    except Exception as e:
        logger.error(f"Error processing sensor data: {str(e)}")
        return jsonify({"error": "Internal server error"}), 500

@app.route('/health', methods=['GET'])
def health_check():
    """Health check endpoint"""
    return jsonify({
        "status": "healthy",
        "timestamp": datetime.now().isoformat(),
        "total_readings": len(recent_data)
    }), 200

@app.route('/recent_data', methods=['GET'])
def get_recent_data():
    """Get recent sensor data (last 100 readings)"""
    limit = request.args.get('limit', 10, type=int)
    limited_data = recent_data[-limit:] if limit < len(recent_data) else recent_data
    
    return jsonify({
        "data": limited_data,
        "total_count": len(recent_data),
        "returned_count": len(limited_data)
    }), 200

@app.route('/stats', methods=['GET'])
def get_stats():
    """Get statistics about received data"""
    if not recent_data:
        return jsonify({
            "total_readings": 0,
            "devices": [],
            "latest_timestamp": None
        }), 200
    
    # Get unique device IDs
    devices = list(set(data["deviceId"] for data in recent_data))
    
    # Get latest timestamp
    latest_timestamp = max(data["timestamp"] for data in recent_data)
    
    return jsonify({
        "total_readings": len(recent_data),
        "devices": devices,
        "latest_timestamp": latest_timestamp,
        "server_time": datetime.now().isoformat()
    }), 200

@app.route('/', methods=['GET'])
def index():
    """Simple index page"""
    return """
    <html>
    <head><title>IoT Sensor Data Server</title></head>
    <body>
        <h1>IoT Sensor Data Server</h1>
        <p>Server is running and ready to receive sensor data.</p>
        <h2>Available Endpoints:</h2>
        <ul>
            <li><a href="/health">GET /health</a> - Health check</li>
            <li><a href="/recent_data">GET /recent_data</a> - Recent sensor data</li>
            <li><a href="/stats">GET /stats</a> - Data statistics</li>
            <li>POST /sensor_data - Receive sensor data (from app)</li>
        </ul>
        <h2>Current Stats:</h2>
        <p>Total readings received: {}</p>
        <p>Server time: {}</p>
    </body>
    </html>
    """.format(len(recent_data), datetime.now().isoformat())

if __name__ == '__main__':
    logger.info("Starting IoT Sensor Data Server...")
    logger.info("Endpoints available:")
    logger.info("  POST /sensor_data - Receive sensor data")
    logger.info("  GET /health - Health check")
    logger.info("  GET /recent_data - Get recent readings")
    logger.info("  GET /stats - Get statistics")
    logger.info("  GET / - Index page")
    
    # Run the server
    # Use 0.0.0.0 to accept connections from any IP address
    app.run(host='0.0.0.0', port=5000, debug=True)
</file>

<file path="README.md">
# IoT Sensor Data Collection App

A React Native Expo app that collects sensor data from iOS devices and transmits it to a Raspberry Pi server. This project is designed for IoT assignments and demonstrates real-time sensor data collection, processing, and wireless transmission.

## 📱 Features

### Sensor Data Collection
- **Accelerometer**: X, Y, Z acceleration values (updated every 100ms)
- **Gyroscope**: X, Y, Z rotation rates (updated every 100ms)
- **GPS Location**: Latitude, longitude, altitude, speed (updated every 2-3 seconds)
- **Device Information**: Unique device ID and orientation
- **Activity Detection**: Automatically detects walking, running, stationary, or driving

### User Interface
- Clean, modern design with real-time sensor displays
- IP address input with validation for Raspberry Pi connection
- Large START/STOP collection buttons
- Connection status indicator (green/red dot)
- Data transmission counter
- Last successful transmission timestamp
- Current activity display

### Data Transmission
- Batches sensor readings every 1-2 seconds
- HTTP POST requests to Raspberry Pi
- Graceful network error handling
- Real-time connection status updates

## 🛠️ Requirements

### Mobile App Requirements
- **iOS Device** (iPhone/iPad) - Physical device required for sensor access
- **Expo SDK 50+**
- **Node.js 18+**
- **npm or yarn**

### Raspberry Pi Server Requirements
- **Raspberry Pi** (any model with WiFi)
- **Python 3.6+**
- **Flask** web framework
- **Network connectivity** (same WiFi network as mobile device)

## 📦 Dependencies

### React Native App
```json
{
  "expo-sensors": "^14.1.4",
  "expo-location": "^18.1.5", 
  "expo-device": "^7.1.4",
  "axios": "^1.9.0"
}
```

### Python Server
```
Flask>=2.0.0
```

## 🚀 Setup Instructions

### 1. Mobile App Setup

```bash
# Clone or navigate to project directory
cd IoTSensorApp

# Install dependencies (already done if following the creation steps)
npm install

# Start the Expo development server
npm start
# or
npx expo start
```

#### Running on iOS Device
1. Install **Expo Go** app from the App Store
2. Scan the QR code displayed in terminal/browser
3. The app will load on your device

**Note**: Physical device is required - iOS Simulator cannot access device sensors.

### 2. Raspberry Pi Server Setup

#### Option A: Direct Setup on Raspberry Pi
```bash
# Copy the server file to your Raspberry Pi
scp raspberry_pi_server.py pi@[PI_IP_ADDRESS]:~/

# SSH into Raspberry Pi
ssh pi@[PI_IP_ADDRESS]

# Install Flask
pip3 install flask

# Run the server
python3 raspberry_pi_server.py
```

#### Option B: Setup from the Project Directory
```bash
# If you have the Raspberry Pi accessible locally
python3 raspberry_pi_server.py
```

The server will start on `http://0.0.0.0:5000` and display available endpoints.

## 📊 Data Format

The app sends JSON data in the following format:

```json
{
  "timestamp": "2025-06-04T10:30:00.000Z",
  "accelerometer": {
    "x": 0.1,
    "y": 0.2, 
    "z": 9.8
  },
  "gyroscope": {
    "x": 0.01,
    "y": 0.02,
    "z": 0.03
  },
  "location": {
    "latitude": 40.7128,
    "longitude": -74.0060,
    "altitude": 10,
    "speed": 0
  },
  "deviceId": "iPhone_12345"
}
```

## 🔧 Usage Instructions

### 1. Start the Raspberry Pi Server
```bash
python3 raspberry_pi_server.py
```
- Server runs on port 5000
- Note the Pi's IP address (displayed in terminal or use `hostname -I`)

### 2. Configure the Mobile App
1. Open the app on your iOS device
2. Enter the Raspberry Pi IP address (e.g., `192.168.1.100`)
3. Tap **START COLLECTION**

### 3. Monitor Data Collection
- Watch real-time sensor values update on screen
- Monitor connection status (green dot = connected)
- Check transmission counter
- Observe activity detection (stationary/walking/running/driving)

### 4. View Collected Data
Access the Raspberry Pi server endpoints:
- `http://[PI_IP]:5000/` - Web interface
- `http://[PI_IP]:5000/health` - Server health check
- `http://[PI_IP]:5000/recent_data` - Recent sensor readings
- `http://[PI_IP]:5000/stats` - Collection statistics

## 📁 Data Storage

The Raspberry Pi server stores data in two ways:

1. **In-Memory**: Last 100 readings for quick access
2. **File Storage**: Daily JSON files in `sensor_data/` directory
   - Format: `sensor_data_YYYY-MM-DD.json`
   - Each line contains one sensor reading

## 🔍 Troubleshooting

### Common Issues

**App won't connect to Pi:**
- Verify both devices are on the same WiFi network
- Check IP address is correct (use `hostname -I` on Pi)
- Ensure Pi server is running on port 5000
- Check firewall settings on Pi

**Sensors not working:**
- Use physical iOS device (not simulator)
- Grant location permissions when prompted
- Ensure app has sensor access permissions

**No GPS data:**
- Enable location services in iOS Settings
- Grant location permission to Expo Go app
- Test outdoors for better GPS signal

**Connection errors:**
- Check network connectivity
- Verify IP address format (e.g., 192.168.1.100)
- Restart both app and server

### Network Setup
Ensure both devices are on the same network:
```bash
# On Raspberry Pi, check IP
hostname -I

# Test connectivity from another device
ping [PI_IP_ADDRESS]
```

## 🎯 Activity Detection Logic

The app automatically detects user activity based on sensor data:

- **Stationary**: Low acceleration and gyroscope values
- **Walking**: Moderate movement, speed < 2 m/s
- **Running**: Higher movement, speed 2-10 m/s  
- **Driving**: High speed > 10 m/s

## 📈 Performance

- **Sensor Update Rate**: 100ms for accelerometer/gyroscope
- **GPS Update Rate**: 2-3 seconds
- **Data Transmission**: Every 1.5 seconds
- **Network Timeout**: 5 seconds
- **Data Buffer**: Latest reading per transmission

## 🔒 Security Notes

- Server accepts connections from any IP (0.0.0.0)
- No authentication implemented (suitable for local networks)
- Data transmitted in plain HTTP (not HTTPS)
- For production use, implement proper security measures

## 📝 Assignment Notes

This project demonstrates:
- **IoT Sensor Integration**: Multiple sensor types with real-time data
- **Wireless Communication**: HTTP-based data transmission
- **Data Processing**: Activity detection and sensor fusion
- **User Interface**: Clean, functional mobile app design
- **Server-Side Handling**: Data reception, validation, and storage
- **Error Handling**: Network failures and graceful degradation

## 🤝 Contributing

For educational use and IoT assignments. Feel free to extend with additional features:
- HTTPS support
- Database integration
- Data visualization
- Additional sensors
- Authentication
- Real-time charting

## 📄 License

Educational use for IoT assignments at Loyalist College.
</file>

<file path="test_server.py">
#!/usr/bin/env python3
"""
Test script to verify the Raspberry Pi server is working correctly.
Sends sample sensor data to test the server endpoints.

Usage:
python3 test_server.py [server_ip]

If no IP is provided, defaults to localhost (127.0.0.1)
"""

import requests
import json
import sys
from datetime import datetime
import time

def test_server(server_ip="127.0.0.1", port=5000):
    """Test the sensor data server"""
    base_url = f"http://{server_ip}:{port}"
    
    print(f"Testing IoT Sensor Data Server at {base_url}")
    print("=" * 50)
    
    # Test 1: Health Check
    print("1. Testing health endpoint...")
    try:
        response = requests.get(f"{base_url}/health", timeout=5)
        if response.status_code == 200:
            print("✅ Health check passed")
            print(f"   Response: {response.json()}")
        else:
            print(f"❌ Health check failed with status {response.status_code}")
    except Exception as e:
        print(f"❌ Health check failed: {e}")
        return False
    
    # Test 2: Send sample sensor data
    print("\n2. Testing sensor data endpoint...")
    sample_data = {
        "timestamp": datetime.now().isoformat() + "Z",
        "accelerometer": {"x": 0.1, "y": 0.2, "z": 9.8},
        "gyroscope": {"x": 0.01, "y": 0.02, "z": 0.03},
        "location": {"latitude": 40.7128, "longitude": -74.0060, "altitude": 10, "speed": 0},
        "deviceId": "TestDevice_12345"
    }
    
    try:
        response = requests.post(
            f"{base_url}/sensor_data",
            json=sample_data,
            headers={"Content-Type": "application/json"},
            timeout=5
        )
        if response.status_code == 200:
            print("✅ Sensor data submission passed")
            print(f"   Response: {response.json()}")
        else:
            print(f"❌ Sensor data submission failed with status {response.status_code}")
            print(f"   Response: {response.text}")
    except Exception as e:
        print(f"❌ Sensor data submission failed: {e}")
        return False
    
    # Test 3: Get recent data
    print("\n3. Testing recent data endpoint...")
    try:
        response = requests.get(f"{base_url}/recent_data?limit=5", timeout=5)
        if response.status_code == 200:
            data = response.json()
            print("✅ Recent data retrieval passed")
            print(f"   Total readings: {data['total_count']}")
            print(f"   Returned readings: {data['returned_count']}")
        else:
            print(f"❌ Recent data retrieval failed with status {response.status_code}")
    except Exception as e:
        print(f"❌ Recent data retrieval failed: {e}")
    
    # Test 4: Get statistics
    print("\n4. Testing statistics endpoint...")
    try:
        response = requests.get(f"{base_url}/stats", timeout=5)
        if response.status_code == 200:
            stats = response.json()
            print("✅ Statistics retrieval passed")
            print(f"   Total readings: {stats['total_readings']}")
            print(f"   Devices: {stats['devices']}")
            print(f"   Latest timestamp: {stats['latest_timestamp']}")
        else:
            print(f"❌ Statistics retrieval failed with status {response.status_code}")
    except Exception as e:
        print(f"❌ Statistics retrieval failed: {e}")
    
    # Test 5: Send multiple data points
    print("\n5. Testing multiple data submissions...")
    for i in range(3):
        test_data = {
            "timestamp": datetime.now().isoformat() + "Z",
            "accelerometer": {"x": 0.1 + i * 0.1, "y": 0.2 + i * 0.1, "z": 9.8 + i * 0.1},
            "gyroscope": {"x": 0.01 + i * 0.01, "y": 0.02 + i * 0.01, "z": 0.03 + i * 0.01},
            "location": {"latitude": 40.7128 + i * 0.001, "longitude": -74.0060 + i * 0.001, "altitude": 10 + i, "speed": i},
            "deviceId": f"TestDevice_{12345 + i}"
        }
        
        try:
            response = requests.post(f"{base_url}/sensor_data", json=test_data, timeout=5)
            if response.status_code == 200:
                print(f"✅ Data point {i+1} submitted successfully")
            else:
                print(f"❌ Data point {i+1} failed with status {response.status_code}")
        except Exception as e:
            print(f"❌ Data point {i+1} failed: {e}")
        
        time.sleep(0.5)  # Small delay between submissions
    
    print("\n" + "=" * 50)
    print("🎉 Server testing completed!")
    print(f"📊 Access web interface at: {base_url}/")
    return True

def main():
    """Main function"""
    if len(sys.argv) > 1:
        server_ip = sys.argv[1]
    else:
        server_ip = "127.0.0.1"
    
    print("IoT Sensor Data Server Test Script")
    print("=" * 50)
    print(f"Target server: {server_ip}:5000")
    print("Make sure the server is running before starting this test!")
    print("")
    
    # Wait for user confirmation
    input("Press Enter to start testing...")
    
    test_server(server_ip)

if __name__ == "__main__":
    main()
</file>

<file path=".gitignore">
# Learn more https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files

# dependencies
node_modules/

# Expo
.expo/
dist/
web-build/
expo-env.d.ts

# Native
.kotlin/
*.orig.*
*.jks
*.p8
*.p12
*.key
*.mobileprovision

# Metro
.metro-health-check*

# debug
npm-debug.*
yarn-debug.*
yarn-error.*

# macOS
.DS_Store
*.pem

# local env files
.env*.local

# typescript
*.tsbuildinfo
</file>

<file path="app.json">
{
  "expo": {
    "name": "IoTSensorApp",
    "slug": "IoTSensorApp",
    "version": "1.0.0",
    "orientation": "portrait",
    "icon": "./assets/icon.png",
    "userInterfaceStyle": "light",
    "newArchEnabled": true,
    "splash": {
      "image": "./assets/splash-icon.png",
      "resizeMode": "contain",
      "backgroundColor": "#ffffff"
    },
    "ios": {
      "supportsTablet": true,
      "infoPlist": {
        "NSLocationWhenInUseUsageDescription": "This app needs access to location for GPS tracking and IoT data collection.",
        "NSLocationAlwaysAndWhenInUseUsageDescription": "This app needs access to location for GPS tracking and IoT data collection.",
        "NSMotionUsageDescription": "This app needs access to motion sensors for accelerometer and gyroscope data collection."
      }
    },
    "android": {
      "adaptiveIcon": {
        "foregroundImage": "./assets/adaptive-icon.png",
        "backgroundColor": "#ffffff"
      },
      "edgeToEdgeEnabled": true,
      "permissions": [
        "ACCESS_FINE_LOCATION",
        "ACCESS_COARSE_LOCATION",
        "BODY_SENSORS",
        "INTERNET",
        "ACCESS_NETWORK_STATE"
      ]
    },
    "web": {
      "favicon": "./assets/favicon.png"
    }
  }
}
</file>

<file path="App.tsx">
import React, { useState, useEffect, useRef } from 'react';
import {
  StyleSheet,
  Text,
  View,
  TextInput,
  TouchableOpacity,
  Alert,
  ScrollView,
  SafeAreaView,
  Platform,
} from 'react-native';
import { StatusBar } from 'expo-status-bar';
import { Accelerometer, Gyroscope } from 'expo-sensors';
import * as Location from 'expo-location';
import * as Device from 'expo-device';
import axios from 'axios';

interface SensorData {
  timestamp: string;
  accelerometer: { x: number; y: number; z: number };
  gyroscope: { x: number; y: number; z: number };
  location: { latitude: number; longitude: number; altitude: number | null; speed: number | null };
  deviceId: string;
}

interface AccelerometerData {
  x: number;
  y: number;
  z: number;
}

interface GyroscopeData {
  x: number;
  y: number;
  z: number;
}

export default function App() {
  // State variables
  const [piIPAddress, setPiIPAddress] = useState('192.168.1.100');
  const [isCollecting, setIsCollecting] = useState(false);
  const [connectionStatus, setConnectionStatus] = useState<'disconnected' | 'connected' | 'error'>('disconnected');
  const [transmissionCount, setTransmissionCount] = useState(0);
  const [lastTransmissionTime, setLastTransmissionTime] = useState<string>('Never');
  const [currentActivity, setCurrentActivity] = useState<string>('stationary');
  
  // Sensor data states
  const [accelerometerData, setAccelerometerData] = useState<AccelerometerData>({ x: 0, y: 0, z: 0 });
  const [gyroscopeData, setGyroscopeData] = useState<GyroscopeData>({ x: 0, y: 0, z: 0 });
  const [locationData, setLocationData] = useState({ latitude: 0, longitude: 0, altitude: null, speed: null });
  const [deviceId, setDeviceId] = useState<string>('');

  // Refs for subscriptions and intervals
  const accelerometerSubscription = useRef<any>(null);
  const gyroscopeSubscription = useRef<any>(null);
  const locationSubscription = useRef<any>(null);
  const transmissionInterval = useRef<any>(null);
  const sensorDataBuffer = useRef<SensorData[]>([]);

  // Initialize device ID and request permissions
  useEffect(() => {
    initializeApp();
    return () => {
      cleanup();
    };
  }, []);

  const initializeApp = async () => {
    console.log('🚀 Initializing IoT Sensor App...');
    
    // Get device ID
    const deviceName = Device.deviceName || 'Unknown';
    const brand = Device.brand || 'Unknown';
    const generatedDeviceId = `${brand}_${deviceName}_${Math.random().toString(36).substr(2, 9)}`;
    setDeviceId(generatedDeviceId);
    
    console.log('📱 Device Info:', {
      deviceName: deviceName,
      brand: brand,
      deviceId: generatedDeviceId,
      platform: Platform.OS
    });

    // Request location permissions
    console.log('🔐 Requesting location permissions...');
    const { status } = await Location.requestForegroundPermissionsAsync();
    if (status !== 'granted') {
      Alert.alert('Permission Denied', 'Location permission is required for GPS tracking');
      console.log('❌ Location permission denied');
    } else {
      console.log('✅ Location permission granted');
    }
    
    console.log('🎉 App initialization complete!');
  };

  const cleanup = () => {
    stopDataCollection();
  };

  const validateIPAddress = (ip: string): boolean => {
    const ipRegex = /^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/;
    return ipRegex.test(ip);
  };

  const determineActivity = (accel: AccelerometerData, gyro: GyroscopeData, speed: number | null): string => {
    const accelMagnitude = Math.sqrt(accel.x ** 2 + accel.y ** 2 + accel.z ** 2);
    const gyroMagnitude = Math.sqrt(gyro.x ** 2 + gyro.y ** 2 + gyro.z ** 2);
    
    if (speed && speed > 10) {
      return 'driving';
    } else if (speed && speed > 2) {
      return 'running';
    } else if (accelMagnitude > 10.5 || gyroMagnitude > 0.5) {
      return 'walking';
    } else {
      return 'stationary';
    }
  };

  const startSensorCollection = async () => {
    console.log('🚀 Starting sensor collection...');
    
    // Set update intervals
    Accelerometer.setUpdateInterval(100); // 100ms
    Gyroscope.setUpdateInterval(100); // 100ms
    
    console.log('📱 Sensor update intervals set: Accelerometer & Gyroscope = 100ms');

    // Start accelerometer
    accelerometerSubscription.current = Accelerometer.addListener((data) => {
      setAccelerometerData(data);
      console.log('📊 Accelerometer data:', {
        x: data.x.toFixed(3),
        y: data.y.toFixed(3),
        z: data.z.toFixed(3)
      });
    });

    // Start gyroscope
    gyroscopeSubscription.current = Gyroscope.addListener((data) => {
      setGyroscopeData(data);
      console.log('🌀 Gyroscope data:', {
        x: data.x.toFixed(3),
        y: data.y.toFixed(3),
        z: data.z.toFixed(3)
      });
    });

    console.log('✅ Accelerometer and Gyroscope listeners started');

    // Start location tracking
    try {
      console.log('🌍 Starting GPS location tracking...');
      locationSubscription.current = await Location.watchPositionAsync(
        {
          accuracy: Location.Accuracy.High,
          timeInterval: 2000, // 2 seconds
          distanceInterval: 1,
        },
        (location) => {
          const locationInfo = {
            latitude: location.coords.latitude,
            longitude: location.coords.longitude,
            altitude: location.coords.altitude,
            speed: location.coords.speed,
          };
          setLocationData(locationInfo);
          console.log('📍 GPS location update:', {
            latitude: locationInfo.latitude.toFixed(6),
            longitude: locationInfo.longitude.toFixed(6),
            altitude: locationInfo.altitude?.toFixed(2) || 'N/A',
            speed: locationInfo.speed?.toFixed(2) || 'N/A'
          });
        }
      );
      console.log('✅ GPS location tracking started');
    } catch (error) {
      console.error('❌ Error starting location tracking:', error);
    }
  };

  const stopSensorCollection = () => {
    console.log('🛑 Stopping sensor collection...');
    
    if (accelerometerSubscription.current) {
      accelerometerSubscription.current.remove();
      accelerometerSubscription.current = null;
      console.log('📊 Accelerometer listener stopped');
    }
    if (gyroscopeSubscription.current) {
      gyroscopeSubscription.current.remove();
      gyroscopeSubscription.current = null;
      console.log('🌀 Gyroscope listener stopped');
    }
    if (locationSubscription.current && locationSubscription.current.remove) {
      locationSubscription.current.remove();
      locationSubscription.current = null;
      console.log('📍 GPS location tracking stopped');
    }
    
    console.log('✅ All sensors stopped successfully');
  };

  const startDataTransmission = () => {
    console.log('🔄 Starting data transmission to Pi (every 1.5 seconds)...');
    
    transmissionInterval.current = setInterval(() => {
      if (sensorDataBuffer.current.length > 0) {
        console.log('📤 Sending buffered sensor data...');
        sendDataToPi();
      } else {
        // Create current sensor reading
        const currentReading: SensorData = {
          timestamp: new Date().toISOString(),
          accelerometer: accelerometerData,
          gyroscope: gyroscopeData,
          location: locationData,
          deviceId: deviceId,
        };
        
        // Update activity based on current data
        const activity = determineActivity(accelerometerData, gyroscopeData, locationData.speed);
        setCurrentActivity(activity);
        
        console.log('📊 Created new sensor reading:', {
          timestamp: currentReading.timestamp,
          activity: activity,
          hasLocation: !!(locationData.latitude && locationData.longitude)
        });
        
        sensorDataBuffer.current = [currentReading];
        sendDataToPi();
      }
    }, 1500); // Send every 1.5 seconds
    
    console.log('✅ Data transmission timer started');
  };

  const stopDataTransmission = () => {
    console.log('🔄 Stopping data transmission...');
    
    if (transmissionInterval.current) {
      clearInterval(transmissionInterval.current);
      transmissionInterval.current = null;
      console.log('✅ Data transmission timer stopped');
    }
  };

  const sendDataToPi = async () => {
    if (!validateIPAddress(piIPAddress)) {
      setConnectionStatus('error');
      Alert.alert('Invalid IP', 'Please enter a valid IP address');
      console.log('❌ Invalid IP address:', piIPAddress);
      return;
    }

    try {
      const url = `http://${piIPAddress}:5000/sensor_data`;
      const dataToSend = sensorDataBuffer.current[0]; // Send latest reading
      
      console.log('📡 Sending data to Pi:', {
        url: url,
        timestamp: dataToSend.timestamp,
        deviceId: dataToSend.deviceId,
        accelerometer: {
          x: dataToSend.accelerometer.x.toFixed(3),
          y: dataToSend.accelerometer.y.toFixed(3),
          z: dataToSend.accelerometer.z.toFixed(3)
        },
        gyroscope: {
          x: dataToSend.gyroscope.x.toFixed(3),
          y: dataToSend.gyroscope.y.toFixed(3),
          z: dataToSend.gyroscope.z.toFixed(3)
        },
        location: {
          latitude: dataToSend.location.latitude?.toFixed(6),
          longitude: dataToSend.location.longitude?.toFixed(6),
          altitude: dataToSend.location.altitude?.toFixed(2),
          speed: dataToSend.location.speed?.toFixed(2)
        }
      });
      
      const response = await axios.post(url, dataToSend, {
        timeout: 5000,
        headers: {
          'Content-Type': 'application/json',
        },
      });

      if (response.status === 200) {
        setConnectionStatus('connected');
        setTransmissionCount(prev => prev + 1);
        setLastTransmissionTime(new Date().toLocaleTimeString());
        sensorDataBuffer.current = [];
        
        console.log('✅ Data sent successfully!', {
          status: response.status,
          transmissionCount: transmissionCount + 1,
          responseData: response.data,
          timestamp: new Date().toLocaleTimeString()
        });
      }
    } catch (error) {
      setConnectionStatus('error');
      console.error('❌ Error sending data to Pi:', {
        error: error.message,
        code: error.code,
        url: `http://${piIPAddress}:5000/sensor_data`,
        timestamp: new Date().toLocaleTimeString()
      });
    }
  };

  const startDataCollection = async () => {
    console.log('🎯 START DATA COLLECTION INITIATED');
    console.log('📱 Target IP:', piIPAddress);
    
    if (!validateIPAddress(piIPAddress)) {
      Alert.alert('Invalid IP', 'Please enter a valid IP address');
      console.log('❌ Data collection failed - Invalid IP address');
      return;
    }
    
    console.log('✅ IP address validated');
    console.log('🚀 Starting IoT sensor data collection...');
    
    setIsCollecting(true);
    setTransmissionCount(0);
    
    console.log('📊 Device ID:', deviceId);
    console.log('🎯 Destination: http://' + piIPAddress + ':5000/sensor_data');
    
    await startSensorCollection();
    startDataTransmission();
    
    console.log('🎉 DATA COLLECTION STARTED SUCCESSFULLY!');
    console.log('=' .repeat(50));
  };

  const stopDataCollection = () => {
    console.log('🛑 STOP DATA COLLECTION INITIATED');
    
    setIsCollecting(false);
    setConnectionStatus('disconnected');
    stopSensorCollection();
    stopDataTransmission();
    sensorDataBuffer.current = [];
    
    console.log('🎉 DATA COLLECTION STOPPED SUCCESSFULLY!');
    console.log('📊 Final transmission count:', transmissionCount);
    console.log('=' .repeat(50));
  };

  const getConnectionStatusColor = () => {
    switch (connectionStatus) {
      case 'connected': return '#4CAF50';
      case 'error': return '#F44336';
      default: return '#9E9E9E';
    }
  };

  const formatNumber = (num: number): string => {
    return num.toFixed(3);
  };

  return (
    <SafeAreaView style={styles.container}>
      <StatusBar style="auto" />
      <ScrollView contentContainerStyle={styles.scrollContainer}>
        
        {/* Header */}
        <View style={styles.header}>
          <Text style={styles.title}>IoT Sensor Data Collector</Text>
          <View style={styles.statusContainer}>
            <View style={[styles.statusDot, { backgroundColor: getConnectionStatusColor() }]} />
            <Text style={styles.statusText}>
              {connectionStatus === 'connected' ? 'Connected' : 
               connectionStatus === 'error' ? 'Error' : 'Disconnected'}
            </Text>
          </View>
        </View>

        {/* IP Address Input */}
        <View style={styles.inputContainer}>
          <Text style={styles.label}>Raspberry Pi IP Address:</Text>
          <TextInput
            style={styles.input}
            value={piIPAddress}
            onChangeText={setPiIPAddress}
            placeholder="192.168.1.100"
            keyboardType="numeric"
            editable={!isCollecting}
          />
        </View>

        {/* Control Buttons */}
        <View style={styles.buttonContainer}>
          <TouchableOpacity
            style={[styles.button, isCollecting ? styles.stopButton : styles.startButton]}
            onPress={isCollecting ? stopDataCollection : startDataCollection}
          >
            <Text style={styles.buttonText}>
              {isCollecting ? 'STOP COLLECTION' : 'START COLLECTION'}
            </Text>
          </TouchableOpacity>
        </View>

        {/* Stats */}
        <View style={styles.statsContainer}>
          <View style={styles.statItem}>
            <Text style={styles.statLabel}>Transmissions:</Text>
            <Text style={styles.statValue}>{transmissionCount}</Text>
          </View>
          <View style={styles.statItem}>
            <Text style={styles.statLabel}>Last Sent:</Text>
            <Text style={styles.statValue}>{lastTransmissionTime}</Text>
          </View>
          <View style={styles.statItem}>
            <Text style={styles.statLabel}>Activity:</Text>
            <Text style={[styles.statValue, styles.activityText]}>{currentActivity}</Text>
          </View>
        </View>

        {/* Sensor Data Display */}
        <View style={styles.sensorContainer}>
          <Text style={styles.sensorTitle}>Real-time Sensor Data</Text>
          
          {/* Accelerometer */}
          <View style={styles.sensorSection}>
            <Text style={styles.sensorLabel}>Accelerometer (m/s²):</Text>
            <View style={styles.sensorData}>
              <Text style={styles.sensorValue}>X: {formatNumber(accelerometerData.x)}</Text>
              <Text style={styles.sensorValue}>Y: {formatNumber(accelerometerData.y)}</Text>
              <Text style={styles.sensorValue}>Z: {formatNumber(accelerometerData.z)}</Text>
            </View>
          </View>

          {/* Gyroscope */}
          <View style={styles.sensorSection}>
            <Text style={styles.sensorLabel}>Gyroscope (rad/s):</Text>
            <View style={styles.sensorData}>
              <Text style={styles.sensorValue}>X: {formatNumber(gyroscopeData.x)}</Text>
              <Text style={styles.sensorValue}>Y: {formatNumber(gyroscopeData.y)}</Text>
              <Text style={styles.sensorValue}>Z: {formatNumber(gyroscopeData.z)}</Text>
            </View>
          </View>

          {/* Location */}
          <View style={styles.sensorSection}>
            <Text style={styles.sensorLabel}>GPS Location:</Text>
            <View style={styles.sensorData}>
              <Text style={styles.sensorValue}>Lat: {formatNumber(locationData.latitude)}</Text>
              <Text style={styles.sensorValue}>Lng: {formatNumber(locationData.longitude)}</Text>
              <Text style={styles.sensorValue}>
                Alt: {locationData.altitude ? formatNumber(locationData.altitude) : 'N/A'}m
              </Text>
              <Text style={styles.sensorValue}>
                Speed: {locationData.speed ? formatNumber(locationData.speed) : '0'} m/s
              </Text>
            </View>
          </View>

          {/* Device Info */}
          <View style={styles.sensorSection}>
            <Text style={styles.sensorLabel}>Device ID:</Text>
            <Text style={styles.deviceId}>{deviceId}</Text>
          </View>
        </View>

      </ScrollView>
    </SafeAreaView>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#f5f5f5',
  },
  scrollContainer: {
    padding: 20,
  },
  header: {
    alignItems: 'center',
    marginBottom: 30,
  },
  title: {
    fontSize: 24,
    fontWeight: 'bold',
    color: '#333',
    marginBottom: 10,
  },
  statusContainer: {
    flexDirection: 'row',
    alignItems: 'center',
  },
  statusDot: {
    width: 12,
    height: 12,
    borderRadius: 6,
    marginRight: 8,
  },
  statusText: {
    fontSize: 16,
    color: '#666',
  },
  inputContainer: {
    marginBottom: 20,
  },
  label: {
    fontSize: 16,
    fontWeight: '600',
    color: '#333',
    marginBottom: 8,
  },
  input: {
    backgroundColor: '#fff',
    borderRadius: 10,
    padding: 15,
    fontSize: 16,
    borderWidth: 1,
    borderColor: '#ddd',
  },
  buttonContainer: {
    marginBottom: 30,
  },
  button: {
    borderRadius: 25,
    padding: 20,
    alignItems: 'center',
    elevation: 3,
    shadowOffset: { width: 0, height: 2 },
    shadowOpacity: 0.2,
    shadowRadius: 4,
  },
  startButton: {
    backgroundColor: '#4CAF50',
  },
  stopButton: {
    backgroundColor: '#F44336',
  },
  buttonText: {
    color: '#fff',
    fontSize: 18,
    fontWeight: 'bold',
  },
  statsContainer: {
    backgroundColor: '#fff',
    borderRadius: 15,
    padding: 20,
    marginBottom: 20,
    elevation: 2,
    shadowOffset: { width: 0, height: 2 },
    shadowOpacity: 0.1,
    shadowRadius: 4,
  },
  statItem: {
    flexDirection: 'row',
    justifyContent: 'space-between',
    marginBottom: 10,
  },
  statLabel: {
    fontSize: 16,
    color: '#666',
  },
  statValue: {
    fontSize: 16,
    fontWeight: '600',
    color: '#333',
  },
  activityText: {
    color: '#2196F3',
    textTransform: 'capitalize',
  },
  sensorContainer: {
    backgroundColor: '#fff',
    borderRadius: 15,
    padding: 20,
    elevation: 2,
    shadowOffset: { width: 0, height: 2 },
    shadowOpacity: 0.1,
    shadowRadius: 4,
  },
  sensorTitle: {
    fontSize: 20,
    fontWeight: 'bold',
    color: '#333',
    marginBottom: 20,
    textAlign: 'center',
  },
  sensorSection: {
    marginBottom: 20,
  },
  sensorLabel: {
    fontSize: 16,
    fontWeight: '600',
    color: '#444',
    marginBottom: 8,
  },
  sensorData: {
    flexDirection: 'row',
    flexWrap: 'wrap',
    justifyContent: 'space-between',
  },
  sensorValue: {
    fontSize: 14,
    color: '#666',
    backgroundColor: '#f8f8f8',
    padding: 8,
    borderRadius: 8,
    marginBottom: 5,
    minWidth: '30%',
    textAlign: 'center',
  },
  deviceId: {
    fontSize: 12,
    color: '#888',
    backgroundColor: '#f8f8f8',
    padding: 10,
    borderRadius: 8,
    textAlign: 'center',
  },
});
</file>

<file path="index.ts">
import { registerRootComponent } from 'expo';

import App from './App';

// registerRootComponent calls AppRegistry.registerComponent('main', () => App);
// It also ensures that whether you load the app in Expo Go or in a native build,
// the environment is set up appropriately
registerRootComponent(App);
</file>

<file path="package.json">
{
  "name": "iotsensorapp",
  "version": "1.0.0",
  "main": "index.ts",
  "scripts": {
    "start": "expo start",
    "android": "expo start --android",
    "ios": "expo start --ios",
    "web": "expo start --web"
  },
  "dependencies": {
    "axios": "^1.9.0",
    "expo": "~53.0.10",
    "expo-device": "^7.1.4",
    "expo-location": "^18.1.5",
    "expo-sensors": "^14.1.4",
    "expo-status-bar": "~2.2.3",
    "react": "19.0.0",
    "react-native": "0.79.3"
  },
  "devDependencies": {
    "@babel/core": "^7.25.2",
    "@types/react": "~19.0.10",
    "typescript": "~5.8.3"
  },
  "private": true
}
</file>

<file path="tsconfig.json">
{
  "extends": "expo/tsconfig.base",
  "compilerOptions": {
    "strict": true
  }
}
</file>

</files>
````

## File: repomix.config.json
````json
{
  "output": {
    "filePath": "repomix-output.md",
    "style": "markdown",
    "parsableStyle": false,
    "fileSummary": true,
    "directoryStructure": true,
    "removeComments": false,
    "removeEmptyLines": false,
    "compress": false,
    "topFilesLength": 5,
    "showLineNumbers": false,
    "copyToClipboard": false,
    "git": {
      "sortByChanges": true,
      "sortByChangesMaxCommits": 100
    }
  },
  "include": [],
  "ignore": {
    "useGitignore": true,
    "useDefaultPatterns": true,
    "customPatterns": []
  },
  "security": {
    "enableSecurityCheck": true
  },
  "tokenCount": {
    "encoding": "o200k_base"
  }
}
````

## File: test_server.py
````python
#!/usr/bin/env python3
"""
Test script to verify the Raspberry Pi server is working correctly.
Sends sample sensor data to test the server endpoints.

Usage:
python3 test_server.py [server_ip]

If no IP is provided, defaults to localhost (127.0.0.1)
"""

import requests
import json
import sys
from datetime import datetime
import time

def test_server(server_ip="127.0.0.1", port=5000):
    """Test the sensor data server"""
    base_url = f"http://{server_ip}:{port}"
    
    print(f"Testing IoT Sensor Data Server at {base_url}")
    print("=" * 50)
    
    # Test 1: Health Check
    print("1. Testing health endpoint...")
    try:
        response = requests.get(f"{base_url}/health", timeout=5)
        if response.status_code == 200:
            print("✅ Health check passed")
            print(f"   Response: {response.json()}")
        else:
            print(f"❌ Health check failed with status {response.status_code}")
    except Exception as e:
        print(f"❌ Health check failed: {e}")
        return False
    
    # Test 2: Send sample sensor data
    print("\n2. Testing sensor data endpoint...")
    sample_data = {
        "timestamp": datetime.now().isoformat() + "Z",
        "accelerometer": {"x": 0.1, "y": 0.2, "z": 9.8},
        "gyroscope": {"x": 0.01, "y": 0.02, "z": 0.03},
        "location": {"latitude": 40.7128, "longitude": -74.0060, "altitude": 10, "speed": 0},
        "deviceId": "TestDevice_12345"
    }
    
    try:
        response = requests.post(
            f"{base_url}/sensor_data",
            json=sample_data,
            headers={"Content-Type": "application/json"},
            timeout=5
        )
        if response.status_code == 200:
            print("✅ Sensor data submission passed")
            print(f"   Response: {response.json()}")
        else:
            print(f"❌ Sensor data submission failed with status {response.status_code}")
            print(f"   Response: {response.text}")
    except Exception as e:
        print(f"❌ Sensor data submission failed: {e}")
        return False
    
    # Test 3: Get recent data
    print("\n3. Testing recent data endpoint...")
    try:
        response = requests.get(f"{base_url}/recent_data?limit=5", timeout=5)
        if response.status_code == 200:
            data = response.json()
            print("✅ Recent data retrieval passed")
            print(f"   Total readings: {data['total_count']}")
            print(f"   Returned readings: {data['returned_count']}")
        else:
            print(f"❌ Recent data retrieval failed with status {response.status_code}")
    except Exception as e:
        print(f"❌ Recent data retrieval failed: {e}")
    
    # Test 4: Get statistics
    print("\n4. Testing statistics endpoint...")
    try:
        response = requests.get(f"{base_url}/stats", timeout=5)
        if response.status_code == 200:
            stats = response.json()
            print("✅ Statistics retrieval passed")
            print(f"   Total readings: {stats['total_readings']}")
            print(f"   Devices: {stats['devices']}")
            print(f"   Latest timestamp: {stats['latest_timestamp']}")
        else:
            print(f"❌ Statistics retrieval failed with status {response.status_code}")
    except Exception as e:
        print(f"❌ Statistics retrieval failed: {e}")
    
    # Test 5: Send multiple data points
    print("\n5. Testing multiple data submissions...")
    for i in range(3):
        test_data = {
            "timestamp": datetime.now().isoformat() + "Z",
            "accelerometer": {"x": 0.1 + i * 0.1, "y": 0.2 + i * 0.1, "z": 9.8 + i * 0.1},
            "gyroscope": {"x": 0.01 + i * 0.01, "y": 0.02 + i * 0.01, "z": 0.03 + i * 0.01},
            "location": {"latitude": 40.7128 + i * 0.001, "longitude": -74.0060 + i * 0.001, "altitude": 10 + i, "speed": i},
            "deviceId": f"TestDevice_{12345 + i}"
        }
        
        try:
            response = requests.post(f"{base_url}/sensor_data", json=test_data, timeout=5)
            if response.status_code == 200:
                print(f"✅ Data point {i+1} submitted successfully")
            else:
                print(f"❌ Data point {i+1} failed with status {response.status_code}")
        except Exception as e:
            print(f"❌ Data point {i+1} failed: {e}")
        
        time.sleep(0.5)  # Small delay between submissions
    
    print("\n" + "=" * 50)
    print("🎉 Server testing completed!")
    print(f"📊 Access web interface at: {base_url}/")
    return True

def main():
    """Main function"""
    if len(sys.argv) > 1:
        server_ip = sys.argv[1]
    else:
        server_ip = "127.0.0.1"
    
    print("IoT Sensor Data Server Test Script")
    print("=" * 50)
    print(f"Target server: {server_ip}:5000")
    print("Make sure the server is running before starting this test!")
    print("")
    
    # Wait for user confirmation
    input("Press Enter to start testing...")
    
    test_server(server_ip)

if __name__ == "__main__":
    main()
````

## File: .gitignore
````
# Learn more https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files

# dependencies
node_modules/

# Expo
.expo/
dist/
web-build/
expo-env.d.ts

# Native
.kotlin/
*.orig.*
*.jks
*.p8
*.p12
*.key
*.mobileprovision

# Metro
.metro-health-check*

# debug
npm-debug.*
yarn-debug.*
yarn-error.*

# macOS
.DS_Store
*.pem

# local env files
.env*.local

# typescript
*.tsbuildinfo
````

## File: app.json
````json
{
  "expo": {
    "name": "IoTSensorApp",
    "slug": "IoTSensorApp",
    "version": "1.0.0",
    "orientation": "portrait",
    "icon": "./assets/icon.png",
    "userInterfaceStyle": "light",
    "newArchEnabled": true,
    "splash": {
      "image": "./assets/splash-icon.png",
      "resizeMode": "contain",
      "backgroundColor": "#ffffff"
    },
    "ios": {
      "supportsTablet": true,
      "infoPlist": {
        "NSLocationWhenInUseUsageDescription": "This app needs access to location for GPS tracking and IoT data collection.",
        "NSLocationAlwaysAndWhenInUseUsageDescription": "This app needs access to location for GPS tracking and IoT data collection.",
        "NSMotionUsageDescription": "This app needs access to motion sensors for accelerometer and gyroscope data collection."
      }
    },
    "android": {
      "adaptiveIcon": {
        "foregroundImage": "./assets/adaptive-icon.png",
        "backgroundColor": "#ffffff"
      },
      "edgeToEdgeEnabled": true,
      "permissions": [
        "ACCESS_FINE_LOCATION",
        "ACCESS_COARSE_LOCATION",
        "BODY_SENSORS",
        "INTERNET",
        "ACCESS_NETWORK_STATE"
      ]
    },
    "web": {
      "favicon": "./assets/favicon.png"
    }
  }
}
````

## File: App.tsx
````typescript
import React, { useState, useEffect, useRef } from 'react';
import {
  StyleSheet,
  Text,
  View,
  TextInput,
  TouchableOpacity,
  Alert,
  ScrollView,
  SafeAreaView,
  Platform,
} from 'react-native';
import { StatusBar } from 'expo-status-bar';
import { Accelerometer, Gyroscope } from 'expo-sensors';
import * as Location from 'expo-location';
import * as Device from 'expo-device';
import axios from 'axios';

interface SensorData {
  timestamp: string;
  accelerometer: { x: number; y: number; z: number };
  gyroscope: { x: number; y: number; z: number };
  location: { latitude: number; longitude: number; altitude: number | null; speed: number | null };
  deviceId: string;
}

interface AccelerometerData {
  x: number;
  y: number;
  z: number;
}

interface GyroscopeData {
  x: number;
  y: number;
  z: number;
}

export default function App() {
  // State variables
  const [piIPAddress, setPiIPAddress] = useState('192.168.1.100');
  const [isCollecting, setIsCollecting] = useState(false);
  const [connectionStatus, setConnectionStatus] = useState<'disconnected' | 'connected' | 'error'>('disconnected');
  const [transmissionCount, setTransmissionCount] = useState(0);
  const [lastTransmissionTime, setLastTransmissionTime] = useState<string>('Never');
  const [currentActivity, setCurrentActivity] = useState<string>('stationary');
  
  // Sensor data states
  const [accelerometerData, setAccelerometerData] = useState<AccelerometerData>({ x: 0, y: 0, z: 0 });
  const [gyroscopeData, setGyroscopeData] = useState<GyroscopeData>({ x: 0, y: 0, z: 0 });
  const [locationData, setLocationData] = useState({ latitude: 0, longitude: 0, altitude: null, speed: null });
  const [deviceId, setDeviceId] = useState<string>('');

  // Refs for subscriptions and intervals
  const accelerometerSubscription = useRef<any>(null);
  const gyroscopeSubscription = useRef<any>(null);
  const locationSubscription = useRef<any>(null);
  const transmissionInterval = useRef<any>(null);
  const sensorDataBuffer = useRef<SensorData[]>([]);

  // Initialize device ID and request permissions
  useEffect(() => {
    initializeApp();
    return () => {
      cleanup();
    };
  }, []);

  const initializeApp = async () => {
    console.log('🚀 Initializing IoT Sensor App...');
    
    // Get device ID
    const deviceName = Device.deviceName || 'Unknown';
    const brand = Device.brand || 'Unknown';
    const generatedDeviceId = `${brand}_${deviceName}_${Math.random().toString(36).substr(2, 9)}`;
    setDeviceId(generatedDeviceId);
    
    console.log('📱 Device Info:', {
      deviceName: deviceName,
      brand: brand,
      deviceId: generatedDeviceId,
      platform: Platform.OS
    });

    // Request location permissions
    console.log('🔐 Requesting location permissions...');
    const { status } = await Location.requestForegroundPermissionsAsync();
    if (status !== 'granted') {
      Alert.alert('Permission Denied', 'Location permission is required for GPS tracking');
      console.log('❌ Location permission denied');
    } else {
      console.log('✅ Location permission granted');
    }
    
    console.log('🎉 App initialization complete!');
  };

  const cleanup = () => {
    stopDataCollection();
  };

  const validateIPAddress = (ip: string): boolean => {
    const ipRegex = /^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/;
    return ipRegex.test(ip);
  };

  const determineActivity = (accel: AccelerometerData, gyro: GyroscopeData, speed: number | null): string => {
    const accelMagnitude = Math.sqrt(accel.x ** 2 + accel.y ** 2 + accel.z ** 2);
    const gyroMagnitude = Math.sqrt(gyro.x ** 2 + gyro.y ** 2 + gyro.z ** 2);
    
    if (speed && speed > 10) {
      return 'driving';
    } else if (speed && speed > 2) {
      return 'running';
    } else if (accelMagnitude > 10.5 || gyroMagnitude > 0.5) {
      return 'walking';
    } else {
      return 'stationary';
    }
  };

  const startSensorCollection = async () => {
    console.log('🚀 Starting sensor collection...');
    
    // Set update intervals
    Accelerometer.setUpdateInterval(100); // 100ms
    Gyroscope.setUpdateInterval(100); // 100ms
    
    console.log('📱 Sensor update intervals set: Accelerometer & Gyroscope = 100ms');

    // Start accelerometer
    accelerometerSubscription.current = Accelerometer.addListener((data) => {
      setAccelerometerData(data);
      console.log('📊 Accelerometer data:', {
        x: data.x.toFixed(3),
        y: data.y.toFixed(3),
        z: data.z.toFixed(3)
      });
    });

    // Start gyroscope
    gyroscopeSubscription.current = Gyroscope.addListener((data) => {
      setGyroscopeData(data);
      console.log('🌀 Gyroscope data:', {
        x: data.x.toFixed(3),
        y: data.y.toFixed(3),
        z: data.z.toFixed(3)
      });
    });

    console.log('✅ Accelerometer and Gyroscope listeners started');

    // Start location tracking
    try {
      console.log('🌍 Starting GPS location tracking...');
      locationSubscription.current = await Location.watchPositionAsync(
        {
          accuracy: Location.Accuracy.High,
          timeInterval: 2000, // 2 seconds
          distanceInterval: 1,
        },
        (location) => {
          const locationInfo = {
            latitude: location.coords.latitude,
            longitude: location.coords.longitude,
            altitude: location.coords.altitude,
            speed: location.coords.speed,
          };
          setLocationData(locationInfo);
          console.log('📍 GPS location update:', {
            latitude: locationInfo.latitude.toFixed(6),
            longitude: locationInfo.longitude.toFixed(6),
            altitude: locationInfo.altitude?.toFixed(2) || 'N/A',
            speed: locationInfo.speed?.toFixed(2) || 'N/A'
          });
        }
      );
      console.log('✅ GPS location tracking started');
    } catch (error) {
      console.error('❌ Error starting location tracking:', error);
    }
  };

  const stopSensorCollection = () => {
    console.log('🛑 Stopping sensor collection...');
    
    if (accelerometerSubscription.current) {
      accelerometerSubscription.current.remove();
      accelerometerSubscription.current = null;
      console.log('📊 Accelerometer listener stopped');
    }
    if (gyroscopeSubscription.current) {
      gyroscopeSubscription.current.remove();
      gyroscopeSubscription.current = null;
      console.log('🌀 Gyroscope listener stopped');
    }
    if (locationSubscription.current && locationSubscription.current.remove) {
      locationSubscription.current.remove();
      locationSubscription.current = null;
      console.log('📍 GPS location tracking stopped');
    }
    
    console.log('✅ All sensors stopped successfully');
  };

  const startDataTransmission = () => {
    console.log('🔄 Starting data transmission to Pi (every 1.5 seconds)...');
    
    transmissionInterval.current = setInterval(() => {
      if (sensorDataBuffer.current.length > 0) {
        console.log('📤 Sending buffered sensor data...');
        sendDataToPi();
      } else {
        // Create current sensor reading
        const currentReading: SensorData = {
          timestamp: new Date().toISOString(),
          accelerometer: accelerometerData,
          gyroscope: gyroscopeData,
          location: locationData,
          deviceId: deviceId,
        };
        
        // Update activity based on current data
        const activity = determineActivity(accelerometerData, gyroscopeData, locationData.speed);
        setCurrentActivity(activity);
        
        console.log('📊 Created new sensor reading:', {
          timestamp: currentReading.timestamp,
          activity: activity,
          hasLocation: !!(locationData.latitude && locationData.longitude)
        });
        
        sensorDataBuffer.current = [currentReading];
        sendDataToPi();
      }
    }, 1500); // Send every 1.5 seconds
    
    console.log('✅ Data transmission timer started');
  };

  const stopDataTransmission = () => {
    console.log('🔄 Stopping data transmission...');
    
    if (transmissionInterval.current) {
      clearInterval(transmissionInterval.current);
      transmissionInterval.current = null;
      console.log('✅ Data transmission timer stopped');
    }
  };

  const sendDataToPi = async () => {
    if (!validateIPAddress(piIPAddress)) {
      setConnectionStatus('error');
      Alert.alert('Invalid IP', 'Please enter a valid IP address');
      console.log('❌ Invalid IP address:', piIPAddress);
      return;
    }

    try {
      const url = `http://${piIPAddress}:5000/sensor_data`;
      const dataToSend = sensorDataBuffer.current[0]; // Send latest reading
      
      console.log('📡 Sending data to Pi:', {
        url: url,
        timestamp: dataToSend.timestamp,
        deviceId: dataToSend.deviceId,
        accelerometer: {
          x: dataToSend.accelerometer.x.toFixed(3),
          y: dataToSend.accelerometer.y.toFixed(3),
          z: dataToSend.accelerometer.z.toFixed(3)
        },
        gyroscope: {
          x: dataToSend.gyroscope.x.toFixed(3),
          y: dataToSend.gyroscope.y.toFixed(3),
          z: dataToSend.gyroscope.z.toFixed(3)
        },
        location: {
          latitude: dataToSend.location.latitude?.toFixed(6),
          longitude: dataToSend.location.longitude?.toFixed(6),
          altitude: dataToSend.location.altitude?.toFixed(2),
          speed: dataToSend.location.speed?.toFixed(2)
        }
      });
      
      const response = await axios.post(url, dataToSend, {
        timeout: 5000,
        headers: {
          'Content-Type': 'application/json',
        },
      });

      if (response.status === 200) {
        setConnectionStatus('connected');
        setTransmissionCount(prev => prev + 1);
        setLastTransmissionTime(new Date().toLocaleTimeString());
        sensorDataBuffer.current = [];
        
        console.log('✅ Data sent successfully!', {
          status: response.status,
          transmissionCount: transmissionCount + 1,
          responseData: response.data,
          timestamp: new Date().toLocaleTimeString()
        });
      }
    } catch (error) {
      setConnectionStatus('error');
      console.error('❌ Error sending data to Pi:', {
        error: error.message,
        code: error.code,
        url: `http://${piIPAddress}:5000/sensor_data`,
        timestamp: new Date().toLocaleTimeString()
      });
    }
  };

  const startDataCollection = async () => {
    console.log('🎯 START DATA COLLECTION INITIATED');
    console.log('📱 Target IP:', piIPAddress);
    
    if (!validateIPAddress(piIPAddress)) {
      Alert.alert('Invalid IP', 'Please enter a valid IP address');
      console.log('❌ Data collection failed - Invalid IP address');
      return;
    }
    
    console.log('✅ IP address validated');
    console.log('🚀 Starting IoT sensor data collection...');
    
    setIsCollecting(true);
    setTransmissionCount(0);
    
    console.log('📊 Device ID:', deviceId);
    console.log('🎯 Destination: http://' + piIPAddress + ':5000/sensor_data');
    
    await startSensorCollection();
    startDataTransmission();
    
    console.log('🎉 DATA COLLECTION STARTED SUCCESSFULLY!');
    console.log('=' .repeat(50));
  };

  const stopDataCollection = () => {
    console.log('🛑 STOP DATA COLLECTION INITIATED');
    
    setIsCollecting(false);
    setConnectionStatus('disconnected');
    stopSensorCollection();
    stopDataTransmission();
    sensorDataBuffer.current = [];
    
    console.log('🎉 DATA COLLECTION STOPPED SUCCESSFULLY!');
    console.log('📊 Final transmission count:', transmissionCount);
    console.log('=' .repeat(50));
  };

  const getConnectionStatusColor = () => {
    switch (connectionStatus) {
      case 'connected': return '#4CAF50';
      case 'error': return '#F44336';
      default: return '#9E9E9E';
    }
  };

  const formatNumber = (num: number): string => {
    return num.toFixed(3);
  };

  return (
    <SafeAreaView style={styles.container}>
      <StatusBar style="auto" />
      <ScrollView contentContainerStyle={styles.scrollContainer}>
        
        {/* Header */}
        <View style={styles.header}>
          <Text style={styles.title}>IoT Sensor Data Collector</Text>
          <View style={styles.statusContainer}>
            <View style={[styles.statusDot, { backgroundColor: getConnectionStatusColor() }]} />
            <Text style={styles.statusText}>
              {connectionStatus === 'connected' ? 'Connected' : 
               connectionStatus === 'error' ? 'Error' : 'Disconnected'}
            </Text>
          </View>
        </View>

        {/* IP Address Input */}
        <View style={styles.inputContainer}>
          <Text style={styles.label}>Raspberry Pi IP Address:</Text>
          <TextInput
            style={styles.input}
            value={piIPAddress}
            onChangeText={setPiIPAddress}
            placeholder="192.168.1.100"
            keyboardType="numeric"
            editable={!isCollecting}
          />
        </View>

        {/* Control Buttons */}
        <View style={styles.buttonContainer}>
          <TouchableOpacity
            style={[styles.button, isCollecting ? styles.stopButton : styles.startButton]}
            onPress={isCollecting ? stopDataCollection : startDataCollection}
          >
            <Text style={styles.buttonText}>
              {isCollecting ? 'STOP COLLECTION' : 'START COLLECTION'}
            </Text>
          </TouchableOpacity>
        </View>

        {/* Stats */}
        <View style={styles.statsContainer}>
          <View style={styles.statItem}>
            <Text style={styles.statLabel}>Transmissions:</Text>
            <Text style={styles.statValue}>{transmissionCount}</Text>
          </View>
          <View style={styles.statItem}>
            <Text style={styles.statLabel}>Last Sent:</Text>
            <Text style={styles.statValue}>{lastTransmissionTime}</Text>
          </View>
          <View style={styles.statItem}>
            <Text style={styles.statLabel}>Activity:</Text>
            <Text style={[styles.statValue, styles.activityText]}>{currentActivity}</Text>
          </View>
        </View>

        {/* Sensor Data Display */}
        <View style={styles.sensorContainer}>
          <Text style={styles.sensorTitle}>Real-time Sensor Data</Text>
          
          {/* Accelerometer */}
          <View style={styles.sensorSection}>
            <Text style={styles.sensorLabel}>Accelerometer (m/s²):</Text>
            <View style={styles.sensorData}>
              <Text style={styles.sensorValue}>X: {formatNumber(accelerometerData.x)}</Text>
              <Text style={styles.sensorValue}>Y: {formatNumber(accelerometerData.y)}</Text>
              <Text style={styles.sensorValue}>Z: {formatNumber(accelerometerData.z)}</Text>
            </View>
          </View>

          {/* Gyroscope */}
          <View style={styles.sensorSection}>
            <Text style={styles.sensorLabel}>Gyroscope (rad/s):</Text>
            <View style={styles.sensorData}>
              <Text style={styles.sensorValue}>X: {formatNumber(gyroscopeData.x)}</Text>
              <Text style={styles.sensorValue}>Y: {formatNumber(gyroscopeData.y)}</Text>
              <Text style={styles.sensorValue}>Z: {formatNumber(gyroscopeData.z)}</Text>
            </View>
          </View>

          {/* Location */}
          <View style={styles.sensorSection}>
            <Text style={styles.sensorLabel}>GPS Location:</Text>
            <View style={styles.sensorData}>
              <Text style={styles.sensorValue}>Lat: {formatNumber(locationData.latitude)}</Text>
              <Text style={styles.sensorValue}>Lng: {formatNumber(locationData.longitude)}</Text>
              <Text style={styles.sensorValue}>
                Alt: {locationData.altitude ? formatNumber(locationData.altitude) : 'N/A'}m
              </Text>
              <Text style={styles.sensorValue}>
                Speed: {locationData.speed ? formatNumber(locationData.speed) : '0'} m/s
              </Text>
            </View>
          </View>

          {/* Device Info */}
          <View style={styles.sensorSection}>
            <Text style={styles.sensorLabel}>Device ID:</Text>
            <Text style={styles.deviceId}>{deviceId}</Text>
          </View>
        </View>

      </ScrollView>
    </SafeAreaView>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#f5f5f5',
  },
  scrollContainer: {
    padding: 20,
  },
  header: {
    alignItems: 'center',
    marginBottom: 30,
  },
  title: {
    fontSize: 24,
    fontWeight: 'bold',
    color: '#333',
    marginBottom: 10,
  },
  statusContainer: {
    flexDirection: 'row',
    alignItems: 'center',
  },
  statusDot: {
    width: 12,
    height: 12,
    borderRadius: 6,
    marginRight: 8,
  },
  statusText: {
    fontSize: 16,
    color: '#666',
  },
  inputContainer: {
    marginBottom: 20,
  },
  label: {
    fontSize: 16,
    fontWeight: '600',
    color: '#333',
    marginBottom: 8,
  },
  input: {
    backgroundColor: '#fff',
    borderRadius: 10,
    padding: 15,
    fontSize: 16,
    borderWidth: 1,
    borderColor: '#ddd',
  },
  buttonContainer: {
    marginBottom: 30,
  },
  button: {
    borderRadius: 25,
    padding: 20,
    alignItems: 'center',
    elevation: 3,
    shadowOffset: { width: 0, height: 2 },
    shadowOpacity: 0.2,
    shadowRadius: 4,
  },
  startButton: {
    backgroundColor: '#4CAF50',
  },
  stopButton: {
    backgroundColor: '#F44336',
  },
  buttonText: {
    color: '#fff',
    fontSize: 18,
    fontWeight: 'bold',
  },
  statsContainer: {
    backgroundColor: '#fff',
    borderRadius: 15,
    padding: 20,
    marginBottom: 20,
    elevation: 2,
    shadowOffset: { width: 0, height: 2 },
    shadowOpacity: 0.1,
    shadowRadius: 4,
  },
  statItem: {
    flexDirection: 'row',
    justifyContent: 'space-between',
    marginBottom: 10,
  },
  statLabel: {
    fontSize: 16,
    color: '#666',
  },
  statValue: {
    fontSize: 16,
    fontWeight: '600',
    color: '#333',
  },
  activityText: {
    color: '#2196F3',
    textTransform: 'capitalize',
  },
  sensorContainer: {
    backgroundColor: '#fff',
    borderRadius: 15,
    padding: 20,
    elevation: 2,
    shadowOffset: { width: 0, height: 2 },
    shadowOpacity: 0.1,
    shadowRadius: 4,
  },
  sensorTitle: {
    fontSize: 20,
    fontWeight: 'bold',
    color: '#333',
    marginBottom: 20,
    textAlign: 'center',
  },
  sensorSection: {
    marginBottom: 20,
  },
  sensorLabel: {
    fontSize: 16,
    fontWeight: '600',
    color: '#444',
    marginBottom: 8,
  },
  sensorData: {
    flexDirection: 'row',
    flexWrap: 'wrap',
    justifyContent: 'space-between',
  },
  sensorValue: {
    fontSize: 14,
    color: '#666',
    backgroundColor: '#f8f8f8',
    padding: 8,
    borderRadius: 8,
    marginBottom: 5,
    minWidth: '30%',
    textAlign: 'center',
  },
  deviceId: {
    fontSize: 12,
    color: '#888',
    backgroundColor: '#f8f8f8',
    padding: 10,
    borderRadius: 8,
    textAlign: 'center',
  },
});
````

## File: index.ts
````typescript
import { registerRootComponent } from 'expo';

import App from './App';

// registerRootComponent calls AppRegistry.registerComponent('main', () => App);
// It also ensures that whether you load the app in Expo Go or in a native build,
// the environment is set up appropriately
registerRootComponent(App);
````

## File: package.json
````json
{
  "name": "iotsensorapp",
  "version": "1.0.0",
  "main": "index.ts",
  "scripts": {
    "start": "expo start",
    "android": "expo start --android",
    "ios": "expo start --ios",
    "web": "expo start --web"
  },
  "dependencies": {
    "axios": "^1.9.0",
    "expo": "~53.0.10",
    "expo-device": "^7.1.4",
    "expo-location": "^18.1.5",
    "expo-sensors": "^14.1.4",
    "expo-status-bar": "~2.2.3",
    "react": "19.0.0",
    "react-native": "0.79.3"
  },
  "devDependencies": {
    "@babel/core": "^7.25.2",
    "@types/react": "~19.0.10",
    "typescript": "~5.8.3"
  },
  "private": true
}
````

## File: tsconfig.json
````json
{
  "extends": "expo/tsconfig.base",
  "compilerOptions": {
    "strict": true
  }
}
````
