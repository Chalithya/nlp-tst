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
database/generated_resumes.sql
package.json
repomix.config.json
src/app.js
src/config/ai.js
src/config/apiVersioning.js
src/config/cache.js
src/config/database.js
src/config/environment.js
src/config/logger.js
src/controllers/BaseController.js
src/controllers/ControllerFactory.js
src/controllers/index.js
src/controllers/ResumeController.js
src/controllers/UserController.js
src/middleware/authMiddleware.js
src/middleware/cacheMiddleware.js
src/middleware/errorHandler.js
src/middleware/rateLimiter.js
src/middleware/routePerformance.js
src/middleware/securityMiddleware.js
src/middleware/validation.js
src/models/schemas/careerSchemas.js
src/models/schemas/index.js
src/models/schemas/resumeSchemas.js
src/models/schemas/userSchemas.js
src/prompts/career.js
src/prompts/index.js
src/prompts/jobs.js
src/prompts/resume.js
src/prompts/resumeGenerator.js
src/repositories/BaseRepository.js
src/repositories/CareerProfileRepository.js
src/repositories/GeneratedResumeRepository.js
src/repositories/index.js
src/repositories/ResumeRepository.js
src/repositories/UserRepository.js
src/routes/__tests__/authRoutes.test.js
src/routes/aiRoutesLocal.js
src/routes/ApiRouter.js
src/routes/authRoutes.js
src/routes/careerRoutes.js
src/routes/monitoringRoutes.js
src/routes/RouteFactory.js
src/routes/v1/aiRoutes.js
src/routes/v1/authRoutes.js
src/routes/v1/careerRoutes.js
src/routes/v1/index.js
src/routes/v1/resumeRoutes.js
src/routes/v1/userRoutes.js
src/server.js
src/services/aiConfig.js
src/services/BaseService.js
src/services/CanadianResumeService.js
src/services/CareerProfileService.js
src/services/documentProcessor.js
src/services/GeminiResumeService.js
src/services/googleAiService.js
src/services/GoogleJobsService.js
src/services/index.js
src/services/ResumeService.js
src/services/ServiceFactory.js
src/services/supabaseDatabase.js
src/services/UserService.js
src/utils/databaseOptimization.js
src/utils/errors/AppError.js
src/utils/errors/AuthenticationError.js
src/utils/errors/DatabaseError.js
src/utils/errors/index.js
src/utils/errors/ValidationError.js
src/utils/performanceTest.js
src/utils/responseFormatter.js
supabase_tables.sql
test-api.js
test-auth.js
```

# Files

## File: .gitignore
````
# Node.js dependencies
node_modules/

# Logs
logs/
*.log
npm-debug.log*

# Environment variables
.env

# Build outputs
dist/
build/

# System files
.DS_Store
Thumbs.db

# IDE settings
.vscode/
.idea/

# Firebase Admin Credentials
serviceAccountKey.json

#test files
tes.html
testPasswordencryption.html
testforgotpassword.html
testresend.html
downloadtest.html
check.html
carlistingtest.html
downloadtest.html
houselistingtest.html
testframe.html
````

## File: .repomixignore
````
# Dependencies
node_modules/
npm-debug.log*
yarn-debug.log*
yarn-error.log*
pnpm-debug.log*
lerna-debug.log*

# Runtime data
pids
*.pid
*.seed
*.pid.lock

# Coverage directory used by tools like istanbul
coverage/
*.lcov

# nyc test coverage
.nyc_output

# Grunt intermediate storage (https://gruntjs.com/creating-plugins#storing-task-files)
.grunt

# Bower dependency directory (https://bower.io/)
bower_components

# node-waf configuration
.lock-wscript

# Compiled binary addons (https://nodejs.org/api/addons.html)
build/Release

# Dependency directories
jspm_packages/

# TypeScript cache
*.tsbuildinfo

# Optional npm cache directory
.npm

# Optional eslint cache
.eslintcache

# Optional stylelint cache
.stylelintcache

# Microbundle cache
.rpt2_cache/
.rts2_cache_cjs/
.rts2_cache_es/
.rts2_cache_umd/

# Optional REPL history
.node_repl_history

# Output of 'npm pack'
*.tgz

# Yarn Integrity file
.yarn-integrity

# dotenv environment variable files
.env
.env.development.local
.env.test.local
.env.production.local
.env.local

# parcel-bundler cache (https://parceljs.org/)
.cache
.parcel-cache

# Next.js build output
.next/
out/

# Nuxt.js build / generate output
.nuxt
dist

# Gatsby files
.cache/
public

# Storybook build outputs
.out
.storybook-out
storybook-static

# Temporary folders
tmp/
temp/

# Logs
logs
*.log

# Runtime data
pids
*.pid
*.seed
*.pid.lock

# Directory for instrumented libs generated by jscoverage/JSCover
lib-cov

# Coverage directory used by tools like istanbul
coverage
*.lcov

# nyc test coverage
.nyc_output

# IDEs and editors
.vscode/
.idea/
*.swp
*.swo
*~

# OS generated files
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db

# Firebase
.firebase/
firebase-debug.log
firebase-debug.*.log

# Database files
*.db
*.sqlite
*.sqlite3

# AI Generated files (Prisma generated client)
# ai-generated/
# **/ai-generated/

# Service account keys and credentials
serviceAccountKey.json
**/serviceAccountKey.json
# key/
# **/key/
BackEnd/key/round-ring-426501-q0-074e8188d20e.json
*.json
!package.json
!package-lock.json
!tsconfig.json
!components.json
!next.config.json
!next.config.ts
!eslint.config.json
!eslint.config.mjs
!postcss.config.json
!postcss.config.mjs
!tailwind.config.json
!tailwind.config.ts
!repomix.config.json

# Uploads and user generated content
# uploads/
# **/uploads/

# Prisma
query_engine-*
*.node
*.tmp*

# Build outputs
build/
dist/
*.tgz
*.tar.gz

# Repomix outputs
*repomix-output.md
repomix-output.md

# Archived/compressed files
*.zip
*.rar
*.7z
*.tar
*.gz

# Backup files
*.bak
*.backup
*~

# Test files that might contain sensitive data
test-db-connection.js

# Next.js specific
.next/
out/
next-env.d.ts

# Vercel
.vercel

# Local env files
.env*.local

# Sentry
.sentryclirc

# TypeScript
*.tsbuildinfo
next-env.d.ts

# Optional directories
old/
# new-frontend/

# Documentation outputs
backend-repomix-output.md

*.md
````

## File: database/generated_resumes.sql
````sql
-- Generated Resumes Table for Resume Generator Feature
-- This table stores AI-generated resumes tailored for specific job applications
-- Compatible with existing ImmiGrowAI database schema (SERIAL IDs, RLS policies)

-- Create the generated_resumes table
CREATE TABLE generated_resumes (
    id SERIAL PRIMARY KEY, -- ✅ Match existing pattern
    user_id INTEGER NOT NULL REFERENCES users(id) ON DELETE CASCADE, -- ✅ Match existing pattern
    original_analysis_id INTEGER NOT NULL REFERENCES resume_analyses(id) ON DELETE CASCADE, -- ✅ Match existing pattern
    
    -- Job Targeting Data
    job_title VARCHAR(255) NOT NULL,
    job_description TEXT NOT NULL,
    company_name VARCHAR(255),
    industry VARCHAR(100),
    location VARCHAR(255),
    
    -- Generated Resume Content (JSONB for flexibility)
    resume_data JSONB NOT NULL,
    
    -- User Customizations & AI Data
    user_edits JSONB DEFAULT '{}',
    ai_suggestions JSONB DEFAULT '[]',
    ats_score INTEGER CHECK (ats_score >= 0 AND ats_score <= 100),
    
    -- Status Tracking
    status VARCHAR(20) DEFAULT 'draft' CHECK (status IN ('draft', 'finalized', 'archived')),
    pdf_downloaded_count INTEGER DEFAULT 0,
    last_pdf_download TIMESTAMP WITH TIME ZONE,
    
    -- Metadata
    template_used VARCHAR(100) DEFAULT 'canadian_classic',
    generation_version VARCHAR(20) DEFAULT '1.0',
    
    -- Timestamps (matching existing table patterns)
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW(),
    last_updated TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Create indexes for better performance
CREATE INDEX idx_generated_resumes_user_id ON generated_resumes(user_id);
CREATE INDEX idx_generated_resumes_analysis_id ON generated_resumes(original_analysis_id);
CREATE INDEX idx_generated_resumes_status ON generated_resumes(status);
CREATE INDEX idx_generated_resumes_created_at ON generated_resumes(created_at DESC);

-- Enable Row Level Security (RLS)
ALTER TABLE generated_resumes ENABLE ROW LEVEL SECURITY;

-- Create RLS policies for security
CREATE POLICY "Service role can manage all generated resumes" ON generated_resumes
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Users can view their own generated resumes" ON generated_resumes
    FOR SELECT USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can insert their own generated resumes" ON generated_resumes
    FOR INSERT WITH CHECK (auth.uid()::text = user_id::text);

CREATE POLICY "Users can update their own generated resumes" ON generated_resumes
    FOR UPDATE USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can delete their own generated resumes" ON generated_resumes
    FOR DELETE USING (auth.uid()::text = user_id::text);

-- Add comments for documentation
COMMENT ON TABLE generated_resumes IS 'Stores AI-generated resumes tailored for specific job applications';
COMMENT ON COLUMN generated_resumes.user_id IS 'Reference to the user who owns this generated resume';
COMMENT ON COLUMN generated_resumes.original_analysis_id IS 'Reference to the original resume analysis used for generation';
COMMENT ON COLUMN generated_resumes.job_title IS 'Target job title for this resume';
COMMENT ON COLUMN generated_resumes.job_description IS 'Job description used for tailoring the resume';
COMMENT ON COLUMN generated_resumes.resume_data IS 'JSONB containing the complete generated resume content';
COMMENT ON COLUMN generated_resumes.user_edits IS 'JSONB tracking user modifications to the generated resume';
COMMENT ON COLUMN generated_resumes.ai_suggestions IS 'JSONB array of AI-generated improvement suggestions';
COMMENT ON COLUMN generated_resumes.ats_score IS 'ATS compatibility score (0-100)';
COMMENT ON COLUMN generated_resumes.status IS 'Current status: draft, finalized, or archived';
COMMENT ON COLUMN generated_resumes.template_used IS 'Resume template used for generation';
COMMENT ON COLUMN generated_resumes.generation_version IS 'Version of the generation algorithm used';
````

## File: package.json
````json
{
  "name": "immigratexai-backend",
  "version": "1.0.0",
  "description": "AI Career Assistant Backend - Resume Analysis and Job Search",
  "main": "src/server.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "nodemon ./src/server.js",
    "start": "node ./src/server.js",
    "build": "echo \"No build step required for Node.js\"",
    "lint": "echo \"Linting not configured yet\"",
    "lint:fix": "echo \"Linting not configured yet\"",
    "security:audit": "npm audit",
    "security:fix": "npm audit fix",
    "performance:test": "node src/utils/performanceTest.js"
  },
  "author": "ImmiGrowAI Team",
  "license": "ISC",
  "dependencies": {
    "@google-cloud/talent": "^7.0.0",
    "@google/generative-ai": "^0.17.2",
    "@supabase/supabase-js": "^2.55.0",
    "axios": "^1.7.9",
    "compression": "^1.7.4",
    "cookie-parser": "^1.4.7",
    "cors": "^2.8.5",
    "dotenv": "^16.4.7",
    "express": "^4.21.2",
    "express-rate-limit": "^7.5.1",
    "helmet": "^8.0.0",
    "joi": "^18.0.0",
    "mammoth": "^1.9.1",
    "multer": "^1.4.5-lts.1",
    "pdf-parse": "^1.1.1",
    "redis": "^4.6.13",
    "sharp": "^0.33.5",
    "tesseract.js": "^4.1.4",
    "winston": "^3.17.0"
  },
  "devDependencies": {
    "nodemon": "^3.1.9"
  }
}
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

## File: src/app.js
````javascript
/**
 * Express Application Configuration
 * Sets up the Express app with middleware and routes
 */

const express = require("express");
const cors = require("cors");
const cookieParser = require("cookie-parser");
const compression = require("compression");
const { getEnvironmentConfig } = require('./config/environment');
const { logger } = require('./config/logger');
const { errorHandler, notFoundHandler } = require('./middleware/errorHandler');
const { createRequestLogger } = require('./config/logger');
const { getApiVersioningInfo } = require('./config/apiVersioning');
const ApiRouter = require('./routes/ApiRouter');

// Import Phase 5 - Performance & Security features
const { cacheConfig } = require('./config/cache');
const { 
  helmetConfig, 
  inputSanitization, 
  sqlInjectionPrevention, 
  xssPrevention, 
  requestSizeLimit, 
  securityHeaders, 
  securityMonitoring 
} = require('./middleware/securityMiddleware');
const { 
  userCache, 
  aiCache, 
  careerCache, 
  resumeCache, 
  staticCache, 
  sessionCache,
  cacheManagement 
} = require('./middleware/cacheMiddleware');
const monitoringRoutes = require('./routes/monitoringRoutes');

// Import legacy routes (to be gradually replaced)
const aiRoutesLocal = require("./routes/aiRoutesLocal");
const careerRoutes = require("./routes/careerRoutes");
const authRoutes = require("./routes/authRoutes");

const app = express();
const config = getEnvironmentConfig();

// Initialize cache system
cacheConfig.initialize().catch(err => {
  logger.error('Failed to initialize cache system:', err);
});

// CORS configuration
const corsOptions = {
  origin: config.cors.allowedOrigins,
  credentials: true,
  methods: ['GET', 'POST', 'PUT', 'DELETE', 'OPTIONS'],
  allowedHeaders: ['Content-Type', 'Authorization', 'X-Requested-With', 'X-API-Version', 'X-Monitoring-Key']
};

// Phase 5 - Security Middleware (apply early)
app.use(helmetConfig);
app.use(securityHeaders);
app.use(securityMonitoring);
app.use(inputSanitization);
app.use(sqlInjectionPrevention);
app.use(xssPrevention);
app.use(requestSizeLimit('10mb'));

// Phase 5 - Performance Middleware
app.use(compression()); // Enable gzip compression
app.use(cors(corsOptions));
app.options("*", cors(corsOptions));

// Standard middleware
app.use(express.urlencoded({ extended: true }));
app.use(express.json({ limit: config.upload.maxSize }));
app.use(cookieParser());
app.use(createRequestLogger());

// Enhanced health check endpoint
app.get('/health', async (req, res) => {
  try {
    // Initialize API router for health check
    await ApiRouter.initialize();
    
    const versioningInfo = getApiVersioningInfo();
    const health = {
      status: 'healthy',
      message: 'ImmiGrowAI Backend is running',
      timestamp: new Date().toISOString(),
      version: '1.0.0',
      environment: config.server.nodeEnv,
      api: {
        versions: versioningInfo.currentVersions,
        defaultVersion: versioningInfo.defaultVersion,
        features: versioningInfo.features
      },
      services: {
        database: 'connected',
        controllers: 'initialized',
        routes: 'ready',
        versioning: 'active',
        cache: cacheConfig.isConnected ? 'connected' : 'disconnected',
        security: 'enabled',
        compression: 'enabled'
      },
      performance: {
        uptime: process.uptime(),
        memory: process.memoryUsage(),
        cache: cacheConfig.isConnected ? 'available' : 'unavailable'
      }
    };
    
    res.status(200).json(health);
  } catch (error) {
    logger.error('Health check failed:', error);
    res.status(503).json({
      status: 'unhealthy',
      message: 'Service health check failed',
      error: error.message,
      timestamp: new Date().toISOString()
    });
  }
});

// API versioning information endpoint
app.get('/api/versions', (req, res) => {
  const versioningInfo = getApiVersioningInfo();
  res.json({
    success: true,
    data: versioningInfo,
    timestamp: new Date().toISOString()
  });
});

// Phase 5 - Cache Management Routes
app.get('/api/cache/stats', cacheManagement.getStats);
app.delete('/api/cache/:type', cacheManagement.clearType);
app.delete('/api/cache', cacheManagement.clearAll);

// Phase 5 - Monitoring Dashboard Routes
app.use('/api/monitoring', monitoringRoutes);

// API Routes
// Legacy routes (to be gradually replaced)
app.use("/api/auth", authRoutes);
app.use("/api/protected/ai-local", aiRoutesLocal);
app.use("/api/protected/career", careerRoutes);

// New version-aware API routes with Phase 5 caching
// Initialize and mount the API router
(async () => {
  try {
    await ApiRouter.initialize();
    const apiRouter = ApiRouter.createRouter();
    app.use("/api", apiRouter);
  } catch (error) {
    logger.error('Failed to initialize API router:', error);
  }
})();

// Phase 5 - Apply caching to specific route patterns
// Note: These would be applied to the actual route handlers in the route files
// This is a demonstration of how caching would be integrated

// Example of how to apply caching to routes (commented out as routes are in separate files)
/*
app.use('/api/v1/auth', userCache, authRoutes);
app.use('/api/v1/ai', aiCache, aiRoutes);
app.use('/api/v1/career', careerCache, careerRoutes);
app.use('/api/v1/resume', resumeCache, resumeRoutes);
app.use('/api/v1/static', staticCache, staticRoutes);
*/

// Error handling middleware
app.use(notFoundHandler);
app.use(errorHandler);

// Graceful shutdown handling
process.on('SIGTERM', async () => {
  logger.info('SIGTERM received, shutting down gracefully');
  
  // Close cache connection
  await cacheConfig.close();
  
  process.exit(0);
});

process.on('SIGINT', async () => {
  logger.info('SIGINT received, shutting down gracefully');
  
  // Close cache connection
  await cacheConfig.close();
  
  process.exit(0);
});

module.exports = app;
````

## File: src/config/ai.js
````javascript
/**
 * AI Service Configuration
 * Manages AI service configurations including Google AI, OpenAI, and other AI providers
 */

const { getEnvironmentConfig } = require('./environment');

/**
 * AI service configuration
 */
const aiConfig = {
  // Google AI Configuration
  google: {
    apiKey: process.env.GOOGLE_AI_API_KEY,
    model: process.env.GOOGLE_AI_MODEL || 'gemini-1.5-flash',
    maxTokens: parseInt(process.env.GOOGLE_AI_MAX_TOKENS) || 8192,
    temperature: parseFloat(process.env.GOOGLE_AI_TEMPERATURE) || 0.7,
    topP: parseFloat(process.env.GOOGLE_AI_TOP_P) || 0.8,
    topK: parseInt(process.env.GOOGLE_AI_TOP_K) || 40,
    timeout: parseInt(process.env.GOOGLE_AI_TIMEOUT) || 30000
  },
  
  // Resume Analysis Configuration
  resumeAnalysis: {
    maxFileSize: parseInt(process.env.RESUME_MAX_FILE_SIZE) || 10 * 1024 * 1024, // 10MB
    allowedFormats: ['pdf', 'doc', 'docx'],
    extractionTimeout: parseInt(process.env.RESUME_EXTRACTION_TIMEOUT) || 60000, // 60 seconds
    analysisTimeout: parseInt(process.env.RESUME_ANALYSIS_TIMEOUT) || 120000, // 2 minutes
    confidenceThreshold: parseFloat(process.env.RESUME_CONFIDENCE_THRESHOLD) || 0.7
  },
  
  // Career Profile Configuration
  careerProfile: {
    analysisTimeout: parseInt(process.env.CAREER_ANALYSIS_TIMEOUT) || 90000, // 90 seconds
    skillExtractionTimeout: parseInt(process.env.SKILL_EXTRACTION_TIMEOUT) || 30000, // 30 seconds
    marketAnalysisTimeout: parseInt(process.env.MARKET_ANALYSIS_TIMEOUT) || 60000, // 60 seconds
    maxSkillsPerProfile: parseInt(process.env.MAX_SKILLS_PER_PROFILE) || 50
  },
  
  // Job Search Configuration
  jobSearch: {
    searchTimeout: parseInt(process.env.JOB_SEARCH_TIMEOUT) || 45000, // 45 seconds
    maxResultsPerSearch: parseInt(process.env.MAX_JOB_RESULTS) || 50,
    relevanceThreshold: parseFloat(process.env.JOB_RELEVANCE_THRESHOLD) || 0.6,
    cacheDuration: parseInt(process.env.JOB_CACHE_DURATION) || 3600000 // 1 hour
  },
  
  // Document Processing Configuration
  documentProcessing: {
    maxConcurrentProcesses: parseInt(process.env.MAX_CONCURRENT_PROCESSES) || 5,
    retryAttempts: parseInt(process.env.DOC_PROCESSING_RETRY_ATTEMPTS) || 3,
    retryDelay: parseInt(process.env.DOC_PROCESSING_RETRY_DELAY) || 5000, // 5 seconds
    cleanupInterval: parseInt(process.env.DOC_CLEANUP_INTERVAL) || 3600000 // 1 hour
  },
  
  // Rate Limiting for AI Services
  rateLimit: {
    requestsPerMinute: parseInt(process.env.AI_RATE_LIMIT_PER_MINUTE) || 60,
    requestsPerHour: parseInt(process.env.AI_RATE_LIMIT_PER_HOUR) || 1000,
    burstLimit: parseInt(process.env.AI_BURST_LIMIT) || 10
  }
};

/**
 * Validate AI configuration
 */
function validateAIConfig() {
  const config = getEnvironmentConfig();
  const errors = [];
  
  if (!config.ai.googleApiKey) {
    errors.push('GOOGLE_AI_API_KEY is required');
  }
  
  if (aiConfig.google.temperature < 0 || aiConfig.google.temperature > 1) {
    errors.push('GOOGLE_AI_TEMPERATURE must be between 0 and 1');
  }
  
  if (aiConfig.google.topP < 0 || aiConfig.google.topP > 1) {
    errors.push('GOOGLE_AI_TOP_P must be between 0 and 1');
  }
  
  if (aiConfig.resumeAnalysis.confidenceThreshold < 0 || aiConfig.resumeAnalysis.confidenceThreshold > 1) {
    errors.push('RESUME_CONFIDENCE_THRESHOLD must be between 0 and 1');
  }
  
  if (errors.length > 0) {
    throw new Error(`AI Configuration validation failed: ${errors.join(', ')}`);
  }
}

/**
 * Get AI configuration for specific service
 */
function getAIConfig(service) {
  validateAIConfig();
  
  switch (service) {
    case 'google':
      return aiConfig.google;
    case 'resumeAnalysis':
      return aiConfig.resumeAnalysis;
    case 'careerProfile':
      return aiConfig.careerProfile;
    case 'jobSearch':
      return aiConfig.jobSearch;
    case 'documentProcessing':
      return aiConfig.documentProcessing;
    case 'rateLimit':
      return aiConfig.rateLimit;
    default:
      throw new Error(`Unknown AI service: ${service}`);
  }
}

/**
 * Get complete AI configuration
 */
function getCompleteAIConfig() {
  validateAIConfig();
  return aiConfig;
}

/**
 * Check if AI service is available
 */
function isAIServiceAvailable(service) {
  try {
    const config = getAIConfig(service);
    return !!config;
  } catch (error) {
    return false;
  }
}

/**
 * Get AI service health status
 */
async function getAIServiceHealth() {
  const health = {
    timestamp: new Date().toISOString(),
    services: {}
  };
  
  // Check Google AI
  try {
    const googleConfig = getAIConfig('google');
    health.services.google = {
      status: 'available',
      model: googleConfig.model,
      maxTokens: googleConfig.maxTokens
    };
  } catch (error) {
    health.services.google = {
      status: 'unavailable',
      error: error.message
    };
  }
  
  // Check other services
  const services = ['resumeAnalysis', 'careerProfile', 'jobSearch', 'documentProcessing'];
  
  for (const service of services) {
    try {
      const config = getAIConfig(service);
      health.services[service] = {
        status: 'configured',
        config: Object.keys(config)
      };
    } catch (error) {
      health.services[service] = {
        status: 'misconfigured',
        error: error.message
      };
    }
  }
  
  return health;
}

module.exports = {
  aiConfig,
  validateAIConfig,
  getAIConfig,
  getCompleteAIConfig,
  isAIServiceAvailable,
  getAIServiceHealth
};
````

## File: src/config/apiVersioning.js
````javascript
/**
 * API Versioning Configuration
 * Manages API versioning strategy, compatibility, and routing
 */

const { logger } = require('./logger');

/**
 * API Version Configuration
 */
const API_VERSIONS = {
  v1: {
    version: '1.0.0',
    status: 'stable',
    releaseDate: '2024-01-01',
    deprecated: false,
    sunsetDate: null,
    features: [
      'user-management',
      'resume-analysis',
      'career-profiles',
      'basic-authentication'
    ],
    breakingChanges: [],
    migrations: []
  },
  v2: {
    version: '2.0.0',
    status: 'beta',
    releaseDate: '2024-08-01',
    deprecated: false,
    sunsetDate: null,
    features: [
      'user-management',
      'resume-analysis',
      'career-profiles',
      'advanced-authentication',
      'real-time-notifications',
      'advanced-search',
      'analytics'
    ],
    breakingChanges: [
      'response-format-changes',
      'pagination-standardization',
      'error-response-enhancement'
    ],
    migrations: [
      'user-schema-update',
      'resume-analysis-enhancement'
    ]
  }
};

/**
 * Default API version
 */
const DEFAULT_VERSION = 'v1';

/**
 * Supported API versions
 */
const SUPPORTED_VERSIONS = Object.keys(API_VERSIONS);

/**
 * Get API version configuration
 * @param {string} version - API version
 * @returns {Object} Version configuration
 */
function getApiVersionConfig(version) {
  if (!API_VERSIONS[version]) {
    throw new Error(`Unsupported API version: ${version}`);
  }
  return API_VERSIONS[version];
}

/**
 * Check if API version is supported
 * @param {string} version - API version
 * @returns {boolean} Whether version is supported
 */
function isVersionSupported(version) {
  return SUPPORTED_VERSIONS.includes(version);
}

/**
 * Check if API version is deprecated
 * @param {string} version - API version
 * @returns {boolean} Whether version is deprecated
 */
function isVersionDeprecated(version) {
  const config = getApiVersionConfig(version);
  return config.deprecated;
}

/**
 * Check if API version is in sunset period
 * @param {string} version - API version
 * @returns {boolean} Whether version is in sunset period
 */
function isVersionInSunset(version) {
  const config = getApiVersionConfig(version);
  if (!config.sunsetDate) return false;
  
  const sunsetDate = new Date(config.sunsetDate);
  const now = new Date();
  return now >= sunsetDate;
}

/**
 * Get recommended API version
 * @param {string} currentVersion - Current API version
 * @returns {string} Recommended version
 */
function getRecommendedVersion(currentVersion) {
  // If current version is deprecated or in sunset, recommend latest stable
  if (isVersionDeprecated(currentVersion) || isVersionInSunset(currentVersion)) {
    const stableVersions = SUPPORTED_VERSIONS.filter(v => 
      API_VERSIONS[v].status === 'stable' && !API_VERSIONS[v].deprecated
    );
    return stableVersions[stableVersions.length - 1] || DEFAULT_VERSION;
  }
  
  return currentVersion;
}

/**
 * Get API version compatibility matrix
 * @returns {Object} Compatibility matrix
 */
function getCompatibilityMatrix() {
  const matrix = {};
  
  for (const version of SUPPORTED_VERSIONS) {
    matrix[version] = {
      compatibleWith: [],
      breakingChanges: API_VERSIONS[version].breakingChanges,
      migrations: API_VERSIONS[version].migrations
    };
    
    // Check compatibility with other versions
    for (const otherVersion of SUPPORTED_VERSIONS) {
      if (version !== otherVersion) {
        const hasBreakingChanges = API_VERSIONS[version].breakingChanges.length > 0;
        matrix[version].compatibleWith.push({
          version: otherVersion,
          compatible: !hasBreakingChanges,
          notes: hasBreakingChanges ? 'Breaking changes detected' : 'Fully compatible'
        });
      }
    }
  }
  
  return matrix;
}

/**
 * Get API version features
 * @param {string} version - API version
 * @returns {Array} List of features
 */
function getVersionFeatures(version) {
  const config = getApiVersionConfig(version);
  return config.features;
}

/**
 * Check if feature is available in version
 * @param {string} version - API version
 * @param {string} feature - Feature name
 * @returns {boolean} Whether feature is available
 */
function isFeatureAvailable(version, feature) {
  const features = getVersionFeatures(version);
  return features.includes(feature);
}

/**
 * Get API versioning headers
 * @param {string} version - API version
 * @param {Object} req - Express request object
 * @returns {Object} Headers object
 */
function getVersioningHeaders(version, req) {
  const config = getApiVersionConfig(version);
  const headers = {
    'X-API-Version': version,
    'X-API-Version-Status': config.status,
    'X-API-Version-Date': config.releaseDate
  };
  
  // Add deprecation warning if version is deprecated
  if (config.deprecated) {
    headers['X-API-Version-Deprecated'] = 'true';
    headers['X-API-Version-Sunset'] = config.sunsetDate || 'TBD';
  }
  
  // Add recommended version if different from current
  const recommended = getRecommendedVersion(version);
  if (recommended !== version) {
    headers['X-API-Version-Recommended'] = recommended;
  }
  
  return headers;
}

/**
 * Validate API version from request
 * @param {Object} req - Express request object
 * @returns {Object} Validation result
 */
function validateApiVersion(req) {
  const version = req.headers['x-api-version'] || 
                 req.query.version || 
                 req.params.version || 
                 DEFAULT_VERSION;
  
  const result = {
    version,
    isValid: false,
    isSupported: false,
    isDeprecated: false,
    isInSunset: false,
    recommended: null,
    error: null
  };
  
  try {
    result.isSupported = isVersionSupported(version);
    result.isValid = result.isSupported;
    
    if (result.isSupported) {
      result.isDeprecated = isVersionDeprecated(version);
      result.isInSunset = isVersionInSunset(version);
      result.recommended = getRecommendedVersion(version);
    } else {
      result.error = `Unsupported API version: ${version}`;
      result.recommended = DEFAULT_VERSION;
    }
  } catch (error) {
    result.error = error.message;
    result.recommended = DEFAULT_VERSION;
  }
  
  return result;
}

/**
 * API versioning middleware
 * @param {Object} options - Middleware options
 * @returns {Function} Express middleware
 */
function apiVersioningMiddleware(options = {}) {
  const {
    strict = false,
    defaultVersion = DEFAULT_VERSION,
    logVersionUsage = true
  } = options;
  
  return (req, res, next) => {
    const validation = validateApiVersion(req);
    
    // Set version in request object
    req.apiVersion = validation.version;
    req.apiVersionInfo = validation;
    
    // Add versioning headers to response
    const headers = getVersioningHeaders(validation.version, req);
    Object.entries(headers).forEach(([key, value]) => {
      res.setHeader(key, value);
    });
    
    // Log version usage if enabled
    if (logVersionUsage) {
      logger.info('API Version Request', {
        version: validation.version,
        path: req.path,
        method: req.method,
        userAgent: req.get('User-Agent'),
        ip: req.ip,
        isDeprecated: validation.isDeprecated,
        isInSunset: validation.isInSunset
      });
    }
    
    // Handle strict mode
    if (strict && !validation.isValid) {
      return res.status(400).json({
        error: 'Invalid API Version',
        message: validation.error,
        supportedVersions: SUPPORTED_VERSIONS,
        recommendedVersion: validation.recommended
      });
    }
    
    // Handle deprecated version warning
    if (validation.isDeprecated) {
      logger.warn('Deprecated API Version Used', {
        version: validation.version,
        path: req.path,
        recommended: validation.recommended
      });
    }
    
    // Handle sunset version
    if (validation.isInSunset) {
      logger.error('Sunset API Version Used', {
        version: validation.version,
        path: req.path,
        sunsetDate: getApiVersionConfig(validation.version).sunsetDate
      });
      
      return res.status(410).json({
        error: 'API Version Sunset',
        message: `API version ${validation.version} has been sunset`,
        sunsetDate: getApiVersionConfig(validation.version).sunsetDate,
        recommendedVersion: validation.recommended
      });
    }
    
    next();
  };
}

/**
 * Get API versioning information for documentation
 * @returns {Object} Versioning information
 */
function getApiVersioningInfo() {
  return {
    currentVersions: SUPPORTED_VERSIONS,
    defaultVersion: DEFAULT_VERSION,
    versions: API_VERSIONS,
    compatibilityMatrix: getCompatibilityMatrix(),
    features: Object.entries(API_VERSIONS).reduce((acc, [version, config]) => {
      acc[version] = config.features;
      return acc;
    }, {}),
    deprecationSchedule: Object.entries(API_VERSIONS)
      .filter(([_, config]) => config.deprecated || config.sunsetDate)
      .reduce((acc, [version, config]) => {
        acc[version] = {
          deprecated: config.deprecated,
          sunsetDate: config.sunsetDate,
          status: config.status
        };
        return acc;
      }, {})
  };
}

module.exports = {
  API_VERSIONS,
  DEFAULT_VERSION,
  SUPPORTED_VERSIONS,
  getApiVersionConfig,
  isVersionSupported,
  isVersionDeprecated,
  isVersionInSunset,
  getRecommendedVersion,
  getCompatibilityMatrix,
  getVersionFeatures,
  isFeatureAvailable,
  getVersioningHeaders,
  validateApiVersion,
  apiVersioningMiddleware,
  getApiVersioningInfo
};
````

## File: src/config/cache.js
````javascript
/**
 * Cache Configuration
 * Redis-based caching system with different strategies for various data types
 * Falls back to in-memory cache when Redis is not available
 */

const redis = require('redis');
const { logger } = require('./logger');

class CacheConfig {
  constructor() {
    this.client = null;
    this.isConnected = false;
    this.useRedis = process.env.CACHE_ENABLED === 'true'; // Only use Redis if explicitly enabled
    this.memoryCache = new Map(); // Fallback in-memory cache
    this.cacheStrategies = {
      // User data cache (5 minutes)
      user: {
        ttl: 300,
        prefix: 'user:',
        description: 'User profile and authentication data'
      },
      // AI analysis results cache (1 hour)
      ai: {
        ttl: 3600,
        prefix: 'ai:',
        description: 'AI analysis results and recommendations'
      },
      // Career data cache (30 minutes)
      career: {
        ttl: 1800,
        prefix: 'career:',
        description: 'Career profiles and job recommendations'
      },
      // Resume data cache (15 minutes)
      resume: {
        ttl: 900,
        prefix: 'resume:',
        description: 'Resume analysis and parsing results'
      },
      // Static data cache (24 hours)
      static: {
        ttl: 86400,
        prefix: 'static:',
        description: 'Static data like job categories, skills, etc.'
      },
      // Session cache (2 hours)
      session: {
        ttl: 7200,
        prefix: 'session:',
        description: 'User sessions and tokens'
      }
    };
  }

  /**
   * Initialize Redis connection
   */
  async initialize() {
    if (!this.useRedis) {
      logger.info('Cache system using in-memory storage only');
      return;
    }

    try {
      const redisUrl = process.env.REDIS_URL || 'redis://localhost:6379';
      
      this.client = redis.createClient({
        url: redisUrl,
        socket: {
          connectTimeout: 5000, // 5 second timeout
          lazyConnect: true // Don't connect immediately
        }
      });

      this.client.on('error', (err) => {
        logger.warn('Redis Client Error - falling back to in-memory cache:', err.message);
        this.isConnected = false;
      });

      this.client.on('connect', () => {
        logger.info('Redis client connected');
        this.isConnected = true;
      });

      this.client.on('ready', () => {
        logger.info('Redis client ready');
        this.isConnected = true;
      });

      this.client.on('end', () => {
        logger.info('Redis client disconnected');
        this.isConnected = false;
      });

      // Try to connect with a timeout
      const connectPromise = this.client.connect();
      const timeoutPromise = new Promise((_, reject) => {
        setTimeout(() => reject(new Error('Connection timeout')), 5000);
      });

      await Promise.race([connectPromise, timeoutPromise]);
      logger.info('Cache system initialized successfully with Redis');
      
    } catch (error) {
      logger.warn('Failed to initialize Redis cache system - using in-memory fallback:', error.message);
      this.isConnected = false;
      // Clean up the client if it was created
      if (this.client) {
        try {
          await this.client.quit();
        } catch (quitError) {
          // Ignore quit errors
        }
        this.client = null;
      }
    }
  }

  /**
   * Get cache strategy for a specific type
   */
  getStrategy(type) {
    return this.cacheStrategies[type] || this.cacheStrategies.static;
  }

  /**
   * Generate cache key
   */
  generateKey(type, identifier) {
    const strategy = this.getStrategy(type);
    return `${strategy.prefix}${identifier}`;
  }

  /**
   * Set cache value
   */
  async set(type, identifier, data) {
    const key = this.generateKey(type, identifier);
    const strategy = this.getStrategy(type);
    const serializedData = JSON.stringify({
      data,
      timestamp: Date.now(),
      ttl: strategy.ttl
    });

    if (this.isConnected && this.client) {
      try {
        await this.client.setEx(key, strategy.ttl, serializedData);
        logger.debug(`Redis cache set: ${key} (TTL: ${strategy.ttl}s)`);
        return true;
      } catch (error) {
        logger.warn('Redis cache set failed, using in-memory:', error.message);
      }
    }

    // Fallback to in-memory cache
    this.memoryCache.set(key, {
      data: serializedData,
      expires: Date.now() + (strategy.ttl * 1000)
    });
    logger.debug(`In-memory cache set: ${key} (TTL: ${strategy.ttl}s)`);
    return true;
  }

  /**
   * Get cache value
   */
  async get(type, identifier) {
    const key = this.generateKey(type, identifier);

    if (this.isConnected && this.client) {
      try {
        const cachedData = await this.client.get(key);
        
        if (cachedData) {
          const parsed = JSON.parse(cachedData);
          logger.debug(`Redis cache hit: ${key}`);
          return parsed.data;
        }
      } catch (error) {
        logger.warn('Redis cache get failed, trying in-memory:', error.message);
      }
    }

    // Fallback to in-memory cache
    const memoryData = this.memoryCache.get(key);
    if (memoryData && memoryData.expires > Date.now()) {
      const parsed = JSON.parse(memoryData.data);
      logger.debug(`In-memory cache hit: ${key}`);
      return parsed.data;
    } else if (memoryData) {
      // Remove expired entry
      this.memoryCache.delete(key);
    }
    
    logger.debug(`Cache miss: ${key}`);
    return null;
  }

  /**
   * Delete cache value
   */
  async delete(type, identifier) {
    const key = this.generateKey(type, identifier);

    if (this.isConnected && this.client) {
      try {
        await this.client.del(key);
        logger.debug(`Redis cache deleted: ${key}`);
      } catch (error) {
        logger.warn('Redis cache delete failed:', error.message);
      }
    }

    // Also delete from memory cache
    this.memoryCache.delete(key);
    logger.debug(`Cache deleted: ${key}`);
    return true;
  }

  /**
   * Clear all cache for a specific type
   */
  async clearType(type) {
    const strategy = this.getStrategy(type);
    const pattern = `${strategy.prefix}*`;

    if (this.isConnected && this.client) {
      try {
        const keys = await this.client.keys(pattern);
        
        if (keys.length > 0) {
          await this.client.del(keys);
          logger.info(`Cleared ${keys.length} Redis cache entries for type: ${type}`);
        }
      } catch (error) {
        logger.warn('Redis cache clear type failed:', error.message);
      }
    }

    // Clear from memory cache
    let memoryCount = 0;
    for (const [key] of this.memoryCache) {
      if (key.startsWith(strategy.prefix)) {
        this.memoryCache.delete(key);
        memoryCount++;
      }
    }
    
    logger.info(`Cleared ${memoryCount} in-memory cache entries for type: ${type}`);
    return true;
  }

  /**
   * Clear all cache
   */
  async clearAll() {
    if (this.isConnected && this.client) {
      try {
        await this.client.flushAll();
        logger.info('All Redis cache cleared');
      } catch (error) {
        logger.warn('Redis cache clear all failed:', error.message);
      }
    }

    // Clear memory cache
    this.memoryCache.clear();
    logger.info('All in-memory cache cleared');
    return true;
  }

  /**
   * Get cache statistics
   */
  async getStats() {
    const stats = {
      connected: this.isConnected,
      strategies: Object.keys(this.cacheStrategies).length,
      useRedis: this.useRedis,
      memoryCacheSize: this.memoryCache.size
    };

    if (this.isConnected && this.client) {
      try {
        const info = await this.client.info();
        stats.redisInfo = info;
      } catch (error) {
        logger.warn('Failed to get Redis info:', error.message);
      }
    }

    // Get key counts for each strategy
    for (const [type, strategy] of Object.entries(this.cacheStrategies)) {
      let count = 0;
      
      if (this.isConnected && this.client) {
        try {
          const pattern = `${strategy.prefix}*`;
          const keys = await this.client.keys(pattern);
          count += keys.length;
        } catch (error) {
          logger.warn(`Failed to get Redis keys for ${type}:`, error.message);
        }
      }

      // Count memory cache entries
      for (const [key] of this.memoryCache) {
        if (key.startsWith(strategy.prefix)) {
          count++;
        }
      }

      stats[type] = {
        count,
        ttl: strategy.ttl,
        description: strategy.description
      };
    }

    return stats;
  }

  /**
   * Close Redis connection
   */
  async close() {
    if (this.client) {
      try {
        await this.client.quit();
        this.isConnected = false;
        logger.info('Redis connection closed');
      } catch (error) {
        logger.warn('Error closing Redis connection:', error.message);
      }
    }
  }
}

// Create singleton instance
const cacheConfig = new CacheConfig();

module.exports = {
  cacheConfig,
  CacheConfig
};
````

## File: src/config/database.js
````javascript
/**
 * Database Configuration
 * Manages Supabase connection and configuration
 */

const { createClient } = require('@supabase/supabase-js');
const { getEnvironmentConfig } = require('./environment');

/**
 * Create Supabase client with configuration
 */
function createSupabaseClient() {
  const config = getEnvironmentConfig();
  
  const supabaseUrl = config.supabase.url;
  const supabaseKey = config.supabase.anonKey;
  
  if (!supabaseUrl || !supabaseKey) {
    throw new Error('Supabase URL and key are required');
  }
  
  return createClient(supabaseUrl, supabaseKey, {
    auth: {
      autoRefreshToken: true,
      persistSession: true,
      detectSessionInUrl: true
    },
    db: {
      schema: 'public'
    },
    global: {
      headers: {
        'X-Client-Info': 'immigrow-ai-backend'
      }
    }
  });
}

/**
 * Create Supabase admin client with service role key
 */
function createSupabaseAdminClient() {
  const config = getEnvironmentConfig();
  
  const supabaseUrl = config.supabase.url;
  const supabaseServiceKey = config.supabase.serviceRoleKey;
  
  if (!supabaseUrl || !supabaseServiceKey) {
    throw new Error('Supabase URL and service role key are required');
  }
  
  return createClient(supabaseUrl, supabaseServiceKey, {
    auth: {
      autoRefreshToken: false,
      persistSession: false
    },
    db: {
      schema: 'public'
    },
    global: {
      headers: {
        'X-Client-Info': 'immigrow-ai-backend-admin'
      }
    }
  });
}

/**
 * Database connection configuration
 */
const dbConfig = {
  // Connection pool settings
  pool: {
    min: 2,
    max: 10,
    acquireTimeoutMillis: 30000,
    createTimeoutMillis: 30000,
    destroyTimeoutMillis: 5000,
    idleTimeoutMillis: 30000,
    reapIntervalMillis: 1000,
    createRetryIntervalMillis: 200
  },
  
  // Query timeout settings
  query: {
    timeout: 30000 // 30 seconds
  },
  
  // Migration settings
  migration: {
    directory: './migrations',
    tableName: 'knex_migrations'
  }
};

/**
 * Health check for database connection
 */
async function checkDatabaseHealth() {
  try {
    const client = createSupabaseClient();
    const { data, error } = await client.from('users').select('count').limit(1);
    
    if (error) {
      throw error;
    }
    
    return {
      status: 'healthy',
      timestamp: new Date().toISOString(),
      message: 'Database connection successful'
    };
  } catch (error) {
    return {
      status: 'unhealthy',
      timestamp: new Date().toISOString(),
      message: error.message,
      error: error
    };
  }
}

/**
 * Get database statistics
 */
async function getDatabaseStats() {
  try {
    const client = createSupabaseClient();
    
    // Get table row counts
    const tables = ['users', 'resume_analyses', 'user_career_profiles', 'job_opportunities'];
    const stats = {};
    
    for (const table of tables) {
      const { count, error } = await client
        .from(table)
        .select('*', { count: 'exact', head: true });
      
      if (!error) {
        stats[table] = count || 0;
      }
    }
    
    return {
      status: 'success',
      timestamp: new Date().toISOString(),
      stats
    };
  } catch (error) {
    return {
      status: 'error',
      timestamp: new Date().toISOString(),
      message: error.message,
      error: error
    };
  }
}

module.exports = {
  createSupabaseClient,
  createSupabaseAdminClient,
  dbConfig,
  checkDatabaseHealth,
  getDatabaseStats
};
````

## File: src/config/environment.js
````javascript
/**
 * Environment Configuration
 * Manages all environment variables with validation and defaults
 */

const requiredEnvVars = [
  'SUPABASE_URL',
  'SUPABASE_ANON_KEY',
  'SUPABASE_SERVICE_ROLE_KEY',
  'JWT_SECRET',
  'GOOGLE_AI_API_KEY'
];

const optionalEnvVars = {
  PORT: 5500,
  NODE_ENV: 'development',
  LOG_LEVEL: 'info',
  CORS_ORIGIN: 'http://localhost:3000',
  RATE_LIMIT_WINDOW_MS: 15 * 60 * 1000, // 15 minutes
  RATE_LIMIT_MAX_REQUESTS: 100,
  UPLOAD_MAX_SIZE: 10 * 1024 * 1024, // 10MB
  SESSION_SECRET: 'your-session-secret-change-in-production',
  
  // Phase 5 - Cache Configuration
  REDIS_URL: 'redis://localhost:6379',
  CACHE_ENABLED: 'true',
  
  // Phase 5 - Security Configuration
  MONITORING_ACCESS_KEY: 'default-monitoring-key-change-in-production',
  SECURITY_HEADERS_ENABLED: 'true',
  INPUT_SANITIZATION_ENABLED: 'true',
  SQL_INJECTION_PREVENTION_ENABLED: 'true',
  XSS_PREVENTION_ENABLED: 'true',
  
  // Phase 5 - Performance Configuration
  COMPRESSION_ENABLED: 'true',
  PERFORMANCE_MONITORING_ENABLED: 'true',
  SLOW_QUERY_THRESHOLD: 1000, // 1 second
  REQUEST_SIZE_LIMIT: '10mb',
  
  // Phase 5 - Monitoring Configuration
  MONITORING_ENABLED: 'true',
  METRICS_RETENTION_HOURS: 24,
  ALERT_THRESHOLD_RESPONSE_TIME: 1000,
  ALERT_THRESHOLD_ERROR_RATE: 0.05, // 5%
  ALERT_THRESHOLD_MEMORY_USAGE: 0.8, // 80%
  ALERT_THRESHOLD_CPU_USAGE: 0.7 // 70%
};

/**
 * Validate required environment variables
 */
function validateEnvironment() {
  const missingVars = requiredEnvVars.filter(varName => !process.env[varName]);
  
  if (missingVars.length > 0) {
    throw new Error(`Missing required environment variables: ${missingVars.join(', ')}`);
  }
}

/**
 * Get environment configuration with defaults
 */
function getEnvironmentConfig() {
  validateEnvironment();
  
  const config = {
    // Required variables
    supabase: {
      url: process.env.SUPABASE_URL,
      anonKey: process.env.SUPABASE_ANON_KEY,
      serviceRoleKey: process.env.SUPABASE_SERVICE_ROLE_KEY
    },
    
    // Authentication
    jwt: {
      secret: process.env.JWT_SECRET,
      expiresIn: process.env.JWT_EXPIRES_IN || '24h'
    },
    
    // AI Services
    ai: {
      googleApiKey: process.env.GOOGLE_AI_API_KEY
    },
    
    // Server configuration
    server: {
      port: parseInt(process.env.PORT) || optionalEnvVars.PORT,
      nodeEnv: process.env.NODE_ENV || optionalEnvVars.NODE_ENV
    },
    
    // CORS configuration
    cors: {
      allowedOrigins: (process.env.CORS_ORIGIN || optionalEnvVars.CORS_ORIGIN).split(',').map(origin => origin.trim())
    },
    
    // Logging
    logging: {
      level: process.env.LOG_LEVEL || optionalEnvVars.LOG_LEVEL
    },
    
    // Rate limiting
    rateLimit: {
      windowMs: parseInt(process.env.RATE_LIMIT_WINDOW_MS) || optionalEnvVars.RATE_LIMIT_WINDOW_MS,
      maxRequests: parseInt(process.env.RATE_LIMIT_MAX_REQUESTS) || optionalEnvVars.RATE_LIMIT_MAX_REQUESTS
    },
    
    // File upload
    upload: {
      maxSize: parseInt(process.env.UPLOAD_MAX_SIZE) || optionalEnvVars.UPLOAD_MAX_SIZE,
      allowedTypes: ['application/pdf', 'application/msword', 'application/vnd.openxmlformats-officedocument.wordprocessingml.document']
    },
    
    // Session
    session: {
      secret: process.env.SESSION_SECRET || optionalEnvVars.SESSION_SECRET
    },
    
    // Phase 5 - Cache Configuration
    cache: {
      redisUrl: process.env.REDIS_URL || 'redis://localhost:6379',
      enabled: process.env.CACHE_ENABLED === 'true', // Default to false (in-memory only)
      fallbackToMemory: true // Always enable memory fallback
    },
    
    // Phase 5 - Security Configuration
    security: {
      monitoringAccessKey: process.env.MONITORING_ACCESS_KEY || optionalEnvVars.MONITORING_ACCESS_KEY,
      headersEnabled: process.env.SECURITY_HEADERS_ENABLED === 'true' || optionalEnvVars.SECURITY_HEADERS_ENABLED === 'true',
      inputSanitizationEnabled: process.env.INPUT_SANITIZATION_ENABLED === 'true' || optionalEnvVars.INPUT_SANITIZATION_ENABLED === 'true',
      sqlInjectionPreventionEnabled: process.env.SQL_INJECTION_PREVENTION_ENABLED === 'true' || optionalEnvVars.SQL_INJECTION_PREVENTION_ENABLED === 'true',
      xssPreventionEnabled: process.env.XSS_PREVENTION_ENABLED === 'true' || optionalEnvVars.XSS_PREVENTION_ENABLED === 'true',
      requestSizeLimit: process.env.REQUEST_SIZE_LIMIT || optionalEnvVars.REQUEST_SIZE_LIMIT
    },
    
    // Phase 5 - Performance Configuration
    performance: {
      compressionEnabled: process.env.COMPRESSION_ENABLED === 'true' || optionalEnvVars.COMPRESSION_ENABLED === 'true',
      monitoringEnabled: process.env.PERFORMANCE_MONITORING_ENABLED === 'true' || optionalEnvVars.PERFORMANCE_MONITORING_ENABLED === 'true',
      slowQueryThreshold: parseInt(process.env.SLOW_QUERY_THRESHOLD) || optionalEnvVars.SLOW_QUERY_THRESHOLD,
      databaseOptimization: {
        connectionPoolSize: 10,
        queryTimeout: 30000,
        batchSize: 100
      }
    },
    
    // Phase 5 - Monitoring Configuration
    monitoring: {
      enabled: process.env.MONITORING_ENABLED === 'true' || optionalEnvVars.MONITORING_ENABLED === 'true',
      metricsRetentionHours: parseInt(process.env.METRICS_RETENTION_HOURS) || optionalEnvVars.METRICS_RETENTION_HOURS,
      alertThresholds: {
        responseTime: parseInt(process.env.ALERT_THRESHOLD_RESPONSE_TIME) || optionalEnvVars.ALERT_THRESHOLD_RESPONSE_TIME,
        errorRate: parseFloat(process.env.ALERT_THRESHOLD_ERROR_RATE) || optionalEnvVars.ALERT_THRESHOLD_ERROR_RATE,
        memoryUsage: parseFloat(process.env.ALERT_THRESHOLD_MEMORY_USAGE) || optionalEnvVars.ALERT_THRESHOLD_MEMORY_USAGE,
        cpuUsage: parseFloat(process.env.ALERT_THRESHOLD_CPU_USAGE) || optionalEnvVars.ALERT_THRESHOLD_CPU_USAGE
      },
      dashboard: {
        refreshInterval: 5000,
        realtimeUpdates: true,
        logRetention: true
      }
    }
  };
  
  return config;
}

/**
 * Check if running in development mode
 */
function isDevelopment() {
  return process.env.NODE_ENV === 'development';
}

/**
 * Check if running in production mode
 */
function isProduction() {
  return process.env.NODE_ENV === 'production';
}

/**
 * Check if running in test mode
 */
function isTest() {
  return process.env.NODE_ENV === 'test';
}

/**
 * Get configuration for a specific environment
 */
function getConfigForEnvironment(env) {
  const originalEnv = process.env.NODE_ENV;
  process.env.NODE_ENV = env;
  const config = getEnvironmentConfig();
  process.env.NODE_ENV = originalEnv;
  return config;
}

/**
 * Phase 5 - Get cache configuration
 */
function getCacheConfig() {
  const config = getEnvironmentConfig();
  return config.cache;
}

/**
 * Phase 5 - Get security configuration
 */
function getSecurityConfig() {
  const config = getEnvironmentConfig();
  return config.security;
}

/**
 * Phase 5 - Get performance configuration
 */
function getPerformanceConfig() {
  const config = getEnvironmentConfig();
  return config.performance;
}

/**
 * Phase 5 - Get monitoring configuration
 */
function getMonitoringConfig() {
  const config = getEnvironmentConfig();
  return config.monitoring;
}

module.exports = {
  getEnvironmentConfig,
  validateEnvironment,
  isDevelopment,
  isProduction,
  isTest,
  getConfigForEnvironment,
  getCacheConfig,
  getSecurityConfig,
  getPerformanceConfig,
  getMonitoringConfig
};
````

## File: src/config/logger.js
````javascript
/**
 * Logger Configuration
 * Configures Winston logger with structured logging and different transports
 */

const winston = require('winston');
const path = require('path');
const { getEnvironmentConfig, isDevelopment, isProduction } = require('./environment');

/**
 * Custom log format for structured logging
 */
const logFormat = winston.format.combine(
  winston.format.timestamp({
    format: 'YYYY-MM-DD HH:mm:ss'
  }),
  winston.format.errors({ stack: true }),
  winston.format.json(),
  winston.format.printf(({ timestamp, level, message, stack, ...meta }) => {
    let log = `${timestamp} [${level.toUpperCase()}]: ${message}`;
    
    if (stack) {
      log += `\n${stack}`;
    }
    
    if (Object.keys(meta).length > 0) {
      log += `\n${JSON.stringify(meta, null, 2)}`;
    }
    
    return log;
  })
);

/**
 * Console transport configuration
 */
const consoleTransport = new winston.transports.Console({
  format: winston.format.combine(
    winston.format.colorize(),
    winston.format.simple(),
    winston.format.printf(({ timestamp, level, message, stack, ...meta }) => {
      let log = `${timestamp} [${level}]: ${message}`;
      
      if (stack) {
        log += `\n${stack}`;
      }
      
      if (Object.keys(meta).length > 0) {
        log += `\n${JSON.stringify(meta, null, 2)}`;
      }
      
      return log;
    })
  )
});

/**
 * File transport configuration for errors
 */
const errorFileTransport = new winston.transports.File({
  filename: path.join(__dirname, '../../logs/error.log'),
  level: 'error',
  format: logFormat,
  maxsize: 5242880, // 5MB
  maxFiles: 5,
  tailable: true
});

/**
 * File transport configuration for combined logs
 */
const combinedFileTransport = new winston.transports.File({
  filename: path.join(__dirname, '../../logs/combined.log'),
  format: logFormat,
  maxsize: 5242880, // 5MB
  maxFiles: 5,
  tailable: true
});

/**
 * Create logger instance
 */
function createLogger() {
  const config = getEnvironmentConfig();
  
  const transports = [];
  
  // Always add console transport
  transports.push(consoleTransport);
  
  // Add file transports in production
  if (isProduction()) {
    transports.push(errorFileTransport);
    transports.push(combinedFileTransport);
  }
  
  const logger = winston.createLogger({
    level: config.logging.level,
    format: logFormat,
    defaultMeta: { 
      service: 'immigrow-ai-backend',
      version: process.env.npm_package_version || '1.0.0'
    },
    transports,
    exitOnError: false
  });
  
  // Handle uncaught exceptions
  logger.exceptions.handle(
    new winston.transports.File({
      filename: path.join(__dirname, '../../logs/exceptions.log'),
      format: logFormat
    })
  );
  
  // Handle unhandled promise rejections
  logger.rejections.handle(
    new winston.transports.File({
      filename: path.join(__dirname, '../../logs/rejections.log'),
      format: logFormat
    })
  );
  
  return logger;
}

/**
 * Create request logger middleware
 */
function createRequestLogger() {
  const logger = createLogger();
  
  return (req, res, next) => {
    const start = Date.now();
    
    // Log request
    logger.info('Incoming request', {
      method: req.method,
      url: req.url,
      ip: req.ip,
      userAgent: req.get('User-Agent'),
      userId: req.user?.id || 'anonymous'
    });
    
    // Override res.end to log response
    const originalEnd = res.end;
    res.end = function(chunk, encoding) {
      const duration = Date.now() - start;
      
      logger.info('Request completed', {
        method: req.method,
        url: req.url,
        statusCode: res.statusCode,
        duration: `${duration}ms`,
        contentLength: res.get('Content-Length'),
        userId: req.user?.id || 'anonymous'
      });
      
      originalEnd.call(this, chunk, encoding);
    };
    
    next();
  };
}

/**
 * Create error logger
 */
function createErrorLogger() {
  const logger = createLogger();
  
  return (error, req, res, next) => {
    logger.error('Application error', {
      error: {
        message: error.message,
        stack: error.stack,
        name: error.name,
        code: error.code
      },
      request: {
        method: req.method,
        url: req.url,
        ip: req.ip,
        userId: req.user?.id || 'anonymous'
      },
      userAgent: req.get('User-Agent')
    });
    
    next(error);
  };
}

/**
 * Performance logger
 */
function createPerformanceLogger() {
  const logger = createLogger();
  
  return (operation, duration, metadata = {}) => {
    const level = duration > 1000 ? 'warn' : 'info';
    
    logger.log(level, 'Performance measurement', {
      operation,
      duration: `${duration}ms`,
      ...metadata
    });
  };
}

/**
 * Security logger
 */
function createSecurityLogger() {
  const logger = createLogger();
  
  return (event, details = {}) => {
    logger.warn('Security event', {
      event,
      timestamp: new Date().toISOString(),
      ...details
    });
  };
}

/**
 * Database logger
 */
function createDatabaseLogger() {
  const logger = createLogger();
  
  return (operation, query, duration, error = null) => {
    const logData = {
      operation,
      query: query?.substring(0, 200) + (query?.length > 200 ? '...' : ''),
      duration: `${duration}ms`
    };
    
    if (error) {
      logData.error = {
        message: error.message,
        code: error.code
      };
      logger.error('Database operation failed', logData);
    } else {
      logger.info('Database operation completed', logData);
    }
  };
}

// Create default logger instance
const logger = createLogger();

module.exports = {
  createLogger,
  createRequestLogger,
  createErrorLogger,
  createPerformanceLogger,
  createSecurityLogger,
  createDatabaseLogger,
  logger
};
````

## File: src/controllers/BaseController.js
````javascript
const { logger } = require('../config/logger');
const { AppError } = require('../utils/errors');
const ResponseFormatter = require('../utils/responseFormatter');

/**
 * Base Controller class providing common controller functionality
 * All specific controllers should extend this class
 */
class BaseController {
  constructor(services = {}) {
    this.services = services;
    this.logger = logger;
  }

  /**
   * Get a service by name
   * @param {string} serviceName - Name of the service
   * @returns {Object} Service instance
   */
  getService(serviceName) {
    const service = this.services[serviceName];
    if (!service) {
      throw new AppError(`Service '${serviceName}' not found`, 500);
    }
    return service;
  }

  /**
   * Log controller method entry
   * @param {string} methodName - Name of the method being called
   * @param {Object} params - Method parameters
   */
  logMethodEntry(methodName, params = {}) {
    this.logger.info(`Controller method entry: ${methodName}`, {
      method: methodName,
      params: this.sanitizeParams(params),
      timestamp: new Date().toISOString()
    });
  }

  /**
   * Log controller method success
   * @param {string} methodName - Name of the method
   * @param {Object} result - Method result
   */
  logMethodSuccess(methodName, result = {}) {
    this.logger.info(`Controller method success: ${methodName}`, {
      method: methodName,
      resultCount: Array.isArray(result) ? result.length : 1,
      timestamp: new Date().toISOString()
    });
  }

  /**
   * Log controller method error
   * @param {string} methodName - Name of the method
   * @param {Error} error - Error object
   */
  logMethodError(methodName, error) {
    this.logger.error(`Controller method error: ${methodName}`, {
      method: methodName,
      error: error.message,
      stack: error.stack,
      timestamp: new Date().toISOString()
    });
  }

  /**
   * Sanitize parameters for logging
   * @param {Object} params - Parameters to sanitize
   * @returns {Object} Sanitized parameters
   */
  sanitizeParams(params) {
    const sanitized = { ...params };
    const sensitiveFields = ['password', 'token', 'secret', 'key', 'authorization'];
    
    sensitiveFields.forEach(field => {
      if (sanitized[field]) {
        sanitized[field] = '[REDACTED]';
      }
    });
    
    return sanitized;
  }

  /**
   * Validate required parameters
   * @param {Object} req - Express request object
   * @param {Array} requiredParams - Array of required parameter names
   * @param {string} source - Source of parameters ('body', 'query', 'params')
   */
  validateRequiredParams(req, requiredParams, source = 'body') {
    const params = req[source] || {};
    const missing = requiredParams.filter(param => !params[param]);
    
    if (missing.length > 0) {
      throw new AppError(`Missing required parameters: ${missing.join(', ')}`, 400);
    }
  }

  /**
   * Validate user ID from request
   * @param {Object} req - Express request object
   * @returns {string} User ID
   */
  validateUserId(req) {
    const userId = req.user?.id || req.body.userId || req.params.userId;
    if (!userId) {
      throw new AppError('User ID is required', 400);
    }
    return userId;
  }

  /**
   * Check if request is authenticated
   * @param {Object} req - Express request object
   * @returns {boolean} Whether request is authenticated
   */
  isAuthenticated(req) {
    return !!(req.user && req.user.id);
  }

  /**
   * Extract user ID from request
   * @param {Object} req - Express request object
   * @returns {string} User ID
   */
  extractUserId(req) {
    return req.user?.id || req.body.userId || req.params.userId;
  }

  /**
   * Execute controller method with error handling and logging
   * @param {string} methodName - Name of the method
   * @param {Function} method - Method to execute
   * @returns {Function} Express middleware function
   */
  executeMethod(methodName, method) {
    return async (req, res, next) => {
      try {
        this.logMethodEntry(methodName, {
          body: req.body,
          query: req.query,
          params: req.params,
          user: req.user ? { id: req.user.id } : null
        });

        const result = await method(req, res, next);
        
        this.logMethodSuccess(methodName, result);
        
        return result;
      } catch (error) {
        this.logMethodError(methodName, error);
        next(error);
      }
    };
  }

  /**
   * Send success response with version-aware formatting
   * @param {Object} res - Express response object
   * @param {Object} data - Response data
   * @param {Object} options - Response options
   */
  sendSuccessResponse(res, data, options = {}) {
    const {
      message = 'Success',
      statusCode = 200,
      meta = {},
      pagination = null
    } = options;

    const version = res.req.apiVersion || 'v1';
    
    // Format response based on version
    const formattedResponse = ResponseFormatter.formatSuccess(data, version, {
      message,
      meta,
      pagination
    });

    // Add version-specific headers
    ResponseFormatter.addResponseHeaders(res, version);

    res.status(statusCode).json(formattedResponse);
  }

  /**
   * Send error response with version-aware formatting
   * @param {Object} res - Express response object
   * @param {Error} error - Error object
   * @param {Object} options - Response options
   */
  sendErrorResponse(res, error, options = {}) {
    const {
      statusCode = 500,
      includeStack = false
    } = options;

    const version = res.req.apiVersion || 'v1';
    
    // Format error response based on version
    const formattedError = ResponseFormatter.formatError(error, version, {
      statusCode,
      includeStack
    });

    // Add version-specific headers
    ResponseFormatter.addResponseHeaders(res, version);

    res.status(statusCode).json(formattedError);
  }

  /**
   * Send paginated response with version-aware formatting
   * @param {Object} res - Express response object
   * @param {Array} data - Data array
   * @param {Object} pagination - Pagination info
   * @param {Object} options - Response options
   */
  sendPaginatedResponse(res, data, pagination, options = {}) {
    const {
      message = 'Success',
      statusCode = 200,
      meta = {}
    } = options;

    const version = res.req.apiVersion || 'v1';
    
    // Format paginated response based on version
    const formattedResponse = ResponseFormatter.formatPagination(data, pagination, version);
    
    // Add additional fields
    formattedResponse.message = message;
    if (meta && Object.keys(meta).length > 0) {
      formattedResponse.meta = meta;
    }

    // Add version-specific headers
    ResponseFormatter.addResponseHeaders(res, version);

    res.status(statusCode).json(formattedResponse);
  }

  /**
   * Send validation error response
   * @param {Object} res - Express response object
   * @param {Array} validationErrors - Validation errors array
   */
  sendValidationError(res, validationErrors) {
    const version = res.req.apiVersion || 'v1';
    
    const formattedError = ResponseFormatter.formatValidationError(validationErrors, version);
    
    // Add version-specific headers
    ResponseFormatter.addResponseHeaders(res, version);

    res.status(400).json(formattedError);
  }

  /**
   * Send not found error response
   * @param {Object} res - Express response object
   * @param {string} resource - Resource name
   */
  sendNotFoundError(res, resource) {
    const version = res.req.apiVersion || 'v1';
    
    const formattedError = ResponseFormatter.formatNotFoundError(resource, version);
    
    // Add version-specific headers
    ResponseFormatter.addResponseHeaders(res, version);

    res.status(404).json(formattedError);
  }

  /**
   * Send unauthorized error response
   * @param {Object} res - Express response object
   * @param {string} message - Error message
   */
  sendUnauthorizedError(res, message = 'Unauthorized') {
    const version = res.req.apiVersion || 'v1';
    
    const formattedError = ResponseFormatter.formatUnauthorizedError(message, version);
    
    // Add version-specific headers
    ResponseFormatter.addResponseHeaders(res, version);

    res.status(401).json(formattedError);
  }

  /**
   * Send forbidden error response
   * @param {Object} res - Express response object
   * @param {string} message - Error message
   */
  sendForbiddenError(res, message = 'Forbidden') {
    const version = res.req.apiVersion || 'v1';
    
    const formattedError = ResponseFormatter.formatForbiddenError(message, version);
    
    // Add version-specific headers
    ResponseFormatter.addResponseHeaders(res, version);

    res.status(403).json(formattedError);
  }

  /**
   * Create paginated response object
   * @param {Array} data - Data array
   * @param {number} page - Current page
   * @param {number} limit - Items per page
   * @param {number} total - Total items
   * @returns {Object} Paginated response object
   */
  createPaginatedResponse(data, page, limit, total) {
    const pages = Math.ceil(total / limit);
    
    return {
      data,
      pagination: {
        page,
        limit,
        total,
        pages
      }
    };
  }

  /**
   * Transform database record to API response format
   * @param {Object} record - Database record
   * @returns {Object} Transformed record
   */
  transformRecord(record) {
    if (!record) return null;
    
    // Transform snake_case to camelCase
    const transformed = {};
    Object.keys(record).forEach(key => {
      const camelKey = key.replace(/_([a-z])/g, (_, letter) => letter.toUpperCase());
      transformed[camelKey] = record[key];
    });
    
    return transformed;
  }

  /**
   * Transform array of database records to API response format
   * @param {Array} records - Array of database records
   * @returns {Array} Transformed records
   */
  transformRecords(records) {
    if (!Array.isArray(records)) return [];
    return records.map(record => this.transformRecord(record));
  }

  /**
   * Check if user has permission to access resource
   * @param {Object} req - Express request object
   * @param {string} resourceId - Resource ID
   * @param {string} resourceType - Type of resource
   * @returns {boolean} Whether user has permission
   */
  hasPermission(req, resourceId, resourceType = 'resource') {
    const userId = this.extractUserId(req);
    
    // Admin users have all permissions
    if (req.user && req.user.role === 'admin') {
      return true;
    }
    
    // Users can only access their own resources
    return userId === resourceId;
  }

  /**
   * Sanitize search criteria
   * @param {Object} criteria - Search criteria
   * @returns {Object} Sanitized criteria
   */
  sanitizeSearchCriteria(criteria) {
    const sanitized = {};
    const allowedFields = ['query', 'status', 'category', 'dateFrom', 'dateTo'];
    
    Object.keys(criteria).forEach(key => {
      if (allowedFields.includes(key) && criteria[key] !== undefined && criteria[key] !== null) {
        sanitized[key] = criteria[key];
      }
    });
    
    return sanitized;
  }

  /**
   * Validate pagination options
   * @param {Object} options - Pagination options
   * @returns {Object} Validated pagination options
   */
  validatePaginationOptions(options) {
    const { page = 1, limit = 10 } = options;
    
    return {
      page: Math.max(1, parseInt(page) || 1),
      limit: Math.min(100, Math.max(1, parseInt(limit) || 10))
    };
  }
}

module.exports = BaseController;
````

## File: src/controllers/ControllerFactory.js
````javascript
const { UserController, ResumeController } = require('./');
const ServiceFactory = require('../services/ServiceFactory');

/**
 * Controller Factory for creating and managing controller instances
 * This factory ensures proper dependency injection and singleton patterns
 */
class ControllerFactory {
  constructor() {
    this.controllers = new Map();
    this.initialized = false;
  }

  /**
   * Initialize the controller factory with services
   */
  async initialize() {
    if (this.initialized) {
      return;
    }

    try {
      // Initialize service factory first
      await ServiceFactory.initialize();
      
      // Get all services
      const services = ServiceFactory.getAllServices();
      
      // Initialize controllers
      await this.initializeControllers(services);
      
      this.initialized = true;
    } catch (error) {
      throw new Error(`Failed to initialize ControllerFactory: ${error.message}`);
    }
  }

  /**
   * Initialize all controllers with their required services
   * @param {Object} services - All available services
   */
  async initializeControllers(services) {
    // Create controller instances with services
    const userController = new UserController(services);
    const resumeController = new ResumeController(services);

    // Store controllers
    this.controllers.set('user', userController);
    this.controllers.set('resume', resumeController);
  }

  /**
   * Get a controller by name
   * @param {string} controllerName - Name of the controller
   * @returns {Object} Controller instance
   */
  getController(controllerName) {
    if (!this.initialized) {
      throw new Error('ControllerFactory not initialized. Call initialize() first.');
    }

    const controller = this.controllers.get(controllerName);
    if (!controller) {
      throw new Error(`Controller '${controllerName}' not found`);
    }

    return controller;
  }

  /**
   * Get all controllers as an object
   * @returns {Object} All controllers
   */
  getAllControllers() {
    if (!this.initialized) {
      throw new Error('ControllerFactory not initialized. Call initialize() first.');
    }

    const controllers = {};
    for (const [name, controller] of this.controllers) {
      controllers[name] = controller;
    }

    return controllers;
  }

  /**
   * Check if a controller exists
   * @param {string} controllerName - Name of the controller
   * @returns {boolean} Whether the controller exists
   */
  hasController(controllerName) {
    return this.controllers.has(controllerName);
  }

  /**
   * Get list of available controller names
   * @returns {Array} Array of controller names
   */
  getAvailableControllers() {
    return Array.from(this.controllers.keys());
  }

  /**
   * Reset the factory (useful for testing)
   */
  reset() {
    this.controllers.clear();
    this.initialized = false;
  }

  /**
   * Health check for all controllers
   * @returns {Object} Health status
   */
  async healthCheck() {
    if (!this.initialized) {
      return {
        status: 'error',
        message: 'ControllerFactory not initialized',
        controllers: {},
        services: {},
        timestamp: new Date().toISOString()
      };
    }

    const health = {
      status: 'healthy',
      message: 'All controllers and services are healthy',
      controllers: {},
      services: {},
      timestamp: new Date().toISOString()
    };

    // Check services first
    try {
      const serviceHealth = await ServiceFactory.healthCheck();
      health.services = serviceHealth;
      
      if (serviceHealth.status !== 'healthy') {
        health.status = serviceHealth.status;
        health.message = serviceHealth.message;
      }
    } catch (error) {
      health.services = {
        status: 'error',
        error: error.message
      };
      health.status = 'error';
      health.message = 'Service health check failed';
    }

    // Check controllers
    for (const [name, controller] of this.controllers) {
      try {
        // Simple health check - check if controller has required services
        const hasServices = controller.services && Object.keys(controller.services).length > 0;
        health.controllers[name] = { 
          status: hasServices ? 'healthy' : 'warning',
          message: hasServices ? 'Controller is healthy' : 'Controller has no services'
        };
        
        if (!hasServices) {
          health.status = health.status === 'error' ? 'error' : 'warning';
          health.message = health.status === 'error' ? health.message : 'Some controllers have warnings';
        }
      } catch (error) {
        health.controllers[name] = { 
          status: 'error', 
          error: error.message 
        };
        health.status = 'error';
        health.message = 'Some controllers are unhealthy';
      }
    }

    return health;
  }

  /**
   * Get controller routes for Express router setup
   * @returns {Object} Routes configuration
   */
  getRoutes() {
    if (!this.initialized) {
      throw new Error('ControllerFactory not initialized. Call initialize() first.');
    }

    const routes = {};

    // User routes
    routes.user = {
      controller: this.getController('user'),
      routes: [
        { method: 'POST', path: '/find-or-create', handler: 'findOrCreateUser' },
        { method: 'GET', path: '/profile', handler: 'getCurrentUserProfile' },
        { method: 'PUT', path: '/profile', handler: 'updateCurrentUserProfile' },
        { method: 'GET', path: '/:userId', handler: 'getUserById' },
        { method: 'PUT', path: '/:userId', handler: 'updateUser' },
        { method: 'DELETE', path: '/:userId', handler: 'deleteUser' },
        { method: 'GET', path: '/email/:email', handler: 'getUserByEmail' },
        { method: 'GET', path: '/search', handler: 'searchUsers' },
        { method: 'GET', path: '/', handler: 'getUsers' },
        { method: 'GET', path: '/role/:roleId', handler: 'getUsersByRole' },
        { method: 'GET', path: '/status/:status', handler: 'getUsersByStatusInCanada' },
        { method: 'GET', path: '/country/:country', handler: 'getUsersByCountryOfOrigin' },
        { method: 'GET', path: '/location/:location', handler: 'getUsersByCurrentLocation' },
        { method: 'GET', path: '/statistics', handler: 'getUserStatistics' },
        { method: 'GET', path: '/:userId/exists', handler: 'userExists' },
        { method: 'GET', path: '/count', handler: 'getUserCount' }
      ]
    };

    // Resume routes
    routes.resume = {
      controller: this.getController('resume'),
      routes: [
        { method: 'POST', path: '/analysis', handler: 'saveResumeAnalysis' },
        { method: 'POST', path: '/upload', handler: 'uploadAndAnalyzeResume' },
        { method: 'GET', path: '/analyses', handler: 'getUserResumeAnalyses' },
        { method: 'GET', path: '/analyses/latest', handler: 'getLatestResumeAnalysis' },
        { method: 'GET', path: '/analyses/count', handler: 'getResumeAnalysisCount' },
        { method: 'GET', path: '/analyses/statistics', handler: 'getResumeAnalysisStatistics' },
        { method: 'GET', path: '/analyses/search', handler: 'searchResumeAnalyses' },
        { method: 'GET', path: '/analyses/:analysisId', handler: 'getResumeAnalysisById' },
        { method: 'GET', path: '/analyses/:analysisId/parsed', handler: 'getResumeAnalysisWithParsedData' },
        { method: 'PUT', path: '/analyses/:analysisId', handler: 'updateResumeAnalysis' },
        { method: 'DELETE', path: '/analyses/:analysisId', handler: 'deleteResumeAnalysis' },
        { method: 'DELETE', path: '/analyses/bulk', handler: 'bulkDeleteResumeAnalyses' },
        { method: 'GET', path: '/analyses/user/:userId', handler: 'getResumeAnalysesByUserId' }
      ]
    };

    return routes;
  }
}

// Create singleton instance
const controllerFactory = new ControllerFactory();

module.exports = controllerFactory;
````

## File: src/controllers/index.js
````javascript
/**
 * Controller exports
 * This file exports all controller classes and the ControllerFactory for easy importing
 */

const BaseController = require('./BaseController');
const UserController = require('./UserController');
const ResumeController = require('./ResumeController');
const ControllerFactory = require('./ControllerFactory');

module.exports = {
  BaseController,
  UserController,
  ResumeController,
  ControllerFactory
};
````

## File: src/controllers/ResumeController.js
````javascript
const BaseController = require('./BaseController');
const { AppError } = require('../utils/errors');

/**
 * Resume Controller for resume analysis-related HTTP requests
 */
class ResumeController extends BaseController {
  constructor(services) {
    super(services);
    this.resumeService = this.getService('resume');
    this.canadianResumeService = this.getService('canadianResume');
  }

  /**
   * Save resume analysis
   * POST /api/resumes/analysis
   */
  async saveResumeAnalysis(req, res, next) {
    return this.executeMethod('saveResumeAnalysis', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      this.validateRequiredParams(req, ['originalFileName'], 'body');

      const userId = this.extractUserId(req);
      const analysisData = {
        originalFileName: req.body.originalFileName,
        rawText: req.body.rawText,
        extractedText: req.body.extractedText,
        structuredData: req.body.structuredData,
        confidenceScores: req.body.confidenceScores,
        canadianMarketAnalysis: req.body.canadianMarketAnalysis,
        personalInfo: req.body.personalInfo,
        professionalSummary: req.body.professionalSummary,
        skills: req.body.skills,
        workExperience: req.body.workExperience,
        education: req.body.education,
        certifications: req.body.certifications,
        projects: req.body.projects,
        metadata: req.body.metadata,
        processingMethod: req.body.processingMethod
      };

      const analysis = await this.resumeService.saveResumeAnalysis(userId, analysisData);
      return this.sendSuccess(res, analysis, 201, 'Resume analysis saved successfully');
    }, req, res, next);
  }

  /**
   * Get user's resume analyses
   * GET /api/resumes/analyses
   */
  async getUserResumeAnalyses(req, res, next) {
    return this.executeMethod('getUserResumeAnalyses', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const useServiceRole = false;
      const analyses = await this.resumeService.getUserResumeAnalyses(userId, useServiceRole);
      
      return this.sendSuccess(res, analyses, 200, 'Resume analyses retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get resume analysis by ID
   * GET /api/resumes/analyses/:analysisId
   */
  async getResumeAnalysisById(req, res, next) {
    return this.executeMethod('getResumeAnalysisById', async (req, res, next) => {
      const analysisId = req.params.analysisId;
      if (!analysisId) {
        throw new AppError('Analysis ID is required', 400);
      }

      const userId = this.isAuthenticated(req) ? this.extractUserId(req) : null;
      const useServiceRole = this.isAdmin(req);
      
      const analysis = await this.resumeService.getResumeAnalysisById(analysisId, userId, useServiceRole);
      
      if (!analysis) {
        throw new AppError('Resume analysis not found', 404);
      }

      return this.sendSuccess(res, analysis, 200, 'Resume analysis retrieved successfully');
    }, req, res, next);
  }

  /**
   * Update resume analysis
   * PUT /api/resumes/analyses/:analysisId
   */
  async updateResumeAnalysis(req, res, next) {
    return this.executeMethod('updateResumeAnalysis', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const analysisId = req.params.analysisId;
      if (!analysisId) {
        throw new AppError('Analysis ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const updateData = {
        originalFileName: req.body.originalFileName,
        extractedText: req.body.extractedText,
        structuredData: req.body.structuredData,
        confidenceScores: req.body.confidenceScores,
        canadianMarketAnalysis: req.body.canadianMarketAnalysis,
        personalInfo: req.body.personalInfo,
        professionalSummary: req.body.professionalSummary,
        skills: req.body.skills,
        workExperience: req.body.workExperience,
        education: req.body.education,
        certifications: req.body.certifications,
        projects: req.body.projects,
        metadata: req.body.metadata,
        processingMethod: req.body.processingMethod
      };

      const useServiceRole = this.isAdmin(req);
      const analysis = await this.resumeService.updateResumeAnalysis(analysisId, userId, updateData, useServiceRole);
      
      return this.sendSuccess(res, analysis, 200, 'Resume analysis updated successfully');
    }, req, res, next);
  }

  /**
   * Delete resume analysis
   * DELETE /api/resumes/analyses/:analysisId
   */
  async deleteResumeAnalysis(req, res, next) {
    return this.executeMethod('deleteResumeAnalysis', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const analysisId = req.params.analysisId;
      if (!analysisId) {
        throw new AppError('Analysis ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const useServiceRole = this.isAdmin(req);
      const success = await this.resumeService.deleteResumeAnalysis(analysisId, userId, useServiceRole);
      
      if (!success) {
        throw new AppError('Failed to delete resume analysis', 500);
      }

      return this.sendSuccess(res, null, 200, 'Resume analysis deleted successfully');
    }, req, res, next);
  }

  /**
   * Search resume analyses
   * GET /api/resumes/analyses/search
   */
  async searchResumeAnalyses(req, res, next) {
    return this.executeMethod('searchResumeAnalyses', async (req, res, next) => {
      // Only admins can search all analyses
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const allowedFields = ['userId', 'fileName', 'processingMethod', 'createdAfter', 'createdBefore'];
      const criteria = this.extractSearchParams(req, allowedFields);
      const pagination = this.extractPaginationParams(req);
      const sortOptions = this.extractSortParams(req, ['fileName', 'createdAt', 'processingMethod'], 'createdAt', 'desc');

      const options = {
        ...pagination,
        ...sortOptions
      };

      const useServiceRole = true;
      const analyses = await this.resumeService.searchResumeAnalyses(criteria, options, useServiceRole);
      
      return this.sendSuccess(res, analyses, 200, 'Resume analyses retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get resume analyses with pagination
   * GET /api/resumes/analyses
   */
  async getResumeAnalysesWithPagination(req, res, next) {
    return this.executeMethod('getResumeAnalysesWithPagination', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const pagination = this.extractPaginationParams(req);
      const sortOptions = this.extractSortParams(req, ['fileName', 'createdAt', 'processingMethod'], 'createdAt', 'desc');

      const options = {
        ...pagination,
        ...sortOptions
      };

      const useServiceRole = this.isAdmin(req);
      const result = await this.resumeService.getResumeAnalysesWithPagination(userId, options, useServiceRole);
      
      return this.sendPaginatedResponse(res, result.analyses, result.pagination, 'Resume analyses retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get resume analysis statistics
   * GET /api/resumes/analyses/statistics
   */
  async getResumeAnalysisStatistics(req, res, next) {
    return this.executeMethod('getResumeAnalysisStatistics', async (req, res, next) => {
      // Only admins can view statistics
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const useServiceRole = true;
      const statistics = await this.resumeService.getResumeAnalysisStatistics(useServiceRole);
      
      return this.sendSuccess(res, statistics, 200, 'Resume analysis statistics retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get resume analysis count for user
   * GET /api/resumes/analyses/count
   */
  async getResumeAnalysisCount(req, res, next) {
    return this.executeMethod('getResumeAnalysisCount', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const useServiceRole = this.isAdmin(req);
      const count = await this.resumeService.getResumeAnalysisCount(userId, useServiceRole);
      
      return this.sendSuccess(res, { count }, 200, 'Resume analysis count retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get latest resume analysis for user
   * GET /api/resumes/analyses/latest
   */
  async getLatestResumeAnalysis(req, res, next) {
    return this.executeMethod('getLatestResumeAnalysis', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const useServiceRole = this.isAdmin(req);
      const analysis = await this.resumeService.getLatestResumeAnalysis(userId, useServiceRole);
      
      if (!analysis) {
        throw new AppError('No resume analysis found', 404);
      }

      return this.sendSuccess(res, analysis, 200, 'Latest resume analysis retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get resume analysis with parsed data
   * GET /api/resumes/analyses/:analysisId/parsed
   */
  async getResumeAnalysisWithParsedData(req, res, next) {
    return this.executeMethod('getResumeAnalysisWithParsedData', async (req, res, next) => {
      const analysisId = req.params.analysisId;
      if (!analysisId) {
        throw new AppError('Analysis ID is required', 400);
      }

      const userId = this.isAuthenticated(req) ? this.extractUserId(req) : null;
      const useServiceRole = this.isAdmin(req);
      
      const analysis = await this.resumeService.getResumeAnalysisWithParsedData(analysisId, userId, useServiceRole);
      
      if (!analysis) {
        throw new AppError('Resume analysis not found', 404);
      }

      return this.sendSuccess(res, analysis, 200, 'Resume analysis with parsed data retrieved successfully');
    }, req, res, next);
  }

  /**
   * Upload and analyze resume
   * POST /api/resumes/upload
   */
  async uploadAndAnalyzeResume(req, res, next) {
    return this.executeMethod('uploadAndAnalyzeResume', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      // Validate file upload
      const allowedTypes = ['application/pdf', 'application/msword', 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'];
      const maxSize = 10 * 1024 * 1024; // 10MB
      const fileInfo = this.validateFileUpload(req, allowedTypes, maxSize);

      const userId = this.extractUserId(req);
      
      // TODO: Integrate with AI service for resume analysis
      // For now, create a basic analysis record
      const analysisData = {
        originalFileName: fileInfo.originalName,
        rawText: 'Text extracted from uploaded resume',
        processingMethod: 'file_upload',
        metadata: {
          uploadedFile: fileInfo.filename,
          fileSize: fileInfo.size,
          mimeType: fileInfo.mimetype
        }
      };

      const analysis = await this.resumeService.saveResumeAnalysis(userId, analysisData);
      
      return this.sendSuccess(res, {
        analysis,
        fileInfo: {
          originalName: fileInfo.originalName,
          filename: fileInfo.filename,
          size: fileInfo.size
        }
      }, 201, 'Resume uploaded and analysis started successfully');
    }, req, res, next);
  }

  /**
   * Get resume analysis by user ID (admin only)
   * GET /api/resumes/analyses/user/:userId
   */
  async getResumeAnalysesByUserId(req, res, next) {
    return this.executeMethod('getResumeAnalysesByUserId', async (req, res, next) => {
      // Only admins can access other users' analyses
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const userId = req.params.userId;
      if (!userId) {
        throw new AppError('User ID is required', 400);
      }

      const pagination = this.extractPaginationParams(req);
      const sortOptions = this.extractSortParams(req, ['fileName', 'createdAt', 'processingMethod'], 'createdAt', 'desc');

      const options = {
        ...pagination,
        ...sortOptions
      };

      const useServiceRole = true;
      const result = await this.resumeService.getResumeAnalysesWithPagination(userId, options, useServiceRole);
      
      return this.sendPaginatedResponse(res, result.analyses, result.pagination, 'User resume analyses retrieved successfully');
    }, req, res, next);
  }

  /**
   * Bulk delete resume analyses (admin only)
   * DELETE /api/resumes/analyses/bulk
   */
  async bulkDeleteResumeAnalyses(req, res, next) {
    return this.executeMethod('bulkDeleteResumeAnalyses', async (req, res, next) => {
      // Only admins can bulk delete
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      this.validateRequiredParams(req, ['analysisIds'], 'body');

      const analysisIds = req.body.analysisIds;
      if (!Array.isArray(analysisIds) || analysisIds.length === 0) {
        throw new AppError('Analysis IDs array is required', 400);
      }

      const useServiceRole = true;
      const results = [];

      for (const analysisId of analysisIds) {
        try {
          const success = await this.resumeService.deleteResumeAnalysis(analysisId, null, useServiceRole);
          results.push({ analysisId, success });
        } catch (error) {
          results.push({ analysisId, success: false, error: error.message });
        }
      }

      const successCount = results.filter(r => r.success).length;
      const failureCount = results.length - successCount;

      return this.sendSuccess(res, {
        results,
        summary: {
          total: results.length,
          successful: successCount,
          failed: failureCount
        }
      }, 200, `Bulk delete completed. ${successCount} successful, ${failureCount} failed`);
    }, req, res, next);
  }

  // ========================================
  // RESUME GENERATOR METHODS
  // ========================================

  /**
   * Generate Canadian resume using AI
   * POST /api/resumes/generate
   */
  async generateCanadianResume(req, res, next) {
    return this.executeMethod('generateCanadianResume', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      this.validateRequiredParams(req, ['originalAnalysisId', 'jobTargeting'], 'body');
      this.validateRequiredParams(req.body.jobTargeting, ['jobTitle', 'companyName'], 'body');

      const userId = this.extractUserId(req);
      const { originalAnalysisId, jobTargeting } = req.body;

      const generatedResume = await this.canadianResumeService.generateCanadianResume(
        userId, 
        originalAnalysisId, 
        jobTargeting
      );

      return this.sendSuccess(res, generatedResume, 201, 'Canadian resume generated successfully');
    }, req, res, next);
  }

  /**
   * Get user's generated resumes
   * GET /api/resumes/generated
   */
  async getUserGeneratedResumes(req, res, next) {
    return this.executeMethod('getUserGeneratedResumes', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const pagination = this.extractPaginationParams(req);
      const sortOptions = this.extractSortParams(req, ['jobTitle', 'companyName', 'createdAt', 'atsScore'], 'createdAt', 'desc');

      const options = {
        ...pagination,
        ...sortOptions
      };

      const result = await this.canadianResumeService.getUserGeneratedResumes(userId, options);
      
      return this.sendPaginatedResponse(res, result.data, result.pagination, 'Generated resumes retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get generated resume by ID
   * GET /api/resumes/generated/:resumeId
   */
  async getGeneratedResumeById(req, res, next) {
    return this.executeMethod('getGeneratedResumeById', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const resumeId = req.params.resumeId;
      if (!resumeId) {
        throw new AppError('Resume ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const resume = await this.canadianResumeService.getGeneratedResumeById(resumeId, userId);
      
      return this.sendSuccess(res, resume, 200, 'Generated resume retrieved successfully');
    }, req, res, next);
  }

  /**
   * Update generated resume
   * PUT /api/resumes/generated/:resumeId
   */
  async updateGeneratedResume(req, res, next) {
    return this.executeMethod('updateGeneratedResume', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const resumeId = req.params.resumeId;
      if (!resumeId) {
        throw new AppError('Resume ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const updateData = req.body;

      const updatedResume = await this.canadianResumeService.updateGeneratedResume(
        resumeId, 
        userId, 
        updateData
      );
      
      return this.sendSuccess(res, updatedResume, 200, 'Generated resume updated successfully');
    }, req, res, next);
  }

  /**
   * Auto-save user edits to generated resume
   * PATCH /api/resumes/generated/:resumeId/auto-save
   */
  async autoSaveUserEdits(req, res, next) {
    return this.executeMethod('autoSaveUserEdits', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      this.validateRequiredParams(req, ['userEdits'], 'body');

      const resumeId = req.params.resumeId;
      if (!resumeId) {
        throw new AppError('Resume ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const { userEdits } = req.body;

      const updatedResume = await this.canadianResumeService.autoSaveUserEdits(
        resumeId, 
        userId, 
        userEdits
      );
      
      return this.sendSuccess(res, updatedResume, 200, 'User edits auto-saved successfully');
    }, req, res, next);
  }

  /**
   * Track PDF download for generated resume
   * POST /api/resumes/generated/:resumeId/track-download
   */
  async trackPDFDownload(req, res, next) {
    return this.executeMethod('trackPDFDownload', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const resumeId = req.params.resumeId;
      if (!resumeId) {
        throw new AppError('Resume ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const updatedResume = await this.canadianResumeService.trackPDFDownload(resumeId, userId);
      
      return this.sendSuccess(res, updatedResume, 200, 'PDF download tracked successfully');
    }, req, res, next);
  }

  /**
   * Delete generated resume
   * DELETE /api/resumes/generated/:resumeId
   */
  async deleteGeneratedResume(req, res, next) {
    return this.executeMethod('deleteGeneratedResume', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const resumeId = req.params.resumeId;
      if (!resumeId) {
        throw new AppError('Resume ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const success = await this.canadianResumeService.deleteGeneratedResume(resumeId, userId);
      
      if (!success) {
        throw new AppError('Failed to delete generated resume', 500);
      }

      return this.sendSuccess(res, null, 200, 'Generated resume deleted successfully');
    }, req, res, next);
  }

  /**
   * Search generated resumes
   * GET /api/resumes/generated/search
   */
  async searchGeneratedResumes(req, res, next) {
    return this.executeMethod('searchGeneratedResumes', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const allowedFields = ['jobTitle', 'companyName', 'industry', 'status', 'createdAfter', 'createdBefore'];
      const criteria = this.extractSearchParams(req, allowedFields);
      const pagination = this.extractPaginationParams(req);
      const sortOptions = this.extractSortParams(req, ['jobTitle', 'companyName', 'createdAt', 'atsScore'], 'createdAt', 'desc');

      const options = {
        ...pagination,
        ...sortOptions
      };

      const resumes = await this.canadianResumeService.searchGeneratedResumes(userId, criteria, options);
      
      return this.sendSuccess(res, resumes, 200, 'Generated resumes search completed successfully');
    }, req, res, next);
  }

  /**
   * Get generated resume statistics
   * GET /api/resumes/generated/statistics
   */
  async getGeneratedResumeStatistics(req, res, next) {
    return this.executeMethod('getGeneratedResumeStatistics', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const statistics = await this.canadianResumeService.getGeneratedResumeStatistics(userId);
      
      return this.sendSuccess(res, statistics, 200, 'Generated resume statistics retrieved successfully');
    }, req, res, next);
  }

  /**
   * Analyze job description for targeting
   * POST /api/resumes/analyze-job-targeting
   */
  async analyzeJobTargeting(req, res, next) {
    return this.executeMethod('analyzeJobTargeting', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      this.validateRequiredParams(req, ['jobDescription'], 'body');

      const { jobDescription, userProfile } = req.body;
      const analysis = await this.canadianResumeService.analyzeJobTargeting(jobDescription, userProfile);
      
      return this.sendSuccess(res, analysis, 200, 'Job targeting analysis completed successfully');
    }, req, res, next);
  }

  /**
   * Translate skills for Canadian market
   * POST /api/resumes/translate-skills
   */
  async translateSkillsForCanadianMarket(req, res, next) {
    return this.executeMethod('translateSkillsForCanadianMarket', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      this.validateRequiredParams(req, ['skills'], 'body');

      const { skills, targetIndustry } = req.body;
      const translatedSkills = await this.canadianResumeService.translateSkillsForCanadianMarket(skills, targetIndustry);
      
      return this.sendSuccess(res, { skills: translatedSkills }, 200, 'Skills translated for Canadian market successfully');
    }, req, res, next);
  }

  /**
   * Export resume in various formats
   * POST /api/resumes/generated/:resumeId/export
   */
  async exportResume(req, res, next) {
    return this.executeMethod('exportResume', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const resumeId = req.params.resumeId;
      if (!resumeId) {
        throw new AppError('Resume ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const exportOptions = req.body;

      const exportResult = await this.canadianResumeService.exportResume(resumeId, userId, exportOptions);
      
      return this.sendSuccess(res, exportResult, 200, 'Resume exported successfully');
    }, req, res, next);
  }

  /**
   * Download resume as PDF
   * GET /api/resumes/generated/:resumeId/download-pdf
   */
  async downloadResumePDF(req, res, next) {
    return this.executeMethod('downloadResumePDF', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const resumeId = req.params.resumeId;
      if (!resumeId) {
        throw new AppError('Resume ID is required', 400);
      }

      const userId = this.extractUserId(req);
      const template = req.query.template || 'professional';

      const pdfBuffer = await this.canadianResumeService.downloadResumePDF(resumeId, userId, template);
      
      res.setHeader('Content-Type', 'application/pdf');
      res.setHeader('Content-Disposition', `attachment; filename="resume-${resumeId}.pdf"`);
      res.send(pdfBuffer);
    }, req, res, next);
  }

  /**
   * Bulk delete generated resumes
   * DELETE /api/resumes/generated/bulk
   */
  async bulkDeleteGeneratedResumes(req, res, next) {
    return this.executeMethod('bulkDeleteGeneratedResumes', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      this.validateRequiredParams(req, ['resumeIds'], 'body');

      const userId = this.extractUserId(req);
      const { resumeIds } = req.body;

      const result = await this.canadianResumeService.bulkDeleteGeneratedResumes(resumeIds, userId);
      
      return this.sendSuccess(res, result, 200, 'Bulk delete completed successfully');
    }, req, res, next);
  }

  /**
   * Bulk export resumes
   * POST /api/resumes/generated/bulk-export
   */
  async bulkExportResumes(req, res, next) {
    return this.executeMethod('bulkExportResumes', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      this.validateRequiredParams(req, ['resumeIds'], 'body');

      const userId = this.extractUserId(req);
      const { resumeIds, options } = req.body;

      const exportResults = await this.canadianResumeService.bulkExportResumes(resumeIds, userId, options);
      
      return this.sendSuccess(res, exportResults, 200, 'Bulk export completed successfully');
    }, req, res, next);
  }

  /**
   * Stream generation progress
   * GET /api/resumes/generate/:resumeId/progress
   */
  async streamGenerationProgress(req, res, next) {
    return this.executeMethod('streamGenerationProgress', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const resumeId = req.params.resumeId;
      if (!resumeId) {
        throw new AppError('Resume ID is required', 400);
      }

      const userId = this.extractUserId(req);

      res.setHeader('Content-Type', 'text/event-stream');
      res.setHeader('Cache-Control', 'no-cache');
      res.setHeader('Connection', 'keep-alive');

      const cleanup = await this.canadianResumeService.streamGenerationProgress(
        resumeId, 
        userId, 
        (progress) => {
          res.write(`data: ${JSON.stringify({ type: 'progress', progress })}\n\n`);
        },
        (result) => {
          res.write(`data: ${JSON.stringify({ type: 'complete', result })}\n\n`);
          res.end();
        },
        (error) => {
          res.write(`data: ${JSON.stringify({ type: 'error', error })}\n\n`);
          res.end();
        }
      );

      req.on('close', cleanup);
    }, req, res, next);
  }

  /**
   * Check generation support
   * GET /api/resumes/generate/support
   */
  async checkGenerationSupport(req, res, next) {
    return this.executeMethod('checkGenerationSupport', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const supportInfo = await this.canadianResumeService.checkGenerationSupport();
      
      return this.sendSuccess(res, supportInfo, 200, 'Generation support information retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get generation templates
   * GET /api/resumes/generate/templates
   */
  async getGenerationTemplates(req, res, next) {
    return this.executeMethod('getGenerationTemplates', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const templates = await this.canadianResumeService.getGenerationTemplates();
      
      return this.sendSuccess(res, templates, 200, 'Generation templates retrieved successfully');
    }, req, res, next);
  }
}

module.exports = ResumeController;
````

## File: src/controllers/UserController.js
````javascript
const BaseController = require('./BaseController');
const { AppError } = require('../utils/errors');

/**
 * User Controller for user-related HTTP requests
 */
class UserController extends BaseController {
  constructor(services) {
    super(services);
    this.userService = this.getService('user');
  }

  /**
   * Find or create a user
   * POST /api/users/find-or-create
   */
  async findOrCreateUser(req, res, next) {
    return this.executeMethod('findOrCreateUser', async (req, res, next) => {
      this.validateRequiredParams(req, ['email'], 'body');

      const userData = {
        email: req.body.email,
        fullName: req.body.fullName,
        phoneNo: req.body.phoneNo,
        statusInCanada: req.body.statusInCanada,
        countryOfOrigin: req.body.countryOfOrigin,
        currentLocation: req.body.currentLocation
      };

      const user = await this.userService.findOrCreateUser(userData);
      return this.sendSuccess(res, user, 200, 'User found or created successfully');
    }, req, res, next);
  }

  /**
   * Update user profile
   * PUT /api/users/:userId
   */
  async updateUser(req, res, next) {
    return this.executeMethod('updateUser', async (req, res, next) => {
      const userId = req.params.userId;
      if (!userId) {
        throw new AppError('User ID is required', 400);
      }

      // Check if user is updating their own profile or is admin
      const currentUserId = this.extractUserId(req);
      if (!this.isAdmin(req) && currentUserId !== userId) {
        throw new AppError('Access denied', 403);
      }

      const userData = {
        fullName: req.body.fullName,
        phoneNo: req.body.phoneNo,
        statusInCanada: req.body.statusInCanada,
        countryOfOrigin: req.body.countryOfOrigin,
        currentLocation: req.body.currentLocation
      };

      const user = await this.userService.updateUser(userId, userData);
      return this.sendSuccess(res, user, 200, 'User updated successfully');
    }, req, res, next);
  }

  /**
   * Get user by ID
   * GET /api/users/:userId
   */
  async getUserById(req, res, next) {
    return this.executeMethod('getUserById', async (req, res, next) => {
      const userId = req.params.userId;
      if (!userId) {
        throw new AppError('User ID is required', 400);
      }

      // Check if user is accessing their own profile or is admin
      const currentUserId = this.extractUserId(req);
      if (!this.isAdmin(req) && currentUserId !== userId) {
        throw new AppError('Access denied', 403);
      }

      const useServiceRole = this.isAdmin(req);
      const user = await this.userService.getUserById(userId, useServiceRole);
      
      if (!user) {
        throw new AppError('User not found', 404);
      }

      return this.sendSuccess(res, user, 200, 'User retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get user by email
   * GET /api/users/email/:email
   */
  async getUserByEmail(req, res, next) {
    return this.executeMethod('getUserByEmail', async (req, res, next) => {
      const email = req.params.email;
      if (!email) {
        throw new AppError('Email is required', 400);
      }

      // Only admins can search by email
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const useServiceRole = true;
      const user = await this.userService.getUserByEmail(email, useServiceRole);
      
      if (!user) {
        throw new AppError('User not found', 404);
      }

      return this.sendSuccess(res, user, 200, 'User retrieved successfully');
    }, req, res, next);
  }

  /**
   * Search users
   * GET /api/users/search
   */
  async searchUsers(req, res, next) {
    return this.executeMethod('searchUsers', async (req, res, next) => {
      // Only admins can search users
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const allowedFields = ['email', 'fullName', 'roleId', 'statusInCanada', 'countryOfOrigin', 'currentLocation'];
      const criteria = this.extractSearchParams(req, allowedFields);
      const pagination = this.extractPaginationParams(req);
      const sortOptions = this.extractSortParams(req, ['email', 'fullName', 'createdAt'], 'createdAt', 'desc');

      const options = {
        ...pagination,
        ...sortOptions
      };

      const useServiceRole = true;
      const users = await this.userService.searchUsers(criteria, options, useServiceRole);
      
      return this.sendSuccess(res, users, 200, 'Users retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get users with pagination
   * GET /api/users
   */
  async getUsers(req, res, next) {
    return this.executeMethod('getUsers', async (req, res, next) => {
      // Only admins can list all users
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const pagination = this.extractPaginationParams(req);
      const sortOptions = this.extractSortParams(req, ['email', 'fullName', 'createdAt'], 'createdAt', 'desc');

      const options = {
        ...pagination,
        ...sortOptions
      };

      const useServiceRole = true;
      const result = await this.userService.getUsersWithPagination(options, useServiceRole);
      
      return this.sendPaginatedResponse(res, result.data, result.pagination, 'Users retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get users by role
   * GET /api/users/role/:roleId
   */
  async getUsersByRole(req, res, next) {
    return this.executeMethod('getUsersByRole', async (req, res, next) => {
      // Only admins can filter by role
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const roleId = req.params.roleId;
      if (!roleId) {
        throw new AppError('Role ID is required', 400);
      }

      const useServiceRole = true;
      const users = await this.userService.getUsersByRole(roleId, useServiceRole);
      
      return this.sendSuccess(res, users, 200, 'Users retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get users by status in Canada
   * GET /api/users/status/:status
   */
  async getUsersByStatusInCanada(req, res, next) {
    return this.executeMethod('getUsersByStatusInCanada', async (req, res, next) => {
      // Only admins can filter by status
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const status = req.params.status;
      if (!status) {
        throw new AppError('Status is required', 400);
      }

      const useServiceRole = true;
      const users = await this.userService.getUsersByStatusInCanada(status, useServiceRole);
      
      return this.sendSuccess(res, users, 200, 'Users retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get users by country of origin
   * GET /api/users/country/:country
   */
  async getUsersByCountryOfOrigin(req, res, next) {
    return this.executeMethod('getUsersByCountryOfOrigin', async (req, res, next) => {
      // Only admins can filter by country
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const country = req.params.country;
      if (!country) {
        throw new AppError('Country is required', 400);
      }

      const useServiceRole = true;
      const users = await this.userService.getUsersByCountryOfOrigin(country, useServiceRole);
      
      return this.sendSuccess(res, users, 200, 'Users retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get users by current location
   * GET /api/users/location/:location
   */
  async getUsersByCurrentLocation(req, res, next) {
    return this.executeMethod('getUsersByCurrentLocation', async (req, res, next) => {
      // Only admins can filter by location
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const location = req.params.location;
      if (!location) {
        throw new AppError('Location is required', 400);
      }

      const useServiceRole = true;
      const users = await this.userService.getUsersByCurrentLocation(location, useServiceRole);
      
      return this.sendSuccess(res, users, 200, 'Users retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get user statistics
   * GET /api/users/statistics
   */
  async getUserStatistics(req, res, next) {
    return this.executeMethod('getUserStatistics', async (req, res, next) => {
      // Only admins can view statistics
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const useServiceRole = true;
      const statistics = await this.userService.getUserStatistics(useServiceRole);
      
      return this.sendSuccess(res, statistics, 200, 'User statistics retrieved successfully');
    }, req, res, next);
  }

  /**
   * Delete user
   * DELETE /api/users/:userId
   */
  async deleteUser(req, res, next) {
    return this.executeMethod('deleteUser', async (req, res, next) => {
      const userId = req.params.userId;
      if (!userId) {
        throw new AppError('User ID is required', 400);
      }

      // Only admins can delete users
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const useServiceRole = true;
      const success = await this.userService.deleteUser(userId, useServiceRole);
      
      if (!success) {
        throw new AppError('Failed to delete user', 500);
      }

      return this.sendSuccess(res, null, 200, 'User deleted successfully');
    }, req, res, next);
  }

  /**
   * Check if user exists
   * GET /api/users/:userId/exists
   */
  async userExists(req, res, next) {
    return this.executeMethod('userExists', async (req, res, next) => {
      const userId = req.params.userId;
      if (!userId) {
        throw new AppError('User ID is required', 400);
      }

      // Only admins can check user existence
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const useServiceRole = true;
      const exists = await this.userService.userExists(userId, useServiceRole);
      
      return this.sendSuccess(res, { exists }, 200, 'User existence checked successfully');
    }, req, res, next);
  }

  /**
   * Get user count
   * GET /api/users/count
   */
  async getUserCount(req, res, next) {
    return this.executeMethod('getUserCount', async (req, res, next) => {
      // Only admins can get user count
      if (!this.isAdmin(req)) {
        throw new AppError('Access denied', 403);
      }

      const filter = this.extractSearchParams(req, ['roleId', 'statusInCanada', 'countryOfOrigin', 'currentLocation']);
      const useServiceRole = true;
      const count = await this.userService.getUserCount(filter, useServiceRole);
      
      return this.sendSuccess(res, { count }, 200, 'User count retrieved successfully');
    }, req, res, next);
  }

  /**
   * Get current user profile
   * GET /api/users/profile
   */
  async getCurrentUserProfile(req, res, next) {
    return this.executeMethod('getCurrentUserProfile', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const useServiceRole = false;
      const user = await this.userService.getUserById(userId, useServiceRole);
      
      if (!user) {
        throw new AppError('User not found', 404);
      }

      return this.sendSuccess(res, user, 200, 'User profile retrieved successfully');
    }, req, res, next);
  }

  /**
   * Update current user profile
   * PUT /api/users/profile
   */
  async updateCurrentUserProfile(req, res, next) {
    return this.executeMethod('updateCurrentUserProfile', async (req, res, next) => {
      if (!this.isAuthenticated(req)) {
        throw new AppError('Authentication required', 401);
      }

      const userId = this.extractUserId(req);
      const userData = {
        fullName: req.body.fullName,
        phoneNo: req.body.phoneNo,
        statusInCanada: req.body.statusInCanada,
        countryOfOrigin: req.body.countryOfOrigin,
        currentLocation: req.body.currentLocation
      };

      const user = await this.userService.updateUser(userId, userData);
      return this.sendSuccess(res, user, 200, 'User profile updated successfully');
    }, req, res, next);
  }
}

module.exports = UserController;
````

## File: src/middleware/authMiddleware.js
````javascript
const { createClient } = require('@supabase/supabase-js');
const SupabaseDatabase = require('../services/supabaseDatabase');

// Create Supabase client for auth verification
const supabase = createClient(
  process.env.SUPABASE_URL,
  process.env.SUPABASE_ANON_KEY
);

// Initialize database service
const supabaseDb = new SupabaseDatabase();

const verifyToken = async (req, res, next) => {
  try {
    const authHeader = req.headers.authorization;
    
    if (!authHeader || !authHeader.startsWith('Bearer ')) {
      console.log('❌ No authorization token provided');
      return res.status(401).json({
        success: false,
        message: 'No authorization token provided'
      });
    }

    const token = authHeader.substring(7); // Remove 'Bearer ' prefix
    console.log('🔐 Verifying token for user...');
    
    // Verify the JWT token with Supabase
    const { data: { user }, error } = await supabase.auth.getUser(token);
    
    if (error || !user) {
      console.error('❌ Token verification failed:', error);
      return res.status(401).json({
        success: false,
        message: 'Invalid or expired token'
      });
    }

    // Get the database user ID by looking up the user by email
    try {
      const dbUser = await supabaseDb.findOrCreateUser({
        email: user.email,
        fullName: user.user_metadata?.full_name || 'User'
      });
      
      // Set user info in request object with database ID
      req.user = {
        id: dbUser.id, // Use database serial ID, not Supabase Auth UUID
        email: user.email,
        role: user.role || 'authenticated',
        supabaseAuthId: user.id // Keep the Supabase Auth UUID for reference
      };

      console.log('✅ User authenticated:', req.user.email, 'with database ID:', req.user.id);
    } catch (dbError) {
      console.error('❌ Database user lookup failed:', dbError);
      return res.status(500).json({
        success: false,
        message: 'User profile not found'
      });
    }

    next();
  } catch (error) {
    console.error('❌ Authentication middleware error:', error);
    return res.status(500).json({
      success: false,
      message: 'Authentication error'
    });
  }
};

// Middleware for optional authentication (allows guest access)
const optionalAuth = async (req, res, next) => {
  try {
    const authHeader = req.headers.authorization;
    
    if (!authHeader || !authHeader.startsWith('Bearer ')) {
      // No token provided, continue as guest
      console.log('👤 No token provided, continuing as guest user');
      req.user = {
        id: null,
        email: 'guest@immigrow.ai',
        role: 'guest'
      };
      return next();
    }

    const token = authHeader.substring(7);
    console.log('🔐 Verifying optional token...');
    
    // Verify the JWT token with Supabase
    const { data: { user }, error } = await supabase.auth.getUser(token);
    
    if (error || !user) {
      // Invalid token, continue as guest
      console.log('❌ Invalid token, continuing as guest user');
      req.user = {
        id: null,
        email: 'guest@immigrow.ai',
        role: 'guest'
      };
      return next();
    }

    // Get the database user ID by looking up the user by email
    try {
      const dbUser = await supabaseDb.findOrCreateUser({
        email: user.email,
        fullName: user.user_metadata?.full_name || 'User'
      });
      
      // Valid token, set user info with database ID
      req.user = {
        id: dbUser.id, // Use database serial ID, not Supabase Auth UUID
        email: user.email,
        role: user.role || 'authenticated',
        supabaseAuthId: user.id // Keep the Supabase Auth UUID for reference
      };

      console.log('✅ User authenticated (optional):', req.user.email, 'with database ID:', req.user.id);
    } catch (dbError) {
      console.error('❌ Database user lookup failed (optional):', dbError);
      // Continue as guest on database error
      console.log('⚠️ Database error, continuing as guest user');
      req.user = {
        id: null,
        email: 'guest@immigrow.ai',
        role: 'guest'
      };
    }
    
    next();
  } catch (error) {
    console.error('❌ Optional auth middleware error:', error);
    // Continue as guest on error
    console.log('⚠️ Auth error, continuing as guest user');
    req.user = {
      id: null,
      email: 'guest@immigrow.ai',
      role: 'guest'
    };
    next();
  }
};

module.exports = { verifyToken, optionalAuth };
````

## File: src/middleware/cacheMiddleware.js
````javascript
/**
 * Cache Middleware
 * Provides response caching for API endpoints using Redis with in-memory fallback
 */

const { cacheConfig } = require('../config/cache');
const { logger } = require('../config/logger');

/**
 * Cache middleware factory
 * @param {string} cacheType - Type of cache strategy to use
 * @param {string} keyGenerator - Function to generate cache key
 * @param {number} customTTL - Custom TTL override (optional)
 * @returns {Function} Express middleware
 */
function createCacheMiddleware(cacheType, keyGenerator = null, customTTL = null) {
  return async (req, res, next) => {
    // Skip caching for non-GET requests
    if (req.method !== 'GET') {
      return next();
    }

    try {
      // Generate cache key
      let cacheKey;
      if (typeof keyGenerator === 'function') {
        cacheKey = keyGenerator(req);
      } else {
        // Default key generation
        const userId = req.user?.id || 'anonymous';
        const queryString = JSON.stringify(req.query);
        cacheKey = `${req.originalUrl}:${userId}:${queryString}`;
      }

      // Check cache (works with both Redis and in-memory fallback)
      const cachedData = await cacheConfig.get(cacheType, cacheKey);
      
      if (cachedData) {
        // Return cached response
        res.set('X-Cache', 'HIT');
        res.set('X-Cache-Key', cacheKey);
        res.set('X-Cache-Type', cacheConfig.isConnected ? 'redis' : 'memory');
        return res.json(cachedData);
      }

      // Cache miss - store original send method
      const originalSend = res.json;
      
      // Override send method to cache response
      res.json = function(data) {
        // Restore original method
        res.json = originalSend;
        
        // Set cache headers
        res.set('X-Cache', 'MISS');
        res.set('X-Cache-Key', cacheKey);
        res.set('X-Cache-Type', cacheConfig.isConnected ? 'redis' : 'memory');
        
        // Cache the response (only cache successful responses)
        if (res.statusCode >= 200 && res.statusCode < 300) {
          cacheConfig.set(cacheType, cacheKey, data)
            .catch(err => logger.error('Failed to cache response:', err));
        }
        
        // Send response
        return originalSend.call(this, data);
      };

      next();
    } catch (error) {
      logger.error('Cache middleware error:', error);
      next();
    }
  };
}

/**
 * Cache invalidation middleware
 * @param {string} cacheType - Type of cache to invalidate
 * @param {string} keyGenerator - Function to generate cache key
 * @returns {Function} Express middleware
 */
function createCacheInvalidationMiddleware(cacheType, keyGenerator = null) {
  return async (req, res, next) => {
    try {
      // Generate cache key
      let cacheKey;
      if (typeof keyGenerator === 'function') {
        cacheKey = keyGenerator(req);
      } else {
        // Default key generation
        const userId = req.user?.id || 'anonymous';
        const queryString = JSON.stringify(req.query);
        cacheKey = `${req.originalUrl}:${userId}:${queryString}`;
      }

      // Store original send method
      const originalSend = res.json;
      
      // Override send method to invalidate cache
      res.json = function(data) {
        // Restore original method
        res.json = originalSend;
        
        // Invalidate cache for successful operations
        if (res.statusCode >= 200 && res.statusCode < 300) {
          cacheConfig.delete(cacheType, cacheKey)
            .catch(err => logger.error('Failed to invalidate cache:', err));
        }
        
        // Send response
        return originalSend.call(this, data);
      };

      next();
    } catch (error) {
      logger.error('Cache invalidation middleware error:', error);
      next();
    }
  };
}

/**
 * Predefined cache middlewares for common use cases
 */

// User data cache (5 minutes)
const userCache = createCacheMiddleware('user', (req) => {
  const userId = req.user?.id || req.params.userId || 'anonymous';
  return `user:${userId}`;
});

// AI analysis cache (1 hour)
const aiCache = createCacheMiddleware('ai', (req) => {
  const userId = req.user?.id || 'anonymous';
  const analysisType = req.params.type || req.query.type || 'general';
  return `ai:${userId}:${analysisType}`;
});

// Career data cache (30 minutes)
const careerCache = createCacheMiddleware('career', (req) => {
  const userId = req.user?.id || 'anonymous';
  const careerType = req.params.type || req.query.type || 'profile';
  return `career:${userId}:${careerType}`;
});

// Resume cache (15 minutes)
const resumeCache = createCacheMiddleware('resume', (req) => {
  const userId = req.user?.id || 'anonymous';
  const resumeId = req.params.resumeId || req.query.resumeId || 'latest';
  return `resume:${userId}:${resumeId}`;
});

// Static data cache (24 hours)
const staticCache = createCacheMiddleware('static', (req) => {
  const dataType = req.params.type || req.query.type || 'general';
  return `static:${dataType}`;
});

// Session cache (2 hours)
const sessionCache = createCacheMiddleware('session', (req) => {
  const sessionId = req.session?.id || req.user?.id || 'anonymous';
  return `session:${sessionId}`;
});

/**
 * Cache invalidation middlewares
 */
const invalidateUserCache = createCacheInvalidationMiddleware('user', (req) => {
  const userId = req.user?.id || req.params.userId || 'anonymous';
  return `user:${userId}`;
});

const invalidateAiCache = createCacheInvalidationMiddleware('ai', (req) => {
  const userId = req.user?.id || 'anonymous';
  const analysisType = req.params.type || req.query.type || 'general';
  return `ai:${userId}:${analysisType}`;
});

const invalidateCareerCache = createCacheInvalidationMiddleware('career', (req) => {
  const userId = req.user?.id || 'anonymous';
  const careerType = req.params.type || req.query.type || 'profile';
  return `career:${userId}:${careerType}`;
});

const invalidateResumeCache = createCacheInvalidationMiddleware('resume', (req) => {
  const userId = req.user?.id || 'anonymous';
  const resumeId = req.params.resumeId || req.query.resumeId || 'latest';
  return `resume:${userId}:${resumeId}`;
});

/**
 * Cache management middleware
 */
const cacheManagement = {
  // Get cache statistics
  getStats: async (req, res) => {
    try {
      const stats = await cacheConfig.getStats();
      res.json({
        success: true,
        data: stats,
        timestamp: new Date().toISOString()
      });
    } catch (error) {
      logger.error('Failed to get cache stats:', error);
      res.status(500).json({
        success: false,
        error: 'Failed to get cache statistics',
        timestamp: new Date().toISOString()
      });
    }
  },

  // Clear specific cache type
  clearType: async (req, res) => {
    try {
      const { type } = req.params;
      const success = await cacheConfig.clearType(type);
      
      res.json({
        success,
        message: success ? `Cache type '${type}' cleared successfully` : 'Failed to clear cache',
        timestamp: new Date().toISOString()
      });
    } catch (error) {
      logger.error('Failed to clear cache type:', error);
      res.status(500).json({
        success: false,
        error: 'Failed to clear cache type',
        timestamp: new Date().toISOString()
      });
    }
  },

  // Clear all cache
  clearAll: async (req, res) => {
    try {
      const success = await cacheConfig.clearAll();
      
      res.json({
        success,
        message: success ? 'All cache cleared successfully' : 'Failed to clear cache',
        timestamp: new Date().toISOString()
      });
    } catch (error) {
      logger.error('Failed to clear all cache:', error);
      res.status(500).json({
        success: false,
        error: 'Failed to clear all cache',
        timestamp: new Date().toISOString()
      });
    }
  }
};

module.exports = {
  createCacheMiddleware,
  createCacheInvalidationMiddleware,
  userCache,
  aiCache,
  careerCache,
  resumeCache,
  staticCache,
  sessionCache,
  invalidateUserCache,
  invalidateAiCache,
  invalidateCareerCache,
  invalidateResumeCache,
  cacheManagement
};
````

## File: src/middleware/errorHandler.js
````javascript
/**
 * Centralized Error Handler Middleware
 * Handles all application errors and provides consistent error responses
 */

const { logger } = require('../config/logger');
const { 
  AppError, 
  ValidationError, 
  AuthenticationError, 
  DatabaseError 
} = require('../utils/errors');
const { isDevelopment, isProduction } = require('../config/environment');

/**
 * Centralized error handler middleware
 */
function errorHandler(error, req, res, next) {
  let appError = error;
  
  // Convert non-AppError to AppError
  if (!(error instanceof AppError)) {
    appError = new AppError(
      error.message || 'Internal server error',
      error.statusCode || 500,
      false,
      'INTERNAL_ERROR'
    );
  }
  
  // Log the error
  logger.error('Application error occurred', {
    ...appError.toLog(),
    request: {
      method: req.method,
      url: req.url,
      ip: req.ip,
      userId: req.user?.id || 'anonymous'
    },
    userAgent: req.get('User-Agent')
  });
  
  // Prepare error response
  const errorResponse = appError.toResponse();
  
  // Add stack trace in development
  if (isDevelopment()) {
    errorResponse.error.stack = appError.stack;
  }
  
  // Add additional context for specific error types
  if (appError instanceof ValidationError) {
    errorResponse.error.type = 'VALIDATION_ERROR';
  } else if (appError instanceof AuthenticationError) {
    errorResponse.error.type = 'AUTHENTICATION_ERROR';
  } else if (appError instanceof DatabaseError) {
    errorResponse.error.type = 'DATABASE_ERROR';
  } else {
    errorResponse.error.type = 'APPLICATION_ERROR';
  }
  
  // Set appropriate status code
  const statusCode = appError.getStatusCode();
  
  // Send error response
  res.status(statusCode).json(errorResponse);
}

/**
 * Handle 404 errors
 */
function notFoundHandler(req, res, next) {
  const error = new AppError(
    `Route ${req.method} ${req.url} not found`,
    404,
    true,
    'NOT_FOUND'
  );
  
  next(error);
}

/**
 * Handle async errors
 */
function asyncErrorHandler(fn) {
  return (req, res, next) => {
    Promise.resolve(fn(req, res, next)).catch(next);
  };
}

/**
 * Handle unhandled promise rejections
 */
function handleUnhandledRejection(reason, promise) {
  logger.error('Unhandled Promise Rejection', {
    reason: reason?.message || reason,
    stack: reason?.stack,
    promise: promise
  });
  
  // In production, you might want to exit the process
  if (isProduction()) {
    process.exit(1);
  }
}

/**
 * Handle uncaught exceptions
 */
function handleUncaughtException(error) {
  logger.error('Uncaught Exception', {
    message: error.message,
    stack: error.stack
  });
  
  // In production, you might want to exit the process
  if (isProduction()) {
    process.exit(1);
  }
}

/**
 * Setup global error handlers
 */
function setupGlobalErrorHandlers() {
  process.on('unhandledRejection', handleUnhandledRejection);
  process.on('uncaughtException', handleUncaughtException);
}

module.exports = {
  errorHandler,
  notFoundHandler,
  asyncErrorHandler,
  handleUnhandledRejection,
  handleUncaughtException,
  setupGlobalErrorHandlers
};
````

## File: src/middleware/rateLimiter.js
````javascript
const rateLimit = require('express-rate-limit');

// Rate limiter for Gemini API calls (1000 requests per minute)
const geminiRateLimit = rateLimit({
  windowMs: 60 * 1000, // 1 minute
  max: 950, // Slightly under the 1000 limit for safety buffer
  message: {
    success: false,
    message: 'Too many AI requests from this IP, please try again later.',
    retryAfter: '1 minute'
  },
  standardHeaders: true,
  legacyHeaders: false,
  keyGenerator: (req) => {
    // Use user ID if authenticated, otherwise IP
    return req.user?.id || req.ip;
  },
  handler: (req, res) => {
    console.log(`🚫 Rate limit exceeded for ${req.user?.email || req.ip}`);
    res.status(429).json({
      success: false,
      message: 'Rate limit exceeded. The Gemini API allows 1000 requests per minute.',
      retryAfter: Math.ceil(req.rateLimit.resetTime / 1000),
      rateLimitInfo: {
        limit: req.rateLimit.limit,
        current: req.rateLimit.current,
        remaining: req.rateLimit.remaining,
        resetTime: new Date(req.rateLimit.resetTime).toISOString()
      }
    });
  }
});

// Rate limiter for file uploads (more restrictive)
const uploadRateLimit = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 10, // 10 uploads per 15 minutes
  message: {
    success: false,
    message: 'Too many file uploads from this IP, please try again later.',
    retryAfter: '15 minutes'
  },
  keyGenerator: (req) => {
    return req.user?.id || req.ip;
  }
});

// Daily limit tracker for Gemini API
class DailyLimitTracker {
  constructor() {
    this.dailyLimits = new Map();
    this.maxDailyRequests = 45000; // Conservative limit under 50k
  }

  checkDailyLimit(userId) {
    const today = new Date().toDateString();
    const userKey = `${userId}-${today}`;
    
    const currentCount = this.dailyLimits.get(userKey) || 0;
    
    if (currentCount >= this.maxDailyRequests) {
      throw new Error(`Daily API limit exceeded (${this.maxDailyRequests} requests per day)`);
    }
    
    return true;
  }

  incrementDailyCount(userId) {
    const today = new Date().toDateString();
    const userKey = `${userId}-${today}`;
    
    const currentCount = this.dailyLimits.get(userKey) || 0;
    this.dailyLimits.set(userKey, currentCount + 1);
    
    // Clean up old entries (keep only today and yesterday)
    const yesterday = new Date();
    yesterday.setDate(yesterday.getDate() - 1);
    const yesterdayStr = yesterday.toDateString();
    
    for (const key of this.dailyLimits.keys()) {
      if (!key.includes(today) && !key.includes(yesterdayStr)) {
        this.dailyLimits.delete(key);
      }
    }
  }

  getDailyUsage(userId) {
    const today = new Date().toDateString();
    const userKey = `${userId}-${today}`;
    return this.dailyLimits.get(userKey) || 0;
  }
}

const dailyTracker = new DailyLimitTracker();

// Middleware to check daily limits
const checkDailyLimit = (req, res, next) => {
  try {
    if (req.user?.id) {
      dailyTracker.checkDailyLimit(req.user.id);
    }
    next();
  } catch (error) {
    res.status(429).json({
      success: false,
      message: error.message,
      dailyUsage: req.user?.id ? dailyTracker.getDailyUsage(req.user.id) : 0,
      dailyLimit: dailyTracker.maxDailyRequests
    });
  }
};

// Middleware to increment daily count after successful API call
const incrementDailyCount = (req, res, next) => {
  if (req.user?.id) {
    dailyTracker.incrementDailyCount(req.user.id);
  }
  next();
};

module.exports = {
  geminiRateLimit,
  uploadRateLimit,
  checkDailyLimit,
  incrementDailyCount,
  dailyTracker
};
````

## File: src/middleware/routePerformance.js
````javascript
/**
 * Route Performance Monitoring Middleware
 * Tracks and logs performance metrics for API routes
 */

const { logger } = require('../config/logger');

/**
 * Performance monitoring middleware
 * Tracks request duration, memory usage, and other metrics
 */
const routePerformanceMiddleware = (options = {}) => {
  const {
    enabled = true,
    logSlowRequests = true,
    slowRequestThreshold = 1000, // 1 second
    logMemoryUsage = false,
    logRequestSize = false,
    trackErrors = true
  } = options;

  return (req, res, next) => {
    if (!enabled) {
      return next();
    }

    const startTime = Date.now();
    const startMemory = process.memoryUsage();
    const originalSend = res.send;
    const originalJson = res.json;

    // Track request size
    let requestSize = 0;
    if (logRequestSize) {
      requestSize = JSON.stringify(req.body).length + JSON.stringify(req.query).length;
    }

    // Override res.send to capture response data
    res.send = function(data) {
      const duration = Date.now() - startTime;
      const endMemory = process.memoryUsage();
      
      logPerformanceMetrics({
        req,
        res,
        duration,
        startMemory,
        endMemory,
        requestSize,
        responseSize: data ? data.length : 0,
        slowRequestThreshold,
        logSlowRequests,
        logMemoryUsage,
        logRequestSize,
        trackErrors
      });

      return originalSend.call(this, data);
    };

    // Override res.json to capture response data
    res.json = function(data) {
      const duration = Date.now() - startTime;
      const endMemory = process.memoryUsage();
      
      logPerformanceMetrics({
        req,
        res,
        duration,
        startMemory,
        endMemory,
        requestSize,
        responseSize: data ? JSON.stringify(data).length : 0,
        slowRequestThreshold,
        logSlowRequests,
        logMemoryUsage,
        logRequestSize,
        trackErrors
      });

      return originalJson.call(this, data);
    };

    // Track errors
    if (trackErrors) {
      res.on('error', (error) => {
        const duration = Date.now() - startTime;
        const endMemory = process.memoryUsage();
        
        logPerformanceMetrics({
          req,
          res,
          duration,
          startMemory,
          endMemory,
          requestSize,
          responseSize: 0,
          slowRequestThreshold,
          logSlowRequests,
          logMemoryUsage,
          logRequestSize,
          trackErrors,
          error
        });
      });
    }

    next();
  };
};

/**
 * Log performance metrics
 */
const logPerformanceMetrics = ({
  req,
  res,
  duration,
  startMemory,
  endMemory,
  requestSize,
  responseSize,
  slowRequestThreshold,
  logSlowRequests,
  logMemoryUsage,
  logRequestSize,
  trackErrors,
  error
}) => {
  const metrics = {
    method: req.method,
    url: req.originalUrl,
    statusCode: res.statusCode,
    duration: `${duration}ms`,
    timestamp: new Date().toISOString(),
    userAgent: req.get('User-Agent'),
    ip: req.ip || req.connection.remoteAddress,
    userId: req.user?.id || 'anonymous'
  };

  // Add memory usage if enabled
  if (logMemoryUsage) {
    const memoryDiff = {
      rss: endMemory.rss - startMemory.rss,
      heapUsed: endMemory.heapUsed - startMemory.heapUsed,
      heapTotal: endMemory.heapTotal - startMemory.heapTotal,
      external: endMemory.external - startMemory.external
    };
    metrics.memoryUsage = memoryDiff;
  }

  // Add request/response size if enabled
  if (logRequestSize) {
    metrics.requestSize = `${requestSize} bytes`;
    metrics.responseSize = `${responseSize} bytes`;
  }

  // Add error information if present
  if (error) {
    metrics.error = {
      message: error.message,
      stack: error.stack,
      code: error.code
    };
  }

  // Log slow requests
  if (logSlowRequests && duration > slowRequestThreshold) {
    logger.warn('Slow request detected', {
      ...metrics,
      threshold: `${slowRequestThreshold}ms`,
      performance: 'slow'
    });
  }

  // Log all requests with performance data
  logger.info('Route performance', {
    ...metrics,
    performance: duration > slowRequestThreshold ? 'slow' : 'normal'
  });
};

/**
 * Performance metrics collector
 */
class PerformanceCollector {
  constructor() {
    this.metrics = {
      requests: 0,
      errors: 0,
      slowRequests: 0,
      totalDuration: 0,
      averageDuration: 0,
      minDuration: Infinity,
      maxDuration: 0,
      routes: new Map()
    };
    this.startTime = Date.now();
  }

  /**
   * Record a request
   */
  recordRequest(route, duration, statusCode, error = null) {
    this.metrics.requests++;
    this.metrics.totalDuration += duration;
    this.metrics.averageDuration = this.metrics.totalDuration / this.metrics.requests;
    this.metrics.minDuration = Math.min(this.metrics.minDuration, duration);
    this.metrics.maxDuration = Math.max(this.metrics.maxDuration, duration);

    if (error) {
      this.metrics.errors++;
    }

    if (duration > 1000) { // 1 second threshold
      this.metrics.slowRequests++;
    }

    // Track per-route metrics
    if (!this.metrics.routes.has(route)) {
      this.metrics.routes.set(route, {
        requests: 0,
        errors: 0,
        totalDuration: 0,
        averageDuration: 0
      });
    }

    const routeMetrics = this.metrics.routes.get(route);
    routeMetrics.requests++;
    routeMetrics.totalDuration += duration;
    routeMetrics.averageDuration = routeMetrics.totalDuration / routeMetrics.requests;

    if (error) {
      routeMetrics.errors++;
    }
  }

  /**
   * Get performance summary
   */
  getSummary() {
    const uptime = Date.now() - this.startTime;
    const requestsPerSecond = this.metrics.requests / (uptime / 1000);
    const errorRate = (this.metrics.errors / this.metrics.requests) * 100;

    return {
      uptime: `${Math.floor(uptime / 1000)}s`,
      requests: this.metrics.requests,
      requestsPerSecond: requestsPerSecond.toFixed(2),
      errors: this.metrics.errors,
      errorRate: `${errorRate.toFixed(2)}%`,
      slowRequests: this.metrics.slowRequests,
      averageDuration: `${this.metrics.averageDuration.toFixed(2)}ms`,
      minDuration: `${this.metrics.minDuration}ms`,
      maxDuration: `${this.metrics.maxDuration}ms`,
      routes: Object.fromEntries(this.metrics.routes)
    };
  }

  /**
   * Reset metrics
   */
  reset() {
    this.metrics = {
      requests: 0,
      errors: 0,
      slowRequests: 0,
      totalDuration: 0,
      averageDuration: 0,
      minDuration: Infinity,
      maxDuration: 0,
      routes: new Map()
    };
    this.startTime = Date.now();
  }
}

// Global performance collector instance
const performanceCollector = new PerformanceCollector();

/**
 * Get performance metrics endpoint middleware
 */
const getPerformanceMetrics = (req, res) => {
  const summary = performanceCollector.getSummary();
  
  res.json({
    success: true,
    data: summary,
    timestamp: new Date().toISOString()
  });
};

/**
 * Reset performance metrics endpoint middleware
 */
const resetPerformanceMetrics = (req, res) => {
  performanceCollector.reset();
  
  res.json({
    success: true,
    message: 'Performance metrics reset successfully',
    timestamp: new Date().toISOString()
  });
};

module.exports = {
  routePerformanceMiddleware,
  PerformanceCollector,
  performanceCollector,
  getPerformanceMetrics,
  resetPerformanceMetrics
};
````

## File: src/middleware/securityMiddleware.js
````javascript
/**
 * Security Middleware
 * Comprehensive security enhancements for the application
 */

const helmet = require('helmet');
const { logger } = require('../config/logger');

/**
 * Input sanitization middleware
 * Removes potentially dangerous characters and patterns
 */
const inputSanitization = (req, res, next) => {
  try {
    // Sanitize request body
    if (req.body) {
      req.body = sanitizeObject(req.body);
    }

    // Sanitize query parameters
    if (req.query) {
      req.query = sanitizeObject(req.query);
    }

    // Sanitize URL parameters
    if (req.params) {
      req.params = sanitizeObject(req.params);
    }

    next();
  } catch (error) {
    logger.error('Input sanitization error:', error);
    res.status(400).json({
      success: false,
      error: 'Invalid input detected',
      timestamp: new Date().toISOString()
    });
  }
};

/**
 * Recursively sanitize object properties
 */
function sanitizeObject(obj) {
  if (typeof obj !== 'object' || obj === null) {
    return sanitizeValue(obj);
  }

  if (Array.isArray(obj)) {
    return obj.map(item => sanitizeObject(item));
  }

  const sanitized = {};
  for (const [key, value] of Object.entries(obj)) {
    sanitized[key] = sanitizeObject(value);
  }
  return sanitized;
}

/**
 * Sanitize individual values
 */
function sanitizeValue(value) {
  if (typeof value !== 'string') {
    return value;
  }

  return value
    // Remove null bytes
    .replace(/\0/g, '')
    // Remove control characters except newlines and tabs
    .replace(/[\x00-\x08\x0B\x0C\x0E-\x1F\x7F]/g, '')
    // Remove potential SQL injection patterns
    .replace(/('|"|;|--|\/\*|\*\/|union|select|insert|update|delete|drop|create|alter|exec|execute|script|javascript|vbscript|onload|onerror|onclick)/gi, '')
    // Remove potential XSS patterns
    .replace(/<script\b[^<]*(?:(?!<\/script>)<[^<]*)*<\/script>/gi, '')
    .replace(/javascript:/gi, '')
    .replace(/on\w+\s*=/gi, '')
    // Trim whitespace
    .trim();
}

/**
 * SQL Injection prevention middleware
 */
const sqlInjectionPrevention = (req, res, next) => {
  const sqlPatterns = [
    /(\b(union|select|insert|update|delete|drop|create|alter|exec|execute)\b)/gi,
    /(--|\/\*|\*\/|;)/g,
    /(\b(and|or)\b\s+\d+\s*=\s*\d+)/gi,
    /(\b(and|or)\b\s+['"]\w+['"]\s*=\s*['"]\w+['"])/gi
  ];

  const checkValue = (value) => {
    if (typeof value === 'string') {
      for (const pattern of sqlPatterns) {
        if (pattern.test(value)) {
          return false;
        }
      }
    }
    return true;
  };

  const checkObject = (obj) => {
    if (typeof obj !== 'object' || obj === null) {
      return checkValue(obj);
    }

    if (Array.isArray(obj)) {
      return obj.every(item => checkObject(item));
    }

    for (const value of Object.values(obj)) {
      if (!checkObject(value)) {
        return false;
      }
    }
    return true;
  };

  // Check request body, query, and params
  const bodySafe = checkObject(req.body);
  const querySafe = checkObject(req.query);
  const paramsSafe = checkObject(req.params);

  if (!bodySafe || !querySafe || !paramsSafe) {
    logger.warn('Potential SQL injection attempt detected', {
      ip: req.ip,
      userAgent: req.get('User-Agent'),
      url: req.originalUrl
    });

    return res.status(400).json({
      success: false,
      error: 'Invalid input detected',
      timestamp: new Date().toISOString()
    });
  }

  next();
};

/**
 * XSS Prevention middleware
 */
const xssPrevention = (req, res, next) => {
  const xssPatterns = [
    /<script\b[^<]*(?:(?!<\/script>)<[^<]*)*<\/script>/gi,
    /javascript:/gi,
    /vbscript:/gi,
    /on\w+\s*=/gi,
    /<iframe\b[^<]*(?:(?!<\/iframe>)<[^<]*)*<\/iframe>/gi,
    /<object\b[^<]*(?:(?!<\/object>)<[^<]*)*<\/object>/gi,
    /<embed\b[^<]*(?:(?!<\/embed>)<[^<]*)*<\/embed>/gi,
    /<link\b[^<]*(?:(?!<\/link>)<[^<]*)*<\/link>/gi,
    /<meta\b[^<]*(?:(?!<\/meta>)<[^<]*)*<\/meta>/gi
  ];

  const checkValue = (value) => {
    if (typeof value === 'string') {
      for (const pattern of xssPatterns) {
        if (pattern.test(value)) {
          return false;
        }
      }
    }
    return true;
  };

  const checkObject = (obj) => {
    if (typeof obj !== 'object' || obj === null) {
      return checkValue(obj);
    }

    if (Array.isArray(obj)) {
      return obj.every(item => checkObject(item));
    }

    for (const value of Object.values(obj)) {
      if (!checkObject(value)) {
        return false;
      }
    }
    return true;
  };

  // Check request body, query, and params
  const bodySafe = checkObject(req.body);
  const querySafe = checkObject(req.query);
  const paramsSafe = checkObject(req.params);

  if (!bodySafe || !querySafe || !paramsSafe) {
    logger.warn('Potential XSS attempt detected', {
      ip: req.ip,
      userAgent: req.get('User-Agent'),
      url: req.originalUrl
    });

    return res.status(400).json({
      success: false,
      error: 'Invalid input detected',
      timestamp: new Date().toISOString()
    });
  }

  next();
};

/**
 * Request size limiting middleware
 */
const requestSizeLimit = (maxSize = '10mb') => {
  return (req, res, next) => {
    const contentLength = parseInt(req.get('Content-Length') || '0');
    const maxSizeBytes = parseSize(maxSize);

    if (contentLength > maxSizeBytes) {
      logger.warn('Request size limit exceeded', {
        ip: req.ip,
        contentLength,
        maxSizeBytes,
        url: req.originalUrl
      });

      return res.status(413).json({
        success: false,
        error: 'Request entity too large',
        timestamp: new Date().toISOString()
      });
    }

    next();
  };
};

/**
 * Parse size string to bytes
 */
function parseSize(size) {
  const units = {
    'b': 1,
    'kb': 1024,
    'mb': 1024 * 1024,
    'gb': 1024 * 1024 * 1024
  };

  const match = size.toLowerCase().match(/^(\d+(?:\.\d+)?)\s*(b|kb|mb|gb)$/);
  if (!match) {
    return 10 * 1024 * 1024; // Default 10MB
  }

  const [, value, unit] = match;
  return parseFloat(value) * units[unit];
}

/**
 * Content Security Policy middleware
 */
const contentSecurityPolicy = (req, res, next) => {
  res.setHeader('Content-Security-Policy', [
    "default-src 'self'",
    "script-src 'self' 'unsafe-inline' 'unsafe-eval' https://cdn.jsdelivr.net https://unpkg.com",
    "style-src 'self' 'unsafe-inline' https://fonts.googleapis.com https://cdn.jsdelivr.net",
    "font-src 'self' https://fonts.gstatic.com https://cdn.jsdelivr.net",
    "img-src 'self' data: https: blob:",
    "connect-src 'self' https://api.openai.com https://generativelanguage.googleapis.com",
    "frame-src 'none'",
    "object-src 'none'",
    "base-uri 'self'",
    "form-action 'self'"
  ].join('; '));

  next();
};

/**
 * Security headers middleware
 */
const securityHeaders = (req, res, next) => {
  // Prevent MIME type sniffing
  res.setHeader('X-Content-Type-Options', 'nosniff');
  
  // Prevent clickjacking
  res.setHeader('X-Frame-Options', 'DENY');
  
  // Enable XSS protection
  res.setHeader('X-XSS-Protection', '1; mode=block');
  
  // Referrer policy
  res.setHeader('Referrer-Policy', 'strict-origin-when-cross-origin');
  
  // Permissions policy
  res.setHeader('Permissions-Policy', [
    'camera=()',
    'microphone=()',
    'geolocation=()',
    'payment=()',
    'usb=()',
    'magnetometer=()',
    'gyroscope=()',
    'accelerometer=()'
  ].join(', '));

  next();
};

/**
 * Rate limiting for security endpoints
 */
const securityRateLimit = (req, res, next) => {
  // Implement stricter rate limiting for security-sensitive endpoints
  const securityEndpoints = [
    '/api/auth/login',
    '/api/auth/register',
    '/api/auth/forgot-password',
    '/api/auth/reset-password'
  ];

  if (securityEndpoints.some(endpoint => req.path.includes(endpoint))) {
    // Apply stricter rate limiting for security endpoints
    // This would integrate with the existing rate limiter
    logger.info('Security endpoint accessed', {
      ip: req.ip,
      path: req.path,
      userAgent: req.get('User-Agent')
    });
  }

  next();
};

/**
 * Helmet configuration
 */
const helmetConfig = helmet({
  contentSecurityPolicy: {
    directives: {
      defaultSrc: ["'self'"],
      scriptSrc: ["'self'", "'unsafe-inline'", "'unsafe-eval'", "https://cdn.jsdelivr.net", "https://unpkg.com"],
      styleSrc: ["'self'", "'unsafe-inline'", "https://fonts.googleapis.com", "https://cdn.jsdelivr.net"],
      fontSrc: ["'self'", "https://fonts.gstatic.com", "https://cdn.jsdelivr.net"],
      imgSrc: ["'self'", "data:", "https:", "blob:"],
      connectSrc: ["'self'", "https://api.openai.com", "https://generativelanguage.googleapis.com"],
      frameSrc: ["'none'"],
      objectSrc: ["'none'"],
      baseUri: ["'self'"],
      formAction: ["'self'"]
    }
  },
  crossOriginEmbedderPolicy: false,
  crossOriginOpenerPolicy: { policy: "same-origin" },
  crossOriginResourcePolicy: { policy: "cross-origin" },
  dnsPrefetchControl: { allow: false },
  frameguard: { action: "deny" },
  hidePoweredBy: true,
  hsts: {
    maxAge: 31536000,
    includeSubDomains: true,
    preload: true
  },
  ieNoOpen: true,
  noSniff: true,
  originAgentCluster: true,
  permittedCrossDomainPolicies: { permittedPolicies: "none" },
  referrerPolicy: { policy: "strict-origin-when-cross-origin" },
  xssFilter: true
});

/**
 * Security monitoring middleware
 */
const securityMonitoring = (req, res, next) => {
  // Log security-relevant information
  const securityInfo = {
    timestamp: new Date().toISOString(),
    ip: req.ip,
    userAgent: req.get('User-Agent'),
    method: req.method,
    url: req.originalUrl,
    referer: req.get('Referer'),
    origin: req.get('Origin'),
    contentType: req.get('Content-Type'),
    contentLength: req.get('Content-Length')
  };

  // Check for suspicious patterns
  const suspiciousPatterns = [
    /\.\.\//, // Directory traversal
    /<script/i, // Script tags
    /javascript:/i, // JavaScript protocol
    /union\s+select/i, // SQL injection
    /exec\s*\(/i, // Command execution
    /eval\s*\(/i, // Code evaluation
  ];

  const isSuspicious = suspiciousPatterns.some(pattern => 
    pattern.test(req.originalUrl) || 
    pattern.test(JSON.stringify(req.body)) || 
    pattern.test(JSON.stringify(req.query))
  );

  if (isSuspicious) {
    logger.warn('Suspicious request detected', securityInfo);
  }

  // Store security info for monitoring
  req.securityInfo = securityInfo;

  next();
};

module.exports = {
  inputSanitization,
  sqlInjectionPrevention,
  xssPrevention,
  requestSizeLimit,
  contentSecurityPolicy,
  securityHeaders,
  securityRateLimit,
  helmetConfig,
  securityMonitoring
};
````

## File: src/middleware/validation.js
````javascript
/**
 * Validation Middleware
 * Middleware for validating request data using Joi schemas
 */

const { ValidationError } = require('../utils/errors');

/**
 * Generic validation middleware
 * @param {Object} schema - Joi schema to validate against
 * @param {string} source - Source of data to validate ('body', 'query', 'params')
 * @returns {Function} Express middleware function
 */
function validate(schema, source = 'body') {
  return (req, res, next) => {
    const dataToValidate = req[source];
    
    const { error, value } = schema.validate(dataToValidate, {
      abortEarly: false,
      stripUnknown: true,
      allowUnknown: false
    });
    
    if (error) {
      const validationError = new ValidationError(
        'Validation failed',
        null,
        dataToValidate,
        'SCHEMA_VALIDATION'
      );
      
      // Add validation details
      error.details.forEach(detail => {
        validationError.addDetail(
          detail.path.join('.'),
          detail.message,
          detail.context?.value,
          detail.type
        );
      });
      
      return next(validationError);
    }
    
    // Replace the original data with validated data
    req[source] = value;
    next();
  };
}

/**
 * Validate request body
 * @param {Object} schema - Joi schema
 * @returns {Function} Express middleware function
 */
function validateBody(schema) {
  return validate(schema, 'body');
}

/**
 * Validate request query parameters
 * @param {Object} schema - Joi schema
 * @returns {Function} Express middleware function
 */
function validateQuery(schema) {
  return validate(schema, 'query');
}

/**
 * Validate request URL parameters
 * @param {Object} schema - Joi schema
 * @returns {Function} Express middleware function
 */
function validateParams(schema) {
  return validate(schema, 'params');
}

/**
 * Validate file upload
 * @param {Object} options - File validation options
 * @returns {Function} Express middleware function
 */
function validateFile(options = {}) {
  const {
    maxSize = 10 * 1024 * 1024, // 10MB
    allowedTypes = ['application/pdf', 'application/msword', 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'],
    fieldName = 'file'
  } = options;
  
  return (req, res, next) => {
    if (!req.file && !req.files) {
      const error = new ValidationError(
        'No file uploaded',
        fieldName,
        null,
        'FILE_MISSING'
      );
      return next(error);
    }
    
    const file = req.file || req.files[fieldName];
    
    if (!file) {
      const error = new ValidationError(
        `File field '${fieldName}' is required`,
        fieldName,
        null,
        'FILE_MISSING'
      );
      return next(error);
    }
    
    // Check file size
    if (file.size > maxSize) {
      const error = ValidationError.fileTooLarge(
        file.originalname,
        maxSize,
        file.size
      );
      return next(error);
    }
    
    // Check file type
    if (!allowedTypes.includes(file.mimetype)) {
      const error = ValidationError.invalidFileType(
        file.originalname,
        allowedTypes,
        file.mimetype
      );
      return next(error);
    }
    
    next();
  };
}

/**
 * Sanitize request data
 * @param {Object} schema - Joi schema with sanitization rules
 * @param {string} source - Source of data to sanitize
 * @returns {Function} Express middleware function
 */
function sanitize(schema, source = 'body') {
  return (req, res, next) => {
    const dataToSanitize = req[source];
    
    const { value } = schema.validate(dataToSanitize, {
      abortEarly: false,
      stripUnknown: true,
      allowUnknown: false
    });
    
    // Replace the original data with sanitized data
    req[source] = value;
    next();
  };
}

/**
 * Validate pagination parameters
 * @returns {Function} Express middleware function
 */
function validatePagination() {
  const paginationSchema = require('joi').object({
    page: require('joi').number().integer().min(1).default(1),
    limit: require('joi').number().integer().min(1).max(100).default(10),
    sort_by: require('joi').string().optional(),
    sort_order: require('joi').string().valid('asc', 'desc').default('desc')
  });
  
  return validateQuery(paginationSchema);
}

/**
 * Validate ID parameter
 * @param {string} paramName - Name of the ID parameter
 * @returns {Function} Express middleware function
 */
function validateId(paramName = 'id') {
  const idSchema = require('joi').object({
    [paramName]: require('joi').number().integer().positive().required()
  });
  
  return validateParams(idSchema);
}

/**
 * Validate UUID parameter
 * @param {string} paramName - Name of the UUID parameter
 * @returns {Function} Express middleware function
 */
function validateUuid(paramName = 'id') {
  const uuidSchema = require('joi').object({
    [paramName]: require('joi').string().uuid().required()
  });
  
  return validateParams(uuidSchema);
}

module.exports = {
  validate,
  validateBody,
  validateQuery,
  validateParams,
  validateFile,
  sanitize,
  validatePagination,
  validateId,
  validateUuid
};
````

## File: src/models/schemas/careerSchemas.js
````javascript
/**
 * Career Profile Validation Schemas
 * Joi schemas for career profile-related data validation
 */

const Joi = require('joi');

/**
 * Career profile creation schema
 */
const careerProfileCreateSchema = Joi.object({
  title: Joi.string()
    .min(1)
    .max(255)
    .required()
    .messages({
      'string.min': 'Career profile title must be at least 1 character long',
      'string.max': 'Career profile title cannot exceed 255 characters',
      'any.required': 'Career profile title is required'
    }),
  
  summary: Joi.string()
    .min(10)
    .max(2000)
    .required()
    .messages({
      'string.min': 'Career summary must be at least 10 characters long',
      'string.max': 'Career summary cannot exceed 2000 characters',
      'any.required': 'Career summary is required'
    }),
  
  skills: Joi.array()
    .items(Joi.string().min(1).max(100))
    .min(1)
    .max(50)
    .required()
    .messages({
      'array.min': 'At least one skill is required',
      'array.max': 'Cannot exceed 50 skills',
      'any.required': 'Skills are required'
    }),
  
  experience_level: Joi.string()
    .valid('entry', 'junior', 'mid', 'senior', 'lead', 'executive')
    .required()
    .messages({
      'any.only': 'Please select a valid experience level',
      'any.required': 'Experience level is required'
    }),
  
  desired_salary_min: Joi.number()
    .positive()
    .optional()
    .messages({
      'number.base': 'Minimum desired salary must be a number',
      'number.positive': 'Minimum desired salary must be positive'
    }),
  
  desired_salary_max: Joi.number()
    .positive()
    .greater(Joi.ref('desired_salary_min'))
    .optional()
    .messages({
      'number.base': 'Maximum desired salary must be a number',
      'number.positive': 'Maximum desired salary must be positive',
      'number.greater': 'Maximum salary must be greater than minimum salary'
    }),
  
  preferred_locations: Joi.array()
    .items(Joi.string().min(2).max(100))
    .max(10)
    .optional()
    .messages({
      'array.max': 'Cannot exceed 10 preferred locations'
    }),
  
  remote_preference: Joi.string()
    .valid('on_site', 'hybrid', 'remote', 'flexible')
    .default('flexible')
    .optional()
    .messages({
      'any.only': 'Please select a valid remote preference'
    }),
  
  industry_preferences: Joi.array()
    .items(Joi.string().min(2).max(100))
    .max(10)
    .optional()
    .messages({
      'array.max': 'Cannot exceed 10 industry preferences'
    }),
  
  work_authorization: Joi.string()
    .valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other')
    .required()
    .messages({
      'any.only': 'Please select a valid work authorization status',
      'any.required': 'Work authorization status is required'
    }),
  
  availability: Joi.string()
    .valid('immediate', 'two_weeks', 'one_month', 'three_months', 'negotiable')
    .default('negotiable')
    .optional()
    .messages({
      'any.only': 'Please select a valid availability option'
    }),
  
  is_public: Joi.boolean()
    .default(false)
    .optional()
});

/**
 * Career profile update schema
 */
const careerProfileUpdateSchema = Joi.object({
  title: Joi.string()
    .min(1)
    .max(255)
    .optional()
    .messages({
      'string.min': 'Career profile title must be at least 1 character long',
      'string.max': 'Career profile title cannot exceed 255 characters'
    }),
  
  summary: Joi.string()
    .min(10)
    .max(2000)
    .optional()
    .messages({
      'string.min': 'Career summary must be at least 10 characters long',
      'string.max': 'Career summary cannot exceed 2000 characters'
    }),
  
  skills: Joi.array()
    .items(Joi.string().min(1).max(100))
    .min(1)
    .max(50)
    .optional()
    .messages({
      'array.min': 'At least one skill is required',
      'array.max': 'Cannot exceed 50 skills'
    }),
  
  experience_level: Joi.string()
    .valid('entry', 'junior', 'mid', 'senior', 'lead', 'executive')
    .optional()
    .messages({
      'any.only': 'Please select a valid experience level'
    }),
  
  desired_salary_min: Joi.number()
    .positive()
    .optional()
    .messages({
      'number.base': 'Minimum desired salary must be a number',
      'number.positive': 'Minimum desired salary must be positive'
    }),
  
  desired_salary_max: Joi.number()
    .positive()
    .greater(Joi.ref('desired_salary_min'))
    .optional()
    .messages({
      'number.base': 'Maximum desired salary must be a number',
      'number.positive': 'Maximum desired salary must be positive',
      'number.greater': 'Maximum salary must be greater than minimum salary'
    }),
  
  preferred_locations: Joi.array()
    .items(Joi.string().min(2).max(100))
    .max(10)
    .optional()
    .messages({
      'array.max': 'Cannot exceed 10 preferred locations'
    }),
  
  remote_preference: Joi.string()
    .valid('on_site', 'hybrid', 'remote', 'flexible')
    .optional()
    .messages({
      'any.only': 'Please select a valid remote preference'
    }),
  
  industry_preferences: Joi.array()
    .items(Joi.string().min(2).max(100))
    .max(10)
    .optional()
    .messages({
      'array.max': 'Cannot exceed 10 industry preferences'
    }),
  
  work_authorization: Joi.string()
    .valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other')
    .optional()
    .messages({
      'any.only': 'Please select a valid work authorization status'
    }),
  
  availability: Joi.string()
    .valid('immediate', 'two_weeks', 'one_month', 'three_months', 'negotiable')
    .optional()
    .messages({
      'any.only': 'Please select a valid availability option'
    }),
  
  is_public: Joi.boolean()
    .optional()
});

/**
 * Job search schema
 */
const jobSearchSchema = Joi.object({
  query: Joi.string()
    .min(1)
    .max(255)
    .optional()
    .messages({
      'string.min': 'Search query must be at least 1 character long',
      'string.max': 'Search query cannot exceed 255 characters'
    }),
  
  location: Joi.string()
    .min(2)
    .max(100)
    .optional()
    .messages({
      'string.min': 'Location must be at least 2 characters long',
      'string.max': 'Location cannot exceed 100 characters'
    }),
  
  experience_level: Joi.string()
    .valid('entry', 'junior', 'mid', 'senior', 'lead', 'executive', 'all')
    .default('all')
    .optional()
    .messages({
      'any.only': 'Please select a valid experience level'
    }),
  
  remote_preference: Joi.string()
    .valid('on_site', 'hybrid', 'remote', 'flexible', 'all')
    .default('all')
    .optional()
    .messages({
      'any.only': 'Please select a valid remote preference'
    }),
  
  salary_min: Joi.number()
    .positive()
    .optional()
    .messages({
      'number.base': 'Minimum salary must be a number',
      'number.positive': 'Minimum salary must be positive'
    }),
  
  salary_max: Joi.number()
    .positive()
    .greater(Joi.ref('salary_min'))
    .optional()
    .messages({
      'number.base': 'Maximum salary must be a number',
      'number.positive': 'Maximum salary must be positive',
      'number.greater': 'Maximum salary must be greater than minimum salary'
    }),
  
  job_type: Joi.string()
    .valid('full_time', 'part_time', 'contract', 'internship', 'all')
    .default('all')
    .optional()
    .messages({
      'any.only': 'Please select a valid job type'
    }),
  
  industry: Joi.string()
    .min(2)
    .max(100)
    .optional()
    .messages({
      'string.min': 'Industry must be at least 2 characters long',
      'string.max': 'Industry cannot exceed 100 characters'
    }),
  
  sort_by: Joi.string()
    .valid('relevance', 'date', 'salary', 'location')
    .default('relevance')
    .optional()
    .messages({
      'any.only': 'Please select a valid sort field'
    }),
  
  sort_order: Joi.string()
    .valid('asc', 'desc')
    .default('desc')
    .optional()
    .messages({
      'any.only': 'Sort order must be either "asc" or "desc"'
    }),
  
  page: Joi.number()
    .integer()
    .min(1)
    .default(1)
    .optional()
    .messages({
      'number.base': 'Page must be a number',
      'number.integer': 'Page must be an integer',
      'number.min': 'Page must be at least 1'
    }),
  
  limit: Joi.number()
    .integer()
    .min(1)
    .max(50)
    .default(10)
    .optional()
    .messages({
      'number.base': 'Limit must be a number',
      'number.integer': 'Limit must be an integer',
      'number.min': 'Limit must be at least 1',
      'number.max': 'Limit cannot exceed 50'
    })
});

/**
 * Job application schema
 */
const jobApplicationSchema = Joi.object({
  job_id: Joi.string()
    .required()
    .messages({
      'any.required': 'Job ID is required'
    }),
  
  resume_id: Joi.number()
    .integer()
    .positive()
    .required()
    .messages({
      'number.base': 'Resume ID must be a number',
      'number.integer': 'Resume ID must be an integer',
      'number.positive': 'Resume ID must be positive',
      'any.required': 'Resume ID is required'
    }),
  
  cover_letter: Joi.string()
    .max(2000)
    .optional()
    .messages({
      'string.max': 'Cover letter cannot exceed 2000 characters'
    }),
  
  expected_salary: Joi.number()
    .positive()
    .optional()
    .messages({
      'number.base': 'Expected salary must be a number',
      'number.positive': 'Expected salary must be positive'
    }),
  
  availability_date: Joi.date()
    .min('now')
    .optional()
    .messages({
      'date.min': 'Availability date must be in the future'
    }),
  
  additional_notes: Joi.string()
    .max(1000)
    .optional()
    .messages({
      'string.max': 'Additional notes cannot exceed 1000 characters'
    })
});

/**
 * Career profile matching schema
 */
const careerProfileMatchingSchema = Joi.object({
  profile_id: Joi.number()
    .integer()
    .positive()
    .required()
    .messages({
      'number.base': 'Profile ID must be a number',
      'number.integer': 'Profile ID must be an integer',
      'number.positive': 'Profile ID must be positive',
      'any.required': 'Profile ID is required'
    }),
  
  match_criteria: Joi.object({
    skills_weight: Joi.number()
      .min(0)
      .max(1)
      .default(0.4)
      .optional(),
    
    experience_weight: Joi.number()
      .min(0)
      .max(1)
      .default(0.3)
      .optional(),
    
    location_weight: Joi.number()
      .min(0)
      .max(1)
      .default(0.2)
      .optional(),
    
    salary_weight: Joi.number()
      .min(0)
      .max(1)
      .default(0.1)
      .optional()
  }).optional(),
  
  limit: Joi.number()
    .integer()
    .min(1)
    .max(50)
    .default(10)
    .optional()
    .messages({
      'number.base': 'Limit must be a number',
      'number.integer': 'Limit must be an integer',
      'number.min': 'Limit must be at least 1',
      'number.max': 'Limit cannot exceed 50'
    })
});

module.exports = {
  careerProfileCreateSchema,
  careerProfileUpdateSchema,
  jobSearchSchema,
  jobApplicationSchema,
  careerProfileMatchingSchema
};
````

## File: src/models/schemas/index.js
````javascript
/**
 * Validation Schemas Index
 * Exports all Joi validation schemas
 */

const userSchemas = require('./userSchemas');
const resumeSchemas = require('./resumeSchemas');
const careerSchemas = require('./careerSchemas');

module.exports = {
  userSchemas,
  resumeSchemas,
  careerSchemas
};
````

## File: src/models/schemas/resumeSchemas.js
````javascript
/**
 * Resume Validation Schemas
 * Joi schemas for resume-related data validation
 */

const Joi = require('joi');

/**
 * Resume upload schema
 */
const resumeUploadSchema = Joi.object({
  title: Joi.string()
    .min(1)
    .max(255)
    .optional()
    .messages({
      'string.min': 'Resume title must be at least 1 character long',
      'string.max': 'Resume title cannot exceed 255 characters'
    }),
  
  description: Joi.string()
    .max(1000)
    .optional()
    .messages({
      'string.max': 'Resume description cannot exceed 1000 characters'
    }),
  
  category: Joi.string()
    .valid('professional', 'academic', 'creative', 'technical', 'general')
    .optional()
    .messages({
      'any.only': 'Please select a valid resume category'
    }),
  
  is_public: Joi.boolean()
    .default(false)
    .optional()
});

/**
 * Resume analysis request schema
 */
const resumeAnalysisRequestSchema = Joi.object({
  resume_id: Joi.number()
    .integer()
    .positive()
    .required()
    .messages({
      'number.base': 'Resume ID must be a number',
      'number.integer': 'Resume ID must be an integer',
      'number.positive': 'Resume ID must be positive',
      'any.required': 'Resume ID is required'
    }),
  
  analysis_type: Joi.string()
    .valid('comprehensive', 'skills', 'experience', 'education', 'formatting')
    .default('comprehensive')
    .optional()
    .messages({
      'any.only': 'Please select a valid analysis type'
    }),
  
  include_suggestions: Joi.boolean()
    .default(true)
    .optional(),
  
  include_skills_extraction: Joi.boolean()
    .default(true)
    .optional(),
  
  include_market_analysis: Joi.boolean()
    .default(false)
    .optional()
});

/**
 * Resume update schema
 */
const resumeUpdateSchema = Joi.object({
  title: Joi.string()
    .min(1)
    .max(255)
    .optional()
    .messages({
      'string.min': 'Resume title must be at least 1 character long',
      'string.max': 'Resume title cannot exceed 255 characters'
    }),
  
  description: Joi.string()
    .max(1000)
    .optional()
    .messages({
      'string.max': 'Resume description cannot exceed 1000 characters'
    }),
  
  category: Joi.string()
    .valid('professional', 'academic', 'creative', 'technical', 'general')
    .optional()
    .messages({
      'any.only': 'Please select a valid resume category'
    }),
  
  is_public: Joi.boolean()
    .optional()
});

/**
 * Resume search schema
 */
const resumeSearchSchema = Joi.object({
  query: Joi.string()
    .min(1)
    .optional()
    .messages({
      'string.min': 'Search query must be at least 1 character long'
    }),
  
  category: Joi.string()
    .valid('professional', 'academic', 'creative', 'technical', 'general')
    .optional()
    .messages({
      'any.only': 'Please select a valid resume category'
    }),
  
  skills: Joi.array()
    .items(Joi.string())
    .optional(),
  
  experience_level: Joi.string()
    .valid('entry', 'mid', 'senior', 'executive')
    .optional()
    .messages({
      'any.only': 'Please select a valid experience level'
    }),
  
  date_from: Joi.date()
    .max('now')
    .optional()
    .messages({
      'date.max': 'Date from cannot be in the future'
    }),
  
  date_to: Joi.date()
    .max('now')
    .optional()
    .messages({
      'date.max': 'Date to cannot be in the future'
    }),
  
  page: Joi.number()
    .integer()
    .min(1)
    .default(1)
    .optional()
    .messages({
      'number.base': 'Page must be a number',
      'number.integer': 'Page must be an integer',
      'number.min': 'Page must be at least 1'
    }),
  
  limit: Joi.number()
    .integer()
    .min(1)
    .max(100)
    .default(10)
    .optional()
    .messages({
      'number.base': 'Limit must be a number',
      'number.integer': 'Limit must be an integer',
      'number.min': 'Limit must be at least 1',
      'number.max': 'Limit cannot exceed 100'
    })
});

/**
 * Resume analysis feedback schema
 */
const resumeAnalysisFeedbackSchema = Joi.object({
  analysis_id: Joi.number()
    .integer()
    .positive()
    .required()
    .messages({
      'number.base': 'Analysis ID must be a number',
      'number.integer': 'Analysis ID must be an integer',
      'number.positive': 'Analysis ID must be positive',
      'any.required': 'Analysis ID is required'
    }),
  
  rating: Joi.number()
    .integer()
    .min(1)
    .max(5)
    .required()
    .messages({
      'number.base': 'Rating must be a number',
      'number.integer': 'Rating must be an integer',
      'number.min': 'Rating must be at least 1',
      'number.max': 'Rating cannot exceed 5',
      'any.required': 'Rating is required'
    }),
  
  feedback: Joi.string()
    .max(1000)
    .optional()
    .messages({
      'string.max': 'Feedback cannot exceed 1000 characters'
    }),
  
  helpful: Joi.boolean()
    .optional()
});

/**
 * Resume sharing schema
 */
const resumeSharingSchema = Joi.object({
  resume_id: Joi.number()
    .integer()
    .positive()
    .required()
    .messages({
      'number.base': 'Resume ID must be a number',
      'number.integer': 'Resume ID must be an integer',
      'number.positive': 'Resume ID must be positive',
      'any.required': 'Resume ID is required'
    }),
  
  share_type: Joi.string()
    .valid('public', 'private', 'link')
    .required()
    .messages({
      'any.only': 'Please select a valid share type',
      'any.required': 'Share type is required'
    }),
  
  expires_at: Joi.date()
    .greater('now')
    .optional()
    .messages({
      'date.greater': 'Expiration date must be in the future'
    }),
  
  allow_download: Joi.boolean()
    .default(false)
    .optional(),
  
  allow_comments: Joi.boolean()
    .default(false)
    .optional()
});

// Additional schemas for controller routes
const saveResumeAnalysis = Joi.object({
  originalFileName: Joi.string().required(),
  analysisData: Joi.object().required(),
  userId: Joi.string().uuid().optional()
});

const uploadAndAnalyzeResume = Joi.object({
  file: Joi.object().required(),
  userId: Joi.string().uuid().optional()
});

const getUserResumeAnalyses = Joi.object({
  userId: Joi.string().uuid().optional(),
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional()
});

const searchResumeAnalyses = Joi.object({
  query: Joi.string().min(1).optional(),
  userId: Joi.string().uuid().optional(),
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional()
});

const getResumeAnalysisById = Joi.object({
  analysisId: Joi.string().uuid().required()
});

const updateResumeAnalysis = Joi.object({
  analysisId: Joi.string().uuid().required(),
  analysisData: Joi.object().optional(),
  userId: Joi.string().uuid().optional()
});

const deleteResumeAnalysis = Joi.object({
  analysisId: Joi.string().uuid().required(),
  userId: Joi.string().uuid().optional()
});

const bulkDeleteResumeAnalyses = Joi.object({
  analysisIds: Joi.array().items(Joi.string().uuid()).required(),
  userId: Joi.string().uuid().optional()
});

const getResumeAnalysesByUserId = Joi.object({
  userId: Joi.string().uuid().required(),
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional()
});

const getResumeAnalysisWithParsedData = Joi.object({
  analysisId: Joi.string().uuid().required()
});

// ========================================
// RESUME GENERATOR VALIDATION SCHEMAS
// ========================================

/**
 * Generate Canadian resume schema
 */
const generateCanadianResume = Joi.object({
  originalAnalysisId: Joi.string().uuid().required()
    .messages({
      'string.guid': 'Original analysis ID must be a valid UUID',
      'any.required': 'Original analysis ID is required'
    }),
  
  jobTargeting: Joi.object({
    jobTitle: Joi.string().min(1).max(255).required()
      .messages({
        'string.min': 'Job title must be at least 1 character long',
        'string.max': 'Job title cannot exceed 255 characters',
        'any.required': 'Job title is required'
      }),
    
    companyName: Joi.string().min(1).max(255).required()
      .messages({
        'string.min': 'Company name must be at least 1 character long',
        'string.max': 'Company name cannot exceed 255 characters',
        'any.required': 'Company name is required'
      }),
    
    jobDescription: Joi.string().min(10).max(10000).optional()
      .messages({
        'string.min': 'Job description must be at least 10 characters long',
        'string.max': 'Job description cannot exceed 10,000 characters'
      }),
    
    industry: Joi.string().min(1).max(100).optional()
      .messages({
        'string.min': 'Industry must be at least 1 character long',
        'string.max': 'Industry cannot exceed 100 characters'
      }),
    
    location: Joi.string().min(1).max(255).optional()
      .messages({
        'string.min': 'Location must be at least 1 character long',
        'string.max': 'Location cannot exceed 255 characters'
      }),
    
    salaryRange: Joi.object({
      min: Joi.number().positive().optional(),
      max: Joi.number().positive().optional()
    }).optional(),
    
    requiredSkills: Joi.array().items(Joi.string().min(1).max(100)).optional(),
    preferredSkills: Joi.array().items(Joi.string().min(1).max(100)).optional(),
    experienceLevel: Joi.string().valid('entry', 'mid', 'senior', 'executive').optional()
  }).required()
    .messages({
      'any.required': 'Job targeting information is required'
    })
});

/**
 * Get user generated resumes schema
 */
const getUserGeneratedResumes = Joi.object({
  page: Joi.number().integer().min(1).default(1).optional()
    .messages({
      'number.base': 'Page must be a number',
      'number.integer': 'Page must be an integer',
      'number.min': 'Page must be at least 1'
    }),
  
  limit: Joi.number().integer().min(1).max(100).default(20).optional()
    .messages({
      'number.base': 'Limit must be a number',
      'number.integer': 'Limit must be an integer',
      'number.min': 'Limit must be at least 1',
      'number.max': 'Limit cannot exceed 100'
    }),
  
  sortBy: Joi.string().valid('jobTitle', 'companyName', 'createdAt', 'atsScore').default('createdAt').optional(),
  sortOrder: Joi.string().valid('asc', 'desc').default('desc').optional()
});

/**
 * Get generated resume by ID schema
 */
const getGeneratedResumeById = Joi.object({
  resumeId: Joi.string().uuid().required()
    .messages({
      'string.guid': 'Resume ID must be a valid UUID',
      'any.required': 'Resume ID is required'
    })
});

/**
 * Update generated resume schema
 */
const updateGeneratedResume = Joi.object({
  resumeId: Joi.string().uuid().required()
    .messages({
      'string.guid': 'Resume ID must be a valid UUID',
      'any.required': 'Resume ID is required'
    }),
  
  personalInfo: Joi.object({
    name: Joi.string().min(1).max(255).optional(),
    email: Joi.string().email().optional(),
    phone: Joi.string().min(10).max(20).optional(),
    location: Joi.string().min(1).max(255).optional(),
    linkedin: Joi.string().uri().optional(),
    website: Joi.string().uri().optional()
  }).optional(),
  
  professionalSummary: Joi.string().min(10).max(2000).optional(),
  
  skills: Joi.array().items(Joi.object({
    name: Joi.string().min(1).max(100).required(),
    level: Joi.string().valid('beginner', 'intermediate', 'advanced', 'expert').optional(),
    category: Joi.string().min(1).max(50).optional()
  })).optional(),
  
  workExperience: Joi.array().items(Joi.object({
    title: Joi.string().min(1).max(255).required(),
    company: Joi.string().min(1).max(255).required(),
    location: Joi.string().min(1).max(255).optional(),
    startDate: Joi.date().optional(),
    endDate: Joi.date().optional(),
    current: Joi.boolean().optional(),
    description: Joi.string().min(10).max(2000).optional(),
    achievements: Joi.array().items(Joi.string().min(1).max(500)).optional()
  })).optional(),
  
  education: Joi.array().items(Joi.object({
    degree: Joi.string().min(1).max(255).required(),
    institution: Joi.string().min(1).max(255).required(),
    location: Joi.string().min(1).max(255).optional(),
    graduationDate: Joi.date().optional(),
    gpa: Joi.number().min(0).max(4).optional(),
    relevantCourses: Joi.array().items(Joi.string().min(1).max(255)).optional()
  })).optional(),
  
  certifications: Joi.array().items(Joi.object({
    name: Joi.string().min(1).max(255).required(),
    issuer: Joi.string().min(1).max(255).required(),
    issueDate: Joi.date().optional(),
    expiryDate: Joi.date().optional(),
    credentialId: Joi.string().min(1).max(100).optional()
  })).optional(),
  
  projects: Joi.array().items(Joi.object({
    name: Joi.string().min(1).max(255).required(),
    description: Joi.string().min(10).max(1000).optional(),
    technologies: Joi.array().items(Joi.string().min(1).max(100)).optional(),
    url: Joi.string().uri().optional(),
    startDate: Joi.date().optional(),
    endDate: Joi.date().optional()
  })).optional(),
  
  atsScore: Joi.number().min(0).max(100).optional(),
  status: Joi.string().valid('draft', 'final', 'archived').optional(),
  metadata: Joi.object().optional()
});

/**
 * Auto-save user edits schema
 */
const autoSaveUserEdits = Joi.object({
  resumeId: Joi.string().uuid().required()
    .messages({
      'string.guid': 'Resume ID must be a valid UUID',
      'any.required': 'Resume ID is required'
    }),
  
  userEdits: Joi.object({
    personalInfo: Joi.object().optional(),
    professionalSummary: Joi.string().optional(),
    skills: Joi.array().optional(),
    workExperience: Joi.array().optional(),
    education: Joi.array().optional(),
    certifications: Joi.array().optional(),
    projects: Joi.array().optional()
  }).required()
    .messages({
      'any.required': 'User edits are required'
    })
});

/**
 * Search generated resumes schema
 */
const searchGeneratedResumes = Joi.object({
  jobTitle: Joi.string().min(1).max(255).optional(),
  companyName: Joi.string().min(1).max(255).optional(),
  industry: Joi.string().min(1).max(100).optional(),
  status: Joi.string().valid('draft', 'final', 'archived').optional(),
  createdAfter: Joi.date().optional(),
  createdBefore: Joi.date().optional(),
  page: Joi.number().integer().min(1).default(1).optional(),
  limit: Joi.number().integer().min(1).max(100).default(20).optional(),
  sortBy: Joi.string().valid('jobTitle', 'companyName', 'createdAt', 'atsScore').default('createdAt').optional(),
  sortOrder: Joi.string().valid('asc', 'desc').default('desc').optional()
});

/**
 * Delete generated resume schema
 */
const deleteGeneratedResume = Joi.object({
  resumeId: Joi.string().uuid().required()
    .messages({
      'string.guid': 'Resume ID must be a valid UUID',
      'any.required': 'Resume ID is required'
    })
});

/**
 * Analyze job targeting schema
 */
const analyzeJobTargeting = Joi.object({
  jobDescription: Joi.string().min(10).max(10000).required()
    .messages({
      'string.min': 'Job description must be at least 10 characters long',
      'string.max': 'Job description cannot exceed 10,000 characters',
      'any.required': 'Job description is required'
    }),
  
  userProfile: Joi.object({
    skills: Joi.array().items(Joi.string().min(1).max(100)).optional(),
    experience: Joi.array().optional(),
    education: Joi.array().optional(),
    targetIndustry: Joi.string().min(1).max(100).optional(),
    targetLocation: Joi.string().min(1).max(255).optional()
  }).optional()
});

/**
 * Translate skills for Canadian market schema
 */
const translateSkillsForCanadianMarket = Joi.object({
  skills: Joi.array().items(Joi.string().min(1).max(100)).required()
    .messages({
      'array.base': 'Skills must be an array',
      'any.required': 'Skills array is required'
    }),
  
  targetIndustry: Joi.string().min(1).max(100).optional()
    .messages({
      'string.min': 'Target industry must be at least 1 character long',
      'string.max': 'Target industry cannot exceed 100 characters'
    }),
  
  sourceCountry: Joi.string().min(2).max(3).optional()
    .messages({
      'string.min': 'Source country code must be at least 2 characters',
      'string.max': 'Source country code cannot exceed 3 characters'
    }),
  
  experienceLevel: Joi.string().valid('entry', 'mid', 'senior', 'executive').optional()
});

/**
 * Export resume schema
 */
const exportResume = Joi.object({
  resumeId: Joi.string().uuid().required()
    .messages({
      'string.guid': 'Resume ID must be a valid UUID',
      'any.required': 'Resume ID is required'
    }),
  
  format: Joi.string().valid('pdf', 'docx', 'txt').default('pdf').optional(),
  template: Joi.string().valid('professional', 'creative', 'minimal', 'executive').default('professional').optional(),
  includeATS: Joi.boolean().default(true).optional(),
  includeSuggestions: Joi.boolean().default(false).optional(),
  watermark: Joi.boolean().default(false).optional()
});

/**
 * Download resume PDF schema
 */
const downloadResumePDF = Joi.object({
  resumeId: Joi.string().uuid().required()
    .messages({
      'string.guid': 'Resume ID must be a valid UUID',
      'any.required': 'Resume ID is required'
    }),
  
  template: Joi.string().valid('professional', 'creative', 'minimal', 'executive').default('professional').optional()
});

/**
 * Bulk delete generated resumes schema
 */
const bulkDeleteGeneratedResumes = Joi.object({
  resumeIds: Joi.array().items(Joi.string().uuid()).min(1).max(50).required()
    .messages({
      'array.base': 'Resume IDs must be an array',
      'array.min': 'At least one resume ID is required',
      'array.max': 'Cannot delete more than 50 resumes at once',
      'any.required': 'Resume IDs array is required'
    })
});

/**
 * Bulk export resumes schema
 */
const bulkExportResumes = Joi.object({
  resumeIds: Joi.array().items(Joi.string().uuid()).min(1).max(10).required()
    .messages({
      'array.base': 'Resume IDs must be an array',
      'array.min': 'At least one resume ID is required',
      'array.max': 'Cannot export more than 10 resumes at once',
      'any.required': 'Resume IDs array is required'
    }),
  
  format: Joi.string().valid('pdf', 'docx', 'txt').default('pdf').optional(),
  template: Joi.string().valid('professional', 'creative', 'minimal', 'executive').default('professional').optional(),
  includeATS: Joi.boolean().default(true).optional(),
  includeSuggestions: Joi.boolean().default(false).optional()
});

module.exports = {
  // Original schemas
  resumeUploadSchema,
  resumeAnalysisRequestSchema,
  resumeUpdateSchema,
  resumeSearchSchema,
  resumeAnalysisFeedbackSchema,
  resumeSharingSchema,
  
  // Controller route schemas
  saveResumeAnalysis,
  uploadAndAnalyzeResume,
  getUserResumeAnalyses,
  searchResumeAnalyses,
  getResumeAnalysisById,
  updateResumeAnalysis,
  deleteResumeAnalysis,
  bulkDeleteResumeAnalyses,
  getResumeAnalysesByUserId,
  getResumeAnalysisWithParsedData,
  
  // Resume generator schemas
  generateCanadianResume,
  getUserGeneratedResumes,
  getGeneratedResumeById,
  updateGeneratedResume,
  autoSaveUserEdits,
  searchGeneratedResumes,
  deleteGeneratedResume,
  analyzeJobTargeting,
  translateSkillsForCanadianMarket,
  exportResume,
  downloadResumePDF,
  bulkDeleteGeneratedResumes,
  bulkExportResumes
};
````

## File: src/models/schemas/userSchemas.js
````javascript
/**
 * User Validation Schemas
 * Joi schemas for user-related data validation
 */

const Joi = require('joi');

/**
 * User registration schema
 */
const userRegistrationSchema = Joi.object({
  email: Joi.string()
    .email()
    .required()
    .messages({
      'string.email': 'Please provide a valid email address',
      'any.required': 'Email is required'
    }),
  
  full_name: Joi.string()
    .min(2)
    .max(100)
    .required()
    .messages({
      'string.min': 'Full name must be at least 2 characters long',
      'string.max': 'Full name cannot exceed 100 characters',
      'any.required': 'Full name is required'
    }),
  
  phone_no: Joi.string()
    .pattern(/^\+?[1-9]\d{1,14}$/)
    .optional()
    .messages({
      'string.pattern.base': 'Please provide a valid phone number'
    }),
  
  dob: Joi.date()
    .max('now')
    .optional()
    .messages({
      'date.max': 'Date of birth cannot be in the future'
    }),
  
  password: Joi.string()
    .min(8)
    .pattern(/^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]/)
    .required()
    .messages({
      'string.min': 'Password must be at least 8 characters long',
      'string.pattern.base': 'Password must contain at least one uppercase letter, one lowercase letter, one number, and one special character',
      'any.required': 'Password is required'
    }),
  
  confirm_password: Joi.string()
    .valid(Joi.ref('password'))
    .required()
    .messages({
      'any.only': 'Passwords must match',
      'any.required': 'Password confirmation is required'
    }),
  
  terms_condition_check: Joi.boolean()
    .valid(true)
    .required()
    .messages({
      'any.only': 'You must accept the terms and conditions',
      'any.required': 'Terms and conditions acceptance is required'
    }),
  
  status_in_canada: Joi.string()
    .valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other')
    .optional()
    .messages({
      'any.only': 'Please select a valid status in Canada'
    }),
  
  already_in_canada: Joi.boolean()
    .optional(),
  
  country_of_origin: Joi.string()
    .min(2)
    .max(100)
    .optional()
    .messages({
      'string.min': 'Country of origin must be at least 2 characters long',
      'string.max': 'Country of origin cannot exceed 100 characters'
    }),
  
  current_location: Joi.string()
    .min(2)
    .max(255)
    .optional()
    .messages({
      'string.min': 'Current location must be at least 2 characters long',
      'string.max': 'Current location cannot exceed 255 characters'
    })
});

/**
 * User login schema
 */
const userLoginSchema = Joi.object({
  email: Joi.string()
    .email()
    .required()
    .messages({
      'string.email': 'Please provide a valid email address',
      'any.required': 'Email is required'
    }),
  
  password: Joi.string()
    .required()
    .messages({
      'any.required': 'Password is required'
    })
});

/**
 * User profile update schema
 */
const userProfileUpdateSchema = Joi.object({
  full_name: Joi.string()
    .min(2)
    .max(100)
    .optional()
    .messages({
      'string.min': 'Full name must be at least 2 characters long',
      'string.max': 'Full name cannot exceed 100 characters'
    }),
  
  phone_no: Joi.string()
    .pattern(/^\+?[1-9]\d{1,14}$/)
    .optional()
    .messages({
      'string.pattern.base': 'Please provide a valid phone number'
    }),
  
  dob: Joi.date()
    .max('now')
    .optional()
    .messages({
      'date.max': 'Date of birth cannot be in the future'
    }),
  
  status_in_canada: Joi.string()
    .valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other')
    .optional()
    .messages({
      'any.only': 'Please select a valid status in Canada'
    }),
  
  already_in_canada: Joi.boolean()
    .optional(),
  
  country_of_origin: Joi.string()
    .min(2)
    .max(100)
    .optional()
    .messages({
      'string.min': 'Country of origin must be at least 2 characters long',
      'string.max': 'Country of origin cannot exceed 100 characters'
    }),
  
  current_location: Joi.string()
    .min(2)
    .max(255)
    .optional()
    .messages({
      'string.min': 'Current location must be at least 2 characters long',
      'string.max': 'Current location cannot exceed 255 characters'
    })
});

/**
 * Password change schema
 */
const passwordChangeSchema = Joi.object({
  current_password: Joi.string()
    .required()
    .messages({
      'any.required': 'Current password is required'
    }),
  
  new_password: Joi.string()
    .min(8)
    .pattern(/^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]/)
    .required()
    .messages({
      'string.min': 'New password must be at least 8 characters long',
      'string.pattern.base': 'New password must contain at least one uppercase letter, one lowercase letter, one number, and one special character',
      'any.required': 'New password is required'
    }),
  
  confirm_new_password: Joi.string()
    .valid(Joi.ref('new_password'))
    .required()
    .messages({
      'any.only': 'New passwords must match',
      'any.required': 'New password confirmation is required'
    })
});

/**
 * Password reset request schema
 */
const passwordResetRequestSchema = Joi.object({
  email: Joi.string()
    .email()
    .required()
    .messages({
      'string.email': 'Please provide a valid email address',
      'any.required': 'Email is required'
    })
});

/**
 * Password reset schema
 */
const passwordResetSchema = Joi.object({
  token: Joi.string()
    .required()
    .messages({
      'any.required': 'Reset token is required'
    }),
  
  new_password: Joi.string()
    .min(8)
    .pattern(/^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]/)
    .required()
    .messages({
      'string.min': 'New password must be at least 8 characters long',
      'string.pattern.base': 'New password must contain at least one uppercase letter, one lowercase letter, one number, and one special character',
      'any.required': 'New password is required'
    }),
  
  confirm_new_password: Joi.string()
    .valid(Joi.ref('new_password'))
    .required()
    .messages({
      'any.only': 'New passwords must match',
      'any.required': 'New password confirmation is required'
    })
});

/**
 * Email verification schema
 */
const emailVerificationSchema = Joi.object({
  token: Joi.string()
    .required()
    .messages({
      'any.required': 'Verification token is required'
    })
});

// Additional schemas for controller routes
const findOrCreateUser = Joi.object({
  email: Joi.string().email().required(),
  fullName: Joi.string().min(2).max(100).optional(),
  phoneNo: Joi.string().pattern(/^\+?[1-9]\d{1,14}$/).optional(),
  statusInCanada: Joi.string().valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other').optional(),
  countryOfOrigin: Joi.string().min(2).max(100).optional(),
  currentLocation: Joi.string().min(2).max(255).optional()
});

const updateProfile = Joi.object({
  fullName: Joi.string().min(2).max(100).optional(),
  phoneNo: Joi.string().pattern(/^\+?[1-9]\d{1,14}$/).optional(),
  statusInCanada: Joi.string().valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other').optional(),
  countryOfOrigin: Joi.string().min(2).max(100).optional(),
  currentLocation: Joi.string().min(2).max(255).optional()
});

const getUserById = Joi.object({
  userId: Joi.string().uuid().required()
});

const updateUser = Joi.object({
  userId: Joi.string().uuid().required(),
  fullName: Joi.string().min(2).max(100).optional(),
  phoneNo: Joi.string().pattern(/^\+?[1-9]\d{1,14}$/).optional(),
  statusInCanada: Joi.string().valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other').optional(),
  countryOfOrigin: Joi.string().min(2).max(100).optional(),
  currentLocation: Joi.string().min(2).max(255).optional()
});

const deleteUser = Joi.object({
  userId: Joi.string().uuid().required()
});

const getUserByEmail = Joi.object({
  email: Joi.string().email().required()
});

const searchUsers = Joi.object({
  query: Joi.string().min(1).optional(),
  statusInCanada: Joi.string().valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other').optional(),
  countryOfOrigin: Joi.string().optional(),
  currentLocation: Joi.string().optional(),
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional()
});

const getUsers = Joi.object({
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional(),
  sortBy: Joi.string().valid('created_at', 'full_name', 'email').optional(),
  sortOrder: Joi.string().valid('asc', 'desc').optional()
});

const getUsersByRole = Joi.object({
  roleId: Joi.string().uuid().required(),
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional()
});

const getUsersByStatusInCanada = Joi.object({
  status: Joi.string().valid('citizen', 'permanent_resident', 'work_permit', 'student_visa', 'visitor', 'other').required(),
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional()
});

const getUsersByCountryOfOrigin = Joi.object({
  country: Joi.string().required(),
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional()
});

const getUsersByCurrentLocation = Joi.object({
  location: Joi.string().required(),
  page: Joi.number().integer().min(1).optional(),
  limit: Joi.number().integer().min(1).max(100).optional()
});

const userExists = Joi.object({
  userId: Joi.string().uuid().required()
});

module.exports = {
  // Original schemas
  userRegistrationSchema,
  userLoginSchema,
  userProfileUpdateSchema,
  passwordChangeSchema,
  passwordResetRequestSchema,
  passwordResetSchema,
  emailVerificationSchema,
  
  // Controller route schemas
  findOrCreateUser,
  updateProfile,
  getUserById,
  updateUser,
  deleteUser,
  getUserByEmail,
  searchUsers,
  getUsers,
  getUsersByRole,
  getUsersByStatusInCanada,
  getUsersByCountryOfOrigin,
  getUsersByCurrentLocation,
  userExists
};
````

## File: src/prompts/career.js
````javascript
// Static prompts - compiled at build time, zero runtime overhead
const POSITION_RECOMMENDATION_PROMPT = (resumeAnalysis, userProfile) => `
Analyze this resume and generate position recommendations with success probabilities for the Canadian job market.

Resume Analysis:
${JSON.stringify(resumeAnalysis, null, 2)}

User Career Profile:
${JSON.stringify(userProfile, null, 2)}

Generate 5-8 position recommendations in this exact JSON structure:
{
  "marketAnalysis": {
    "overallMarketHealth": "Strong/Moderate/Weak",
    "keyTrends": [],
    "newcomerOpportunities": [],
    "regionalConsiderations": []
  },
  "positions": [
    {
      "title": "",
      "industry": "",
      "level": "Entry/Junior/Mid/Senior/Executive",
      "successProbability": 0.85,
      "matchScore": 0.92,
      "salaryRange": {
        "min": 50000,
        "max": 70000,
        "currency": "CAD"
      },
      "requiredSkills": [],
      "preferredSkills": [],
      "skillsMatch": {
        "matching": [],
        "missing": [],
        "transferable": []
      },
      "canadianRelevance": {
        "workExperienceValue": "High/Medium/Low",
        "educationRecognition": "Fully/Partially/Not Recognized",
        "certificationNeeds": [],
        "languageRequirements": "English/French/Bilingual"
      },
      "careerGrowth": {
        "nextLevelPositions": [],
        "typicalProgression": "",
        "timeToAdvancement": ""
      },
      "applicationStrategy": {
        "keyFocusAreas": [],
        "resumeOptimizations": [],
        "networkingTips": [],
        "interviewPreparation": []
      },
      "newcomerConsiderations": {
        "culturalAdaptation": [],
        "professionalNetworking": [],
        "credentialRecognition": []
      }
    }
  ],
  "overallRecommendations": {
    "topPriorities": [],
    "skillDevelopmentFocus": [],
    "networkingStrategy": [],
    "timelineRecommendations": ""
  }
}

Guidelines:
- Success probability: 0.0-1.0 based on skill match, experience, and market demand
- Match score: How well the candidate fits the role requirements
- Focus on Canadian job market specifics and newcomer-friendly opportunities
- Consider both immediate opportunities and career growth potential
- Include practical application strategies for each position
- Sort positions by success probability (highest first)

Return only valid JSON.`;

const ENHANCED_PROFILE_PROMPT = (resumeAnalysis, targetPosition, userPreferences) => `
Generate an enhanced career profile tailored for this specific position in the Canadian job market.

Resume Analysis:
${JSON.stringify(resumeAnalysis, null, 2)}

Target Position:
${JSON.stringify(targetPosition, null, 2)}

User Preferences:
${JSON.stringify(userPreferences, null, 2)}

Generate enhanced profile in this exact JSON structure:
{
  "enhancedProfile": {
    "optimizedSummary": "",
    "keyStrengths": [],
    "skillsPresentation": {
      "technical": {
        "core": [],
        "supporting": [],
        "emerging": []
      },
      "soft": {
        "leadership": [],
        "communication": [],
        "problemSolving": []
      },
      "adaptability": []
    },
    "experienceRepositioning": [
      {
        "originalRole": "",
        "enhancedPresentation": "",
        "keyAchievements": [],
        "quantifiedImpacts": [],
        "canadianContextualization": ""
      }
    ],
    "educationHighlights": {
      "relevantCourses": [],
      "canadianEquivalency": "",
      "additionalValue": []
    }
  },
  "applicationStrategy": {
    "coverLetterTemplate": "",
    "resumeOptimizations": {
      "structuralChanges": [],
      "contentEnhancements": [],
      "keywordOptimization": []
    },
    "interviewPreparation": {
      "expectedQuestions": [],
      "strengthBasedAnswers": [],
      "canadianWorkplaceTips": []
    },
    "portfolioRecommendations": []
  },
  "skillDevelopment": {
    "immediateActions": [
      {
        "skill": "",
        "priority": "High/Medium/Low",
        "learningPath": "",
        "timeEstimate": "",
        "resources": []
      }
    ],
    "mediumTermGoals": [],
    "certificationRoadmap": []
  },
  "networkingStrategy": {
    "targetProfessionals": [],
    "industryEvents": [],
    "onlinePlatforms": [],
    "informationalInterviews": []
  },
  "newcomerSupport": {
    "culturalAdaptation": [],
    "professionalEtiquette": [],
    "canadianWorkplaceNorms": [],
    "settlingInCanada": []
  },
  "careerProjection": {
    "shortTerm": {
      "timeline": "3-6 months",
      "milestones": [],
      "successMetrics": []
    },
    "mediumTerm": {
      "timeline": "1-2 years",
      "careerProgression": [],
      "skillAdvancement": []
    },
    "longTerm": {
      "timeline": "3-5 years",
      "leadershipPotential": [],
      "industryExpertise": []
    }
  }
}

Guidelines:
- Focus on Canadian job market requirements and cultural fit
- Provide specific, actionable recommendations
- Consider newcomer challenges and opportunities
- Include quantifiable goals and timelines
- Emphasize transferable skills and international experience value

Return only valid JSON.`;

const SKILL_GAP_ANALYSIS_PROMPT = (resumeAnalysis, targetPosition) => `
Perform detailed skill gap analysis comparing current capabilities with target position requirements.

Current Resume Analysis:
${JSON.stringify(resumeAnalysis, null, 2)}

Target Position:
${JSON.stringify(targetPosition, null, 2)}

Generate skill gap analysis in this exact JSON structure:
{
  "skillGapAnalysis": {
    "overallGapScore": 0.25,
    "readinessLevel": "Ready/Nearly Ready/Needs Development/Significant Gap",
    "strengths": [
      {
        "skill": "",
        "proficiencyLevel": "Expert/Advanced/Intermediate/Basic",
        "marketValue": "High/Medium/Low",
        "evidence": []
      }
    ],
    "gaps": [
      {
        "skill": "",
        "currentLevel": "None/Basic/Intermediate",
        "requiredLevel": "Basic/Intermediate/Advanced/Expert",
        "priority": "Critical/High/Medium/Low",
        "impact": "",
        "learningPath": {
          "timeEstimate": "",
          "difficulty": "Easy/Moderate/Challenging",
          "resources": [],
          "prerequisites": []
        }
      }
    ],
    "transferableSkills": [
      {
        "currentSkill": "",
        "applicableAs": "",
        "adaptationNeeded": "",
        "strengthenedBy": []
      }
    ]
  },
  "developmentRoadmap": {
    "phase1": {
      "duration": "1-3 months",
      "focus": "Critical Skills",
      "skills": [],
      "milestones": []
    },
    "phase2": {
      "duration": "3-6 months",
      "focus": "Enhancement",
      "skills": [],
      "milestones": []
    },
    "phase3": {
      "duration": "6+ months",
      "focus": "Mastery & Specialization",
      "skills": [],
      "milestones": []
    }
  },
  "learningRecommendations": {
    "formalEducation": [],
    "onlineCourses": [],
    "certifications": [],
    "practicalExperience": [],
    "mentorship": []
  },
  "competitiveAdvantage": {
    "uniqueStrengths": [],
    "differentiators": [],
    "marketPositioning": ""
  }
}

Guidelines:
- Gap score: 0.0 (perfect fit) to 1.0 (major gaps)
- Focus on Canadian market standards and expectations
- Include both technical and soft skill gaps
- Provide realistic timelines and learning paths
- Consider newcomer context and international experience

Return only valid JSON.`;

const RESUME_GENERATION_PROMPT = (userProfile, targetPosition, existingAnalysis) => {
  const existingData = existingAnalysis ? `
Existing Resume Analysis for Reference:
${JSON.stringify(existingAnalysis.structuredData || existingAnalysis, null, 2)}
` : '';

  return `
Generate a professional resume optimized for the Canadian job market and tailored specifically for this position:

Target Position: ${targetPosition.title}
Industry: ${targetPosition.industry}
Level: ${targetPosition.level}
Required Skills: ${targetPosition.requiredSkills.join(', ')}
Salary Range: ${targetPosition.salaryRange.min} - ${targetPosition.salaryRange.max} ${targetPosition.salaryRange.currency}

User Profile Information:
${JSON.stringify(userProfile, null, 2)}

${existingData}

Generate a complete resume in this exact JSON structure that matches our system format:
{
  "personalInfo": {
    "name": "Professional Full Name",
    "email": "professional.email@example.com",
    "phone": "+1 (xxx) xxx-xxxx",
    "location": "City, Province, Canada",
    "linkedin": "linkedin.com/in/profile",
    "website": "Optional professional website",
    "confidence": 1.0
  },
  "professionalSummary": {
    "summary": "3-4 line compelling summary tailored for ${targetPosition.title} in ${targetPosition.industry}, highlighting Canadian market relevance",
    "careerLevel": "${targetPosition.level}",
    "yearsOfExperience": [calculated years],
    "confidence": 1.0
  },
  "workExperience": [
    {
      "title": "Job Title optimized for Canadian market",
      "company": "Company Name",
      "startDate": "YYYY-MM",
      "endDate": "YYYY-MM or Present",
      "location": "City, Province/Country",
      "responsibilities": [
        "Action-oriented responsibility using Canadian business terminology",
        "Quantified achievement with metrics",
        "Responsibility highlighting transferable skills for ${targetPosition.title}"
      ],
      "achievements": [
        "Specific achievement with numbers/percentages",
        "Achievement demonstrating ${targetPosition.requiredSkills[0]} skills",
        "Result that shows impact and Canadian workplace value"
      ],
      "canadianRelevance": "High",
      "confidence": 1.0
    }
  ],
  "education": [
    {
      "degree": "Degree Name",
      "institution": "Institution Name",
      "year": "YYYY",
      "location": "City, Province/Country",
      "gpa": "Optional if strong",
      "relevantCoursework": ["Course relevant to ${targetPosition.title}"],
      "canadianEquivalency": "Canadian education equivalent assessment",
      "confidence": 1.0
    }
  ],
  "skills": {
    "technical": [${targetPosition.requiredSkills.map(skill => `"${skill}"`).join(', ')}],
    "soft": ["Communication", "Leadership", "Problem-solving", "Team collaboration"],
    "languages": [
      {
        "language": "English",
        "proficiency": "Native/Fluent"
      },
      {
        "language": "French",
        "proficiency": "Basic/Intermediate (if relevant for Canadian bilingual advantage)"
      }
    ],
    "canadianWorkplaceRelevance": "High",
    "confidence": 1.0
  },
  "certifications": [
    {
      "name": "Relevant certification for ${targetPosition.title}",
      "issuer": "Recognized Canadian/International body",
      "year": "YYYY",
      "expiryDate": "YYYY-MM (if applicable)",
      "canadianRecognition": "Recognized",
      "confidence": 1.0
    }
  ],
  "projects": [
    {
      "name": "Project Name relevant to ${targetPosition.title}",
      "description": "Brief description highlighting skills used in ${targetPosition.industry}",
      "technologies": ["Tech stack relevant to position"],
      "role": "Your role in the project",
      "year": "YYYY",
      "confidence": 1.0
    }
  ],
  "canadianMarketAnalysis": {
    "overallRelevance": "High",
    "strengthsForCanadianMarket": [
      "Key strength for Canadian ${targetPosition.industry} market",
      "Advantage in Canadian workplace culture",
      "Skill particularly valued in Canada"
    ],
    "potentialChallenges": [
      "Minor challenge that can be addressed",
      "Area for improvement in Canadian context"
    ],
    "recommendedImprovements": [
      "Specific action to enhance Canadian market appeal",
      "Certification or training to pursue in Canada"
    ],
    "targetIndustries": ["${targetPosition.industry}", "Related industry"],
    "salaryRangeEstimate": "${targetPosition.salaryRange.min} - ${targetPosition.salaryRange.max} ${targetPosition.salaryRange.currency}",
    "confidence": 1.0
  },
  "metadata": {
    "generatedFor": "${targetPosition.title}",
    "targetIndustry": "${targetPosition.industry}",
    "optimizationLevel": "${targetPosition.level}",
    "canadianMarketFocus": true,
    "generatedAt": "${new Date().toISOString()}",
    "aiModel": "gemini-1.5-pro"
  }
}

IMPORTANT REQUIREMENTS:
1. Make it specific to ${targetPosition.title} in ${targetPosition.industry}
2. Optimize for Canadian job market expectations
3. Include quantified achievements and metrics
4. Use Canadian business terminology and spellings
5. Highlight skills that match the required skills: ${targetPosition.requiredSkills.join(', ')}
6. Ensure all data is realistic and professional
7. Include bilingual capabilities if relevant for the Canadian market
8. Focus on newcomer-friendly aspects if applicable
9. Make the summary compelling and tailored specifically for this position
10. Ensure all sections are complete and professionally written

Generate only the JSON, no additional text.`;
};

module.exports = {
  POSITION_RECOMMENDATION_PROMPT,
  ENHANCED_PROFILE_PROMPT,
  SKILL_GAP_ANALYSIS_PROMPT,
  RESUME_GENERATION_PROMPT
};
````

## File: src/prompts/index.js
````javascript
// Central export - tree-shakeable imports
module.exports = {
  ...require('./resume'),
  ...require('./career'),
  ...require('./jobs'),
  ...require('./resumeGenerator')
};
````

## File: src/prompts/jobs.js
````javascript
// Static prompts - compiled at build time, zero runtime overhead
const RESUME_ANALYSIS_PROMPT = (extractedText, userProfile) => `
Analyze this resume and extract structured data in JSON format. Provide confidence scores for each field (0-1).

Resume Text:
${extractedText}

User Context:
${JSON.stringify(userProfile)}

Extract the following information in this exact JSON structure:
{
  "personalInfo": {
    "name": "",
    "email": "",
    "phone": "",
    "location": "",
    "confidence": 0.0
  },
  "education": [
    {
      "degree": "",
      "institution": "",
      "year": "",
      "location": "",
      "confidence": 0.0
    }
  ],
  "workExperience": [
    {
      "title": "",
      "company": "",
      "startDate": "",
      "endDate": "",
      "location": "",
      "responsibilities": [],
      "confidence": 0.0
    }
  ],
  "skills": {
    "technical": [],
    "soft": [],
    "languages": [],
    "confidence": 0.0
  },
  "certifications": [
    {
      "name": "",
      "issuer": "",
      "year": "",
      "confidence": 0.0
    }
  ],
  "summary": {
    "professionalSummary": "",
    "careerLevel": "",
    "industries": [],
    "confidence": 0.0
  }
}

Return only valid JSON. For missing information, use empty strings or arrays.`;

const CAREER_PROFILE_PROMPT = (resumeData, userObjectives) => `
Create a comprehensive career profile for a newcomer to Canada based on resume data and career objectives.

Resume Data:
${JSON.stringify(resumeData)}

User Objectives:
${JSON.stringify(userObjectives)}

Generate a detailed career profile in this JSON structure:
{
  "professionalSummary": "3-4 paragraph professional summary highlighting experience, strengths, and Canadian market relevance",
  "skillsCategories": {
    "technical": {
      "skills": [],
      "marketRelevance": "High/Medium/Low",
      "improvement_suggestions": []
    },
    "soft": {
      "skills": [],
      "marketRelevance": "High/Medium/Low", 
      "improvement_suggestions": []
    },
    "industry": {
      "skills": [],
      "marketRelevance": "High/Medium/Low",
      "improvement_suggestions": []
    }
  },
  "marketAlignmentScore": 85,
  "skillGaps": [
    {
      "skill": "",
      "priority": "High/Medium/Low",
      "learningPath": "",
      "estimatedTime": ""
    }
  ],
  "improvementRoadmap": {
    "immediate": ["0-3 months actions"],
    "shortTerm": ["3-6 months goals"],
    "mediumTerm": ["6-12 months objectives"],
    "longTerm": ["1-2 years vision"]
  },
  "canadianMarketInsights": {
    "industryDemand": "",
    "salaryExpectations": "",
    "certificationRecommendations": [],
    "networkingOpportunities": []
  }
}

Focus on Canadian job market alignment, newcomer advantages, and specific improvement paths.`;

const MENTOR_COMPATIBILITY_PROMPT = (menteeProfile, mentorProfile) => `
Analyze mentor-mentee compatibility for Canadian career development context.

Mentee Profile:
${JSON.stringify(menteeProfile)}

Mentor Profile:
${JSON.stringify(mentorProfile)}

Calculate compatibility and return this JSON structure:
{
  "compatibilityScore": 85,
  "compatibilityBreakdown": {
    "industryAlignment": {
      "score": 90,
      "reasoning": "Direct experience in target industry"
    },
    "experienceLevel": {
      "score": 80,
      "reasoning": "Appropriate mentor experience for mentee level"
    },
    "culturalCompatibility": {
      "score": 85,
      "reasoning": "Shared cultural background and language"
    },
    "careerGoals": {
      "score": 88,
      "reasoning": "Aligned career objectives and growth path"
    },
    "communicationStyle": {
      "score": 75,
      "reasoning": "Compatible communication preferences"
    }
  },
  "matchReasoning": {
    "strengths": ["Why this is a good match"],
    "potential_challenges": ["What to be aware of"],
    "recommended_approach": "How to structure the mentorship",
    "expected_outcomes": ["What mentee can expect to gain"]
  },
  "actionPlan": {
    "first_meeting": "Suggested agenda for initial meeting",
    "ongoing_structure": "Recommended meeting frequency and format",
    "success_metrics": ["How to measure progress"]
  }
}

Consider Canadian workplace culture, newcomer needs, and professional development best practices.`;

const COACHING_QUERY_PROMPT = (query, userProfile, sessionHistory) => `
You are an AI career coach specializing in helping newcomers to Canada navigate their career development.

User Profile:
${JSON.stringify(userProfile)}

Session History (last 5 interactions):
${JSON.stringify(sessionHistory.slice(-5))}

User Query: "${query}"

Provide coaching response in this JSON structure:
{
  "response": "Detailed coaching response addressing the user's query",
  "actionItems": ["Specific actionable steps the user should take"],
  "resources": [
    {
      "title": "Resource name",
      "type": "website/course/certification/book",
      "url": "URL if available",
      "description": "How this resource helps"
    }
  ],
  "followUpQuestions": ["Questions to ask in next session"],
  "sessionSummary": "Key points covered in this interaction",
  "progressMetrics": {
    "area": "What area this helps improve",
    "measurable_outcome": "How user can measure progress"
  }
}

Coaching Guidelines:
- Focus on Canadian job market specifics
- Consider newcomer challenges (credential recognition, cultural adaptation)
- Provide practical, actionable advice
- Encourage confidence building
- Suggest networking and skill development opportunities
- Be supportive and understanding of immigrant experience`;

const JOB_COMPATIBILITY_PROMPT = (userProfile, jobDescription) => `
Analyze job compatibility for a newcomer to Canada.

User Profile:
${JSON.stringify(userProfile)}

Job Description:
${jobDescription}

Analyze compatibility and return this JSON structure:
{
  "matchScore": 85,
  "compatibility": {
    "skills": {
      "score": 90,
      "matched": ["Skills that match"],
      "missing": ["Skills that are missing"],
      "transferable": ["International skills that transfer"]
    },
    "experience": {
      "score": 80,
      "relevance": "How relevant is the experience",
      "gaps": ["Experience gaps to address"]
    },
    "education": {
      "score": 85,
      "alignment": "How education aligns with requirements",
      "additional_needed": ["Additional education/certifications needed"]
    },
    "cultural_fit": {
      "score": 75,
      "newcomer_advantages": ["Advantages as a newcomer"],
      "adaptation_areas": ["Areas requiring cultural adaptation"]
    }
  },
  "preparation": {
    "immediate": ["What to do before applying"],
    "short_term": ["Skills to develop in 1-3 months"],
    "application_strategy": "How to position yourself for this role"
  },
  "coverLetter": {
    "key_points": ["Main points to emphasize"],
    "newcomer_positioning": "How to address newcomer status positively",
    "template_suggestions": ["Specific phrases or approaches"]
  },
  "interview_prep": {
    "likely_questions": ["Questions they might ask"],
    "strength_examples": ["Examples to showcase strengths"],
    "cultural_considerations": ["Canadian interview norms to consider"]
  }
}

Focus on realistic assessment while being encouraging about newcomer potential.`;

const SKILL_GAP_ANALYSIS_PROMPT = (currentSkills, targetRole, marketData) => `
Perform comprehensive skill gap analysis for Canadian job market.

Current Skills:
${JSON.stringify(currentSkills)}

Target Role:
${targetRole}

Market Data:
${JSON.stringify(marketData)}

Return detailed analysis in this JSON structure:
{
  "analysis": {
    "current_strengths": ["Skills that are strong and marketable"],
    "skill_gaps": [
      {
        "skill": "Missing skill name",
        "importance": "Critical/Important/Nice-to-have",
        "market_demand": "High/Medium/Low",
        "learning_difficulty": "Easy/Medium/Hard",
        "time_to_acquire": "Estimated time",
        "priority_score": 95
      }
    ],
    "transferable_skills": ["International skills that apply in Canada"],
    "market_advantages": ["Unique advantages in Canadian market"]
  },
  "learning_path": {
    "phase_1": {
      "duration": "0-3 months",
      "focus": ["Most critical skills to learn first"],
      "resources": [
        {
          "type": "course/certification/practice",
          "name": "Resource name",
          "provider": "Where to get it",
          "cost": "Free/Paid/Estimate",
          "url": "URL if available"
        }
      ]
    },
    "phase_2": {
      "duration": "3-6 months", 
      "focus": ["Next priority skills"],
      "resources": []
    },
    "phase_3": {
      "duration": "6-12 months",
      "focus": ["Advanced skills for career growth"],
      "resources": []
    }
  },
  "canadian_certifications": [
    {
      "certification": "Name",
      "relevance": "How it helps",
      "provider": "Who offers it",
      "timeline": "How long to complete",
      "cost": "Estimated cost"
    }
  ],
  "progress_tracking": {
    "milestones": ["How to measure progress"],
    "portfolio_projects": ["Projects to demonstrate skills"],
    "networking_opportunities": ["Where to connect with industry professionals"]
  }
}

Focus on practical, achievable learning paths specific to the Canadian job market.`;

const CULTURAL_GUIDANCE_PROMPT = (userBackground, targetWorkplace) => `
Provide cultural integration guidance for Canadian workplace.

User Background:
${JSON.stringify(userBackground)}

Target Workplace/Industry:
${JSON.stringify(targetWorkplace)}

Generate guidance in this JSON structure:
{
  "workplace_culture": {
    "communication": {
      "key_differences": ["How Canadian communication differs"],
      "best_practices": ["What to do"],
      "common_mistakes": ["What to avoid"],
      "examples": ["Specific scenarios and responses"]
    },
    "hierarchy": {
      "structure": "How Canadian workplaces are structured",
      "interaction_norms": ["How to interact with managers/colleagues"],
      "feedback_culture": "How feedback works in Canada"
    },
    "meeting_culture": {
      "participation": "How to contribute effectively",
      "etiquette": ["Meeting norms and expectations"],
      "follow_up": "Post-meeting protocols"
    }
  },
  "networking": {
    "professional_associations": ["Relevant associations to join"],
    "networking_events": ["Types of events to attend"],
    "online_presence": ["How to build professional online presence"],
    "conversation_starters": ["What to talk about at networking events"]
  },
  "career_development": {
    "performance_reviews": "How they work in Canada",
    "promotion_pathways": "How to advance in Canadian companies",
    "professional_development": ["Expected self-improvement activities"]
  },
  "practical_tips": {
    "first_90_days": ["What to focus on in first 3 months"],
    "building_relationships": ["How to connect with colleagues"],
    "work_life_balance": ["Canadian expectations and norms"]
  },
  "potential_challenges": [
    {
      "challenge": "Common challenge newcomers face",
      "solution": "How to address it",
      "resources": ["Where to get help"]
    }
  ]
}

Be specific about Canadian workplace norms and practical integration strategies.`;

const CAREER_PROFILE_WITH_GEMINI_PROMPT = (data) => `
Analyze the following resume data and user profile to create an intelligent career profile suitable for the Canadian job market.

Resume Analysis:
${JSON.stringify(data.resumeAnalysis)}

User Profile:
${JSON.stringify(data.userProfile)}

Generate a comprehensive career profile in this JSON structure:
{
  "profile_summary": {
    "title": "Professional title based on background",
    "summary": "2-3 sentence professional summary",
    "unique_value_proposition": "What makes this person valuable",
    "years_experience": "Total years of relevant experience"
  },
  "skills_analysis": {
    "core_skills": [
      {
        "skill": "Skill name",
        "level": "Beginner/Intermediate/Advanced/Expert",
        "years_experience": 3,
        "market_demand": "High/Medium/Low",
        "canadian_relevance": "How relevant in Canadian market"
      }
    ],
    "transferable_skills": ["Skills that transfer well to Canada"],
    "skill_gaps": ["Key skills missing for Canadian market"],
    "emerging_skills": ["New skills to consider learning"]
  },
  "canadian_market_analysis": {
    "overall_marketability": {
      "score": 85,
      "reasoning": "Why this score was given",
      "improvement_areas": ["Areas to focus on for better marketability"]
    },
    "industry_fit": [
      {
        "industry": "Technology",
        "fit_score": 90,
        "opportunities": ["Specific opportunities in this industry"],
        "entry_barriers": ["Challenges to overcome"],
        "growth_potential": "Career growth prospects"
      }
    ],
    "geographic_recommendations": [
      {
        "location": "Toronto, ON",
        "reasoning": "Why this location is recommended",
        "industry_presence": "Strong tech industry",
        "newcomer_support": "Available support systems",
        "cost_of_living": "Relative cost considerations"
      }
    ],
    "salary_expectations": {
      "entry_level": "$50,000 - $65,000",
      "mid_level": "$65,000 - $85,000",
      "senior_level": "$85,000 - $120,000",
      "factors_affecting_salary": ["Location", "Company size", "Industry"]
    }
  },
  "career_pathways": [
    {
      "pathway": "Software Developer",
      "match_score": 88,
      "timeline": "3-6 months preparation",
      "required_skills": ["Skills needed for this path"],
      "certification_recommendations": ["Relevant certifications"],
      "typical_progression": "Career advancement path",
      "market_demand": "High",
      "advantages": ["Why this is a good fit"],
      "challenges": ["Potential obstacles"]
    }
  ],
  "next_steps": {
    "immediate": ["Actions to take in next 30 days"],
    "short_term": ["Goals for next 3-6 months"],
    "long_term": ["Career goals for next 1-2 years"]
  },
  "newcomer_specific": {
    "strengths": ["Advantages as a newcomer"],
    "cultural_considerations": ["Things to be aware of"],
    "networking_strategies": ["How to build professional network"],
    "credential_recognition": "Status of credentials in Canada"
  }
}

Focus on providing actionable, Canada-specific guidance that acknowledges both opportunities and challenges for newcomers.`;

const POSITION_RECOMMENDATIONS_WITH_GEMINI_PROMPT = (resumeAnalysis) => `
Based on the following resume analysis, generate specific position recommendations for the Canadian job market.

Resume Analysis:
${JSON.stringify(resumeAnalysis)}

Generate position recommendations in this JSON structure:
{
  "recommendations": [
    {
      "position_title": "Software Developer",
      "match_score": 88,
      "success_probability": 85,
      "reasoning": "Why this position is a good match",
      "required_skills": ["Skills needed for this position"],
      "matching_skills": ["Current skills that match"],
      "skill_gaps": ["Skills that need development"],
      "experience_relevance": {
        "score": 80,
        "relevant_experience": ["Which experiences are applicable"],
        "transferable_experience": ["How international experience applies"]
      },
      "market_analysis": {
        "demand": "High/Medium/Low",
        "growth_trend": "Growing/Stable/Declining",
        "average_salary": "$65,000 - $85,000",
        "top_hiring_companies": ["Company names"],
        "job_locations": ["Cities with most opportunities"]
      },
      "preparation_timeline": "3-6 months",
      "immediate_actions": ["What to do first"],
      "certification_recommendations": ["Relevant certifications"],
      "canadian_specific_requirements": ["Canada-specific needs"],
      "newcomer_advantages": ["How being a newcomer helps"],
      "potential_challenges": ["Obstacles to overcome"]
    }
  ],
  "overall_assessment": {
    "profile_strength": "Strong/Moderate/Developing",
    "market_readiness": "Ready/Needs preparation/Significant development needed",
    "key_recommendations": ["Top 3 recommendations"],
    "timeline_to_employment": "Estimated time to find suitable position"
  },
  "industry_insights": {
    "best_fit_industries": ["Industries that match well"],
    "emerging_opportunities": ["New areas to consider"],
    "market_trends": ["Current trends affecting job search"]
  }
}

Provide realistic but encouraging recommendations that consider the unique position of newcomers to Canada.`;

const ENHANCED_PROFILE_WITH_GEMINI_PROMPT = (targetPosition, resumeAnalysis) => `
Create an enhanced career profile tailored specifically for the target position, based on the resume analysis.

Target Position:
${JSON.stringify(targetPosition)}

Resume Analysis:
${JSON.stringify(resumeAnalysis)}

Generate an enhanced profile in this JSON structure:
{
  "optimized_profile": {
    "professional_title": "Title optimized for target position",
    "elevator_pitch": "30-second introduction tailored to this role",
    "value_proposition": "Unique value for this specific position",
    "key_achievements": ["Top achievements relevant to this role"]
  },
  "skills_positioning": {
    "primary_skills": [
      {
        "skill": "Skill name",
        "relevance_to_role": "How it applies to target position",
        "evidence": "Proof/examples of this skill",
        "positioning_statement": "How to present this skill"
      }
    ],
    "skill_development_plan": [
      {
        "skill": "Skill to develop",
        "importance": "Critical/Important/Beneficial",
        "learning_path": "How to acquire this skill",
        "timeline": "Time needed",
        "resources": ["Where to learn"]
      }
    ]
  },
  "experience_repositioning": {
    "relevant_experience": [
      {
        "original_role": "Previous job title",
        "repositioned_as": "How to present this role",
        "key_transferable_elements": ["What transfers to target role"],
        "success_metrics": ["Quantifiable achievements"],
        "canadian_context": "How to frame for Canadian employers"
      }
    ],
    "project_highlights": [
      {
        "project": "Project name",
        "relevance": "Why it matters for target role",
        "technologies_used": ["Relevant technologies"],
        "impact": "Measurable impact/results",
        "presentation_tip": "How to discuss in interviews"
      }
    ]
  },
  "application_strategy": {
    "resume_optimization": {
      "key_changes": ["Main changes to make to resume"],
      "keywords_to_include": ["Important keywords for ATS"],
      "sections_to_emphasize": ["Which resume sections to highlight"],
      "formatting_tips": ["How to structure for this role"]
    },
    "cover_letter_strategy": {
      "opening_approach": "How to start the cover letter",
      "key_points_to_address": ["Main points to cover"],
      "company_research_areas": ["What to research about companies"],
      "closing_strategy": "How to end strongly"
    },
    "networking_approach": {
      "target_professionals": ["Types of people to connect with"],
      "conversation_starters": ["How to initiate conversations"],
      "value_you_bring": ["What you offer to your network"],
      "follow_up_strategies": ["How to maintain connections"]
    }
  },
  "interview_preparation": {
    "common_questions": [
      {
        "question": "Likely interview question",
        "strategy": "How to approach this question",
        "key_points": ["Main points to cover"],
        "example_answer_structure": "Framework for answering"
      }
    ],
    "behavioral_examples": [
      {
        "situation": "STAR method situation",
        "task": "Task you had",
        "action": "Action you took",
        "result": "Result achieved",
        "relevance": "Why this example works for target role"
      }
    ],
    "technical_preparation": {
      "skills_to_demonstrate": ["Technical skills to showcase"],
      "portfolio_items": ["What to include in portfolio"],
      "coding_challenges": ["Types of challenges to practice"],
      "system_design_topics": ["Areas to study"]
    },
    "cultural_fit_preparation": {
      "company_culture_research": ["What to research"],
      "canadian_workplace_norms": ["Cultural aspects to understand"],
      "questions_to_ask": ["Good questions to ask interviewer"]
    }
  },
  "90_day_action_plan": {
    "week_1_2": ["Immediate actions"],
    "month_1": ["Goals for first month"],
    "month_2": ["Second month objectives"],
    "month_3": ["Third month targets"],
    "success_metrics": ["How to measure progress"]
  }
}

Create a comprehensive, actionable plan that positions the candidate optimally for the specific target role.`;

module.exports = {
  RESUME_ANALYSIS_PROMPT,
  CAREER_PROFILE_PROMPT,
  MENTOR_COMPATIBILITY_PROMPT,
  COACHING_QUERY_PROMPT,
  JOB_COMPATIBILITY_PROMPT,
  SKILL_GAP_ANALYSIS_PROMPT,
  CULTURAL_GUIDANCE_PROMPT,
  CAREER_PROFILE_WITH_GEMINI_PROMPT,
  POSITION_RECOMMENDATIONS_WITH_GEMINI_PROMPT,
  ENHANCED_PROFILE_WITH_GEMINI_PROMPT
};
````

## File: src/prompts/resume.js
````javascript
// Static prompts - compiled at build time, zero runtime overhead
const ANALYSIS_PROMPT = `Analyze this resume and extract structured data with Canadian job market focus. Provide confidence scores (0-1).

Extract in this exact JSON structure:
{
  "personalInfo": {
    "name": "",
    "email": "",
    "phone": "",
    "location": "",
    "linkedin": "",
    "website": "",
    "confidence": 0.0
  },
  "professionalSummary": {
    "summary": "",
    "careerLevel": "Entry/Mid/Senior/Executive",
    "yearsOfExperience": 0,
    "confidence": 0.0
  },
  "education": [
    {
      "degree": "",
      "institution": "",
      "year": "",
      "location": "",
      "gpa": "",
      "relevantCoursework": [],
      "canadianEquivalency": "",
      "confidence": 0.0
    }
  ],
  "workExperience": [
    {
      "title": "",
      "company": "",
      "startDate": "",
      "endDate": "",
      "location": "",
      "responsibilities": [],
      "achievements": [],
      "canadianRelevance": "High/Medium/Low",
      "confidence": 0.0
    }
  ],
  "skills": {
    "technical": [],
    "soft": [],
    "languages": [
      {
        "language": "",
        "proficiency": "Native/Fluent/Intermediate/Basic"
      }
    ],
    "canadianWorkplaceRelevance": "High/Medium/Low",
    "confidence": 0.0
  },
  "certifications": [
    {
      "name": "",
      "issuer": "",
      "year": "",
      "expiryDate": "",
      "canadianRecognition": "Recognized/Partially/Not Recognized",
      "confidence": 0.0
    }
  ],
  "projects": [
    {
      "name": "",
      "description": "",
      "technologies": [],
      "role": "",
      "year": "",
      "confidence": 0.0
    }
  ],
  "canadianMarketAnalysis": {
    "overallRelevance": "High/Medium/Low",
    "strengthsForCanadianMarket": [],
    "potentialChallenges": [],
    "recommendedImprovements": [],
    "targetIndustries": [],
    "salaryRangeEstimate": "",
    "confidence": 0.0
  },
  "confidenceScores": {
    "overall": 0.0,
    "dataExtraction": 0.0,
    "marketAnalysis": 0.0
  }
}

Canadian Context:
- Assess education equivalency to Canadian standards
- Evaluate work experience relevance to Canadian job market
- Consider language proficiency requirements
- Analyze certification recognition in Canada
- Provide Canadian-specific career guidance

Return only valid JSON. Use empty strings/arrays for missing data.`;

const TEXT_ANALYSIS_PROMPT = (extractedText, originalFileName) => `
${ANALYSIS_PROMPT}

Resume Text:
${extractedText}

File: ${originalFileName}`;

const BASIC_ANALYSIS_STRUCTURE = {
  personalInfo: {
    name: "Unable to extract",
    email: "Unable to extract",
    phone: "Unable to extract",
    location: "Unable to extract",
    linkedin: "",
    website: "",
    confidence: 0.0
  },
  professionalSummary: {
    summary: "Resume analysis temporarily unavailable due to API overload. Please try again in a few minutes.",
    careerLevel: "Unknown",
    yearsOfExperience: 0,
    confidence: 0.0
  },
  education: [],
  workExperience: [],
  skills: {
    technical: [],
    soft: [],
    languages: [],
    confidence: 0.0
  },
  certifications: [],
  projects: [],
  canadianMarketAnalysis: {
    strengthsForCanadianMarket: ["Analysis temporarily unavailable"],
    recommendedImprovements: ["Please try again later"],
    marketAlignmentScore: 0.0,
    confidence: 0.0
  },
  confidenceScores: {
    overall: 0.0,
    personalInfo: 0.0,
    workExperience: 0.0,
    education: 0.0,
    skills: 0.0
  }
};

// Dynamic prompts - use functions for variable content
const createBasicAnalysis = (originalFileName) => ({
  ...BASIC_ANALYSIS_STRUCTURE,
  metadata: {
    fileName: originalFileName,
    processingMethod: "fallback_basic",
    processingTime: new Date().toISOString(),
    error: "Gemini API overload - basic analysis provided"
  }
});

module.exports = {
  ANALYSIS_PROMPT,
  TEXT_ANALYSIS_PROMPT,
  BASIC_ANALYSIS_STRUCTURE,
  createBasicAnalysis
};
````

## File: src/prompts/resumeGenerator.js
````javascript
// Static prompts - compiled at build time, zero runtime overhead
const RESUME_GENERATION_PROMPT = (resumeAnalysis, jobTargeting) => `
Generate a professional Canadian resume optimized for ATS systems and tailored for this specific job opportunity.

Original Resume Analysis:
${JSON.stringify(resumeAnalysis, null, 2)}

Job Targeting Information:
${JSON.stringify(jobTargeting, null, 2)}

Generate a complete Canadian resume in this exact JSON structure:
{
  "personalInfo": {
    "name": "Professional Full Name",
    "email": "professional.email@example.com",
    "phone": "+1 (xxx) xxx-xxxx",
    "location": "City, Province, Canada",
    "linkedin": "linkedin.com/in/profile",
    "website": "Optional professional website",
    "confidence": 1.0
  },
  "professionalSummary": {
    "summary": "3-4 line compelling summary tailored for ${jobTargeting.jobTitle} at ${jobTargeting.companyName}, highlighting Canadian market relevance and key achievements",
    "careerLevel": "Entry/Mid/Senior/Executive",
    "yearsOfExperience": [calculated from work experience],
    "confidence": 1.0
  },
  "workExperience": [
    {
      "title": "Job Title optimized for Canadian market",
      "company": "Company Name",
      "startDate": "YYYY-MM",
      "endDate": "YYYY-MM or Present",
      "location": "City, Province/Country",
      "responsibilities": [
        "Action-oriented responsibility using Canadian business terminology",
        "Quantified achievement with metrics",
        "Responsibility highlighting transferable skills for ${jobTargeting.jobTitle}"
      ],
      "achievements": [
        "Specific achievement with numbers/percentages",
        "Achievement demonstrating relevant skills for ${jobTargeting.jobTitle}",
        "Result that shows impact and Canadian workplace value"
      ],
      "canadianRelevance": "High/Medium/Low",
      "confidence": 1.0
    }
  ],
  "education": [
    {
      "degree": "Degree Name",
      "institution": "Institution Name",
      "year": "YYYY",
      "location": "City, Province/Country",
      "gpa": "Optional if strong",
      "relevantCoursework": ["Course relevant to ${jobTargeting.jobTitle}"],
      "canadianEquivalency": "Canadian education equivalent assessment",
      "confidence": 1.0
    }
  ],
  "skills": {
    "technical": ["Skills relevant to ${jobTargeting.jobTitle}"],
    "soft": ["Communication", "Leadership", "Problem-solving", "Team collaboration"],
    "languages": [
      {
        "language": "English",
        "proficiency": "Native/Fluent"
      },
      {
        "language": "French",
        "proficiency": "Basic/Intermediate (if relevant for Canadian bilingual advantage)"
      }
    ],
    "canadianWorkplaceRelevance": "High",
    "confidence": 1.0
  },
  "certifications": [
    {
      "name": "Relevant certification for ${jobTargeting.jobTitle}",
      "issuer": "Recognized Canadian/International body",
      "year": "YYYY",
      "expiryDate": "YYYY-MM (if applicable)",
      "canadianRecognition": "Recognized",
      "confidence": 1.0
    }
  ],
  "projects": [
    {
      "name": "Project Name relevant to ${jobTargeting.jobTitle}",
      "description": "Brief description highlighting skills used in ${jobTargeting.industry}",
      "technologies": ["Tech stack relevant to position"],
      "role": "Your role in the project",
      "year": "YYYY",
      "confidence": 1.0
    }
  ],
  "canadianMarketAnalysis": {
    "overallRelevance": "High",
    "strengthsForCanadianMarket": [
      "Key strength for Canadian ${jobTargeting.industry} market",
      "Advantage in Canadian workplace culture",
      "Skill particularly valued in Canada"
    ],
    "potentialChallenges": [
      "Minor challenge that can be addressed",
      "Area for improvement in Canadian context"
    ],
    "recommendedImprovements": [
      "Specific action to enhance Canadian market appeal",
      "Certification or training to pursue in Canada"
    ],
    "targetIndustries": ["${jobTargeting.industry}", "Related industry"],
    "salaryRangeEstimate": "Based on Canadian market standards",
    "confidence": 1.0
  },
  "metadata": {
    "generatedFor": "${jobTargeting.jobTitle}",
    "targetCompany": "${jobTargeting.companyName}",
    "targetIndustry": "${jobTargeting.industry}",
    "canadianMarketFocus": true,
    "atsOptimized": true,
    "generatedAt": "${new Date().toISOString()}",
    "aiModel": "gemini-1.5-pro"
  }
}

IMPORTANT REQUIREMENTS:
1. Make it specific to ${jobTargeting.jobTitle} at ${jobTargeting.companyName}
2. Optimize for Canadian job market expectations and ATS systems
3. Include quantified achievements and metrics
4. Use Canadian business terminology and spellings
5. Highlight skills that match the job description
6. Ensure all data is realistic and professional
7. Include bilingual capabilities if relevant for the Canadian market
8. Focus on newcomer-friendly aspects if applicable
9. Make the summary compelling and tailored specifically for this position
10. Ensure all sections are complete and professionally written

Generate only the JSON, no additional text.`;

const JOB_TARGETING_ANALYSIS_PROMPT = (jobDescription, resumeAnalysis) => `
Analyze this job description and provide detailed targeting recommendations for resume optimization.

Job Description:
${jobDescription}

Resume Analysis:
${JSON.stringify(resumeAnalysis, null, 2)}

Generate job targeting analysis in this exact JSON structure:
{
  "jobAnalysis": {
    "keyRequirements": [
      {
        "requirement": "",
        "importance": "Critical/High/Medium/Low",
        "foundInResume": true/false,
        "matchStrength": 0.0-1.0,
        "optimizationNeeded": "Add/Enhance/Reposition/Remove"
      }
    ],
    "preferredQualifications": [
      {
        "qualification": "",
        "foundInResume": true/false,
        "matchStrength": 0.0-1.0,
        "optimizationNeeded": "Add/Enhance/Reposition/Remove"
      }
    ],
    "companyCulture": {
      "values": [],
      "workStyle": "",
      "growthOpportunities": [],
      "culturalFit": "High/Medium/Low"
    },
    "industryContext": {
      "marketTrends": [],
      "skillDemand": "High/Medium/Low",
      "salaryBenchmarks": "",
      "competitionLevel": "High/Medium/Low"
    }
  },
  "resumeOptimization": {
    "keywordOptimization": [
      {
        "keyword": "",
        "currentUsage": "Present/Missing/Weak",
        "recommendedAction": "Add/Enhance/Reposition",
        "placement": "Summary/Experience/Skills"
      }
    ],
    "contentEnhancements": [
      {
        "section": "",
        "currentContent": "",
        "recommendedEnhancement": "",
        "priority": "High/Medium/Low"
      }
    ],
    "structuralChanges": [
      {
        "change": "",
        "rationale": "",
        "impact": "High/Medium/Low"
      }
    ]
  },
  "atsOptimization": {
    "formattingRecommendations": [
      {
        "element": "",
        "currentState": "",
        "recommendedState": "",
        "reason": ""
      }
    ],
    "keywordDensity": {
      "criticalKeywords": [],
      "currentDensity": 0.0,
      "targetDensity": 0.0,
      "recommendations": []
    },
    "readabilityScore": {
      "current": 0.0,
      "target": 0.0,
      "improvements": []
    }
  },
  "competitiveAdvantage": {
    "uniqueStrengths": [
      {
        "strength": "",
        "relevance": "High/Medium/Low",
        "differentiation": ""
      }
    ],
    "weaknesses": [
      {
        "weakness": "",
        "mitigation": "",
        "priority": "High/Medium/Low"
      }
    ],
    "opportunities": [
      {
        "opportunity": "",
        "action": "",
        "timeline": ""
      }
    ]
  },
  "applicationStrategy": {
    "resumeFocus": "",
    "coverLetterHighlights": [],
    "interviewPreparation": [],
    "followUpStrategy": ""
  }
}

Guidelines:
- Focus on Canadian job market standards
- Consider ATS optimization requirements
- Provide specific, actionable recommendations
- Include both technical and soft skill analysis
- Consider newcomer context and international experience

Return only valid JSON.`;

const ATS_OPTIMIZATION_PROMPT = (resumeData, jobDescription) => `
Optimize this resume for Applicant Tracking System (ATS) compatibility and Canadian job market standards.

Resume Data:
${JSON.stringify(resumeData, null, 2)}

Job Description:
${jobDescription}

Generate ATS optimization recommendations in this exact JSON structure:
{
  "atsScore": {
    "overall": 0.0-100,
    "keywordMatch": 0.0-100,
    "formatCompliance": 0.0-100,
    "contentQuality": 0.0-100,
    "readability": 0.0-100
  },
  "keywordAnalysis": {
    "requiredKeywords": [
      {
        "keyword": "",
        "found": true/false,
        "frequency": 0,
        "placement": ["Summary", "Experience", "Skills"],
        "optimization": "Add/Increase/Reposition"
      }
    ],
    "preferredKeywords": [
      {
        "keyword": "",
        "found": true/false,
        "frequency": 0,
        "placement": ["Summary", "Experience", "Skills"],
        "optimization": "Add/Increase/Reposition"
      }
    ],
    "keywordDensity": {
      "current": 0.0,
      "optimal": 0.0,
      "recommendations": []
    }
  },
  "formatOptimization": {
    "structure": {
      "current": "",
      "recommended": "",
      "changes": []
    },
    "sections": [
      {
        "section": "",
        "currentOrder": 0,
        "recommendedOrder": 0,
        "reason": ""
      }
    ],
    "formatting": [
      {
        "element": "",
        "current": "",
        "recommended": "",
        "atsCompatibility": "Good/Fair/Poor"
      }
    ]
  },
  "contentOptimization": {
    "summary": {
      "current": "",
      "optimized": "",
      "keywordEnhancement": [],
      "impact": "High/Medium/Low"
    },
    "experience": [
      {
        "position": "",
        "current": "",
        "optimized": "",
        "keywordEnhancement": [],
        "quantification": []
      }
    ],
    "skills": {
      "current": [],
      "optimized": [],
      "keywordAlignment": [],
      "missing": []
    }
  },
  "readabilityOptimization": {
    "sentenceStructure": {
      "averageLength": 0,
      "recommendedLength": 0,
      "improvements": []
    },
    "actionVerbs": {
      "current": [],
      "recommended": [],
      "replacements": []
    },
    "bulletPoints": {
      "current": 0,
      "recommended": 0,
      "optimization": []
    }
  },
  "canadianOptimization": {
    "terminology": [
      {
        "current": "",
        "recommended": "",
        "reason": ""
      }
    ],
    "spelling": [
      {
        "current": "",
        "recommended": "",
        "reason": "Canadian spelling"
      }
    ],
    "culturalContext": [
      {
        "element": "",
        "optimization": "",
        "reason": ""
      }
    ]
  },
  "implementationPriority": [
    {
      "action": "",
      "priority": "Critical/High/Medium/Low",
      "impact": "High/Medium/Low",
      "effort": "High/Medium/Low",
      "timeline": ""
    }
  ]
}

Guidelines:
- Focus on Canadian ATS systems and standards
- Ensure keyword optimization without stuffing
- Maintain professional readability
- Consider Canadian workplace terminology
- Provide specific, actionable recommendations

Return only valid JSON.`;

const SKILLS_TRANSLATION_PROMPT = (originalSkills, targetIndustry, canadianContext) => `
Translate and adapt these skills for the Canadian job market and target industry.

Original Skills:
${JSON.stringify(originalSkills, null, 2)}

Target Industry: ${targetIndustry}
Canadian Context: ${JSON.stringify(canadianContext, null, 2)}

Generate skills translation in this exact JSON structure:
{
  "translatedSkills": {
    "technical": [
      {
        "original": "",
        "translated": "",
        "canadianEquivalent": "",
        "industryRelevance": "High/Medium/Low",
        "certificationNeeded": "Yes/No",
        "confidence": 0.0-1.0
      }
    ],
    "soft": [
      {
        "original": "",
        "translated": "",
        "canadianContext": "",
        "workplaceRelevance": "High/Medium/Low",
        "culturalAdaptation": "",
        "confidence": 0.0-1.0
      }
    ],
    "languages": [
      {
        "language": "",
        "proficiency": "Native/Fluent/Intermediate/Basic",
        "canadianValue": "High/Medium/Low",
        "certification": "Required/Recommended/Optional",
        "confidence": 0.0-1.0
      }
    ]
  },
  "skillGaps": [
    {
      "missingSkill": "",
      "importance": "Critical/High/Medium/Low",
      "canadianRequirement": "",
      "acquisitionPath": "",
      "timeline": "",
      "priority": "High/Medium/Low"
    }
  ],
  "certificationMapping": [
    {
      "originalCertification": "",
      "canadianEquivalent": "",
      "recognitionStatus": "Fully/Partially/Not Recognized",
      "upgradePath": "",
      "cost": "",
      "timeline": ""
    }
  ],
  "industrySpecific": {
    "technicalStandards": [
      {
        "standard": "",
        "canadianVersion": "",
        "compliance": "Required/Recommended/Optional",
        "implementation": ""
      }
    ],
    "regulatoryRequirements": [
      {
        "requirement": "",
        "canadianEquivalent": "",
        "compliance": "Required/Recommended/Optional",
        "process": ""
      }
    ],
    "bestPractices": [
      {
        "practice": "",
        "canadianAdaptation": "",
        "benefit": "",
        "implementation": ""
      }
    ]
  },
  "culturalAdaptation": {
    "workplaceNorms": [
      {
        "norm": "",
        "canadianExpectation": "",
        "adaptation": "",
        "importance": "High/Medium/Low"
      }
    ],
    "communicationStyle": [
      {
        "style": "",
        "canadianEquivalent": "",
        "adjustment": "",
        "context": ""
      }
    ],
    "professionalEtiquette": [
      {
        "etiquette": "",
        "canadianStandard": "",
        "adaptation": "",
        "importance": "High/Medium/Low"
      }
    ]
  },
  "implementationStrategy": {
    "immediateActions": [
      {
        "action": "",
        "priority": "High/Medium/Low",
        "timeline": "",
        "resources": []
      }
    ],
    "shortTerm": [
      {
        "goal": "",
        "timeline": "1-3 months",
        "actions": [],
        "successMetrics": []
      }
    ],
    "longTerm": [
      {
        "goal": "",
        "timeline": "6+ months",
        "actions": [],
        "successMetrics": []
      }
    ]
  }
}

Guidelines:
- Focus on Canadian industry standards and requirements
- Consider newcomer context and international experience
- Provide specific, actionable recommendations
- Include certification and regulatory requirements
- Address cultural adaptation needs

Return only valid JSON.`;

const CANADIAN_MARKET_INTELLIGENCE_PROMPT = (jobTitle, industry, location) => `
Provide comprehensive Canadian market intelligence for this job opportunity.

Job Title: ${jobTitle}
Industry: ${industry}
Location: ${location}

Generate Canadian market intelligence in this exact JSON structure:
{
  "marketOverview": {
    "industryHealth": "Strong/Moderate/Weak",
    "growthTrend": "Growing/Stable/Declining",
    "keyDrivers": [],
    "challenges": [],
    "opportunities": []
  },
  "regionalAnalysis": {
    "location": "${location}",
    "marketStrength": "High/Medium/Low",
    "competitionLevel": "High/Medium/Low",
    "salaryBenchmarks": {
      "entry": 0,
      "mid": 0,
      "senior": 0,
      "currency": "CAD"
    },
    "costOfLiving": "High/Medium/Low",
    "qualityOfLife": "High/Medium/Low"
  },
  "jobMarket": {
    "demand": "High/Medium/Low",
    "supply": "High/Medium/Low",
    "growthRate": "0.0%",
    "newcomerFriendly": true/false,
    "remoteWork": "Common/Some/Rare",
    "contractWork": "Common/Some/Rare"
  },
  "skillDemand": {
    "hotSkills": [
      {
        "skill": "",
        "demand": "High/Medium/Low",
        "growth": "Growing/Stable/Declining",
        "salaryImpact": "High/Medium/Low"
      }
    ],
    "emergingSkills": [
      {
        "skill": "",
        "adoption": "Early/Mid/Late",
        "futureDemand": "High/Medium/Low",
        "learningPath": ""
      }
    ],
    "decliningSkills": [
      {
        "skill": "",
        "reason": "",
        "replacement": "",
        "timeline": ""
      }
    ]
  },
  "companyLandscape": {
    "majorEmployers": [
      {
        "name": "",
        "size": "Large/Medium/Small",
        "reputation": "Excellent/Good/Fair",
        "newcomerFriendly": true/false,
        "growth": "Growing/Stable/Declining"
      }
    ],
    "startupEcosystem": {
      "vibrancy": "High/Medium/Low",
      "funding": "High/Medium/Low",
      "opportunities": []
    },
    "governmentSector": {
      "opportunities": "High/Medium/Low",
      "requirements": [],
      "benefits": []
    }
  },
  "newcomerConsiderations": {
    "credentialRecognition": {
      "process": "",
      "timeline": "",
      "cost": "",
      "successRate": "0.0%"
    },
    "languageRequirements": {
      "english": "Required/Preferred",
      "french": "Required/Preferred",
      "bilingual": "Required/Preferred",
      "certification": "Required/Recommended"
    },
    "culturalAdaptation": {
      "challenges": [],
      "resources": [],
      "timeline": "",
      "support": []
    },
    "networking": {
      "professionalAssociations": [],
      "events": [],
      "onlinePlatforms": [],
      "mentorship": []
    }
  },
  "salaryInsights": {
    "currentRange": {
      "min": 0,
      "max": 0,
      "median": 0,
      "currency": "CAD"
    },
    "factors": [
      {
        "factor": "",
        "impact": "High/Medium/Low",
        "description": ""
      }
    ],
    "negotiation": {
      "leverage": "High/Medium/Low",
      "strategies": [],
      "timing": ""
    }
  },
  "careerProgression": {
    "typicalPath": [
      {
        "level": "",
        "title": "",
        "experience": "",
        "salary": ""
      }
    ],
    "advancement": {
      "timeline": "",
      "requirements": [],
      "opportunities": []
    },
    "specialization": {
      "areas": [],
      "demand": "High/Medium/Low",
      "salary": ""
    }
  },
  "recommendations": {
    "immediate": [
      {
        "action": "",
        "priority": "High/Medium/Low",
        "timeline": "",
        "impact": "High/Medium/Low"
      }
    ],
    "shortTerm": [
      {
        "goal": "",
        "actions": [],
        "timeline": "3-6 months",
        "successMetrics": []
      }
    ],
    "longTerm": [
      {
        "goal": "",
        "actions": [],
        "timeline": "1-2 years",
        "successMetrics": []
      }
    ]
  }
}

Guidelines:
- Focus on Canadian market specifics
- Include newcomer-friendly insights
- Provide actionable recommendations
- Consider regional variations
- Address cultural and regulatory factors

Return only valid JSON.`;

// Dynamic prompts - use functions for variable content
const createResumeGenerationPrompt = (resumeAnalysis, jobTargeting) => RESUME_GENERATION_PROMPT(resumeAnalysis, jobTargeting);
const createJobTargetingAnalysisPrompt = (jobDescription, resumeAnalysis) => JOB_TARGETING_ANALYSIS_PROMPT(jobDescription, resumeAnalysis);
const createATSOptimizationPrompt = (resumeData, jobDescription) => ATS_OPTIMIZATION_PROMPT(resumeData, jobDescription);
const createSkillsTranslationPrompt = (originalSkills, targetIndustry, canadianContext) => SKILLS_TRANSLATION_PROMPT(originalSkills, targetIndustry, canadianContext);
const createCanadianMarketIntelligencePrompt = (jobTitle, industry, location) => CANADIAN_MARKET_INTELLIGENCE_PROMPT(jobTitle, industry, location);

module.exports = {
  RESUME_GENERATION_PROMPT,
  JOB_TARGETING_ANALYSIS_PROMPT,
  ATS_OPTIMIZATION_PROMPT,
  SKILLS_TRANSLATION_PROMPT,
  CANADIAN_MARKET_INTELLIGENCE_PROMPT,
  createResumeGenerationPrompt,
  createJobTargetingAnalysisPrompt,
  createATSOptimizationPrompt,
  createSkillsTranslationPrompt,
  createCanadianMarketIntelligencePrompt
};
````

## File: src/repositories/BaseRepository.js
````javascript
const { DatabaseError } = require('../utils/errors');
const { logger } = require('../config/logger');

/**
 * Base Repository class providing common CRUD operations
 * All specific repositories should extend this class
 */
class BaseRepository {
  constructor(tableName, supabaseClient, supabaseServiceClient) {
    this.tableName = tableName;
    this.supabase = supabaseClient;
    this.supabaseService = supabaseServiceClient;
  }

  /**
   * Create a new record
   * @param {Object} data - Data to insert
   * @param {boolean} useServiceRole - Whether to use service role client (bypasses RLS)
   * @returns {Promise<Object>} Created record
   */
  async create(data, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { data: result, error } = await client
        .from(this.tableName)
        .insert(data)
        .select()
        .single();

      if (error) {
        logger.error(`Error creating ${this.tableName} record:`, error);
        throw new DatabaseError(`Failed to create ${this.tableName} record`, 500, error);
      }

      logger.info(`Created ${this.tableName} record with ID: ${result.id}`);
      return result;
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error creating ${this.tableName} record:`, error);
      throw new DatabaseError(`Failed to create ${this.tableName} record`, 500, error);
    }
  }

  /**
   * Find a record by ID
   * @param {string|number} id - Record ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} Found record or null
   */
  async findById(id, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { data: result, error } = await client
        .from(this.tableName)
        .select('*')
        .eq('id', id)
        .single();

      if (error && error.code !== 'PGRST116') {
        logger.error(`Error finding ${this.tableName} by ID ${id}:`, error);
        throw new DatabaseError(`Failed to find ${this.tableName} by ID`, 500, error);
      }

      return result || null;
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error finding ${this.tableName} by ID:`, error);
      throw new DatabaseError(`Failed to find ${this.tableName} by ID`, 500, error);
    }
  }

  /**
   * Find records by a specific field
   * @param {string} field - Field name
   * @param {any} value - Field value
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Found records
   */
  async findByField(field, value, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { data: results, error } = await client
        .from(this.tableName)
        .select('*')
        .eq(field, value);

      if (error) {
        logger.error(`Error finding ${this.tableName} by ${field}:`, error);
        throw new DatabaseError(`Failed to find ${this.tableName} by ${field}`, 500, error);
      }

      return results || [];
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error finding ${this.tableName} by ${field}:`, error);
      throw new DatabaseError(`Failed to find ${this.tableName} by ${field}`, 500, error);
    }
  }

  /**
   * Find a single record by a specific field
   * @param {string} field - Field name
   * @param {any} value - Field value
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} Found record or null
   */
  async findOneByField(field, value, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { data: result, error } = await client
        .from(this.tableName)
        .select('*')
        .eq(field, value)
        .single();

      if (error && error.code !== 'PGRST116') {
        logger.error(`Error finding ${this.tableName} by ${field}:`, error);
        throw new DatabaseError(`Failed to find ${this.tableName} by ${field}`, 500, error);
      }

      return result || null;
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error finding ${this.tableName} by ${field}:`, error);
      throw new DatabaseError(`Failed to find ${this.tableName} by ${field}`, 500, error);
    }
  }

  /**
   * Update a record by ID
   * @param {string|number} id - Record ID
   * @param {Object} data - Data to update
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated record
   */
  async updateById(id, data, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { data: result, error } = await client
        .from(this.tableName)
        .update(data)
        .eq('id', id)
        .select()
        .single();

      if (error) {
        logger.error(`Error updating ${this.tableName} with ID ${id}:`, error);
        throw new DatabaseError(`Failed to update ${this.tableName}`, 500, error);
      }

      logger.info(`Updated ${this.tableName} record with ID: ${id}`);
      return result;
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error updating ${this.tableName}:`, error);
      throw new DatabaseError(`Failed to update ${this.tableName}`, 500, error);
    }
  }

  /**
   * Delete a record by ID
   * @param {string|number} id - Record ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<boolean>} Success status
   */
  async deleteById(id, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { error } = await client
        .from(this.tableName)
        .delete()
        .eq('id', id);

      if (error) {
        logger.error(`Error deleting ${this.tableName} with ID ${id}:`, error);
        throw new DatabaseError(`Failed to delete ${this.tableName}`, 500, error);
      }

      logger.info(`Deleted ${this.tableName} record with ID: ${id}`);
      return true;
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error deleting ${this.tableName}:`, error);
      throw new DatabaseError(`Failed to delete ${this.tableName}`, 500, error);
    }
  }

  /**
   * Find all records with optional pagination
   * @param {Object} options - Query options
   * @param {number} options.limit - Number of records to return
   * @param {number} options.offset - Number of records to skip
   * @param {string} options.orderBy - Field to order by
   * @param {string} options.orderDirection - Order direction (asc/desc)
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Found records
   */
  async findAll(options = {}, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      let query = client.from(this.tableName).select('*');

      if (options.limit) {
        query = query.limit(options.limit);
      }

      if (options.offset) {
        query = query.range(options.offset, options.offset + (options.limit || 100) - 1);
      }

      if (options.orderBy) {
        const direction = options.orderDirection || 'asc';
        query = query.order(options.orderBy, { ascending: direction === 'asc' });
      }

      const { data: results, error } = await query;

      if (error) {
        logger.error(`Error finding all ${this.tableName}:`, error);
        throw new DatabaseError(`Failed to find ${this.tableName} records`, 500, error);
      }

      return results || [];
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error finding all ${this.tableName}:`, error);
      throw new DatabaseError(`Failed to find ${this.tableName} records`, 500, error);
    }
  }

  /**
   * Count records with optional filter
   * @param {Object} filter - Filter conditions
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<number>} Count of records
   */
  async count(filter = {}, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      let query = client.from(this.tableName).select('*', { count: 'exact', head: true });

      // Apply filters
      Object.entries(filter).forEach(([field, value]) => {
        query = query.eq(field, value);
      });

      const { count, error } = await query;

      if (error) {
        logger.error(`Error counting ${this.tableName}:`, error);
        throw new DatabaseError(`Failed to count ${this.tableName} records`, 500, error);
      }

      return count || 0;
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error counting ${this.tableName}:`, error);
      throw new DatabaseError(`Failed to count ${this.tableName} records`, 500, error);
    }
  }

  /**
   * Upsert a record (insert or update)
   * @param {Object} data - Data to upsert
   * @param {string} conflictField - Field to check for conflicts
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Upserted record
   */
  async upsert(data, conflictField = 'id', useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { data: result, error } = await client
        .from(this.tableName)
        .upsert(data, { onConflict: conflictField })
        .select()
        .single();

      if (error) {
        logger.error(`Error upserting ${this.tableName}:`, error);
        throw new DatabaseError(`Failed to upsert ${this.tableName} record`, 500, error);
      }

      logger.info(`Upserted ${this.tableName} record with ID: ${result.id}`);
      return result;
    } catch (error) {
      if (error instanceof DatabaseError) throw error;
      logger.error(`Unexpected error upserting ${this.tableName}:`, error);
      throw new DatabaseError(`Failed to upsert ${this.tableName} record`, 500, error);
    }
  }
}

module.exports = BaseRepository;
````

## File: src/repositories/CareerProfileRepository.js
````javascript
const BaseRepository = require('./BaseRepository');
const { logger } = require('../config/logger');

/**
 * Career Profile Repository for career profile-related database operations
 */
class CareerProfileRepository extends BaseRepository {
  constructor(supabaseClient, supabaseServiceClient) {
    super('user_career_profiles', supabaseClient, supabaseServiceClient);
  }

  /**
   * Save or update career profile
   * @param {string|number} userId - User ID
   * @param {Object} profileData - Career profile data
   * @returns {Promise<Object>} Saved/updated profile record
   */
  async saveCareerProfile(userId, profileData) {
    try {
      logger.info('💾 Starting saveCareerProfile for user:', userId);
      
      const profileRecord = await this.upsert({
        user_id: parseInt(userId),
        professional_summary: profileData.professionalSummary,
        skills_categories: profileData.skillsCategories,
        career_objectives: profileData.careerObjectives,
        target_industries: profileData.targetIndustries,
        market_alignment_score: profileData.marketAlignmentScore,
        skill_gaps: profileData.skillGaps,
        improvement_roadmap: profileData.improvementRoadmap,
        last_updated: new Date().toISOString()
      }, 'user_id', true);

      logger.info('✅ Career profile saved/updated successfully:', { id: profileRecord.id, userId: profileRecord.user_id });
      return profileRecord;

    } catch (error) {
      logger.error('❌ Error saving career profile:', error);
      throw error;
    }
  }

  /**
   * Get career profile by user ID
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} Career profile record or null
   */
  async getCareerProfileByUserId(userId, useServiceRole = false) {
    try {
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }

      return this.findOneByField('user_id', numericUserId, useServiceRole);
    } catch (error) {
      logger.error('❌ Error fetching career profile:', error);
      throw error;
    }
  }

  /**
   * Update career profile
   * @param {string|number} userId - User ID
   * @param {Object} updateData - Data to update
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated profile record
   */
  async updateCareerProfile(userId, updateData, useServiceRole = false) {
    try {
      logger.info('🔍 Starting updateCareerProfile for user:', userId);
      
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }

      // Add last_updated timestamp
      updateData.last_updated = new Date().toISOString();

      // Find the profile first to get its ID
      const existingProfile = await this.findOneByField('user_id', numericUserId, useServiceRole);
      if (!existingProfile) {
        throw new Error(`Career profile not found for user ID: ${userId}`);
      }

      const updatedProfile = await this.updateById(existingProfile.id, updateData, useServiceRole);
      logger.info('✅ Career profile updated successfully:', { id: updatedProfile.id, userId: updatedProfile.user_id });
      return updatedProfile;

    } catch (error) {
      logger.error('❌ Error updating career profile:', error);
      throw error;
    }
  }

  /**
   * Delete career profile
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<boolean>} Success status
   */
  async deleteCareerProfile(userId, useServiceRole = false) {
    try {
      logger.info('🗑️ Starting deleteCareerProfile for user:', userId);
      
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }

      // Find the profile first to get its ID
      const existingProfile = await this.findOneByField('user_id', numericUserId, useServiceRole);
      if (!existingProfile) {
        logger.warn('Career profile not found for deletion:', { userId });
        return true; // Consider it successfully deleted if it doesn't exist
      }

      const success = await this.deleteById(existingProfile.id, useServiceRole);
      logger.info('✅ Career profile deleted successfully:', { userId });
      return success;

    } catch (error) {
      logger.error('❌ Error deleting career profile:', error);
      throw error;
    }
  }

  /**
   * Search career profiles with criteria
   * @param {Object} criteria - Search criteria
   * @param {string} criteria.targetIndustry - Target industry (partial match)
   * @param {number} criteria.minMarketAlignmentScore - Minimum market alignment score
   * @param {number} criteria.maxMarketAlignmentScore - Maximum market alignment score
   * @param {Date} criteria.updatedAfter - Updated after date
   * @param {Date} criteria.updatedBefore - Updated before date
   * @param {Object} options - Query options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Matching career profiles
   */
  async searchCareerProfiles(criteria = {}, options = {}, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      let query = client.from(this.tableName).select('*');

      // Apply search criteria
      if (criteria.targetIndustry) {
        query = query.ilike('target_industries', `%${criteria.targetIndustry}%`);
      }

      if (criteria.minMarketAlignmentScore !== undefined) {
        query = query.gte('market_alignment_score', criteria.minMarketAlignmentScore);
      }

      if (criteria.maxMarketAlignmentScore !== undefined) {
        query = query.lte('market_alignment_score', criteria.maxMarketAlignmentScore);
      }

      if (criteria.updatedAfter) {
        query = query.gte('last_updated', criteria.updatedAfter.toISOString());
      }

      if (criteria.updatedBefore) {
        query = query.lte('last_updated', criteria.updatedBefore.toISOString());
      }

      // Apply pagination and ordering
      if (options.limit) {
        query = query.limit(options.limit);
      }

      if (options.offset) {
        query = query.range(options.offset, options.offset + (options.limit || 100) - 1);
      }

      if (options.orderBy) {
        const direction = options.orderDirection || 'desc';
        query = query.order(options.orderBy, { ascending: direction === 'asc' });
      } else {
        // Default ordering by last_updated desc
        query = query.order('last_updated', { ascending: false });
      }

      const { data: results, error } = await query;

      if (error) {
        logger.error('Error searching career profiles:', error);
        throw error;
      }

      return results || [];
    } catch (error) {
      logger.error('Unexpected error searching career profiles:', error);
      throw error;
    }
  }

  /**
   * Get career profiles with pagination
   * @param {Object} options - Pagination options
   * @param {number} options.limit - Number of records to return
   * @param {number} options.offset - Number of records to skip
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Career profiles with pagination info
   */
  async getCareerProfilesWithPagination(options = {}, useServiceRole = false) {
    try {
      const limit = options.limit || 10;
      const offset = options.offset || 0;

      const client = useServiceRole ? this.supabaseService : this.supabase;
      
      // Get total count
      const { count: totalCount, error: countError } = await client
        .from(this.tableName)
        .select('*', { count: 'exact', head: true });

      if (countError) {
        logger.error('Error getting total count:', countError);
        throw countError;
      }

      // Get paginated results
      const { data: profiles, error } = await client
        .from(this.tableName)
        .select('*')
        .order('last_updated', { ascending: false })
        .range(offset, offset + limit - 1);

      if (error) {
        logger.error('Error getting paginated profiles:', error);
        throw error;
      }

      return {
        profiles: profiles || [],
        pagination: {
          total: totalCount || 0,
          limit,
          offset,
          hasMore: (offset + limit) < (totalCount || 0),
          totalPages: Math.ceil((totalCount || 0) / limit)
        }
      };
    } catch (error) {
      logger.error('Error getting career profiles with pagination:', error);
      throw error;
    }
  }

  /**
   * Get career profile statistics
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Career profile statistics
   */
  async getCareerProfileStatistics(useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      
      // Get total profile count
      const { count: totalProfiles, error: totalError } = await client
        .from(this.tableName)
        .select('*', { count: 'exact', head: true });

      if (totalError) {
        logger.error('Error getting total profile count:', totalError);
        throw totalError;
      }

      // Get average market alignment score
      const { data: avgScoreData, error: avgScoreError } = await client
        .from(this.tableName)
        .select('market_alignment_score')
        .not('market_alignment_score', 'is', null);

      if (avgScoreError) {
        logger.error('Error getting average market alignment score:', avgScoreError);
        throw avgScoreError;
      }

      const avgMarketAlignmentScore = avgScoreData && avgScoreData.length > 0
        ? avgScoreData.reduce((sum, profile) => sum + (profile.market_alignment_score || 0), 0) / avgScoreData.length
        : 0;

      // Get profiles by market alignment score ranges
      const scoreRanges = {
        '0-25': 0,
        '26-50': 0,
        '51-75': 0,
        '76-100': 0
      };

      avgScoreData?.forEach(profile => {
        const score = profile.market_alignment_score || 0;
        if (score <= 25) scoreRanges['0-25']++;
        else if (score <= 50) scoreRanges['26-50']++;
        else if (score <= 75) scoreRanges['51-75']++;
        else scoreRanges['76-100']++;
      });

      // Get recently updated profiles (last 30 days)
      const thirtyDaysAgo = new Date();
      thirtyDaysAgo.setDate(thirtyDaysAgo.getDate() - 30);
      
      const { data: recentProfiles, error: recentError } = await client
        .from(this.tableName)
        .select('last_updated')
        .gte('last_updated', thirtyDaysAgo.toISOString());

      if (recentError) {
        logger.error('Error getting recent profile count:', recentError);
        throw recentError;
      }

      return {
        totalProfiles: totalProfiles || 0,
        averageMarketAlignmentScore: Math.round(avgMarketAlignmentScore * 100) / 100,
        byMarketAlignmentScore: scoreRanges,
        recentlyUpdated: recentProfiles ? recentProfiles.length : 0
      };
    } catch (error) {
      logger.error('Error getting career profile statistics:', error);
      throw error;
    }
  }

  /**
   * Get career profiles by market alignment score range
   * @param {number} minScore - Minimum score
   * @param {number} maxScore - Maximum score
   * @param {Object} options - Query options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Career profiles in the score range
   */
  async getCareerProfilesByMarketAlignmentScore(minScore, maxScore, options = {}, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      let query = client.from(this.tableName).select('*');

      // Apply score range filter
      if (minScore !== undefined) {
        query = query.gte('market_alignment_score', minScore);
      }

      if (maxScore !== undefined) {
        query = query.lte('market_alignment_score', maxScore);
      }

      // Apply pagination and ordering
      if (options.limit) {
        query = query.limit(options.limit);
      }

      if (options.offset) {
        query = query.range(options.offset, options.offset + (options.limit || 100) - 1);
      }

      if (options.orderBy) {
        const direction = options.orderDirection || 'desc';
        query = query.order(options.orderBy, { ascending: direction === 'asc' });
      } else {
        // Default ordering by market_alignment_score desc
        query = query.order('market_alignment_score', { ascending: false });
      }

      const { data: results, error } = await query;

      if (error) {
        logger.error('Error getting career profiles by market alignment score:', error);
        throw error;
      }

      return results || [];
    } catch (error) {
      logger.error('Unexpected error getting career profiles by market alignment score:', error);
      throw error;
    }
  }

  /**
   * Get career profiles with skill gaps
   * @param {Object} options - Query options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Career profiles with skill gaps
   */
  async getCareerProfilesWithSkillGaps(options = {}, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      let query = client.from(this.tableName).select('*');

      // Filter profiles that have skill gaps
      query = query.not('skill_gaps', 'is', null);

      // Apply pagination and ordering
      if (options.limit) {
        query = query.limit(options.limit);
      }

      if (options.offset) {
        query = query.range(options.offset, options.offset + (options.limit || 100) - 1);
      }

      if (options.orderBy) {
        const direction = options.orderDirection || 'desc';
        query = query.order(options.orderBy, { ascending: direction === 'asc' });
      } else {
        // Default ordering by last_updated desc
        query = query.order('last_updated', { ascending: false });
      }

      const { data: results, error } = await query;

      if (error) {
        logger.error('Error getting career profiles with skill gaps:', error);
        throw error;
      }

      return results || [];
    } catch (error) {
      logger.error('Unexpected error getting career profiles with skill gaps:', error);
      throw error;
    }
  }
}

module.exports = CareerProfileRepository;
````

## File: src/repositories/GeneratedResumeRepository.js
````javascript
const BaseRepository = require('./BaseRepository');
const { logger } = require('../config/logger');

/**
 * Generated Resume Repository for AI-generated resume database operations
 */
class GeneratedResumeRepository extends BaseRepository {
  constructor(supabaseClient, supabaseServiceClient) {
    super('generated_resumes', supabaseClient, supabaseServiceClient);
  }

  /**
   * Create a new generated resume
   * @param {Object} resumeData - Generated resume data
   * @param {number} userId - User ID
   * @param {number} originalAnalysisId - Original resume analysis ID
   * @param {Object} jobTargeting - Job targeting information
   * @returns {Promise<Object>} Created generated resume record
   */
  async createGeneratedResume(resumeData, userId, originalAnalysisId, jobTargeting) {
    try {
      logger.info('💾 Starting createGeneratedResume for user:', userId);
      logger.info('💾 Job targeting:', jobTargeting);
      
      // Ensure userId and analysisId are valid numbers
      const numericUserId = parseInt(userId);
      const numericAnalysisId = parseInt(originalAnalysisId);
      
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      if (isNaN(numericAnalysisId)) {
        throw new Error(`Invalid analysis ID: ${originalAnalysisId}. Expected a numeric database analysis ID.`);
      }
      
      const generatedResumeRecord = await this.create({
        user_id: numericUserId,
        original_analysis_id: numericAnalysisId,
        job_title: jobTargeting.jobTitle || '',
        job_description: jobTargeting.jobDescription || '',
        company_name: jobTargeting.companyName || '',
        industry: jobTargeting.industry || '',
        location: jobTargeting.location || '',
        resume_data: JSON.stringify(resumeData),
        user_edits: JSON.stringify({}),
        ai_suggestions: JSON.stringify([]),
        ats_score: null, // Will be calculated later
        status: 'draft',
        pdf_downloaded_count: 0,
        template_used: jobTargeting.template || 'canadian_classic',
        generation_version: '1.0',
        created_at: new Date().toISOString(),
        last_updated: new Date().toISOString()
      }, true);

      logger.info('✅ Generated resume created successfully with ID:', generatedResumeRecord.id);
      logger.info('✅ Created resume data:', {
        id: generatedResumeRecord.id,
        userId: generatedResumeRecord.user_id,
        analysisId: generatedResumeRecord.original_analysis_id,
        jobTitle: generatedResumeRecord.job_title,
        status: generatedResumeRecord.status,
        createdAt: generatedResumeRecord.created_at
      });

      return generatedResumeRecord;
    } catch (error) {
      logger.error('❌ Error creating generated resume:', error);
      throw error;
    }
  }

  /**
   * Get generated resumes for a user
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Generated resumes for the user
   */
  async getGeneratedResumes(userId, useServiceRole = false) {
    try {
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      return this.findByField('user_id', numericUserId, useServiceRole);
    } catch (error) {
      logger.error('❌ Error fetching generated resumes:', error);
      throw error;
    }
  }

  /**
   * Get generated resumes for a user with ordering
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Generated resumes for the user ordered by creation date
   */
  async getUserGeneratedResumes(userId, useServiceRole = false) {
    try {
      logger.info('🔍 Starting getUserGeneratedResumes for user:', userId);
      
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { data: resumes, error } = await client
        .from(this.tableName)
        .select('*')
        .eq('user_id', numericUserId)
        .order('created_at', { ascending: false });

      if (error) {
        logger.error('❌ Error fetching generated resumes:', error);
        throw error;
      }

      logger.info('✅ Retrieved', resumes.length, 'generated resumes for user:', userId);
      if (resumes.length > 0) {
        logger.info('✅ Sample resume:', {
          id: resumes[0].id,
          jobTitle: resumes[0].job_title,
          companyName: resumes[0].company_name,
          status: resumes[0].status,
          createdAt: resumes[0].created_at
        });
      }

      return resumes || [];
    } catch (error) {
      logger.error('❌ Error fetching generated resumes:', error);
      throw error;
    }
  }

  /**
   * Get generated resume by ID
   * @param {string|number} resumeId - Generated resume ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} Generated resume record or null
   */
  async getGeneratedResumeById(resumeId, useServiceRole = false) {
    return this.findById(resumeId, useServiceRole);
  }

  /**
   * Update generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {Object} updateData - Data to update
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated resume record
   */
  async updateGeneratedResume(resumeId, updateData, useServiceRole = false) {
    try {
      logger.info('🔍 Starting updateGeneratedResume for ID:', resumeId);
      
      // Add last_updated timestamp
      updateData.last_updated = new Date().toISOString();

      const updatedResume = await this.updateById(resumeId, updateData, useServiceRole);
      logger.info('✅ Generated resume updated successfully:', { id: updatedResume.id });
      return updatedResume;

    } catch (error) {
      logger.error('❌ Error updating generated resume:', error);
      throw error;
    }
  }

  /**
   * Auto-save user edits to generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {Object} userEdits - User edits data
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated resume record
   */
  async autoSaveUserEdits(resumeId, userEdits, useServiceRole = false) {
    try {
      logger.info('💾 Auto-saving user edits for resume ID:', resumeId);
      
      const updateData = {
        user_edits: JSON.stringify(userEdits),
        last_updated: new Date().toISOString()
      };

      const updatedResume = await this.updateById(resumeId, updateData, useServiceRole);
      logger.info('✅ User edits auto-saved successfully:', { id: updatedResume.id });
      return updatedResume;

    } catch (error) {
      logger.error('❌ Error auto-saving user edits:', error);
      throw error;
    }
  }

  /**
   * Update ATS score for generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {number} atsScore - ATS score (0-100)
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated resume record
   */
  async updateATSScore(resumeId, atsScore, useServiceRole = false) {
    try {
      logger.info('📊 Updating ATS score for resume ID:', resumeId, 'Score:', atsScore);
      
      if (atsScore < 0 || atsScore > 100) {
        throw new Error('ATS score must be between 0 and 100');
      }

      const updateData = {
        ats_score: atsScore,
        last_updated: new Date().toISOString()
      };

      const updatedResume = await this.updateById(resumeId, updateData, useServiceRole);
      logger.info('✅ ATS score updated successfully:', { id: updatedResume.id, score: updatedResume.ats_score });
      return updatedResume;

    } catch (error) {
      logger.error('❌ Error updating ATS score:', error);
      throw error;
    }
  }

  /**
   * Track PDF download for generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated resume record
   */
  async trackPDFDownload(resumeId, useServiceRole = false) {
    try {
      logger.info('📥 Tracking PDF download for resume ID:', resumeId);
      
      // First get current record to increment download count
      const currentResume = await this.findById(resumeId, useServiceRole);
      if (!currentResume) {
        throw new Error(`Generated resume with ID ${resumeId} not found`);
      }

      const updateData = {
        pdf_downloaded_count: (currentResume.pdf_downloaded_count || 0) + 1,
        last_pdf_download: new Date().toISOString(),
        last_updated: new Date().toISOString()
      };

      const updatedResume = await this.updateById(resumeId, updateData, useServiceRole);
      logger.info('✅ PDF download tracked successfully:', { 
        id: updatedResume.id, 
        downloadCount: updatedResume.pdf_downloaded_count 
      });
      return updatedResume;

    } catch (error) {
      logger.error('❌ Error tracking PDF download:', error);
      throw error;
    }
  }

  /**
   * Update AI suggestions for generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {Array} aiSuggestions - AI suggestions data
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated resume record
   */
  async updateAISuggestions(resumeId, aiSuggestions, useServiceRole = false) {
    try {
      logger.info('🤖 Updating AI suggestions for resume ID:', resumeId);
      
      const updateData = {
        ai_suggestions: JSON.stringify(aiSuggestions),
        last_updated: new Date().toISOString()
      };

      const updatedResume = await this.updateById(resumeId, updateData, useServiceRole);
      logger.info('✅ AI suggestions updated successfully:', { id: updatedResume.id });
      return updatedResume;

    } catch (error) {
      logger.error('❌ Error updating AI suggestions:', error);
      throw error;
    }
  }

  /**
   * Change status of generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {string} status - New status (draft/finalized/archived)
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated resume record
   */
  async changeStatus(resumeId, status, useServiceRole = false) {
    try {
      logger.info('🔄 Changing status for resume ID:', resumeId, 'New status:', status);
      
      const validStatuses = ['draft', 'finalized', 'archived'];
      if (!validStatuses.includes(status)) {
        throw new Error(`Invalid status: ${status}. Must be one of: ${validStatuses.join(', ')}`);
      }

      const updateData = {
        status: status,
        last_updated: new Date().toISOString()
      };

      const updatedResume = await this.updateById(resumeId, updateData, useServiceRole);
      logger.info('✅ Status changed successfully:', { id: updatedResume.id, status: updatedResume.status });
      return updatedResume;

    } catch (error) {
      logger.error('❌ Error changing status:', error);
      throw error;
    }
  }

  /**
   * Delete generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<boolean>} Success status
   */
  async deleteGeneratedResume(resumeId, useServiceRole = false) {
    try {
      logger.info('🗑️ Starting deleteGeneratedResume for ID:', resumeId);
      
      const success = await this.deleteById(resumeId, useServiceRole);
      logger.info('✅ Generated resume deleted successfully:', { id: resumeId });
      return success;

    } catch (error) {
      logger.error('❌ Error deleting generated resume:', error);
      throw error;
    }
  }

  /**
   * Search generated resumes with criteria
   * @param {Object} criteria - Search criteria
   * @param {string|number} criteria.userId - User ID
   * @param {string} criteria.jobTitle - Job title (partial match)
   * @param {string} criteria.companyName - Company name (partial match)
   * @param {string} criteria.status - Resume status
   * @param {Date} criteria.createdAfter - Created after date
   * @param {Date} criteria.createdBefore - Created before date
   * @param {Object} options - Query options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Matching generated resumes
   */
  async searchGeneratedResumes(criteria = {}, options = {}, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      let query = client.from(this.tableName).select('*');

      // Apply search criteria
      if (criteria.userId) {
        const numericUserId = parseInt(criteria.userId);
        if (!isNaN(numericUserId)) {
          query = query.eq('user_id', numericUserId);
        }
      }

      if (criteria.jobTitle) {
        query = query.ilike('job_title', `%${criteria.jobTitle}%`);
      }

      if (criteria.companyName) {
        query = query.ilike('company_name', `%${criteria.companyName}%`);
      }

      if (criteria.status) {
        query = query.eq('status', criteria.status);
      }

      if (criteria.createdAfter) {
        query = query.gte('created_at', criteria.createdAfter.toISOString());
      }

      if (criteria.createdBefore) {
        query = query.lte('created_at', criteria.createdBefore.toISOString());
      }

      // Apply pagination and ordering
      if (options.limit) {
        query = query.limit(options.limit);
      }

      if (options.offset) {
        query = query.range(options.offset, options.offset + (options.limit || 100) - 1);
      }

      if (options.orderBy) {
        const direction = options.orderDirection || 'desc';
        query = query.order(options.orderBy, { ascending: direction === 'asc' });
      } else {
        // Default ordering by created_at desc
        query = query.order('created_at', { ascending: false });
      }

      const { data: results, error } = await query;

      if (error) {
        logger.error('Error searching generated resumes:', error);
        throw error;
      }

      return results || [];
    } catch (error) {
      logger.error('Unexpected error searching generated resumes:', error);
      throw error;
    }
  }

  /**
   * Get generated resume statistics
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Generated resume statistics
   */
  async getGeneratedResumeStatistics(useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      
      // Get total generated resumes count
      const { count: totalResumes, error: totalError } = await client
        .from(this.tableName)
        .select('*', { count: 'exact', head: true });

      if (totalError) {
        logger.error('Error getting total generated resumes count:', totalError);
        throw totalError;
      }

      // Get resumes by status
      const { data: statusStats, error: statusError } = await client
        .from(this.tableName)
        .select('status')
        .then(result => {
          if (result.error) throw result.error;
          const stats = {};
          result.data.forEach(resume => {
            const status = resume.status || 'draft';
            stats[status] = (stats[status] || 0) + 1;
          });
          return { data: stats, error: null };
        });

      if (statusError) {
        logger.error('Error getting status statistics:', statusError);
        throw statusError;
      }

      // Get resumes by template
      const { data: templateStats, error: templateError } = await client
        .from(this.tableName)
        .select('template_used')
        .then(result => {
          if (result.error) throw result.error;
          const stats = {};
          result.data.forEach(resume => {
            const template = resume.template_used || 'canadian_classic';
            stats[template] = (stats[template] || 0) + 1;
          });
          return { data: stats, error: null };
        });

      if (templateError) {
        logger.error('Error getting template statistics:', templateError);
        throw templateError;
      }

      // Get resumes by date (last 30 days)
      const thirtyDaysAgo = new Date();
      thirtyDaysAgo.setDate(thirtyDaysAgo.getDate() - 30);
      
      const { data: recentResumes, error: recentError } = await client
        .from(this.tableName)
        .select('created_at')
        .gte('created_at', thirtyDaysAgo.toISOString());

      if (recentError) {
        logger.error('Error getting recent generated resumes count:', recentError);
        throw recentError;
      }

      return {
        totalResumes: totalResumes || 0,
        byStatus: statusStats,
        byTemplate: templateStats,
        recentResumes: recentResumes ? recentResumes.length : 0
      };
    } catch (error) {
      logger.error('Error getting generated resume statistics:', error);
      throw error;
    }
  }

  /**
   * Get generated resumes with pagination
   * @param {string|number} userId - User ID
   * @param {Object} options - Pagination options
   * @param {number} options.limit - Number of records to return
   * @param {number} options.offset - Number of records to skip
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Generated resumes with pagination info
   */
  async getGeneratedResumesWithPagination(userId, options = {}, useServiceRole = false) {
    try {
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }

      const limit = options.limit || 10;
      const offset = options.offset || 0;

      const client = useServiceRole ? this.supabaseService : this.supabase;
      
      // Get total count for this user
      const { count: totalCount, error: countError } = await client
        .from(this.tableName)
        .select('*', { count: 'exact', head: true })
        .eq('user_id', numericUserId);

      if (countError) {
        logger.error('Error getting total count:', countError);
        throw countError;
      }

      // Get paginated results
      const { data: resumes, error } = await client
        .from(this.tableName)
        .select('*')
        .eq('user_id', numericUserId)
        .order('created_at', { ascending: false })
        .range(offset, offset + limit - 1);

      if (error) {
        logger.error('Error getting paginated resumes:', error);
        throw error;
      }

      return {
        resumes: resumes || [],
        pagination: {
          total: totalCount || 0,
          limit,
          offset,
          hasMore: (offset + limit) < (totalCount || 0),
          totalPages: Math.ceil((totalCount || 0) / limit)
        }
      };
    } catch (error) {
      logger.error('Error getting generated resumes with pagination:', error);
      throw error;
    }
  }

  /**
   * Get generated resumes by original analysis ID
   * @param {string|number} analysisId - Original resume analysis ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Generated resumes for the analysis
   */
  async getGeneratedResumesByAnalysisId(analysisId, useServiceRole = false) {
    try {
      const numericAnalysisId = parseInt(analysisId);
      if (isNaN(numericAnalysisId)) {
        throw new Error(`Invalid analysis ID: ${analysisId}. Expected a numeric database analysis ID.`);
      }
      
      return this.findByField('original_analysis_id', numericAnalysisId, useServiceRole);
    } catch (error) {
      logger.error('❌ Error fetching generated resumes by analysis ID:', error);
      throw error;
    }
  }
}

module.exports = GeneratedResumeRepository;
````

## File: src/repositories/index.js
````javascript
/**
 * Repository exports
 * This file exports all repository classes for easy importing
 */

const BaseRepository = require('./BaseRepository');
const UserRepository = require('./UserRepository');
const ResumeRepository = require('./ResumeRepository');
const CareerProfileRepository = require('./CareerProfileRepository');
const GeneratedResumeRepository = require('./GeneratedResumeRepository');

module.exports = {
  BaseRepository,
  UserRepository,
  ResumeRepository,
  CareerProfileRepository,
  GeneratedResumeRepository
};
````

## File: src/repositories/ResumeRepository.js
````javascript
const BaseRepository = require('./BaseRepository');
const { logger } = require('../config/logger');

/**
 * Resume Repository for resume analysis-related database operations
 */
class ResumeRepository extends BaseRepository {
  constructor(supabaseClient, supabaseServiceClient) {
    super('resume_analyses', supabaseClient, supabaseServiceClient);
  }

  /**
   * Save resume analysis data
   * @param {string|number} userId - User ID
   * @param {Object} analysisData - Resume analysis data
   * @returns {Promise<Object>} Saved analysis record
   */
  async saveResumeAnalysis(userId, analysisData) {
    try {
      logger.info('💾 Starting saveResumeAnalysis for user:', userId);
      logger.info('💾 Analysis data keys:', Object.keys(analysisData));
      
      // Ensure userId is a valid number (database serial ID)
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      const analysisRecord = await this.create({
        user_id: numericUserId,
        original_file_name: analysisData.originalFileName,
        extracted_text: analysisData.rawText || analysisData.extractedText || 'Text extracted from resume',
        structured_data: analysisData.structuredData || null,
        confidence_scores: JSON.stringify(analysisData.confidenceScores || {}),
        canadian_market_analysis: JSON.stringify(analysisData.canadianMarketAnalysis || {}),
        personal_info: JSON.stringify(analysisData.personalInfo || {}),
        professional_summary: analysisData.professionalSummary || '',
        skills: JSON.stringify(analysisData.skills || {}),
        work_experience: JSON.stringify(analysisData.workExperience || []),
        education: JSON.stringify(analysisData.education || []),
        certifications: JSON.stringify(analysisData.certifications || []),
        projects: JSON.stringify(analysisData.projects || []),
        metadata: JSON.stringify(analysisData.metadata || {}),
        processing_method: analysisData.processingMethod || 'unknown',
        created_at: new Date().toISOString()
      }, true);

      logger.info('✅ Resume analysis saved successfully with ID:', analysisRecord.id);
      logger.info('✅ Saved analysis data:', {
        id: analysisRecord.id,
        userId: analysisRecord.user_id,
        fileName: analysisRecord.original_file_name,
        createdAt: analysisRecord.created_at
      });

      return analysisRecord;
    } catch (error) {
      logger.error('❌ Error saving resume analysis:', error);
      throw error;
    }
  }

  /**
   * Get resume analyses for a user
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Resume analyses for the user
   */
  async getResumeAnalyses(userId, useServiceRole = false) {
    try {
      // Ensure userId is a valid number (database serial ID)
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      return this.findByField('user_id', numericUserId, useServiceRole);
    } catch (error) {
      logger.error('❌ Error fetching resume analyses:', error);
      throw error;
    }
  }

  /**
   * Get resume analyses for a user with ordering
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Resume analyses for the user ordered by creation date
   */
  async getUserResumeAnalyses(userId, useServiceRole = false) {
    try {
      logger.info('🔍 Starting getUserResumeAnalyses for user:', userId);
      
      // Ensure userId is a valid number (database serial ID)
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      const client = useServiceRole ? this.supabaseService : this.supabase;
      const { data: analyses, error } = await client
        .from(this.tableName)
        .select('*')
        .eq('user_id', numericUserId)
        .order('created_at', { ascending: false });

      if (error) {
        logger.error('❌ Error fetching resume analyses:', error);
        throw error;
      }

      logger.info('✅ Retrieved', analyses.length, 'resume analyses for user:', userId);
      if (analyses.length > 0) {
        logger.info('✅ Sample analysis:', {
          id: analyses[0].id,
          fileName: analyses[0].original_file_name,
          createdAt: analyses[0].created_at
        });
      }

      return analyses || [];
    } catch (error) {
      logger.error('❌ Error fetching resume analyses:', error);
      throw error;
    }
  }

  /**
   * Get resume analysis by ID
   * @param {string|number} analysisId - Analysis ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} Resume analysis record or null
   */
  async getResumeAnalysisById(analysisId, useServiceRole = false) {
    return this.findById(analysisId, useServiceRole);
  }

  /**
   * Update resume analysis
   * @param {string|number} analysisId - Analysis ID
   * @param {Object} updateData - Data to update
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated analysis record
   */
  async updateResumeAnalysis(analysisId, updateData, useServiceRole = false) {
    try {
      logger.info('🔍 Starting updateResumeAnalysis for ID:', analysisId);
      
      // Add updated_at timestamp
      updateData.updated_at = new Date().toISOString();

      const updatedAnalysis = await this.updateById(analysisId, updateData, useServiceRole);
      logger.info('✅ Resume analysis updated successfully:', { id: updatedAnalysis.id });
      return updatedAnalysis;

    } catch (error) {
      logger.error('❌ Error updating resume analysis:', error);
      throw error;
    }
  }

  /**
   * Delete resume analysis
   * @param {string|number} analysisId - Analysis ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<boolean>} Success status
   */
  async deleteResumeAnalysis(analysisId, useServiceRole = false) {
    try {
      logger.info('🗑️ Starting deleteResumeAnalysis for ID:', analysisId);
      
      const success = await this.deleteById(analysisId, useServiceRole);
      logger.info('✅ Resume analysis deleted successfully:', { id: analysisId });
      return success;

    } catch (error) {
      logger.error('❌ Error deleting resume analysis:', error);
      throw error;
    }
  }

  /**
   * Search resume analyses with criteria
   * @param {Object} criteria - Search criteria
   * @param {string|number} criteria.userId - User ID
   * @param {string} criteria.fileName - File name (partial match)
   * @param {string} criteria.processingMethod - Processing method
   * @param {Date} criteria.createdAfter - Created after date
   * @param {Date} criteria.createdBefore - Created before date
   * @param {Object} options - Query options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Matching resume analyses
   */
  async searchResumeAnalyses(criteria = {}, options = {}, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      let query = client.from(this.tableName).select('*');

      // Apply search criteria
      if (criteria.userId) {
        const numericUserId = parseInt(criteria.userId);
        if (!isNaN(numericUserId)) {
          query = query.eq('user_id', numericUserId);
        }
      }

      if (criteria.fileName) {
        query = query.ilike('original_file_name', `%${criteria.fileName}%`);
      }

      if (criteria.processingMethod) {
        query = query.eq('processing_method', criteria.processingMethod);
      }

      if (criteria.createdAfter) {
        query = query.gte('created_at', criteria.createdAfter.toISOString());
      }

      if (criteria.createdBefore) {
        query = query.lte('created_at', criteria.createdBefore.toISOString());
      }

      // Apply pagination and ordering
      if (options.limit) {
        query = query.limit(options.limit);
      }

      if (options.offset) {
        query = query.range(options.offset, options.offset + (options.limit || 100) - 1);
      }

      if (options.orderBy) {
        const direction = options.orderDirection || 'desc';
        query = query.order(options.orderBy, { ascending: direction === 'asc' });
      } else {
        // Default ordering by created_at desc
        query = query.order('created_at', { ascending: false });
      }

      const { data: results, error } = await query;

      if (error) {
        logger.error('Error searching resume analyses:', error);
        throw error;
      }

      return results || [];
    } catch (error) {
      logger.error('Unexpected error searching resume analyses:', error);
      throw error;
    }
  }

  /**
   * Get resume analysis statistics
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Resume analysis statistics
   */
  async getResumeAnalysisStatistics(useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      
      // Get total analysis count
      const { count: totalAnalyses, error: totalError } = await client
        .from(this.tableName)
        .select('*', { count: 'exact', head: true });

      if (totalError) {
        logger.error('Error getting total analysis count:', totalError);
        throw totalError;
      }

      // Get analyses by processing method
      const { data: methodStats, error: methodError } = await client
        .from(this.tableName)
        .select('processing_method')
        .then(result => {
          if (result.error) throw result.error;
          const stats = {};
          result.data.forEach(analysis => {
            const method = analysis.processing_method || 'unknown';
            stats[method] = (stats[method] || 0) + 1;
          });
          return { data: stats, error: null };
        });

      if (methodError) {
        logger.error('Error getting processing method statistics:', methodError);
        throw methodError;
      }

      // Get analyses by date (last 30 days)
      const thirtyDaysAgo = new Date();
      thirtyDaysAgo.setDate(thirtyDaysAgo.getDate() - 30);
      
      const { data: recentAnalyses, error: recentError } = await client
        .from(this.tableName)
        .select('created_at')
        .gte('created_at', thirtyDaysAgo.toISOString());

      if (recentError) {
        logger.error('Error getting recent analysis count:', recentError);
        throw recentError;
      }

      return {
        totalAnalyses: totalAnalyses || 0,
        byProcessingMethod: methodStats,
        recentAnalyses: recentAnalyses ? recentAnalyses.length : 0
      };
    } catch (error) {
      logger.error('Error getting resume analysis statistics:', error);
      throw error;
    }
  }

  /**
   * Get resume analysis by user with pagination
   * @param {string|number} userId - User ID
   * @param {Object} options - Pagination options
   * @param {number} options.limit - Number of records to return
   * @param {number} options.offset - Number of records to skip
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Resume analyses with pagination info
   */
  async getResumeAnalysesWithPagination(userId, options = {}, useServiceRole = false) {
    try {
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }

      const limit = options.limit || 10;
      const offset = options.offset || 0;

      const client = useServiceRole ? this.supabaseService : this.supabase;
      
      // Get total count for this user
      const { count: totalCount, error: countError } = await client
        .from(this.tableName)
        .select('*', { count: 'exact', head: true })
        .eq('user_id', numericUserId);

      if (countError) {
        logger.error('Error getting total count:', countError);
        throw countError;
      }

      // Get paginated results
      const { data: analyses, error } = await client
        .from(this.tableName)
        .select('*')
        .eq('user_id', numericUserId)
        .order('created_at', { ascending: false })
        .range(offset, offset + limit - 1);

      if (error) {
        logger.error('Error getting paginated analyses:', error);
        throw error;
      }

      return {
        analyses: analyses || [],
        pagination: {
          total: totalCount || 0,
          limit,
          offset,
          hasMore: (offset + limit) < (totalCount || 0),
          totalPages: Math.ceil((totalCount || 0) / limit)
        }
      };
    } catch (error) {
      logger.error('Error getting resume analyses with pagination:', error);
      throw error;
    }
  }
}

module.exports = ResumeRepository;
````

## File: src/repositories/UserRepository.js
````javascript
const BaseRepository = require('./BaseRepository');
const { logger } = require('../config/logger');

/**
 * User Repository for user-related database operations
 */
class UserRepository extends BaseRepository {
  constructor(supabaseClient, supabaseServiceClient) {
    super('users', supabaseClient, supabaseServiceClient);
  }

  /**
   * Find or create a user by email
   * @param {Object} userData - User data
   * @returns {Promise<Object>} User record
   */
  async findOrCreateUser(userData) {
    try {
      logger.info('🔍 Starting findOrCreateUser with:', { email: userData.email });
      
      // Try to find existing user by email using service role to bypass RLS
      const existingUser = await this.findOneByField('email', userData.email, true);

      if (existingUser) {
        logger.info('✅ Found existing user by email:', { email: existingUser.email, id: existingUser.id });
        return existingUser;
      }

      // If user doesn't exist, create them using service role to bypass RLS
      const newUser = await this.create({
        email: userData.email,
        full_name: userData.fullName || 'User',
        phone_no: userData.phoneNo,
        status_in_canada: userData.statusInCanada,
        country_of_origin: userData.countryOfOrigin,
        current_location: userData.currentLocation,
        role_id: 3, // Immigrant role (ID 3 based on database)
        created_at: new Date().toISOString()
      }, true);

      logger.info('✅ New user created:', { id: newUser.id, email: newUser.email });
      return newUser;

    } catch (error) {
      logger.error('❌ Error finding/creating user:', error);
      throw error;
    }
  }

  /**
   * Update user profile
   * @param {string|number} userId - User ID
   * @param {Object} userData - User data to update
   * @returns {Promise<Object>} Updated user record
   */
  async updateUser(userId, userData) {
    try {
      logger.info('🔍 Starting updateUser for ID:', userId);
      
      const updateData = {};
      
      if (userData.fullName) updateData.full_name = userData.fullName;
      if (userData.phoneNo) updateData.phone_no = userData.phoneNo;
      if (userData.statusInCanada) updateData.status_in_canada = userData.statusInCanada;
      if (userData.countryOfOrigin) updateData.country_of_origin = userData.countryOfOrigin;
      if (userData.currentLocation) updateData.current_location = userData.currentLocation;
      
      updateData.updated_at = new Date().toISOString();

      const updatedUser = await this.updateById(userId, updateData, true);
      logger.info('✅ User updated successfully:', { id: updatedUser.id });
      return updatedUser;

    } catch (error) {
      logger.error('❌ Error updating user:', error);
      throw error;
    }
  }

  /**
   * Get user by email
   * @param {string} email - User email
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} User record or null
   */
  async findByEmail(email, useServiceRole = false) {
    return this.findOneByField('email', email, useServiceRole);
  }

  /**
   * Get users by role
   * @param {number} roleId - Role ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Users with the specified role
   */
  async findByRole(roleId, useServiceRole = false) {
    return this.findByField('role_id', roleId, useServiceRole);
  }

  /**
   * Get users by status in Canada
   * @param {string} status - Status in Canada
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Users with the specified status
   */
  async findByStatusInCanada(status, useServiceRole = false) {
    return this.findByField('status_in_canada', status, useServiceRole);
  }

  /**
   * Get users by country of origin
   * @param {string} country - Country of origin
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Users from the specified country
   */
  async findByCountryOfOrigin(country, useServiceRole = false) {
    return this.findByField('country_of_origin', country, useServiceRole);
  }

  /**
   * Get users by current location
   * @param {string} location - Current location
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Users in the specified location
   */
  async findByCurrentLocation(location, useServiceRole = false) {
    return this.findByField('current_location', location, useServiceRole);
  }

  /**
   * Search users with multiple criteria
   * @param {Object} criteria - Search criteria
   * @param {string} criteria.email - Email (partial match)
   * @param {string} criteria.fullName - Full name (partial match)
   * @param {number} criteria.roleId - Role ID
   * @param {string} criteria.statusInCanada - Status in Canada
   * @param {string} criteria.countryOfOrigin - Country of origin
   * @param {string} criteria.currentLocation - Current location
   * @param {Object} options - Query options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Matching users
   */
  async searchUsers(criteria = {}, options = {}, useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      let query = client.from(this.tableName).select('*');

      // Apply search criteria
      if (criteria.email) {
        query = query.ilike('email', `%${criteria.email}%`);
      }

      if (criteria.fullName) {
        query = query.ilike('full_name', `%${criteria.fullName}%`);
      }

      if (criteria.roleId) {
        query = query.eq('role_id', criteria.roleId);
      }

      if (criteria.statusInCanada) {
        query = query.eq('status_in_canada', criteria.statusInCanada);
      }

      if (criteria.countryOfOrigin) {
        query = query.eq('country_of_origin', criteria.countryOfOrigin);
      }

      if (criteria.currentLocation) {
        query = query.eq('current_location', criteria.currentLocation);
      }

      // Apply pagination and ordering
      if (options.limit) {
        query = query.limit(options.limit);
      }

      if (options.offset) {
        query = query.range(options.offset, options.offset + (options.limit || 100) - 1);
      }

      if (options.orderBy) {
        const direction = options.orderDirection || 'asc';
        query = query.order(options.orderBy, { ascending: direction === 'asc' });
      } else {
        // Default ordering by created_at desc
        query = query.order('created_at', { ascending: false });
      }

      const { data: results, error } = await query;

      if (error) {
        logger.error('Error searching users:', error);
        throw error;
      }

      return results || [];
    } catch (error) {
      logger.error('Unexpected error searching users:', error);
      throw error;
    }
  }

  /**
   * Get user statistics
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} User statistics
   */
  async getUserStatistics(useServiceRole = false) {
    try {
      const client = useServiceRole ? this.supabaseService : this.supabase;
      
      // Get total user count
      const { count: totalUsers, error: totalError } = await client
        .from(this.tableName)
        .select('*', { count: 'exact', head: true });

      if (totalError) {
        logger.error('Error getting total user count:', totalError);
        throw totalError;
      }

      // Get users by role
      const { data: roleStats, error: roleError } = await client
        .from(this.tableName)
        .select('role_id')
        .then(result => {
          if (result.error) throw result.error;
          const stats = {};
          result.data.forEach(user => {
            stats[user.role_id] = (stats[user.role_id] || 0) + 1;
          });
          return { data: stats, error: null };
        });

      if (roleError) {
        logger.error('Error getting role statistics:', roleError);
        throw roleError;
      }

      // Get users by status in Canada
      const { data: statusStats, error: statusError } = await client
        .from(this.tableName)
        .select('status_in_canada')
        .then(result => {
          if (result.error) throw result.error;
          const stats = {};
          result.data.forEach(user => {
            const status = user.status_in_canada || 'Unknown';
            stats[status] = (stats[status] || 0) + 1;
          });
          return { data: stats, error: null };
        });

      if (statusError) {
        logger.error('Error getting status statistics:', statusError);
        throw statusError;
      }

      return {
        totalUsers: totalUsers || 0,
        byRole: roleStats,
        byStatusInCanada: statusStats
      };
    } catch (error) {
      logger.error('Error getting user statistics:', error);
      throw error;
    }
  }
}

module.exports = UserRepository;
````

## File: src/routes/__tests__/authRoutes.test.js
````javascript
/**
 * Auth Routes Tests
 * Tests for authentication-related API endpoints
 */

const request = require('supertest');
const express = require('express');
const { createClient } = require('@supabase/supabase-js');

// Mock dependencies
jest.mock('@supabase/supabase-js');
jest.mock('../../middleware/validation');
jest.mock('../../middleware/authMiddleware');
jest.mock('../../middleware/rateLimiter');
jest.mock('../../config/logger');
jest.mock('../../controllers/ControllerFactory');

const app = express();
app.use(express.json());

// Import the route after mocking
const authRoutes = require('../v1/authRoutes');
app.use('/api/v1/auth', authRoutes);

describe('Auth Routes', () => {
  let mockSupabase;
  let mockAuthController;

  beforeEach(() => {
    // Reset all mocks
    jest.clearAllMocks();

    // Mock Supabase client
    mockSupabase = {
      auth: {
        signUp: jest.fn(),
        signInWithPassword: jest.fn(),
        signOut: jest.fn(),
        refreshSession: jest.fn(),
        getUser: jest.fn(),
        resetPasswordForEmail: jest.fn(),
        updateUser: jest.fn(),
        verifyOtp: jest.fn()
      }
    };
    createClient.mockReturnValue(mockSupabase);

    // Mock controller
    mockAuthController = {
      register: jest.fn(),
      login: jest.fn(),
      logout: jest.fn(),
      refreshToken: jest.fn(),
      getCurrentUser: jest.fn(),
      forgotPassword: jest.fn(),
      resetPassword: jest.fn(),
      verifyEmail: jest.fn()
    };

    const ControllerFactory = require('../../controllers/ControllerFactory');
    ControllerFactory.getController.mockReturnValue(mockAuthController);
  });

  describe('POST /api/v1/auth/register', () => {
    const validRegistrationData = {
      email: 'test@example.com',
      password: 'password123',
      fullName: 'Test User',
      phoneNo: '+1234567890',
      statusInCanada: 'Permanent Resident',
      countryOfOrigin: 'India',
      currentLocation: 'Toronto, ON'
    };

    it('should register a new user successfully', async () => {
      const mockUser = {
        id: 'user-123',
        email: 'test@example.com',
        full_name: 'Test User'
      };

      mockAuthController.register.mockResolvedValue({
        user: mockUser,
        session: { access_token: 'token-123' }
      });

      const response = await request(app)
        .post('/api/v1/auth/register')
        .send(validRegistrationData)
        .expect(201);

      expect(response.body.success).toBe(true);
      expect(response.body.message).toBe('User registered successfully');
      expect(response.body.data.user).toEqual(mockUser);
      expect(mockAuthController.register).toHaveBeenCalledWith(validRegistrationData);
    });

    it('should return 400 for invalid registration data', async () => {
      const invalidData = {
        email: 'invalid-email',
        password: '123' // Too short
      };

      mockAuthController.register.mockRejectedValue(new Error('Invalid data'));

      const response = await request(app)
        .post('/api/v1/auth/register')
        .send(invalidData)
        .expect(400);

      expect(response.body.success).toBe(false);
    });

    it('should handle registration errors gracefully', async () => {
      mockAuthController.register.mockRejectedValue(new Error('Email already exists'));

      const response = await request(app)
        .post('/api/v1/auth/register')
        .send(validRegistrationData)
        .expect(500);

      expect(response.body.success).toBe(false);
      expect(response.body.message).toContain('Email already exists');
    });
  });

  describe('POST /api/v1/auth/login', () => {
    const validLoginData = {
      email: 'test@example.com',
      password: 'password123'
    };

    it('should login user successfully', async () => {
      const mockUser = {
        id: 'user-123',
        email: 'test@example.com',
        full_name: 'Test User'
      };

      mockAuthController.login.mockResolvedValue({
        user: mockUser,
        session: { access_token: 'token-123' }
      });

      const response = await request(app)
        .post('/api/v1/auth/login')
        .send(validLoginData)
        .expect(200);

      expect(response.body.success).toBe(true);
      expect(response.body.message).toBe('Login successful');
      expect(response.body.data.user).toEqual(mockUser);
      expect(mockAuthController.login).toHaveBeenCalledWith(validLoginData);
    });

    it('should return 400 for invalid login credentials', async () => {
      mockAuthController.login.mockRejectedValue(new Error('Invalid credentials'));

      const response = await request(app)
        .post('/api/v1/auth/login')
        .send(validLoginData)
        .expect(400);

      expect(response.body.success).toBe(false);
    });
  });

  describe('POST /api/v1/auth/logout', () => {
    it('should logout user successfully', async () => {
      mockAuthController.logout.mockResolvedValue();

      const response = await request(app)
        .post('/api/v1/auth/logout')
        .set('Authorization', 'Bearer valid-token')
        .expect(200);

      expect(response.body.success).toBe(true);
      expect(response.body.message).toBe('Logout successful');
      expect(mockAuthController.logout).toHaveBeenCalledWith('user-123');
    });

    it('should return 401 for unauthorized logout attempt', async () => {
      const response = await request(app)
        .post('/api/v1/auth/logout')
        .expect(401);

      expect(response.body.success).toBe(false);
    });
  });

  describe('POST /api/v1/auth/refresh', () => {
    it('should refresh token successfully', async () => {
      const mockUser = {
        id: 'user-123',
        email: 'test@example.com'
      };

      mockAuthController.refreshToken.mockResolvedValue({
        user: mockUser,
        session: { access_token: 'new-token-123' }
      });

      const response = await request(app)
        .post('/api/v1/auth/refresh')
        .send({ refreshToken: 'refresh-token-123' })
        .expect(200);

      expect(response.body.success).toBe(true);
      expect(response.body.message).toBe('Token refreshed successfully');
      expect(mockAuthController.refreshToken).toHaveBeenCalledWith('refresh-token-123');
    });
  });

  describe('GET /api/v1/auth/me', () => {
    it('should get current user profile', async () => {
      const mockUser = {
        id: 'user-123',
        email: 'test@example.com',
        full_name: 'Test User'
      };

      mockAuthController.getCurrentUser.mockResolvedValue(mockUser);

      const response = await request(app)
        .get('/api/v1/auth/me')
        .set('Authorization', 'Bearer valid-token')
        .expect(200);

      expect(response.body.success).toBe(true);
      expect(response.body.data).toEqual(mockUser);
      expect(mockAuthController.getCurrentUser).toHaveBeenCalledWith('user-123');
    });
  });

  describe('POST /api/v1/auth/forgot-password', () => {
    it('should send password reset email', async () => {
      mockAuthController.forgotPassword.mockResolvedValue();

      const response = await request(app)
        .post('/api/v1/auth/forgot-password')
        .send({ email: 'test@example.com' })
        .expect(200);

      expect(response.body.success).toBe(true);
      expect(response.body.message).toBe('Password reset email sent successfully');
      expect(mockAuthController.forgotPassword).toHaveBeenCalledWith('test@example.com');
    });
  });

  describe('POST /api/v1/auth/reset-password', () => {
    it('should reset password successfully', async () => {
      mockAuthController.resetPassword.mockResolvedValue();

      const response = await request(app)
        .post('/api/v1/auth/reset-password')
        .send({
          token: 'reset-token-123',
          password: 'newpassword123'
        })
        .expect(200);

      expect(response.body.success).toBe(true);
      expect(response.body.message).toBe('Password reset successful');
      expect(mockAuthController.resetPassword).toHaveBeenCalledWith('reset-token-123', 'newpassword123');
    });
  });

  describe('POST /api/v1/auth/verify-email', () => {
    it('should verify email successfully', async () => {
      mockAuthController.verifyEmail.mockResolvedValue();

      const response = await request(app)
        .post('/api/v1/auth/verify-email')
        .send({ token: 'verification-token-123' })
        .expect(200);

      expect(response.body.success).toBe(true);
      expect(response.body.message).toBe('Email verified successfully');
      expect(mockAuthController.verifyEmail).toHaveBeenCalledWith('verification-token-123');
    });
  });
});
````

## File: src/routes/aiRoutesLocal.js
````javascript
const express = require('express');
const router = express.Router();
const multer = require('multer');
const path = require('path');
const fs = require('fs');
const SupabaseDatabase = require('../services/supabaseDatabase');
const DocumentProcessor = require('../services/documentProcessor');
const documentProcessor = new DocumentProcessor();
const GeminiResumeService = require('../services/GeminiResumeService');
const { generateCareerProfileWithGemini, generatePositionRecommendationsWithGemini, generateEnhancedProfileWithGemini } = require('../services/googleAiService');
const { geminiRateLimit, uploadRateLimit, checkDailyLimit, incrementDailyCount } = require('../middleware/rateLimiter');

// Initialize Supabase database
const supabaseDb = new SupabaseDatabase();

// Initialize Gemini service
const geminiService = new GeminiResumeService();

// Connect to database on startup
supabaseDb.connect().catch(console.error);

// Configure multer for file uploads
const storage = multer.diskStorage({
  destination: (req, file, cb) => {
    const uploadPath = path.join(__dirname, '../uploads/resumes');
    if (!fs.existsSync(uploadPath)) {
      fs.mkdirSync(uploadPath, { recursive: true });
    }
    cb(null, uploadPath);
  },
  filename: (req, file, cb) => {
    const uniqueSuffix = Date.now() + '-' + Math.round(Math.random() * 1E9);
    cb(null, `resume-${uniqueSuffix}${path.extname(file.originalname)}`);
  }
});

const upload = multer({
  storage: storage,
  limits: { fileSize: 10 * 1024 * 1024 }, // 10MB limit (increased for better PDF support)
  fileFilter: (req, file, cb) => {
    const allowedTypes = /pdf|docx|jpg|jpeg|png/;
    const extname = allowedTypes.test(path.extname(file.originalname).toLowerCase());
    const mimetype = allowedTypes.test(file.mimetype);
    
    if (mimetype && extname) {
      return cb(null, true);
    } else {
      cb(new Error('Only PDF, DOCX, JPG, JPEG, and PNG files are allowed'));
    }
  }
});

const { optionalAuth } = require('../middleware/authMiddleware');

// Authentication middleware that allows both authenticated users and guests
const authenticateUser = async (req, res, next) => {
  console.log('🔐 Starting authenticateUser middleware');
  
  try {
    // Use optional auth to handle both authenticated users and guests
    await optionalAuth(req, res, () => {
      // If no user is set (guest), create a guest user
      if (!req.user || !req.user.id) {
        const guestUser = {
          email: 'guest@immigrow.ai',
          fullName: 'Guest User'
        };
        
        // For guest users, we'll handle them differently in the routes
        req.user = {
          id: null,
          email: guestUser.email,
          fullName: guestUser.fullName,
          role: 'guest'
        };
      }
      
      console.log('🔐 User authenticated:', req.user.email, '(Role:', req.user.role + ')');
      next();
    });
  } catch (error) {
    console.error('❌ Authentication error:', error);
    res.status(500).json({ 
      success: false, 
      message: 'Authentication error: ' + error.message 
    });
  }
};

// Simplified role check - allow all users to access AI features
const checkImmigrantRole = async (req, res, next) => {
  console.log('👤 Starting simplified checkImmigrantRole middleware (allows all users)');
  console.log('👤 User object:', JSON.stringify(req.user, null, 2));
  
  try {
    console.log('✅ Allowing all users to access AI features');
    next();
  } catch (error) {
    console.error('❌ Role check error - FULL:', error);
    console.error('❌ Role check error stack:', error.stack);
    res.status(500).json({
      success: false,
      message: 'Internal server error during role verification'
    });
  }
};

// Resume upload and analysis route with Gemini Developer API
router.post('/resume/upload', 
  uploadRateLimit, 
  authenticateUser, 
  checkImmigrantRole, 
  checkDailyLimit,
  geminiRateLimit,
  upload.single('resume'), 
  async (req, res) => {
  try {
    if (!req.file) {
      return res.status(400).json({
        success: false,
        message: 'No file uploaded'
      });
    }

    console.log('📄 Processing resume upload for user:', req.user.id || 'guest');
    console.log('📁 File details:', {
      filename: req.file.filename,
      size: req.file.size,
      mimetype: req.file.mimetype
    });

    let analysis;
    const isPDF = req.file.originalname.toLowerCase().endsWith('.pdf');

    if (isPDF) {
      // Use direct PDF processing with Gemini (NEW FEATURE)
      console.log('🚀 Using direct PDF processing with Gemini Developer API...');
      analysis = await geminiService.analyzeResumePDF(req.file.path, req.file.originalname);
    } else {
      // Fallback to text extraction for non-PDF files
      console.log('📄 Processing non-PDF file with text extraction...');
      const documentData = await documentProcessor.processDocument(req.file.path, req.file.originalname);
      const extractedText = documentData.extractedText;
      
      if (!extractedText || extractedText.trim().length === 0) {
        return res.status(400).json({
          success: false,
          message: 'Could not extract text from the uploaded file'
        });
      }

      console.log('✅ Text extracted successfully, length:', extractedText.length);
      analysis = await geminiService.analyzeResumeText(extractedText, req.file.originalname);
    }
    
    console.log('🤖 Enhanced AI analysis completed with Canadian market insights');

    // Save enhanced analysis to AI database (only for authenticated users)
    let resumeAnalysis = null;
    if (req.user.id) {
      console.log('💾 Saving analysis to database for authenticated user:', req.user.id);
      
      try {
        resumeAnalysis = await supabaseDb.saveResumeAnalysis(req.user.id, {
          personalInfo: analysis.personalInfo,
          professionalSummary: analysis.professionalSummary,
          skills: analysis.skills,
          workExperience: analysis.workExperience,
          education: analysis.education,
          certifications: analysis.certifications,
          projects: analysis.projects,
          canadianMarketAnalysis: analysis.canadianMarketAnalysis,
          confidenceScores: analysis.confidenceScores,
          metadata: analysis.metadata,
          rawText: isPDF ? 'PDF processed directly' : analysis.rawText, // Will be mapped to extractedText in aiDatabase
          originalFileName: req.file.originalname,
          processingMethod: isPDF ? 'direct_pdf' : 'text_extraction'
        });

        console.log('✅ Enhanced analysis saved to database with ID:', resumeAnalysis.id);
      } catch (saveError) {
        console.error('❌ Failed to save analysis to database:', saveError);
        console.error('❌ Save error details:', {
          message: saveError.message,
          stack: saveError.stack
        });
        // Continue with response even if save fails
        resumeAnalysis = { id: 'save_failed', error: saveError.message };
      }
    } else {
      console.log('📝 Guest user - analysis not saved to database');
    }

    // Increment daily API usage count
    incrementDailyCount(req, res, () => {});

    // Clean up uploaded file
    fs.unlinkSync(req.file.path);

    // Get rate limit status
    const rateLimitStatus = geminiService.getRateLimitStatus();

    res.json({
      success: true,
      message: `Resume analyzed successfully using ${isPDF ? 'direct PDF processing' : 'text extraction'}`,
      data: {
        analysisId: resumeAnalysis?.id || null,
        analysis: {
          personalInfo: analysis.personalInfo,
          professionalSummary: analysis.professionalSummary,
          skills: analysis.skills,
          workExperience: analysis.workExperience,
          education: analysis.education,
          certifications: analysis.certifications,
          projects: analysis.projects,
          canadianMarketAnalysis: analysis.canadianMarketAnalysis,
          confidenceScores: analysis.confidenceScores,
          metadata: analysis.metadata
        },
        rateLimitStatus: rateLimitStatus,
        processingMethod: isPDF ? 'direct_pdf' : 'text_extraction',
        isGuest: !req.user.id
      }
    });

  } catch (error) {
    console.error('❌ Resume analysis error:', error);
    
    // Clean up uploaded file in case of error
    if (req.file && fs.existsSync(req.file.path)) {
      fs.unlinkSync(req.file.path);
    }
    
    // Provide specific error messages for different scenarios
    let errorMessage = 'Failed to analyze resume';
    let isRetryable = false;
    
    if (error.message.includes('Service Unavailable') || error.message.includes('overloaded')) {
      errorMessage = 'The AI service is temporarily overloaded. Please try again in a few minutes.';
      isRetryable = true;
    } else if (error.message.includes('Rate limit exceeded')) {
      errorMessage = 'Rate limit exceeded. Please wait a moment before trying again.';
      isRetryable = true;
    } else if (error.message.includes('Failed to parse AI response')) {
      errorMessage = 'The AI response could not be processed. Please try again.';
      isRetryable = true;
    }
    
    res.status(500).json({
      success: false,
      message: errorMessage,
      error: process.env.NODE_ENV === 'development' ? error.message : 'Internal server error',
      rateLimitStatus: geminiService.getRateLimitStatus(),
      isRetryable: isRetryable,
      retryAfter: isRetryable ? 30 : null // Suggest retry after 30 seconds
    });
  }
});

// Career profile generation route
router.post('/career-profile/generate', authenticateUser, checkImmigrantRole, async (req, res) => {
  try {
    const { resumeAnalysisId } = req.body;

    // Get user's latest resume analysis if no specific ID provided
    let resumeData;
    if (resumeAnalysisId) {
      const analyses = await supabaseDb.getUserResumeAnalyses(req.user.id);
      resumeData = analyses.find(a => a.id === resumeAnalysisId);
    } else {
      const analyses = await supabaseDb.getUserResumeAnalyses(req.user.id);
      resumeData = analyses[0]; // Get the most recent one
    }

    if (!resumeData) {
      return res.status(400).json({
        success: false,
        message: 'No resume analysis found. Please upload a resume first.'
      });
    }

    console.log('🎯 Generating career profile for user:', req.user.id);

    // Parse the stored JSON data
    const parsedPersonalInfo = JSON.parse(resumeData.personalInfo || '{}');
    const parsedSkills = JSON.parse(resumeData.skills || '[]');
    const parsedWorkExperience = JSON.parse(resumeData.workExperience || '[]');
    const parsedEducation = JSON.parse(resumeData.education || '[]');

    // Generate career profile with Google AI
    const careerProfile = await generateCareerProfileWithGemini({
      personalInfo: parsedPersonalInfo,
      skills: parsedSkills,
      workExperience: parsedWorkExperience,
      education: parsedEducation
    });

    console.log('🤖 Career profile generated successfully');

    // Save career profile to AI database
    const savedProfile = await supabaseDb.saveCareerProfile(req.user.id, careerProfile);

    console.log('💾 Career profile saved to database');

    res.json({
      success: true,
      message: 'Career profile generated successfully',
      data: {
        profileId: savedProfile.id,
        profile: careerProfile
      }
    });

  } catch (error) {
    console.error('❌ Career profile generation error:', error);
    res.status(500).json({
      success: false,
      message: 'Failed to generate career profile',
      error: process.env.NODE_ENV === 'development' ? error.message : 'Internal server error'
    });
  }
});

// NEW: Position recommendations route
router.post('/career-profile/position-recommendations', authenticateUser, checkImmigrantRole, async (req, res) => {
  try {
    const { resumeAnalysis } = req.body;

    if (!resumeAnalysis) {
      return res.status(400).json({
        success: false,
        message: 'Resume analysis data is required'
      });
    }

    console.log('🎯 Generating position recommendations for user:', req.user.id);

    // Generate position recommendations using Gemini AI
    const positionRecommendations = await generatePositionRecommendationsWithGemini(resumeAnalysis);

    console.log('🤖 Position recommendations generated successfully');

    res.json({
      success: true,
      message: 'Position recommendations generated successfully',
      data: {
        positions: positionRecommendations,
        analysisId: resumeAnalysis.analysisId || Date.now().toString()
      }
    });

  } catch (error) {
    console.error('❌ Position recommendations error:', error);
    res.status(500).json({
      success: false,
      message: 'Failed to generate position recommendations',
      error: process.env.NODE_ENV === 'development' ? error.message : 'Internal server error'
    });
  }
});

// NEW: Enhanced profile generation route - Simplified and More Reliable
router.post('/career-profile/enhanced-profile', authenticateUser, checkImmigrantRole, async (req, res) => {
  console.log('🚀 Starting enhanced-profile route');
  console.log('📊 Request method:', req.method);
  console.log('📊 Request URL:', req.url);
  console.log('📊 Request headers:', JSON.stringify(req.headers, null, 2));
  console.log('📊 Request body keys:', Object.keys(req.body || {}));
  console.log('📊 Full request body:', JSON.stringify(req.body, null, 2));
  
  try {
    console.log('✅ Inside try block');
    
    const { targetPosition, resumeAnalysis } = req.body;
    console.log('📋 Extracted targetPosition:', JSON.stringify(targetPosition, null, 2));
    console.log('📋 Extracted resumeAnalysis keys:', Object.keys(resumeAnalysis || {}));

    if (!targetPosition || !resumeAnalysis) {
      console.log('❌ Missing required fields - targetPosition:', !!targetPosition, 'resumeAnalysis:', !!resumeAnalysis);
      return res.status(400).json({
        success: false,
        message: 'Target position and resume analysis are required'
      });
    }

    console.log('🎯 Generating enhanced profile for user:', req.user?.id);
    console.log('🎯 User object:', JSON.stringify(req.user, null, 2));
    console.log('🎯 Target position:', JSON.stringify(targetPosition, null, 2));

    // Safe JSON parsing helper function
    const safeJsonParse = (jsonString, fallback = []) => {
      try {
        if (typeof jsonString === 'string') {
          const parsed = JSON.parse(jsonString);
          return Array.isArray(parsed) ? parsed : fallback;
        }
        return Array.isArray(jsonString) ? jsonString : fallback;
      } catch (error) {
        console.warn('🔶 JSON parsing failed:', error.message, 'for:', jsonString?.substring(0, 100));
        return fallback;
      }
    };

    // Parse JSON fields that might be stored as strings
    const workExperience = safeJsonParse(resumeAnalysis.workExperience, []);
    const projects = safeJsonParse(resumeAnalysis.projects, []);
    const skills = typeof resumeAnalysis.skills === 'string' ? JSON.parse(resumeAnalysis.skills || '{}') : (resumeAnalysis.skills || {});
    const education = safeJsonParse(resumeAnalysis.education, []);

    console.log('📊 Parsed data structures:');
    console.log('  - workExperience array length:', workExperience.length);
    console.log('  - projects array length:', projects.length);
    console.log('  - skills type:', typeof skills, 'keys:', Object.keys(skills));
    console.log('  - education array length:', education.length);

    // Create a simplified enhanced profile using the available data
    const enhancedProfile = {
      optimized_profile: {
        professional_title: `${targetPosition.title || 'Professional'} - Canadian Market Ready`,
        elevator_pitch: `Experienced ${targetPosition.title || 'professional'} with proven skills in ${resumeAnalysis.canadianMarketAnalysis?.strengthsForCanadianMarket?.slice(0, 3).join(', ') || 'key technologies'}, seeking opportunities in the Canadian market.`,
        value_proposition: `Brings international experience and ${targetPosition.industry || 'industry'} expertise to Canadian organizations.`,
        key_achievements: workExperience?.slice(0, 3).map(exp => 
          `${exp.achievements?.[0] || `Successful experience at ${exp.company}`}`) || []
      },
      skills_positioning: {
        primary_skills: skills?.technical?.slice(0, 5).map(skill => ({
          skill: skill,
          relevance_to_role: `Essential for ${targetPosition.title || 'this role'}`,
          evidence: "Demonstrated through work experience",
          positioning_statement: `Strong proficiency in ${skill}`
        })) || [],
        skill_development_plan: resumeAnalysis.canadianMarketAnalysis?.recommendedImprovements?.slice(0, 3).map(improvement => ({
          skill: improvement,
          importance: "High",
          learning_path: "Online courses and practical application",
          timeline: "3-6 months",
          resources: ["Online platforms", "Professional development courses"]
        })) || []
      },
      experience_repositioning: {
        relevant_experience: workExperience?.slice(0, 2).map(exp => ({
          original_role: exp.position || 'Previous Role',
          repositioned_as: `${exp.position || 'Professional'} with Canadian Market Focus`,
          key_transferable_elements: exp.responsibilities?.slice(0, 3) || [],
          success_metrics: exp.achievements || [],
          canadian_context: "Experience adapted for Canadian workplace standards"
        })) || [],
        project_highlights: projects?.slice(0, 2).map(project => ({
          project: project.name || 'Professional Project',
          relevance: `Directly applicable to ${targetPosition.title || 'target role'}`,
          technologies_used: project.technologies || [],
          impact: project.description || 'Significant professional impact',
          presentation_tip: "Emphasize problem-solving and results achieved"
        })) || []
      },
      application_strategy: {
        resume_optimization: {
          key_changes: [
            "Highlight Canadian market-relevant skills",
            "Emphasize transferable experience",
            "Include keywords specific to Canadian job market"
          ],
          keywords_to_include: skills?.technical?.slice(0, 8) || [],
          sections_to_emphasize: ["Professional Experience", "Skills", "Education"],
          formatting_tips: ["Use Canadian resume format", "Include relevant certifications"]
        },
        cover_letter_strategy: {
          opening_approach: `Express enthusiasm for ${targetPosition.title || 'the role'} opportunities in Canada`,
          key_points_to_address: [
            "International experience value",
            "Commitment to Canadian market",
            "Relevant technical skills"
          ],
          company_research_areas: ["Company culture", "Recent projects", "Market position"],
          closing_strategy: "Express eagerness for interview and integration"
        },
        networking_approach: {
          target_professionals: [`${targetPosition.title || 'Industry'} professionals in Canada`, "Recent immigrants in similar roles"],
          conversation_starters: ["Industry trends discussion", "Canadian market insights"],
          value_you_bring: ["International perspective", "Technical expertise"],
          follow_up_strategies: ["LinkedIn connections", "Industry event participation"]
        }
      },
      interview_preparation: {
        common_questions: [
          {
            question: `Why are you interested in ${targetPosition.title || 'this position'} in Canada?`,
            strategy: "Connect personal goals with Canadian opportunities",
            key_points: ["Career growth", "Market innovation", "Cultural fit"],
            example_answer_structure: "Personal motivation + Professional goals + Cultural alignment"
          }
        ],
        behavioral_examples: workExperience?.slice(0, 2).map(exp => ({
          situation: `Professional challenge at ${exp.company || 'previous role'}`,
          task: "Problem-solving requirement",
          action: "Strategic approach taken",
          result: "Positive outcome achieved",
          relevance: `Demonstrates skills for ${targetPosition.title || 'target role'}`
        })) || [],
        technical_preparation: {
          skills_to_demonstrate: skills?.technical?.slice(0, 5) || [],
          portfolio_items: ["Relevant project examples", "Technical achievements"],
          coding_challenges: ["Industry-specific problems", "Canadian market scenarios"],
          system_design_topics: ["Scalability", "Best practices", "Industry standards"]
        },
        cultural_fit_preparation: {
          company_culture_research: ["Values alignment", "Team dynamics", "Work environment"],
          canadian_workplace_norms: ["Communication style", "Collaboration approach", "Professional etiquette"],
          questions_to_ask: ["Team structure", "Growth opportunities", "Company vision"]
        }
      },
      "90_day_action_plan": {
        week_1_2: [
          "Research Canadian market trends",
          "Update resume with Canadian format",
          "Identify key networking opportunities"
        ],
        month_1: [
          "Apply to relevant positions",
          "Attend industry networking events",
          "Complete relevant online courses"
        ],
        month_2: [
          "Follow up on applications",
          "Expand professional network",
          "Gain Canadian work experience"
        ],
        month_3: [
          "Evaluate progress and opportunities",
          "Adjust strategy based on feedback",
          "Secure position or continue optimization"
        ],
        success_metrics: [
          "Number of applications submitted",
          "Networking connections made",
          "Interview opportunities secured"
        ]
      }
    };

    console.log('🤖 Enhanced profile generated successfully');
    console.log('📏 Enhanced profile size:', JSON.stringify(enhancedProfile).length, 'characters');

    // Save enhanced profile to AI database
    console.log('💾 Attempting to save enhanced profile to database...');
    console.log('💾 Save parameters - userId:', req.user?.id, 'hasTargetPosition:', !!targetPosition, 'hasEnhancedProfile:', !!enhancedProfile);
    
    try {
      console.log('💾 Before saveEnhancedCareerProfile call');
      const savedProfile = await supabaseDb.saveEnhancedCareerProfile(req.user.id, {
        targetPosition,
        enhancedProfile,
        resumeAnalysisId: resumeAnalysis.analysisId
      });
      console.log('💾 Enhanced profile saved to database successfully:', savedProfile);
    } catch (saveError) {
      console.error('⚠️ Warning: Could not save to database - Full Error:', saveError);
      console.error('⚠️ Error message:', saveError.message);
      console.error('⚠️ Error stack:', saveError.stack);
      // Continue with response even if save fails
    }

    console.log('📤 Preparing response...');
    console.log('📤 Response data size:', JSON.stringify({ enhancedProfile, targetPosition }).length, 'characters');
    
    res.json({
      success: true,
      message: 'Enhanced career profile generated successfully',
      data: {
        enhancedProfile,
        targetPosition
      }
    });
    
    console.log('✅ Response sent successfully');

  } catch (error) {
    console.error('❌ Enhanced profile generation error - FULL ERROR:', error);
    console.error('❌ Error name:', error.name);
    console.error('❌ Error message:', error.message);
    console.error('❌ Error stack:', error.stack);
    console.error('❌ Error properties:', Object.keys(error));
    
    res.status(500).json({
      success: false,
      message: 'Failed to generate enhanced profile',
      error: process.env.NODE_ENV === 'development' ? error.message : 'Internal server error'
    });
    
    console.log('❌ Error response sent');
  }
});

// Get user's resume analyses
router.get('/resume/analyses', authenticateUser, checkImmigrantRole, async (req, res) => {
  try {
    console.log('🔍 Fetching resume analyses for user:', req.user.id || 'guest');
    
    // For guest users, return empty array
    if (!req.user.id) {
      console.log('👤 Guest user - returning empty analyses array');
      return res.json({
        success: true,
        data: [],
        message: 'Guest users cannot access saved analyses. Please log in to save and view your analyses.'
      });
    }

    console.log('🔍 Fetching analyses from database for user ID:', req.user.id);
    const analyses = await supabaseDb.getUserResumeAnalyses(req.user.id);
    
    console.log('✅ Retrieved', analyses.length, 'analyses from database');
    
    // Parse JSON strings back to objects for response
    const formattedAnalyses = analyses.map(analysis => {
      try {
        return {
          ...analysis,
          personalInfo: JSON.parse(analysis.personal_info || '{}'),
          skills: JSON.parse(analysis.skills || '[]'),
          workExperience: JSON.parse(analysis.work_experience || '[]'),
          education: JSON.parse(analysis.education || '[]'),
          canadianMarketAnalysis: JSON.parse(analysis.canadian_market_analysis || '{}'),
          confidenceScores: JSON.parse(analysis.confidence_scores || '{}'),
          metadata: JSON.parse(analysis.metadata || '{}'),
          // Map database fields to frontend expected fields
          originalFileName: analysis.original_file_name,
          createdAt: analysis.created_at,
          id: analysis.id
        };
      } catch (parseError) {
        console.error('❌ Error parsing analysis data:', parseError);
        return analysis; // Return raw data if parsing fails
      }
    });

    console.log('✅ Returning', formattedAnalyses.length, 'formatted analyses');

    res.json({
      success: true,
      data: formattedAnalyses
    });
  } catch (error) {
    console.error('❌ Error fetching resume analyses:', error);
    console.error('❌ Error stack:', error.stack);
    res.status(500).json({
      success: false,
      message: 'Failed to fetch resume analyses',
      error: process.env.NODE_ENV === 'development' ? error.message : 'Internal server error'
    });
  }
});

// Get user's career profile
router.get('/career-profile', authenticateUser, checkImmigrantRole, async (req, res) => {
  try {
    const profile = await supabaseDb.getUserCareerProfile(req.user.id);
    
    if (!profile) {
      return res.status(404).json({
        success: false,
        message: 'No career profile found'
      });
    }

    // Parse JSON strings back to objects for response
    const formattedProfile = {
      ...profile,
      skills: JSON.parse(profile.skills || '[]'),
      targetIndustries: JSON.parse(profile.targetIndustries || '[]')
    };

    res.json({
      success: true,
      data: formattedProfile
    });
  } catch (error) {
    console.error('❌ Error fetching career profile:', error);
    res.status(500).json({
      success: false,
      message: 'Failed to fetch career profile'
    });
  }
});

// Get API rate limit status
router.get('/rate-limit-status', authenticateUser, (req, res) => {
  try {
    const rateLimitStatus = geminiService.getRateLimitStatus();
    
    res.json({
      success: true,
      data: {
        rateLimits: rateLimitStatus,
        apiInfo: {
          provider: 'Gemini Developer API',
          model: 'gemini-1.5-flash',
          features: [
            'Direct PDF processing',
            '1000 requests/minute',
            '50,000 requests/day',
            'Canadian job market analysis',
            'Enhanced confidence scoring'
          ]
        },
        improvements: {
          rateLimitIncrease: '67x faster (1000 vs 15 req/min)',
          directPdfSupport: true,
          fileSizeLimit: '10MB (vs 5MB)',
          canadianMarketFocus: true
        }
      }
    });
  } catch (error) {
    res.status(500).json({
      success: false,
      message: 'Failed to get rate limit status',
      error: error.message
    });
  }
});

// NEW: API status and health check endpoint
router.get('/status', authenticateUser, async (req, res) => {
  try {
    const rateLimitStatus = geminiService.getRateLimitStatus();
    
    // Check if we can connect to Gemini API
    let apiStatus = 'unknown';
    let lastError = null;
    
    try {
      // Try a simple test request
      const testResult = await geminiService.model.generateContent('Hello');
      const response = await testResult.response;
      apiStatus = 'operational';
    } catch (apiError) {
      if (apiError.status === 503 || apiError.message.includes('overloaded')) {
        apiStatus = 'overloaded';
        lastError = 'Service temporarily overloaded';
      } else {
        apiStatus = 'error';
        lastError = apiError.message;
      }
    }
    
    res.json({
      success: true,
      data: {
        apiStatus: {
          status: apiStatus,
          lastError: lastError,
          timestamp: new Date().toISOString()
        },
        rateLimits: rateLimitStatus,
        features: {
          retryMechanism: true,
          fallbackProcessing: true,
          exponentialBackoff: true,
          maxRetries: 3
        },
        recommendations: {
          ifOverloaded: 'Wait 1-2 minutes before retrying',
          ifRateLimited: 'Wait for rate limit reset',
          bestPractices: [
            'Upload files during off-peak hours',
            'Use PDF format for best results',
            'Keep file size under 10MB'
          ]
        }
      }
    });
  } catch (error) {
    res.status(500).json({
      success: false,
      message: 'Failed to get API status',
      error: error.message
    });
  }
});

// Debug endpoint to check authentication and user status
router.get('/debug-auth', authenticateUser, checkImmigrantRole, async (req, res) => {
  try {
    console.log('🔍 Debug auth request received');
    console.log('👤 User object:', JSON.stringify(req.user, null, 2));
    
    // Get user from database to verify ID mapping
    let dbUser = null;
    try {
      dbUser = await supabaseDb.findOrCreateUser({
        email: req.user.email,
        fullName: req.user.fullName || 'User'
      });
    } catch (dbError) {
      console.error('❌ Database user lookup failed:', dbError);
    }
    
    res.json({
      success: true,
      data: {
        requestUser: req.user,
        databaseUser: dbUser ? {
          id: dbUser.id,
          email: dbUser.email,
          fullName: dbUser.full_name
        } : null,
        authenticationStatus: {
          isAuthenticated: !!req.user.id,
          isGuest: !req.user.id,
          userIdType: typeof req.user.id,
          userIdValue: req.user.id
        },
        databaseStatus: {
          userFound: !!dbUser,
          userIdMatch: req.user.id === dbUser?.id,
          databaseUserId: dbUser?.id
        }
      }
    });
  } catch (error) {
    console.error('❌ Debug auth error:', error);
    res.status(500).json({
      success: false,
      message: 'Debug endpoint error',
      error: error.message
    });
  }
});

// Health check endpoint
router.get('/health', (req, res) => {
  res.json({
    success: true,
    message: 'AI Routes (Local) are working!',
    database: 'Supabase',
    timestamp: new Date().toISOString(),
    apiProvider: 'Gemini Developer API',
    improvements: '67x faster rate limits, direct PDF processing'
  });
});

module.exports = router;
````

## File: src/routes/ApiRouter.js
````javascript
const express = require('express');
const { logger } = require('../config/logger');
const { 
  apiVersioningMiddleware, 
  isVersionSupported,
  getApiVersionConfig,
  isFeatureAvailable,
  getApiVersioningInfo
} = require('../config/apiVersioning');
const RouteFactory = require('./RouteFactory');

/**
 * Version-aware API Router
 * Handles dynamic routing based on API version
 */
class ApiRouter {
  constructor() {
    this.router = express.Router();
    this.initialized = false;
    this.versionRoutes = new Map();
  }

  /**
   * Initialize the API router
   */
  async initialize() {
    if (this.initialized) {
      return;
    }

    try {
      await RouteFactory.initialize();
      await this.setupVersionRoutes();
      this.initialized = true;
    } catch (error) {
      throw new Error(`Failed to initialize ApiRouter: ${error.message}`);
    }
  }

  /**
   * Setup routes for all supported versions
   */
  async setupVersionRoutes() {
    const versioningInfo = getApiVersioningInfo();
    
    for (const version of versioningInfo.currentVersions) {
      try {
        const routes = await RouteFactory.createVersionRoutes(version);
        this.versionRoutes.set(version, routes);
        
        logger.info(`Setup routes for API version ${version}`, {
          version,
          availableRoutes: Object.keys(routes)
        });
      } catch (error) {
        logger.error(`Failed to setup routes for version ${version}`, {
          version,
          error: error.message
        });
      }
    }
  }

  /**
   * Create the main API router with version handling
   * @returns {Object} Express router
   */
  createRouter() {
    // Apply API versioning middleware
    this.router.use(apiVersioningMiddleware({
      strict: false,
      logVersionUsage: true
    }));

    // API versioning information endpoint
    this.router.get('/versions', (req, res) => {
      const versioningInfo = getApiVersioningInfo();
      res.json({
        success: true,
        data: versioningInfo,
        timestamp: new Date().toISOString()
      });
    });

    // Health check endpoint
    this.router.get('/health', async (req, res) => {
      try {
        const health = {
          status: 'healthy',
          timestamp: new Date().toISOString(),
          version: req.apiVersion,
          versionInfo: req.apiVersionInfo,
          services: {
            database: 'connected',
            controllers: 'initialized',
            routes: 'ready'
          }
        };

        res.json(health);
      } catch (error) {
        logger.error('Health check failed', error);
        res.status(503).json({
          status: 'unhealthy',
          error: error.message,
          timestamp: new Date().toISOString()
        });
      }
    });

    // Dynamic version routing
    this.router.use('/:version/*', async (req, res, next) => {
      const requestedVersion = req.params.version;
      
      // Create a copy of the URL for route matching without modifying the original
      const pathWithoutVersion = req.url.replace(`/${requestedVersion}`, '');
      
      // Validate version
      if (!isVersionSupported(requestedVersion)) {
        return res.status(400).json({
          error: 'Unsupported API Version',
          message: `API version '${requestedVersion}' is not supported`,
          supportedVersions: getApiVersioningInfo().currentVersions,
          recommendedVersion: getApiVersioningInfo().defaultVersion
        });
      }

      // Get routes for the requested version
      const versionRoutes = this.versionRoutes.get(requestedVersion);
      if (!versionRoutes) {
        return res.status(500).json({
          error: 'Version Routes Not Available',
          message: `Routes for version '${requestedVersion}' are not available`
        });
      }

      // Route to appropriate version-specific routes
      await this.routeToVersion(req, res, next, requestedVersion, versionRoutes, pathWithoutVersion);
    });

    // Default version routing (when no version specified)
    this.router.use('/*', async (req, res, next) => {
      const defaultVersion = getApiVersioningInfo().defaultVersion;
      const versionRoutes = this.versionRoutes.get(defaultVersion);
      
      if (!versionRoutes) {
        return res.status(500).json({
          error: 'Default Version Routes Not Available',
          message: `Routes for default version '${defaultVersion}' are not available`
        });
      }

      // Route to default version
      await this.routeToVersion(req, res, next, defaultVersion, versionRoutes, req.path);
    });

    return this.router;
  }

  /**
   * Route request to specific version
   * @param {Object} req - Express request
   * @param {Object} res - Express response
   * @param {Function} next - Express next function
   * @param {string} version - API version
   * @param {Object} versionRoutes - Routes for the version
   * @param {string} pathWithoutVersion - Request path without version prefix
   */
  async routeToVersion(req, res, next, version, versionRoutes, pathWithoutVersion) {
    const path = pathWithoutVersion || req.path;
    const method = req.method.toLowerCase();

    // Determine which route group to use based on path
    let routeGroup = null;
    let routePath = path;

    if (path.startsWith('/users') || path.startsWith('/user')) {
      routeGroup = 'userRoutes';
      routePath = path.replace(/^\/users?/, '');
    } else if (path.startsWith('/resumes') || path.startsWith('/resume')) {
      routeGroup = 'resumeRoutes';
      routePath = path.replace(/^\/resumes?/, '');
    } else if (path.startsWith('/career') || path.startsWith('/careers')) {
      routeGroup = 'careerRoutes';
      routePath = path.replace(/^\/careers?/, '');
    } else if (path.startsWith('/analytics')) {
      routeGroup = 'analyticsRoutes';
      routePath = path.replace(/^\/analytics/, '');
    } else if (path.startsWith('/notifications') || path.startsWith('/notification')) {
      routeGroup = 'notificationRoutes';
      routePath = path.replace(/^\/notifications?/, '');
    }

    // Check if route group exists and feature is available
    if (routeGroup && versionRoutes[routeGroup]) {
      const feature = this.getFeatureForRouteGroup(routeGroup);
      
      if (feature && !isFeatureAvailable(version, feature)) {
        return res.status(404).json({
          error: 'Feature Not Available',
          message: `Feature '${feature}' is not available in API version '${version}'`,
          availableFeatures: getApiVersionConfig(version).features,
          recommendedVersion: getApiVersioningInfo().defaultVersion
        });
      }

      // Use the version-specific route
      return versionRoutes[routeGroup](req, res, next);
    }

    // If no specific route group found, try to match any route
    for (const [groupName, router] of Object.entries(versionRoutes)) {
      try {
        // Check if the router can handle this request
        const canHandle = this.canRouterHandleRequest(router, path, method);
        if (canHandle) {
          return router(req, res, next);
        }
      } catch (error) {
        logger.warn(`Error checking route group ${groupName}`, {
          error: error.message,
          path,
          method,
          version
        });
      }
    }

    // No matching route found
    return res.status(404).json({
      error: 'Route Not Found',
      message: `Route '${path}' not found in API version '${version}'`,
      version,
      availableRoutes: Object.keys(versionRoutes),
      supportedVersions: getApiVersioningInfo().currentVersions
    });
  }

  /**
   * Get feature name for route group
   * @param {string} routeGroup - Route group name
   * @returns {string} Feature name
   */
  getFeatureForRouteGroup(routeGroup) {
    const featureMap = {
      userRoutes: 'user-management',
      resumeRoutes: 'resume-analysis',
      careerRoutes: 'career-profiles',
      analyticsRoutes: 'analytics',
      notificationRoutes: 'real-time-notifications'
    };
    
    return featureMap[routeGroup];
  }

  /**
   * Check if router can handle the request
   * @param {Object} router - Express router
   * @param {string} path - Request path
   * @param {string} method - Request method
   * @returns {boolean} Whether router can handle request
   */
  canRouterHandleRequest(router, path, method) {
    if (!router || !router.stack) return false;
    
    return router.stack.some(layer => {
      if (!layer.route) return false;
      
      const routePath = layer.route.path;
      const routeMethods = Object.keys(layer.route.methods);
      
      // Check if path matches (with parameter support)
      const pathMatches = this.pathMatches(routePath, path);
      const methodMatches = routeMethods.includes(method);
      
      return pathMatches && methodMatches;
    });
  }

  /**
   * Check if route path matches request path
   * @param {string} routePath - Route path pattern
   * @param {string} requestPath - Request path
   * @returns {boolean} Whether paths match
   */
  pathMatches(routePath, requestPath) {
    // Simple path matching - can be enhanced with regex
    if (routePath === requestPath) return true;
    
    // Handle parameterized routes
    const routeSegments = routePath.split('/').filter(Boolean);
    const requestSegments = requestPath.split('/').filter(Boolean);
    
    if (routeSegments.length !== requestSegments.length) return false;
    
    return routeSegments.every((segment, index) => {
      return segment.startsWith(':') || segment === requestSegments[index];
    });
  }

  /**
   * Get route information for documentation
   * @param {string} version - API version
   * @returns {Object} Route information
   */
  async getRouteInfo(version) {
    return await RouteFactory.getRouteInfo(version);
  }

  /**
   * Get all available routes for a version
   * @param {string} version - API version
   * @returns {Array} Available routes
   */
  async getAvailableRoutes(version) {
    return await RouteFactory.getAvailableRoutes(version);
  }

  /**
   * Check if route is available in version
   * @param {string} version - API version
   * @param {string} routeName - Route name
   * @returns {boolean} Whether route is available
   */
  async isRouteAvailable(version, routeName) {
    return await RouteFactory.isRouteAvailable(version, routeName);
  }
}

// Create singleton instance
const apiRouter = new ApiRouter();

module.exports = apiRouter;
````

## File: src/routes/authRoutes.js
````javascript
const express = require('express');
const { createClient } = require('@supabase/supabase-js');
const { verifyToken } = require('../middleware/authMiddleware');
const SupabaseDatabase = require('../services/supabaseDatabase');

const router = express.Router();
const supabaseDb = new SupabaseDatabase();

// Create Supabase client for auth operations
const supabase = createClient(
  process.env.SUPABASE_URL,
  process.env.SUPABASE_ANON_KEY
);

// User registration
router.post('/register', async (req, res) => {
  try {
    const { email, password, fullName, phoneNo, statusInCanada, countryOfOrigin, currentLocation } = req.body;

    if (!email || !password || !fullName) {
      return res.status(400).json({
        success: false,
        message: 'Email, password, and full name are required'
      });
    }

    console.log('🔐 Starting user registration for:', email);

    // Create user in Supabase Auth
    const { data: authData, error: authError } = await supabase.auth.signUp({
      email,
      password,
      options: {
        data: {
          full_name: fullName,
          phone_no: phoneNo,
          status_in_canada: statusInCanada,
          country_of_origin: countryOfOrigin,
          current_location: currentLocation
        }
      }
    });

    if (authError) {
      console.error('❌ Auth registration error:', authError);
      return res.status(400).json({
        success: false,
        message: authError.message
      });
    }

    if (!authData.user) {
      return res.status(400).json({
        success: false,
        message: 'Failed to create user account'
      });
    }

    // Create user profile in our database
    const userProfile = {
      email: authData.user.email,
      fullName: fullName,
      phoneNo,
      statusInCanada,
      countryOfOrigin,
      currentLocation
    };

    const user = await supabaseDb.findOrCreateUser(userProfile);

    console.log('✅ User registered successfully:', user.email);

    res.status(201).json({
      success: true,
      message: 'User registered successfully',
      user: {
        id: user.id,
        email: user.email,
        fullName: user.full_name
      },
      session: authData.session
    });

  } catch (error) {
    console.error('❌ Registration error:', error);
    res.status(500).json({
      success: false,
      message: 'Registration failed: ' + error.message
    });
  }
});

// User login
router.post('/login', async (req, res) => {
  try {
    const { email, password } = req.body;

    if (!email || !password) {
      return res.status(400).json({
        success: false,
        message: 'Email and password are required'
      });
    }

    console.log('🔐 Starting user login for:', email);

    // Sign in with Supabase Auth
    const { data: authData, error: authError } = await supabase.auth.signInWithPassword({
      email,
      password
    });

    if (authError) {
      console.error('❌ Auth login error:', authError);
      return res.status(401).json({
        success: false,
        message: 'Invalid email or password'
      });
    }

    if (!authData.user) {
      return res.status(401).json({
        success: false,
        message: 'Login failed'
      });
    }

    // Get user profile from our database
    const user = await supabaseDb.findOrCreateUser({
      email: authData.user.email,
      fullName: authData.user.user_metadata?.full_name || 'User'
    });

    console.log('✅ User logged in successfully:', user.email);

    res.json({
      success: true,
      message: 'Login successful',
      user: {
        id: user.id,
        email: user.email,
        fullName: user.full_name
      },
      session: authData.session
    });

  } catch (error) {
    console.error('❌ Login error:', error);
    res.status(500).json({
      success: false,
      message: 'Login failed: ' + error.message
    });
  }
});

// User logout
router.post('/logout', verifyToken, async (req, res) => {
  try {
    const authHeader = req.headers.authorization;
    const token = authHeader.substring(7);

    // Sign out from Supabase Auth
    const { error } = await supabase.auth.signOut();

    if (error) {
      console.error('❌ Logout error:', error);
      return res.status(500).json({
        success: false,
        message: 'Logout failed'
      });
    }

    console.log('✅ User logged out successfully:', req.user.email);

    res.json({
      success: true,
      message: 'Logout successful'
    });

  } catch (error) {
    console.error('❌ Logout error:', error);
    res.status(500).json({
      success: false,
      message: 'Logout failed: ' + error.message
    });
  }
});

// Get current user profile
router.get('/profile', verifyToken, async (req, res) => {
  try {
    const user = await supabaseDb.findOrCreateUser({
      email: req.user.email,
      fullName: req.user.fullName || 'User'
    });

    res.json({
      success: true,
      user: {
        id: user.id,
        email: user.email,
        fullName: user.full_name,
        phoneNo: user.phone_no,
        statusInCanada: user.status_in_canada,
        countryOfOrigin: user.country_of_origin,
        currentLocation: user.current_location,
        roleId: user.role_id,
        createdAt: user.created_at
      }
    });

  } catch (error) {
    console.error('❌ Get profile error:', error);
    res.status(500).json({
      success: false,
      message: 'Failed to get user profile: ' + error.message
    });
  }
});

// Update user profile
router.put('/profile', verifyToken, async (req, res) => {
  try {
    const { fullName, phoneNo, statusInCanada, countryOfOrigin, currentLocation } = req.body;

    const updatedUser = await supabaseDb.updateUser(req.user.id, {
      fullName,
      phoneNo,
      statusInCanada,
      countryOfOrigin,
      currentLocation
    });

    res.json({
      success: true,
      message: 'Profile updated successfully',
      user: {
        id: updatedUser.id,
        email: updatedUser.email,
        fullName: updatedUser.full_name,
        phoneNo: updatedUser.phone_no,
        statusInCanada: updatedUser.status_in_canada,
        countryOfOrigin: updatedUser.country_of_origin,
        currentLocation: updatedUser.current_location
      }
    });

  } catch (error) {
    console.error('❌ Update profile error:', error);
    res.status(500).json({
      success: false,
      message: 'Failed to update profile: ' + error.message
    });
  }
});

// Refresh token
router.post('/refresh', async (req, res) => {
  try {
    const { refresh_token } = req.body;

    if (!refresh_token) {
      return res.status(400).json({
        success: false,
        message: 'Refresh token is required'
      });
    }

    const { data, error } = await supabase.auth.refreshSession({
      refresh_token
    });

    if (error) {
      console.error('❌ Token refresh error:', error);
      return res.status(401).json({
        success: false,
        message: 'Invalid refresh token'
      });
    }

    res.json({
      success: true,
      session: data.session
    });

  } catch (error) {
    console.error('❌ Refresh token error:', error);
    res.status(500).json({
      success: false,
      message: 'Token refresh failed: ' + error.message
    });
  }
});

module.exports = router;
````

## File: src/routes/careerRoutes.js
````javascript
const express = require('express');
const router = express.Router();
const multer = require('multer');
const path = require('path');
const CareerProfileService = require('../services/CareerProfileService');
const SupabaseDatabase = require('../services/supabaseDatabase');
const { verifyToken } = require('../middleware/authMiddleware');
const GoogleJobsService = require('../services/GoogleJobsService');

const supabaseDb = new SupabaseDatabase();
const careerService = new CareerProfileService();

// Configure multer for resume uploads
const storage = multer.diskStorage({
  destination: (req, file, cb) => {
    cb(null, './uploads/resumes/');
  },
  filename: (req, file, cb) => {
    const uniqueSuffix = Date.now() + '-' + Math.round(Math.random() * 1E9);
    cb(null, `resume-${uniqueSuffix}${path.extname(file.originalname)}`);
  }
});

const upload = multer({
  storage: storage,
  limits: { fileSize: 5 * 1024 * 1024 }, // 5MB limit
  fileFilter: (req, file, cb) => {
    const allowedTypes = ['.pdf', '.doc', '.docx'];
    const ext = path.extname(file.originalname).toLowerCase();
    if (allowedTypes.includes(ext)) {
      cb(null, true);
    } else {
      cb(new Error('Only PDF, DOC, and DOCX files are allowed'));
    }
  }
});

/**
 * POST /api/career/analyze-resume
 * Analyze resume and generate position recommendations
 */
router.post('/analyze-resume', verifyToken, upload.single('resume'), async (req, res) => {
  try {
    const userId = req.user.id;
    const file = req.file;
    
    if (!file) {
      return res.status(400).json({
        success: false,
        error: 'Resume file is required'
      });
    }

    console.log(`📄 Processing resume for user: ${userId}`);

    // Analyze resume
    const resumeAnalysis = await careerService.analyzeResumePDF(file.path, file.originalname);
    
    // Save resume analysis to database
    const savedAnalysis = await supabaseDb.createResumeAnalysis({
      userId: parseInt(userId),
      originalFileName: file.originalname,
      structuredData: resumeAnalysis,
      personalInfo: resumeAnalysis.personalInfo,
      professionalSummary: resumeAnalysis.professionalSummary?.summary,
      skills: resumeAnalysis.skills,
      workExperience: resumeAnalysis.workExperience,
      education: resumeAnalysis.education,
      certifications: resumeAnalysis.certifications,
      projects: resumeAnalysis.projects,
      canadianMarketAnalysis: resumeAnalysis.canadianMarketAnalysis,
      confidenceScores: resumeAnalysis.confidenceScores,
      metadata: resumeAnalysis.metadata,
      processingMethod: 'direct_pdf'
    });

    // Get existing career profile if available
    const existingProfile = await supabaseDb.getUserCareerProfile(parseInt(userId));

    // Generate position recommendations
    const recommendations = await careerService.generatePositionRecommendations(
      resumeAnalysis, 
      existingProfile || {}
    );

    // Save job matches
    if (recommendations.positions && recommendations.positions.length > 0) {
      await careerService.saveJobMatches(parseInt(userId), recommendations.positions);
    }

    res.json({
      success: true,
      data: {
        analysisId: savedAnalysis.id,
        resumeAnalysis,
        positionRecommendations: recommendations,
        rateLimitStatus: careerService.getRateLimitStatus()
      }
    });

  } catch (error) {
    console.error('❌ Resume analysis error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Resume analysis failed'
    });
  }
});

/**
 * POST /api/career/enhanced-profile
 * Generate enhanced profile for a specific position
 */
router.post('/enhanced-profile', verifyToken, async (req, res) => {
  try {
    const userId = req.user.id;
    const { targetPosition, resumeAnalysisId, userPreferences } = req.body;

    if (!targetPosition || !resumeAnalysisId) {
      return res.status(400).json({
        success: false,
        error: 'Target position and resume analysis ID are required'
      });
    }

    console.log(`🚀 Generating enhanced profile for user: ${userId}`);

    // Get resume analysis
    const resumeAnalysis = await supabaseDb.getResumeAnalysisById(resumeAnalysisId);

    if (!resumeAnalysis) {
      return res.status(404).json({
        success: false,
        error: 'Resume analysis not found'
      });
    }

    // Generate enhanced profile
    const enhancedProfile = await careerService.generateEnhancedProfile(
      resumeAnalysis.structuredData,
      targetPosition,
      userPreferences || {}
    );

    // Generate skill gap analysis
    const skillGapAnalysis = await careerService.generateSkillGapAnalysis(
      resumeAnalysis.structuredData,
      targetPosition
    );

    // Save career profile
    const savedProfile = await careerService.saveCareerProfile(parseInt(userId), {
      ...enhancedProfile,
      targetPosition,
      skillGapAnalysis,
      overallMatchScore: targetPosition.matchScore || 0
    });

    // Save skill gap analysis
    await supabaseDb.createSkillGapAnalysis({
      userId: parseInt(userId),
      currentSkills: resumeAnalysis.structuredData?.skills,
      targetSkills: targetPosition.requiredSkills,
      identifiedGaps: skillGapAnalysis.skillGapAnalysis?.gaps,
      learningPath: skillGapAnalysis.developmentRoadmap,
      progressTracking: skillGapAnalysis.learningRecommendations
    });

    res.json({
      success: true,
      data: {
        enhancedProfile,
        skillGapAnalysis,
        careerProfileId: savedProfile.id,
        rateLimitStatus: careerService.getRateLimitStatus()
      }
    });

  } catch (error) {
    console.error('❌ Enhanced profile generation error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Enhanced profile generation failed'
    });
  }
});

/**
 * GET /api/career/position-recommendations/:analysisId
 * Get position recommendations for a resume analysis
 */
router.get('/position-recommendations/:analysisId', verifyToken, async (req, res) => {
  try {
    const userId = req.user.id;
    const { analysisId } = req.params;

    // Get resume analysis
    const resumeAnalysis = await supabaseDb.getResumeAnalysisById(analysisId);

    if (!resumeAnalysis) {
      return res.status(404).json({
        success: false,
        error: 'Resume analysis not found'
      });
    }

    // Get existing career profile
    const careerProfile = await supabaseDb.getUserCareerProfile(parseInt(userId));

    // Generate fresh position recommendations
    const recommendations = await careerService.generatePositionRecommendations(
      resumeAnalysis.structuredData,
      careerProfile || {}
    );

    res.json({
      success: true,
      data: {
        recommendations,
        analysisId: resumeAnalysis.id,
        rateLimitStatus: careerService.getRateLimitStatus()
      }
    });

  } catch (error) {
    console.error('❌ Position recommendations error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Failed to get position recommendations'
    });
  }
});

/**
 * GET /api/career/job-matches
 * Get saved job matches for the user
 */
router.get('/job-matches', verifyToken, async (req, res) => {
  try {
    const userId = req.user.id;

    const jobMatches = await supabaseDb.getJobMatches(parseInt(userId));

    res.json({
      success: true,
      data: {
        jobMatches,
        totalMatches: jobMatches.length
      }
    });

  } catch (error) {
    console.error('❌ Job matches retrieval error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Failed to retrieve job matches'
    });
  }
});

/**
 * GET /api/career/profile
 * Get user's career profile
 */
router.get('/profile', verifyToken, async (req, res) => {
  try {
    const userId = req.user.id;

    const careerProfile = await supabaseDb.getUserCareerProfile(parseInt(userId));

    const skillGapAnalyses = await supabaseDb.getSkillGapAnalyses(parseInt(userId));

    const resumeAnalyses = await supabaseDb.getResumeAnalyses(parseInt(userId));

    res.json({
      success: true,
      data: {
        careerProfile,
        skillGapAnalyses,
        resumeAnalyses
      }
    });

  } catch (error) {
    console.error('❌ Career profile retrieval error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Failed to retrieve career profile'
    });
  }
});

/**
 * PUT /api/career/application-status
 * Update job application status
 */
router.put('/application-status', verifyToken, async (req, res) => {
  try {
    const userId = req.user.id;
    const { jobMatchId, status } = req.body;

    if (!jobMatchId || !status) {
      return res.status(400).json({
        success: false,
        error: 'Job match ID and status are required'
      });
    }

    const updatedMatch = await supabaseDb.updateJobMatchStatus(jobMatchId, status);

    if (updatedMatch.count === 0) {
      return res.status(404).json({
        success: false,
        error: 'Job match not found'
      });
    }

    res.json({
      success: true,
      message: 'Application status updated successfully'
    });

  } catch (error) {
    console.error('❌ Application status update error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Failed to update application status'
    });
  }
});

/**
 * GET /api/career/skill-gap/:analysisId
 * Get skill gap analysis for a specific target position
 */
router.get('/skill-gap/:analysisId', verifyToken, async (req, res) => {
  try {
    const userId = req.user.id;
    const { analysisId } = req.params;
    const { targetPosition } = req.query;

    if (!targetPosition) {
      return res.status(400).json({
        success: false,
        error: 'Target position data is required'
      });
    }

    // Get resume analysis
    const resumeAnalysis = await supabaseDb.getResumeAnalysisById(analysisId);

    if (!resumeAnalysis) {
      return res.status(404).json({
        success: false,
        error: 'Resume analysis not found'
      });
    }

    // Parse target position from query parameter
    const parsedTargetPosition = JSON.parse(decodeURIComponent(targetPosition));

    // Generate skill gap analysis
    const skillGapAnalysis = await careerService.generateSkillGapAnalysis(
      resumeAnalysis.structuredData,
      parsedTargetPosition
    );

    res.json({
      success: true,
      data: {
        skillGapAnalysis,
        targetPosition: parsedTargetPosition,
        rateLimitStatus: careerService.getRateLimitStatus()
      }
    });

  } catch (error) {
    console.error('❌ Skill gap analysis error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Skill gap analysis failed'
    });
  }
});

/**
 * POST /api/career/generate-resume
 * Generate an optimized resume for a specific career path
 */
router.post('/generate-resume', verifyToken, async (req, res) => {
  try {
    const userId = req.user.id;
    const { targetPosition, userProfile, existingAnalysisId } = req.body;
    
    if (!targetPosition) {
      return res.status(400).json({
        success: false,
        error: 'Target position is required'
      });
    }

    console.log(`📝 Generating resume for user: ${userId}, position: ${targetPosition.title}`);

    // Get existing analysis if provided
    let existingAnalysis = null;
    if (existingAnalysisId) {
      existingAnalysis = await supabaseDb.getResumeAnalysisById(existingAnalysisId);
    }

    // Get user's career profile if available
    let userCareerProfile = userProfile;
    if (!userCareerProfile) {
      userCareerProfile = await supabaseDb.getUserCareerProfile(parseInt(userId));
    }

    // Generate optimized resume
    const generatedResume = await careerService.generateOptimizedResume(
      userCareerProfile || {},
      targetPosition,
      existingAnalysis
    );

    // Save generated resume to database
    const savedResume = await careerService.saveGeneratedResume(
      parseInt(userId),
      generatedResume,
      targetPosition
    );

    res.json({
      success: true,
      data: {
        resumeId: savedResume.id,
        generatedResume,
        targetPosition,
        rateLimitStatus: careerService.getRateLimitStatus()
      }
    });

  } catch (error) {
    console.error('❌ Resume generation error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Resume generation failed'
    });
  }
});

/**
 * POST /api/career/search-jobs
 * Search for jobs based on career path recommendation
 */
router.post('/search-jobs', verifyToken, async (req, res) => {
  try {
    const userId = req.user.id;
    const { careerPath, location = 'Canada', filters = {} } = req.body;

    // Validate input
    if (!careerPath || !careerPath.title) {
      return res.status(400).json({
        success: false,
        error: 'Career path with title is required'
      });
    }

    console.log(`🔍 Job search request for: ${careerPath.title} by user: ${userId}`);

    // Initialize Google Jobs Service
    const googleJobsService = new GoogleJobsService();

    // Add user context to filters
    const searchFilters = {
      ...filters,
      userId: userId,
      sessionId: req.sessionID || `session_${Date.now()}`
    };

    // Search for jobs
    const jobResults = await googleJobsService.searchJobs(careerPath, location, searchFilters);

    // Return results
    res.json({
      success: true,
      data: {
        ...jobResults,
        careerPath: {
          title: careerPath.title,
          industry: careerPath.industry
        },
        searchLocation: location
      }
    });

  } catch (error) {
    console.error('❌ Job search error:', error);
    res.status(500).json({
      success: false,
      error: error.message || 'Failed to search for jobs',
      fallbackMessage: 'Job search temporarily unavailable. Please try searching directly on job sites like Indeed.ca, LinkedIn, or Workopolis.'
    });
  }
});

module.exports = router;
````

## File: src/routes/monitoringRoutes.js
````javascript
/**
 * Monitoring Dashboard Routes
 * Provides real-time performance metrics, security alerts, and system health data
 */

const express = require('express');
const router = express.Router();
const { logger } = require('../config/logger');
const { cacheConfig } = require('../config/cache');
const { databaseOptimizer } = require('../utils/databaseOptimization');
const { routePerformance } = require('../middleware/routePerformance');

/**
 * Authentication middleware for monitoring endpoints
 * Only allow access to authorized users/admins
 */
const requireMonitoringAccess = (req, res, next) => {
  // Check if user has monitoring access
  const monitoringKey = req.headers['x-monitoring-key'] || req.query.monitoringKey;
  const expectedKey = process.env.MONITORING_ACCESS_KEY || 'default-monitoring-key';
  
  if (monitoringKey !== expectedKey) {
    return res.status(401).json({
      success: false,
      error: 'Unauthorized access to monitoring endpoints',
      timestamp: new Date().toISOString()
    });
  }
  
  next();
};

/**
 * Get overall system health
 */
router.get('/health', requireMonitoringAccess, async (req, res) => {
  try {
    const health = {
      status: 'healthy',
      timestamp: new Date().toISOString(),
      uptime: process.uptime(),
      memory: process.memoryUsage(),
      cpu: process.cpuUsage(),
      environment: process.env.NODE_ENV || 'development',
      version: process.version,
      services: {
        cache: cacheConfig.isConnected ? 'connected' : 'disconnected',
        database: 'connected', // Assuming database is always connected
        routes: 'active',
        security: 'enabled'
      }
    };

    res.json({
      success: true,
      data: health,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Health check failed:', error);
    res.status(500).json({
      success: false,
      error: 'Health check failed',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get performance metrics
 */
router.get('/performance', requireMonitoringAccess, async (req, res) => {
  try {
    const performance = {
      route: routePerformance.getMetrics(),
      database: databaseOptimizer.getQueryStats(),
      cache: await cacheConfig.getStats(),
      system: {
        memory: process.memoryUsage(),
        cpu: process.cpuUsage(),
        uptime: process.uptime(),
        loadAverage: process.loadavg ? process.loadavg() : null
      }
    };

    res.json({
      success: true,
      data: performance,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Performance metrics failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to get performance metrics',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get cache statistics
 */
router.get('/cache', requireMonitoringAccess, async (req, res) => {
  try {
    const stats = await cacheConfig.getStats();
    
    if (!stats) {
      return res.status(503).json({
        success: false,
        error: 'Cache service unavailable',
        timestamp: new Date().toISOString()
      });
    }

    res.json({
      success: true,
      data: stats,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Cache stats failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to get cache statistics',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get database performance metrics
 */
router.get('/database', requireMonitoringAccess, (req, res) => {
  try {
    const dbStats = databaseOptimizer.getQueryStats();
    
    res.json({
      success: true,
      data: dbStats,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Database stats failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to get database statistics',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get route performance metrics
 */
router.get('/routes', requireMonitoringAccess, (req, res) => {
  try {
    const routeStats = routePerformance.getMetrics();
    
    res.json({
      success: true,
      data: routeStats,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Route stats failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to get route statistics',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get security alerts and incidents
 */
router.get('/security', requireMonitoringAccess, (req, res) => {
  try {
    // This would typically come from a security monitoring service
    const securityAlerts = {
      recentIncidents: [],
      blockedRequests: 0,
      suspiciousActivities: 0,
      failedLogins: 0,
      lastUpdated: new Date().toISOString()
    };

    res.json({
      success: true,
      data: securityAlerts,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Security alerts failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to get security alerts',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get system logs (recent entries)
 */
router.get('/logs', requireMonitoringAccess, (req, res) => {
  try {
    const { level = 'error', limit = 100 } = req.query;
    
    // This would typically read from log files or a log service
    const logs = {
      entries: [],
      total: 0,
      level: level,
      limit: parseInt(limit)
    };

    res.json({
      success: true,
      data: logs,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Log retrieval failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to get logs',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Reset performance metrics
 */
router.post('/reset', requireMonitoringAccess, (req, res) => {
  try {
    const { type } = req.body;
    
    switch (type) {
      case 'route':
        routePerformance.resetMetrics();
        break;
      case 'database':
        databaseOptimizer.resetMetrics();
        break;
      case 'cache':
        cacheConfig.clearAll();
        break;
      case 'all':
        routePerformance.resetMetrics();
        databaseOptimizer.resetMetrics();
        cacheConfig.clearAll();
        break;
      default:
        return res.status(400).json({
          success: false,
          error: 'Invalid reset type. Use: route, database, cache, or all',
          timestamp: new Date().toISOString()
        });
    }

    res.json({
      success: true,
      message: `${type} metrics reset successfully`,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Metrics reset failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to reset metrics',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get real-time metrics (WebSocket endpoint placeholder)
 */
router.get('/realtime', requireMonitoringAccess, (req, res) => {
  try {
    // This would typically be a WebSocket endpoint for real-time updates
    const realtimeData = {
      activeConnections: 0,
      requestsPerSecond: 0,
      averageResponseTime: 0,
      errorRate: 0,
      lastUpdated: new Date().toISOString()
    };

    res.json({
      success: true,
      data: realtimeData,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Real-time metrics failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to get real-time metrics',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get monitoring dashboard configuration
 */
router.get('/config', requireMonitoringAccess, (req, res) => {
  try {
    const config = {
      refreshInterval: 5000, // 5 seconds
      retentionPeriod: 24 * 60 * 60 * 1000, // 24 hours
      alertThresholds: {
        responseTime: 1000, // 1 second
        errorRate: 0.05, // 5%
        memoryUsage: 0.8, // 80%
        cpuUsage: 0.7 // 70%
      },
      features: {
        realtimeUpdates: true,
        alerting: true,
        logRetention: true,
        performanceTracking: true
      }
    };

    res.json({
      success: true,
      data: config,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Config retrieval failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to get monitoring configuration',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Update monitoring configuration
 */
router.put('/config', requireMonitoringAccess, (req, res) => {
  try {
    const { refreshInterval, retentionPeriod, alertThresholds } = req.body;
    
    // Validate and update configuration
    const updates = {};
    
    if (refreshInterval && typeof refreshInterval === 'number') {
      updates.refreshInterval = refreshInterval;
    }
    
    if (retentionPeriod && typeof retentionPeriod === 'number') {
      updates.retentionPeriod = retentionPeriod;
    }
    
    if (alertThresholds && typeof alertThresholds === 'object') {
      updates.alertThresholds = alertThresholds;
    }

    res.json({
      success: true,
      message: 'Configuration updated successfully',
      data: updates,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Config update failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to update configuration',
      timestamp: new Date().toISOString()
    });
  }
});

/**
 * Get monitoring dashboard summary
 */
router.get('/summary', requireMonitoringAccess, async (req, res) => {
  try {
    const summary = {
      system: {
        status: 'healthy',
        uptime: process.uptime(),
        memory: process.memoryUsage(),
        cpu: process.cpuUsage()
      },
      performance: {
        averageResponseTime: routePerformance.getMetrics().averageResponseTime || 0,
        requestsPerMinute: routePerformance.getMetrics().requestsPerMinute || 0,
        errorRate: routePerformance.getMetrics().errorRate || 0
      },
      cache: {
        hitRate: '0%',
        connected: cacheConfig.isConnected,
        totalKeys: 0
      },
      database: {
        totalQueries: databaseOptimizer.getQueryStats().overall?.totalQueries || 0,
        slowQueries: databaseOptimizer.getQueryStats().overall?.slowQueries || 0,
        averageQueryTime: databaseOptimizer.getQueryStats().summary?.averageTime || 0
      },
      security: {
        blockedRequests: 0,
        suspiciousActivities: 0,
        lastIncident: null
      }
    };

    // Get cache hit rate if available
    if (cacheConfig.isConnected) {
      const cacheStats = await cacheConfig.getStats();
      if (cacheStats) {
        summary.cache.totalKeys = Object.values(cacheStats)
          .filter(stat => typeof stat === 'object' && stat.count)
          .reduce((sum, stat) => sum + stat.count, 0);
      }
    }

    res.json({
      success: true,
      data: summary,
      timestamp: new Date().toISOString()
    });
  } catch (error) {
    logger.error('Summary generation failed:', error);
    res.status(500).json({
      success: false,
      error: 'Failed to generate summary',
      timestamp: new Date().toISOString()
    });
  }
});

module.exports = router;
````

## File: src/routes/RouteFactory.js
````javascript
const express = require('express');
const { logger } = require('../config/logger');
const { 
  isFeatureAvailable, 
  getApiVersionConfig,
  isVersionSupported 
} = require('../config/apiVersioning');
const ControllerFactory = require('../controllers/ControllerFactory');

/**
 * Route Factory for creating version-aware API routes
 * This factory handles route creation for different API versions
 */
class RouteFactory {
  constructor() {
    this.routes = new Map();
    this.initialized = false;
  }

  /**
   * Initialize the route factory
   */
  async initialize() {
    if (this.initialized) {
      return;
    }

    try {
      await ControllerFactory.initialize();
      this.initialized = true;
    } catch (error) {
      throw new Error(`Failed to initialize RouteFactory: ${error.message}`);
    }
  }

  /**
   * Create routes for a specific API version
   * @param {string} version - API version
   * @returns {Object} Routes object
   */
  async createVersionRoutes(version) {
    if (!this.initialized) {
      await this.initialize();
    }

    if (!isVersionSupported(version)) {
      throw new Error(`Unsupported API version: ${version}`);
    }

    const versionConfig = getApiVersionConfig(version);
    const routes = {};

    // Create user routes if user-management feature is available
    if (isFeatureAvailable(version, 'user-management')) {
      routes.userRoutes = this.createUserRoutes(version);
    }

    // Create resume routes if resume-analysis feature is available
    if (isFeatureAvailable(version, 'resume-analysis')) {
      routes.resumeRoutes = this.createResumeRoutes(version);
    }

    // Create career routes if career-profiles feature is available
    if (isFeatureAvailable(version, 'career-profiles')) {
      routes.careerRoutes = this.createCareerRoutes(version);
    }

    // Create analytics routes if analytics feature is available (v2+)
    if (isFeatureAvailable(version, 'analytics')) {
      routes.analyticsRoutes = this.createAnalyticsRoutes(version);
    }

    // Create notification routes if real-time-notifications feature is available (v2+)
    if (isFeatureAvailable(version, 'real-time-notifications')) {
      routes.notificationRoutes = this.createNotificationRoutes(version);
    }

    logger.info(`Created routes for API version ${version}`, {
      version,
      features: versionConfig.features,
      routes: Object.keys(routes)
    });

    return routes;
  }

  /**
   * Create user routes for specific version
   * @param {string} version - API version
   * @returns {Object} Express router
   */
  createUserRoutes(version) {
    const router = express.Router();
    const userController = ControllerFactory.getController('user');

    // Version-specific route configurations
    const routeConfigs = {
      v1: {
        findOrCreateUser: { path: '/find-or-create', method: 'POST' },
        getCurrentUserProfile: { path: '/profile', method: 'GET' },
        updateCurrentUserProfile: { path: '/profile', method: 'PUT' },
        getUserById: { path: '/:userId', method: 'GET' },
        updateUser: { path: '/:userId', method: 'PUT' },
        deleteUser: { path: '/:userId', method: 'DELETE' },
        getUserByEmail: { path: '/email/:email', method: 'GET' },
        searchUsers: { path: '/search', method: 'GET' },
        getUsers: { path: '/', method: 'GET' },
        getUsersByRole: { path: '/role/:roleId', method: 'GET' },
        getUsersByStatusInCanada: { path: '/status/:status', method: 'GET' },
        getUsersByCountryOfOrigin: { path: '/country/:country', method: 'GET' },
        getUsersByCurrentLocation: { path: '/location/:location', method: 'GET' },
        getUserStatistics: { path: '/statistics', method: 'GET' },
        userExists: { path: '/:userId/exists', method: 'GET' },
        getUserCount: { path: '/count', method: 'GET' }
      },
      v2: {
        findOrCreateUser: { path: '/find-or-create', method: 'POST' },
        getCurrentUserProfile: { path: '/profile', method: 'GET' },
        updateCurrentUserProfile: { path: '/profile', method: 'PUT' },
        getUserById: { path: '/:userId', method: 'GET' },
        updateUser: { path: '/:userId', method: 'PUT' },
        deleteUser: { path: '/:userId', method: 'DELETE' },
        getUserByEmail: { path: '/email/:email', method: 'GET' },
        searchUsers: { path: '/search', method: 'GET' },
        getUsers: { path: '/', method: 'GET' },
        getUsersByRole: { path: '/role/:roleId', method: 'GET' },
        getUsersByStatusInCanada: { path: '/status/:status', method: 'GET' },
        getUsersByCountryOfOrigin: { path: '/country/:country', method: 'GET' },
        getUsersByCurrentLocation: { path: '/location/:location', method: 'GET' },
        getUserStatistics: { path: '/statistics', method: 'GET' },
        userExists: { path: '/:userId/exists', method: 'GET' },
        getUserCount: { path: '/count', method: 'GET' },
        // v2 specific routes
        getUserPreferences: { path: '/preferences', method: 'GET' },
        updateUserPreferences: { path: '/preferences', method: 'PUT' },
        getUserActivity: { path: '/activity', method: 'GET' }
      }
    };

    const config = routeConfigs[version] || routeConfigs.v1;

    // Create routes dynamically
    Object.entries(config).forEach(([handlerName, routeConfig]) => {
      if (typeof userController[handlerName] === 'function') {
        const { path, method } = routeConfig;
        router[method.toLowerCase()](path, userController[handlerName].bind(userController));
      }
    });

    return router;
  }

  /**
   * Create resume routes for specific version
   * @param {string} version - API version
   * @returns {Object} Express router
   */
  createResumeRoutes(version) {
    const router = express.Router();
    const resumeController = ControllerFactory.getController('resume');

    // Version-specific route configurations
    const routeConfigs = {
      v1: {
        saveResumeAnalysis: { path: '/analysis', method: 'POST' },
        uploadAndAnalyzeResume: { path: '/upload', method: 'POST' },
        getUserResumeAnalyses: { path: '/analyses', method: 'GET' },
        getLatestResumeAnalysis: { path: '/analyses/latest', method: 'GET' },
        getResumeAnalysisCount: { path: '/analyses/count', method: 'GET' },
        getResumeAnalysisStatistics: { path: '/analyses/statistics', method: 'GET' },
        searchResumeAnalyses: { path: '/analyses/search', method: 'GET' },
        getResumeAnalysisById: { path: '/analyses/:analysisId', method: 'GET' },
        getResumeAnalysisWithParsedData: { path: '/analyses/:analysisId/parsed', method: 'GET' },
        updateResumeAnalysis: { path: '/analyses/:analysisId', method: 'PUT' },
        deleteResumeAnalysis: { path: '/analyses/:analysisId', method: 'DELETE' },
        bulkDeleteResumeAnalyses: { path: '/analyses/bulk', method: 'DELETE' },
        getResumeAnalysesByUserId: { path: '/analyses/user/:userId', method: 'GET' },
        // Resume generation routes
        generateCanadianResume: { path: '/generate', method: 'POST' },
        getUserGeneratedResumes: { path: '/generated', method: 'GET' },
        getGeneratedResumeById: { path: '/generated/:resumeId', method: 'GET' },
        updateGeneratedResume: { path: '/generated/:resumeId', method: 'PUT' },
        deleteGeneratedResume: { path: '/generated/:resumeId', method: 'DELETE' },
        autoSaveUserEdits: { path: '/generated/:resumeId/auto-save', method: 'PATCH' },
        trackPDFDownload: { path: '/generated/:resumeId/track-download', method: 'POST' },
        searchGeneratedResumes: { path: '/generated/search', method: 'GET' },
        getGeneratedResumeStatistics: { path: '/generated/statistics', method: 'GET' },
        analyzeJobTargeting: { path: '/analyze-job-targeting', method: 'POST' },
        translateSkillsForCanadianMarket: { path: '/translate-skills', method: 'POST' },
        exportResume: { path: '/generated/:resumeId/export', method: 'POST' },
        downloadResumePDF: { path: '/generated/:resumeId/download-pdf', method: 'GET' },
        bulkDeleteGeneratedResumes: { path: '/generated/bulk', method: 'DELETE' },
        bulkExportResumes: { path: '/generated/bulk-export', method: 'POST' },
        streamGenerationProgress: { path: '/generate/:resumeId/progress', method: 'GET' },
        checkGenerationSupport: { path: '/generate/support', method: 'GET' },
        getGenerationTemplates: { path: '/generate/templates', method: 'GET' }
      },
      v2: {
        saveResumeAnalysis: { path: '/analysis', method: 'POST' },
        uploadAndAnalyzeResume: { path: '/upload', method: 'POST' },
        getUserResumeAnalyses: { path: '/analyses', method: 'GET' },
        getLatestResumeAnalysis: { path: '/analyses/latest', method: 'GET' },
        getResumeAnalysisCount: { path: '/analyses/count', method: 'GET' },
        getResumeAnalysisStatistics: { path: '/analyses/statistics', method: 'GET' },
        searchResumeAnalyses: { path: '/analyses/search', method: 'GET' },
        getResumeAnalysisById: { path: '/analyses/:analysisId', method: 'GET' },
        getResumeAnalysisWithParsedData: { path: '/analyses/:analysisId/parsed', method: 'GET' },
        updateResumeAnalysis: { path: '/analyses/:analysisId', method: 'PUT' },
        deleteResumeAnalysis: { path: '/analyses/:analysisId', method: 'DELETE' },
        bulkDeleteResumeAnalyses: { path: '/analyses/bulk', method: 'DELETE' },
        getResumeAnalysesByUserId: { path: '/analyses/user/:userId', method: 'GET' },
        // v2 specific routes
        getResumeAnalytics: { path: '/analytics', method: 'GET' },
        compareResumes: { path: '/compare', method: 'POST' },
        exportResumeAnalysis: { path: '/analyses/:analysisId/export', method: 'GET' },
        // Resume generation routes (same as v1 for now)
        generateCanadianResume: { path: '/generate', method: 'POST' },
        getUserGeneratedResumes: { path: '/generated', method: 'GET' },
        getGeneratedResumeById: { path: '/generated/:resumeId', method: 'GET' },
        updateGeneratedResume: { path: '/generated/:resumeId', method: 'PUT' },
        deleteGeneratedResume: { path: '/generated/:resumeId', method: 'DELETE' },
        autoSaveUserEdits: { path: '/generated/:resumeId/auto-save', method: 'PATCH' },
        trackPDFDownload: { path: '/generated/:resumeId/track-download', method: 'POST' },
        searchGeneratedResumes: { path: '/generated/search', method: 'GET' },
        getGeneratedResumeStatistics: { path: '/generated/statistics', method: 'GET' },
        analyzeJobTargeting: { path: '/analyze-job-targeting', method: 'POST' },
        translateSkillsForCanadianMarket: { path: '/translate-skills', method: 'POST' },
        exportResume: { path: '/generated/:resumeId/export', method: 'POST' },
        downloadResumePDF: { path: '/generated/:resumeId/download-pdf', method: 'GET' },
        bulkDeleteGeneratedResumes: { path: '/generated/bulk', method: 'DELETE' },
        bulkExportResumes: { path: '/generated/bulk-export', method: 'POST' },
        streamGenerationProgress: { path: '/generate/:resumeId/progress', method: 'GET' },
        checkGenerationSupport: { path: '/generate/support', method: 'GET' },
        getGenerationTemplates: { path: '/generate/templates', method: 'GET' }
      }
    };

    const config = routeConfigs[version] || routeConfigs.v1;

    // Create routes dynamically
    Object.entries(config).forEach(([handlerName, routeConfig]) => {
      if (typeof resumeController[handlerName] === 'function') {
        const { path, method } = routeConfig;
        router[method.toLowerCase()](path, resumeController[handlerName].bind(resumeController));
      }
    });

    return router;
  }

  /**
   * Create career routes for specific version
   * @param {string} version - API version
   * @returns {Object} Express router
   */
  createCareerRoutes(version) {
    const router = express.Router();
    
    // For now, we'll use the legacy career routes
    // TODO: Create career controller and implement version-specific routes
    const legacyCareerRoutes = require('./careerRoutes');
    
    // Apply legacy routes with version-specific modifications
    router.use('/', legacyCareerRoutes);

    return router;
  }

  /**
   * Create analytics routes for specific version (v2+)
   * @param {string} version - API version
   * @returns {Object} Express router
   */
  createAnalyticsRoutes(version) {
    const router = express.Router();

    // Analytics routes for v2+
    router.get('/dashboard', (req, res) => {
      res.json({
        message: 'Analytics dashboard endpoint',
        version,
        features: ['user-analytics', 'resume-analytics', 'career-analytics']
      });
    });

    router.get('/user-metrics', (req, res) => {
      res.json({
        message: 'User metrics endpoint',
        version,
        metrics: ['registration-rate', 'engagement-rate', 'retention-rate']
      });
    });

    router.get('/resume-metrics', (req, res) => {
      res.json({
        message: 'Resume analysis metrics endpoint',
        version,
        metrics: ['analysis-count', 'success-rate', 'popular-skills']
      });
    });

    return router;
  }

  /**
   * Create notification routes for specific version (v2+)
   * @param {string} version - API version
   * @returns {Object} Express router
   */
  createNotificationRoutes(version) {
    const router = express.Router();

    // Notification routes for v2+
    router.get('/subscriptions', (req, res) => {
      res.json({
        message: 'Notification subscriptions endpoint',
        version,
        types: ['email', 'push', 'sms']
      });
    });

    router.post('/subscribe', (req, res) => {
      res.json({
        message: 'Subscribe to notifications endpoint',
        version,
        subscription: req.body
      });
    });

    router.delete('/unsubscribe', (req, res) => {
      res.json({
        message: 'Unsubscribe from notifications endpoint',
        version
      });
    });

    return router;
  }

  /**
   * Get all routes for a specific version
   * @param {string} version - API version
   * @returns {Object} All routes for the version
   */
  async getAllRoutes(version) {
    return await this.createVersionRoutes(version);
  }

  /**
   * Get route information for documentation
   * @param {string} version - API version
   * @returns {Object} Route information
   */
  async getRouteInfo(version) {
    const routes = await this.createVersionRoutes(version);
    const routeInfo = {};

    Object.entries(routes).forEach(([routeName, router]) => {
      routeInfo[routeName] = {
        name: routeName,
        version,
        stack: router.stack ? router.stack.map(layer => ({
          path: layer.route?.path,
          methods: layer.route?.methods
        })).filter(item => item.path) : []
      };
    });

    return routeInfo;
  }

  /**
   * Check if route is available in version
   * @param {string} version - API version
   * @param {string} routeName - Route name
   * @returns {boolean} Whether route is available
   */
  async isRouteAvailable(version, routeName) {
    const routes = await this.createVersionRoutes(version);
    return !!routes[routeName];
  }

  /**
   * Get available routes for version
   * @param {string} version - API version
   * @returns {Array} Available route names
   */
  async getAvailableRoutes(version) {
    const routes = await this.createVersionRoutes(version);
    return Object.keys(routes);
  }
}

// Create singleton instance
const routeFactory = new RouteFactory();

module.exports = routeFactory;
````

## File: src/routes/v1/aiRoutes.js
````javascript
/**
 * API v1 AI Routes
 * Handles AI-powered resume analysis, career profile generation, and job recommendations
 */

const express = require('express');
const multer = require('multer');
const path = require('path');
const fs = require('fs');
const { validateRequest } = require('../../middleware/validation');
const { aiSchemas } = require('../../models/schemas');
const { verifyToken, optionalAuth } = require('../../middleware/authMiddleware');
const { rateLimit, geminiRateLimit, uploadRateLimit } = require('../../middleware/rateLimiter');
const { logger } = require('../../config/logger');
const ControllerFactory = require('../../controllers/ControllerFactory');

const router = express.Router();

// Configure multer for file uploads
const storage = multer.diskStorage({
  destination: (req, file, cb) => {
    const uploadPath = path.join(__dirname, '../../uploads/resumes');
    if (!fs.existsSync(uploadPath)) {
      fs.mkdirSync(uploadPath, { recursive: true });
    }
    cb(null, uploadPath);
  },
  filename: (req, file, cb) => {
    const uniqueSuffix = Date.now() + '-' + Math.round(Math.random() * 1E9);
    cb(null, `resume-${uniqueSuffix}${path.extname(file.originalname)}`);
  }
});

const upload = multer({
  storage: storage,
  limits: { fileSize: 10 * 1024 * 1024 }, // 10MB limit
  fileFilter: (req, file, cb) => {
    const allowedTypes = /pdf|docx|jpg|jpeg|png/;
    const extname = allowedTypes.test(path.extname(file.originalname).toLowerCase());
    const mimetype = allowedTypes.test(file.mimetype);
    
    if (mimetype && extname) {
      return cb(null, true);
    } else {
      cb(new Error('Only PDF, DOCX, JPG, JPEG, and PNG files are allowed'));
    }
  }
});

/**
 * @route POST /api/v1/ai/analyze-resume
 * @desc Analyze uploaded resume using AI
 * @access Private
 * @body {file} resume - Resume file (PDF, DOCX, JPG, JPEG, PNG)
 * @body {string} [jobTitle] - Target job title for analysis
 * @body {string} [company] - Target company for analysis
 */
router.post('/analyze-resume',
  optionalAuth,
  uploadRateLimit,
  upload.single('resume'),
  validateRequest(aiSchemas.analyzeResume),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      const result = await aiController.analyzeResume({
        file: req.file,
        jobTitle: req.body.jobTitle,
        company: req.body.company,
        userId: req.user?.id
      });
      
      logger.info('Resume analysis completed', {
        userId: req.user?.id || 'guest',
        fileName: req.file?.originalname,
        analysisId: result.analysisId
      });

      res.json({
        success: true,
        message: 'Resume analysis completed successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/ai/resume-analysis/:analysisId
 * @desc Get resume analysis results
 * @access Private
 * @param {string} analysisId - Analysis ID
 */
router.get('/resume-analysis/:analysisId',
  verifyToken,
  validateRequest(aiSchemas.getAnalysis),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      const result = await aiController.getResumeAnalysis(req.params.analysisId, req.user.id);
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/ai/resume-analyses
 * @desc Get user's resume analysis history
 * @access Private
 * @query {number} [page=1] - Page number
 * @query {number} [limit=10] - Items per page
 */
router.get('/resume-analyses',
  verifyToken,
  validateRequest(aiSchemas.getAnalyses),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      const result = await aiController.getResumeAnalyses(req.user.id, {
        page: parseInt(req.query.page) || 1,
        limit: parseInt(req.query.limit) || 10
      });
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/ai/generate-career-profile
 * @desc Generate AI-powered career profile
 * @access Private
 * @body {string} resumeText - Resume text content
 * @body {string} [jobTitle] - Current or target job title
 * @body {string} [experience] - Years of experience
 * @body {string} [skills] - Skills list
 */
router.post('/generate-career-profile',
  verifyToken,
  geminiRateLimit,
  validateRequest(aiSchemas.generateCareerProfile),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      const result = await aiController.generateCareerProfile({
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Career profile generated', {
        userId: req.user.id,
        profileId: result.profileId
      });

      res.json({
        success: true,
        message: 'Career profile generated successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/ai/career-profile/:profileId
 * @desc Get generated career profile
 * @access Private
 * @param {string} profileId - Profile ID
 */
router.get('/career-profile/:profileId',
  verifyToken,
  validateRequest(aiSchemas.getCareerProfile),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      const result = await aiController.getCareerProfile(req.params.profileId, req.user.id);
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/ai/enhance-career-profile
 * @desc Enhance existing career profile with AI
 * @access Private
 * @body {string} profileId - Career profile ID
 * @body {string} [enhancementType] - Type of enhancement
 * @body {object} [additionalData] - Additional data for enhancement
 */
router.post('/enhance-career-profile',
  verifyToken,
  geminiRateLimit,
  validateRequest(aiSchemas.enhanceCareerProfile),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      const result = await aiController.enhanceCareerProfile({
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Career profile enhanced', {
        userId: req.user.id,
        profileId: req.body.profileId
      });

      res.json({
        success: true,
        message: 'Career profile enhanced successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/ai/job-recommendations
 * @desc Get AI-powered job recommendations
 * @access Private
 * @body {string} [resumeText] - Resume text content
 * @body {string} [careerProfileId] - Career profile ID
 * @body {string} [location] - Preferred location
 * @body {string} [jobType] - Job type preference
 * @body {number} [limit=10] - Number of recommendations
 */
router.post('/job-recommendations',
  verifyToken,
  geminiRateLimit,
  validateRequest(aiSchemas.getJobRecommendations),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      const result = await aiController.getJobRecommendations({
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Job recommendations generated', {
        userId: req.user.id,
        recommendationsCount: result.recommendations.length
      });

      res.json({
        success: true,
        message: 'Job recommendations generated successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/ai/skill-analysis
 * @desc Analyze skills from resume or profile
 * @access Private
 * @body {string} content - Resume or profile content
 * @body {string} [analysisType] - Type of analysis
 */
router.post('/skill-analysis',
  verifyToken,
  geminiRateLimit,
  validateRequest(aiSchemas.skillAnalysis),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      const result = await aiController.analyzeSkills({
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Skill analysis completed', {
        userId: req.user.id,
        analysisType: req.body.analysisType
      });

      res.json({
        success: true,
        message: 'Skill analysis completed successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route DELETE /api/v1/ai/resume-analysis/:analysisId
 * @desc Delete resume analysis
 * @access Private
 * @param {string} analysisId - Analysis ID
 */
router.delete('/resume-analysis/:analysisId',
  verifyToken,
  validateRequest(aiSchemas.deleteAnalysis),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      await aiController.deleteResumeAnalysis(req.params.analysisId, req.user.id);
      
      logger.info('Resume analysis deleted', {
        userId: req.user.id,
        analysisId: req.params.analysisId
      });

      res.json({
        success: true,
        message: 'Resume analysis deleted successfully'
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route DELETE /api/v1/ai/career-profile/:profileId
 * @desc Delete career profile
 * @access Private
 * @param {string} profileId - Profile ID
 */
router.delete('/career-profile/:profileId',
  verifyToken,
  validateRequest(aiSchemas.deleteCareerProfile),
  async (req, res, next) => {
    try {
      const aiController = ControllerFactory.getController('ai');
      await aiController.deleteCareerProfile(req.params.profileId, req.user.id);
      
      logger.info('Career profile deleted', {
        userId: req.user.id,
        profileId: req.params.profileId
      });

      res.json({
        success: true,
        message: 'Career profile deleted successfully'
      });
    } catch (error) {
      next(error);
    }
  }
);

module.exports = router;
````

## File: src/routes/v1/authRoutes.js
````javascript
/**
 * API v1 Authentication Routes
 * Handles user authentication, registration, and session management
 */

const express = require('express');
const { validateRequest } = require('../../middleware/validation');
const { authSchemas } = require('../../models/schemas');
const { verifyToken, optionalAuth } = require('../../middleware/authMiddleware');
const { rateLimit } = require('../../middleware/rateLimiter');
const { logger } = require('../../config/logger');
const ControllerFactory = require('../../controllers/ControllerFactory');

const router = express.Router();

/**
 * @route POST /api/v1/auth/register
 * @desc Register a new user
 * @access Public
 * @body {string} email - User email
 * @body {string} password - User password
 * @body {string} fullName - User full name
 * @body {string} [phoneNo] - User phone number
 * @body {string} [statusInCanada] - Immigration status
 * @body {string} [countryOfOrigin] - Country of origin
 * @body {string} [currentLocation] - Current location
 */
router.post('/register',
  rateLimit({ windowMs: 15 * 60 * 1000, max: 5 }), // 5 requests per 15 minutes
  validateRequest(authSchemas.register),
  async (req, res, next) => {
    try {
      const authController = ControllerFactory.getController('auth');
      const result = await authController.register(req.body);
      
      logger.info('User registration successful', {
        email: req.body.email,
        userId: result.user.id
      });

      res.status(201).json({
        success: true,
        message: 'User registered successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/auth/login
 * @desc Authenticate user and return session
 * @access Public
 * @body {string} email - User email
 * @body {string} password - User password
 */
router.post('/login',
  rateLimit({ windowMs: 15 * 60 * 1000, max: 10 }), // 10 requests per 15 minutes
  validateRequest(authSchemas.login),
  async (req, res, next) => {
    try {
      const authController = ControllerFactory.getController('auth');
      const result = await authController.login(req.body);
      
      logger.info('User login successful', {
        email: req.body.email,
        userId: result.user.id
      });

      res.json({
        success: true,
        message: 'Login successful',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/auth/logout
 * @desc Logout user and invalidate session
 * @access Private
 */
router.post('/logout',
  verifyToken,
  async (req, res, next) => {
    try {
      const authController = ControllerFactory.getController('auth');
      await authController.logout(req.user.id);
      
      logger.info('User logout successful', {
        userId: req.user.id
      });

      res.json({
        success: true,
        message: 'Logout successful'
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/auth/refresh
 * @desc Refresh access token using refresh token
 * @access Public
 * @body {string} refreshToken - Refresh token
 */
router.post('/refresh',
  rateLimit({ windowMs: 15 * 60 * 1000, max: 20 }), // 20 requests per 15 minutes
  validateRequest(authSchemas.refreshToken),
  async (req, res, next) => {
    try {
      const authController = ControllerFactory.getController('auth');
      const result = await authController.refreshToken(req.body.refreshToken);
      
      logger.info('Token refresh successful', {
        userId: result.user.id
      });

      res.json({
        success: true,
        message: 'Token refreshed successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/auth/me
 * @desc Get current user profile
 * @access Private
 */
router.get('/me',
  verifyToken,
  async (req, res, next) => {
    try {
      const authController = ControllerFactory.getController('auth');
      const user = await authController.getCurrentUser(req.user.id);
      
      res.json({
        success: true,
        data: user
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/auth/forgot-password
 * @desc Send password reset email
 * @access Public
 * @body {string} email - User email
 */
router.post('/forgot-password',
  rateLimit({ windowMs: 60 * 60 * 1000, max: 3 }), // 3 requests per hour
  validateRequest(authSchemas.forgotPassword),
  async (req, res, next) => {
    try {
      const authController = ControllerFactory.getController('auth');
      await authController.forgotPassword(req.body.email);
      
      logger.info('Password reset email sent', {
        email: req.body.email
      });

      res.json({
        success: true,
        message: 'Password reset email sent successfully'
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/auth/reset-password
 * @desc Reset password using token
 * @access Public
 * @body {string} token - Reset token
 * @body {string} password - New password
 */
router.post('/reset-password',
  rateLimit({ windowMs: 60 * 60 * 1000, max: 5 }), // 5 requests per hour
  validateRequest(authSchemas.resetPassword),
  async (req, res, next) => {
    try {
      const authController = ControllerFactory.getController('auth');
      await authController.resetPassword(req.body.token, req.body.password);
      
      logger.info('Password reset successful', {
        token: req.body.token
      });

      res.json({
        success: true,
        message: 'Password reset successful'
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/auth/verify-email
 * @desc Verify email address
 * @access Public
 * @body {string} token - Email verification token
 */
router.post('/verify-email',
  rateLimit({ windowMs: 60 * 60 * 1000, max: 10 }), // 10 requests per hour
  validateRequest(authSchemas.verifyEmail),
  async (req, res, next) => {
    try {
      const authController = ControllerFactory.getController('auth');
      await authController.verifyEmail(req.body.token);
      
      logger.info('Email verification successful', {
        token: req.body.token
      });

      res.json({
        success: true,
        message: 'Email verified successfully'
      });
    } catch (error) {
      next(error);
    }
  }
);

module.exports = router;
````

## File: src/routes/v1/careerRoutes.js
````javascript
/**
 * API v1 Career Routes
 * Handles career profile management, job search, and career development features
 */

const express = require('express');
const { validateRequest } = require('../../middleware/validation');
const { careerSchemas } = require('../../models/schemas');
const { verifyToken } = require('../../middleware/authMiddleware');
const { rateLimit } = require('../../middleware/rateLimiter');
const { logger } = require('../../config/logger');
const ControllerFactory = require('../../controllers/ControllerFactory');

const router = express.Router();

/**
 * @route POST /api/v1/career/profile
 * @desc Create or update career profile
 * @access Private
 * @body {object} profile - Career profile data
 */
router.post('/profile',
  verifyToken,
  rateLimit({ windowMs: 15 * 60 * 1000, max: 10 }), // 10 requests per 15 minutes
  validateRequest(careerSchemas.createProfile),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.createOrUpdateProfile({
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Career profile created/updated', {
        userId: req.user.id,
        profileId: result.profileId
      });

      res.status(201).json({
        success: true,
        message: 'Career profile created successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/career/profile
 * @desc Get user's career profile
 * @access Private
 */
router.get('/profile',
  verifyToken,
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.getProfile(req.user.id);
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route PUT /api/v1/career/profile
 * @desc Update career profile
 * @access Private
 * @body {object} profile - Updated career profile data
 */
router.put('/profile',
  verifyToken,
  rateLimit({ windowMs: 15 * 60 * 1000, max: 10 }), // 10 requests per 15 minutes
  validateRequest(careerSchemas.updateProfile),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.updateProfile({
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Career profile updated', {
        userId: req.user.id
      });

      res.json({
        success: true,
        message: 'Career profile updated successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route DELETE /api/v1/career/profile
 * @desc Delete career profile
 * @access Private
 */
router.delete('/profile',
  verifyToken,
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      await careerController.deleteProfile(req.user.id);
      
      logger.info('Career profile deleted', {
        userId: req.user.id
      });

      res.json({
        success: true,
        message: 'Career profile deleted successfully'
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/career/search-jobs
 * @desc Search for jobs based on career profile and preferences
 * @access Private
 * @body {string} [query] - Job search query
 * @body {string} [location] - Job location
 * @body {string} [jobType] - Job type
 * @body {number} [page=1] - Page number
 * @body {number} [limit=20] - Results per page
 */
router.post('/search-jobs',
  verifyToken,
  rateLimit({ windowMs: 5 * 60 * 1000, max: 30 }), // 30 requests per 5 minutes
  validateRequest(careerSchemas.searchJobs),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.searchJobs({
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Job search completed', {
        userId: req.user.id,
        query: req.body.query,
        resultsCount: result.jobs.length
      });

      res.json({
        success: true,
        message: 'Job search completed successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/career/job/:jobId
 * @desc Get detailed job information
 * @access Private
 * @param {string} jobId - Job ID
 */
router.get('/job/:jobId',
  verifyToken,
  validateRequest(careerSchemas.getJob),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.getJobDetails(req.params.jobId);
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/career/job/:jobId/apply
 * @desc Apply for a job
 * @access Private
 * @param {string} jobId - Job ID
 * @body {string} [coverLetter] - Cover letter text
 * @body {string} [resumeId] - Resume ID to use
 */
router.post('/job/:jobId/apply',
  verifyToken,
  rateLimit({ windowMs: 60 * 60 * 1000, max: 10 }), // 10 applications per hour
  validateRequest(careerSchemas.applyForJob),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.applyForJob({
        jobId: req.params.jobId,
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Job application submitted', {
        userId: req.user.id,
        jobId: req.params.jobId,
        applicationId: result.applicationId
      });

      res.status(201).json({
        success: true,
        message: 'Job application submitted successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/career/applications
 * @desc Get user's job applications
 * @access Private
 * @query {number} [page=1] - Page number
 * @query {number} [limit=10] - Items per page
 * @query {string} [status] - Application status filter
 */
router.get('/applications',
  verifyToken,
  validateRequest(careerSchemas.getApplications),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.getApplications(req.user.id, {
        page: parseInt(req.query.page) || 1,
        limit: parseInt(req.query.limit) || 10,
        status: req.query.status
      });
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/career/application/:applicationId
 * @desc Get specific job application details
 * @access Private
 * @param {string} applicationId - Application ID
 */
router.get('/application/:applicationId',
  verifyToken,
  validateRequest(careerSchemas.getApplication),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.getApplicationDetails(
        req.params.applicationId,
        req.user.id
      );
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route DELETE /api/v1/career/application/:applicationId
 * @desc Withdraw job application
 * @access Private
 * @param {string} applicationId - Application ID
 */
router.delete('/application/:applicationId',
  verifyToken,
  validateRequest(careerSchemas.withdrawApplication),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      await careerController.withdrawApplication(
        req.params.applicationId,
        req.user.id
      );
      
      logger.info('Job application withdrawn', {
        userId: req.user.id,
        applicationId: req.params.applicationId
      });

      res.json({
        success: true,
        message: 'Job application withdrawn successfully'
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/career/skills
 * @desc Add or update skills in career profile
 * @access Private
 * @body {array} skills - Array of skills
 */
router.post('/skills',
  verifyToken,
  rateLimit({ windowMs: 15 * 60 * 1000, max: 20 }), // 20 requests per 15 minutes
  validateRequest(careerSchemas.updateSkills),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.updateSkills({
        skills: req.body.skills,
        userId: req.user.id
      });
      
      logger.info('Skills updated', {
        userId: req.user.id,
        skillsCount: req.body.skills.length
      });

      res.json({
        success: true,
        message: 'Skills updated successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/career/skills
 * @desc Get user's skills
 * @access Private
 */
router.get('/skills',
  verifyToken,
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.getSkills(req.user.id);
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route POST /api/v1/career/experience
 * @desc Add work experience to career profile
 * @access Private
 * @body {object} experience - Work experience data
 */
router.post('/experience',
  verifyToken,
  rateLimit({ windowMs: 15 * 60 * 1000, max: 10 }), // 10 requests per 15 minutes
  validateRequest(careerSchemas.addExperience),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.addExperience({
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Work experience added', {
        userId: req.user.id,
        experienceId: result.experienceId
      });

      res.status(201).json({
        success: true,
        message: 'Work experience added successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route GET /api/v1/career/experience
 * @desc Get user's work experience
 * @access Private
 */
router.get('/experience',
  verifyToken,
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.getExperience(req.user.id);
      
      res.json({
        success: true,
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route PUT /api/v1/career/experience/:experienceId
 * @desc Update work experience
 * @access Private
 * @param {string} experienceId - Experience ID
 * @body {object} experience - Updated experience data
 */
router.put('/experience/:experienceId',
  verifyToken,
  rateLimit({ windowMs: 15 * 60 * 1000, max: 10 }), // 10 requests per 15 minutes
  validateRequest(careerSchemas.updateExperience),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      const result = await careerController.updateExperience({
        experienceId: req.params.experienceId,
        ...req.body,
        userId: req.user.id
      });
      
      logger.info('Work experience updated', {
        userId: req.user.id,
        experienceId: req.params.experienceId
      });

      res.json({
        success: true,
        message: 'Work experience updated successfully',
        data: result
      });
    } catch (error) {
      next(error);
    }
  }
);

/**
 * @route DELETE /api/v1/career/experience/:experienceId
 * @desc Delete work experience
 * @access Private
 * @param {string} experienceId - Experience ID
 */
router.delete('/experience/:experienceId',
  verifyToken,
  validateRequest(careerSchemas.deleteExperience),
  async (req, res, next) => {
    try {
      const careerController = ControllerFactory.getController('career');
      await careerController.deleteExperience(
        req.params.experienceId,
        req.user.id
      );
      
      logger.info('Work experience deleted', {
        userId: req.user.id,
        experienceId: req.params.experienceId
      });

      res.json({
        success: true,
        message: 'Work experience deleted successfully'
      });
    } catch (error) {
      next(error);
    }
  }
);

module.exports = router;
````

## File: src/routes/v1/index.js
````javascript
/**
 * API v1 Routes
 * This file exports all v1 API routes
 */

const userRoutes = require('./userRoutes');
const resumeRoutes = require('./resumeRoutes');
const authRoutes = require('./authRoutes');
const aiRoutes = require('./aiRoutes');
const careerRoutes = require('./careerRoutes');

module.exports = {
  userRoutes,
  resumeRoutes,
  authRoutes,
  aiRoutes,
  careerRoutes
};
````

## File: src/routes/v1/resumeRoutes.js
````javascript
const express = require('express');
const { validate } = require('../../middleware/validation');
const { resumeSchemas } = require('../../models/schemas');
const ControllerFactory = require('../../controllers/ControllerFactory');

const router = express.Router();

/**
 * Initialize resume routes with controller factory
 */
const initializeResumeRoutes = async () => {
  try {
    await ControllerFactory.initialize();
    const resumeController = ControllerFactory.getController('resume');

    // Resume analysis routes
    router.post('/analysis', 
      validate(resumeSchemas.saveResumeAnalysis), 
      resumeController.saveResumeAnalysis.bind(resumeController)
    );

    router.post('/upload', 
      validate(resumeSchemas.uploadAndAnalyzeResume), 
      resumeController.uploadAndAnalyzeResume.bind(resumeController)
    );

    // Resume analysis retrieval routes
    router.get('/analyses', 
      validate(resumeSchemas.getUserResumeAnalyses), 
      resumeController.getUserResumeAnalyses.bind(resumeController)
    );

    router.get('/analyses/latest', 
      resumeController.getLatestResumeAnalysis.bind(resumeController)
    );

    router.get('/analyses/count', 
      resumeController.getResumeAnalysisCount.bind(resumeController)
    );

    router.get('/analyses/statistics', 
      resumeController.getResumeAnalysisStatistics.bind(resumeController)
    );

    // Resume analysis search routes
    router.get('/analyses/search', 
      validate(resumeSchemas.searchResumeAnalyses), 
      resumeController.searchResumeAnalyses.bind(resumeController)
    );

    // Individual resume analysis routes
    router.get('/analyses/:analysisId', 
      validate(resumeSchemas.getResumeAnalysisById), 
      resumeController.getResumeAnalysisById.bind(resumeController)
    );

    router.get('/analyses/:analysisId/parsed', 
      validate(resumeSchemas.getResumeAnalysisWithParsedData), 
      resumeController.getResumeAnalysisWithParsedData.bind(resumeController)
    );

    router.put('/analyses/:analysisId', 
      validate(resumeSchemas.updateResumeAnalysis), 
      resumeController.updateResumeAnalysis.bind(resumeController)
    );

    router.delete('/analyses/:analysisId', 
      validate(resumeSchemas.deleteResumeAnalysis), 
      resumeController.deleteResumeAnalysis.bind(resumeController)
    );

    // Bulk operations
    router.delete('/analyses/bulk', 
      validate(resumeSchemas.bulkDeleteResumeAnalyses), 
      resumeController.bulkDeleteResumeAnalyses.bind(resumeController)
    );

    // User-specific resume analyses
    router.get('/analyses/user/:userId', 
      validate(resumeSchemas.getResumeAnalysesByUserId), 
      resumeController.getResumeAnalysesByUserId.bind(resumeController)
    );

    // ========================================
    // RESUME GENERATOR ROUTES
    // ========================================

    // Core resume generation
    router.post('/generate', 
      validate(resumeSchemas.generateCanadianResume), 
      resumeController.generateCanadianResume.bind(resumeController)
    );

    // Generated resume management
    router.get('/generated', 
      validate(resumeSchemas.getUserGeneratedResumes), 
      resumeController.getUserGeneratedResumes.bind(resumeController)
    );

    router.get('/generated/:resumeId', 
      validate(resumeSchemas.getGeneratedResumeById), 
      resumeController.getGeneratedResumeById.bind(resumeController)
    );

    router.put('/generated/:resumeId', 
      validate(resumeSchemas.updateGeneratedResume), 
      resumeController.updateGeneratedResume.bind(resumeController)
    );

    router.delete('/generated/:resumeId', 
      validate(resumeSchemas.deleteGeneratedResume), 
      resumeController.deleteGeneratedResume.bind(resumeController)
    );

    // Auto-save functionality
    router.patch('/generated/:resumeId/auto-save', 
      validate(resumeSchemas.autoSaveUserEdits), 
      resumeController.autoSaveUserEdits.bind(resumeController)
    );

    // Download tracking
    router.post('/generated/:resumeId/track-download', 
      resumeController.trackPDFDownload.bind(resumeController)
    );

    // Search and statistics
    router.get('/generated/search', 
      validate(resumeSchemas.searchGeneratedResumes), 
      resumeController.searchGeneratedResumes.bind(resumeController)
    );

    router.get('/generated/statistics', 
      resumeController.getGeneratedResumeStatistics.bind(resumeController)
    );

    // AI analysis and translation
    router.post('/analyze-job-targeting', 
      validate(resumeSchemas.analyzeJobTargeting), 
      resumeController.analyzeJobTargeting.bind(resumeController)
    );

    router.post('/translate-skills', 
      validate(resumeSchemas.translateSkillsForCanadianMarket), 
      resumeController.translateSkillsForCanadianMarket.bind(resumeController)
    );

    // Export functionality
    router.post('/generated/:resumeId/export', 
      validate(resumeSchemas.exportResume), 
      resumeController.exportResume.bind(resumeController)
    );

    router.get('/generated/:resumeId/download-pdf', 
      validate(resumeSchemas.downloadResumePDF), 
      resumeController.downloadResumePDF.bind(resumeController)
    );

    // Bulk operations for generated resumes
    router.delete('/generated/bulk', 
      validate(resumeSchemas.bulkDeleteGeneratedResumes), 
      resumeController.bulkDeleteGeneratedResumes.bind(resumeController)
    );

    router.post('/generated/bulk-export', 
      validate(resumeSchemas.bulkExportResumes), 
      resumeController.bulkExportResumes.bind(resumeController)
    );

    // Generation progress streaming
    router.get('/generate/:resumeId/progress', 
      resumeController.streamGenerationProgress.bind(resumeController)
    );

    // Support and templates
    router.get('/generate/support', 
      resumeController.checkGenerationSupport.bind(resumeController)
    );

    router.get('/generate/templates', 
      resumeController.getGenerationTemplates.bind(resumeController)
    );

  } catch (error) {
    console.error('Failed to initialize resume routes:', error);
    throw error;
  }
};

// Initialize routes immediately
initializeResumeRoutes().catch(console.error);

module.exports = router;
````

## File: src/routes/v1/userRoutes.js
````javascript
const express = require('express');
const { validate } = require('../../middleware/validation');
const { userSchemas } = require('../../models/schemas');
const ControllerFactory = require('../../controllers/ControllerFactory');

const router = express.Router();

/**
 * Initialize user routes with controller factory
 */
const initializeUserRoutes = async () => {
  try {
    await ControllerFactory.initialize();
    const userController = ControllerFactory.getController('user');

    // User profile routes
    router.post('/find-or-create', 
      validate(userSchemas.findOrCreateUser), 
      userController.findOrCreateUser.bind(userController)
    );

    router.get('/profile', 
      userController.getCurrentUserProfile.bind(userController)
    );

    router.put('/profile', 
      validate(userSchemas.updateProfile), 
      userController.updateCurrentUserProfile.bind(userController)
    );

    // User management routes
    router.get('/:userId', 
      validate(userSchemas.getUserById), 
      userController.getUserById.bind(userController)
    );

    router.put('/:userId', 
      validate(userSchemas.updateUser), 
      userController.updateUser.bind(userController)
    );

    router.delete('/:userId', 
      validate(userSchemas.deleteUser), 
      userController.deleteUser.bind(userController)
    );

    // User search and query routes
    router.get('/email/:email', 
      validate(userSchemas.getUserByEmail), 
      userController.getUserByEmail.bind(userController)
    );

    router.get('/search', 
      validate(userSchemas.searchUsers), 
      userController.searchUsers.bind(userController)
    );

    router.get('/', 
      validate(userSchemas.getUsers), 
      userController.getUsers.bind(userController)
    );

    // User filtering routes
    router.get('/role/:roleId', 
      validate(userSchemas.getUsersByRole), 
      userController.getUsersByRole.bind(userController)
    );

    router.get('/status/:status', 
      validate(userSchemas.getUsersByStatusInCanada), 
      userController.getUsersByStatusInCanada.bind(userController)
    );

    router.get('/country/:country', 
      validate(userSchemas.getUsersByCountryOfOrigin), 
      userController.getUsersByCountryOfOrigin.bind(userController)
    );

    router.get('/location/:location', 
      validate(userSchemas.getUsersByCurrentLocation), 
      userController.getUsersByCurrentLocation.bind(userController)
    );

    // User statistics routes
    router.get('/statistics', 
      userController.getUserStatistics.bind(userController)
    );

    router.get('/:userId/exists', 
      validate(userSchemas.userExists), 
      userController.userExists.bind(userController)
    );

    router.get('/count', 
      userController.getUserCount.bind(userController)
    );

  } catch (error) {
    console.error('Failed to initialize user routes:', error);
    throw error;
  }
};

// Initialize routes immediately
initializeUserRoutes().catch(console.error);

module.exports = router;
````

## File: src/server.js
````javascript
/**
 * Main Server Entry Point
 * Imports and configures the Express application
 */

require('dotenv').config();

const { logger } = require('./config/logger');
const { setupGlobalErrorHandlers } = require('./middleware/errorHandler');
const { getEnvironmentConfig } = require('./config/environment');

// Import the Express app
const app = require('./app');

// Setup global error handlers
setupGlobalErrorHandlers();

// Get environment configuration
const config = getEnvironmentConfig();

// Start the server
const PORT = config.server.port;

app.listen(PORT, () => {
  logger.info(`🚀 ImmiGrowAI Backend Server running on port ${PORT}`, {
    environment: config.server.nodeEnv,
    port: PORT,
    timestamp: new Date().toISOString()
  });
});

// Graceful shutdown
process.on('SIGTERM', () => {
  logger.info('SIGTERM received, shutting down gracefully');
  process.exit(0);
});

process.on('SIGINT', () => {
  logger.info('SIGINT received, shutting down gracefully');
  process.exit(0);
});
````

## File: src/services/aiConfig.js
````javascript
require('dotenv').config();

// Google AI Configuration
const aiConfig = {
  // Google AI API Settings
  googleAI: {
    apiKey: process.env.GOOGLE_AI_API_KEY || '',
    baseUrl: 'https://generativelanguage.googleapis.com',
    models: {
      flash: 'gemini-1.5-flash-001',
      pro: 'gemini-1.5-pro-001'
    }
  },
  
  // Google Custom Search Settings
  customSearch: {
    apiKey: process.env.GOOGLE_CUSTOM_SEARCH_API_KEY || '',
    engineId: process.env.GOOGLE_CUSTOM_SEARCH_ENGINE_ID || '',
    baseUrl: 'https://customsearch.googleapis.com'
  },
  
  // Rate Limiting (Google AI Free Tier)
  rateLimits: {
    maxRequestsPerMinute: parseInt(process.env.MAX_REQUESTS_PER_MINUTE) || 15,
    maxTokensPerMinute: parseInt(process.env.MAX_TOKENS_PER_MINUTE) || 1000000,
    maxRequestsPerDay: parseInt(process.env.MAX_REQUESTS_PER_DAY) || 1500
  },
  
  // File Upload Settings
  fileUpload: {
    maxFileSize: parseInt(process.env.MAX_FILE_SIZE) || 5242880, // 5MB
    allowedTypes: (process.env.ALLOWED_FILE_TYPES || '.pdf,.docx,.jpg,.jpeg,.png').split(','),
    uploadDir: './uploads/resumes'
  },
  
  // AI Feature Settings
  features: {
    resumeAnalysis: {
      enabled: true,
      maxRetries: 3,
      confidenceThreshold: 0.6
    },
    careerProfile: {
      enabled: true,
      marketAlignmentThreshold: 70
    },
    mentorMatching: {
      enabled: true,
      maxMatches: 10,
      minCompatibilityScore: 60
    },
    jobDiscovery: {
      enabled: true,
      searchInterval: 24, // hours
      maxJobsPerSearch: 100
    },
    coaching: {
      enabled: true,
      maxSessionHistory: 50,
      sessionTimeoutMinutes: 30
    }
  },
  
  // Validation
  validate() {
    const required = ['GOOGLE_AI_API_KEY'];
    const missing = required.filter(key => !process.env[key]);
    
    if (missing.length > 0) {
      throw new Error(`Missing required environment variables: ${missing.join(', ')}`);
    }
    
    return true;
  }
};

module.exports = aiConfig;
````

## File: src/services/BaseService.js
````javascript
const { logger } = require('../config/logger');
const { AppError } = require('../utils/errors');

/**
 * Base Service class providing common service functionality
 * All specific services should extend this class
 */
class BaseService {
  constructor(repositories = {}) {
    this.repositories = repositories;
    this.logger = logger;
  }

  /**
   * Get a repository by name
   * @param {string} repositoryName - Name of the repository
   * @returns {Object} Repository instance
   */
  getRepository(repositoryName) {
    const repository = this.repositories[repositoryName];
    if (!repository) {
      throw new AppError(`Repository '${repositoryName}' not found`, 500);
    }
    return repository;
  }

  /**
   * Log service method entry
   * @param {string} methodName - Name of the method being called
   * @param {Object} params - Method parameters
   */
  logMethodEntry(methodName, params = {}) {
    this.logger.info(`Service method called: ${this.constructor.name}.${methodName}`, {
      method: methodName,
      params: this.sanitizeParams(params),
      timestamp: new Date().toISOString()
    });
  }

  /**
   * Log service method success
   * @param {string} methodName - Name of the method
   * @param {Object} result - Method result
   */
  logMethodSuccess(methodName, result = {}) {
    this.logger.info(`Service method completed: ${this.constructor.name}.${methodName}`, {
      method: methodName,
      resultType: typeof result,
      resultKeys: Array.isArray(result) ? `Array(${result.length})` : (result && typeof result === 'object' ? Object.keys(result) : 'primitive'),
      timestamp: new Date().toISOString()
    });
  }

  /**
   * Log service method error
   * @param {string} methodName - Name of the method
   * @param {Error} error - Error that occurred
   */
  logMethodError(methodName, error) {
    this.logger.error(`Service method failed: ${this.constructor.name}.${methodName}`, {
      method: methodName,
      error: error.message,
      stack: error.stack,
      timestamp: new Date().toISOString()
    });
  }

  /**
   * Sanitize parameters for logging (remove sensitive data)
   * @param {Object} params - Parameters to sanitize
   * @returns {Object} Sanitized parameters
   */
  sanitizeParams(params) {
    if (!params || typeof params !== 'object') {
      return params;
    }

    const sanitized = { ...params };
    const sensitiveFields = ['password', 'token', 'secret', 'key', 'authorization'];

    // Remove sensitive fields
    sensitiveFields.forEach(field => {
      if (sanitized[field]) {
        sanitized[field] = '[REDACTED]';
      }
    });

    // Handle nested objects
    Object.keys(sanitized).forEach(key => {
      if (sanitized[key] && typeof sanitized[key] === 'object') {
        sanitized[key] = this.sanitizeParams(sanitized[key]);
      }
    });

    return sanitized;
  }

  /**
   * Validate required parameters
   * @param {Object} params - Parameters to validate
   * @param {Array} requiredFields - Array of required field names
   * @throws {AppError} If required fields are missing
   */
  validateRequiredParams(params, requiredFields) {
    if (!params || typeof params !== 'object') {
      throw new AppError('Invalid parameters provided', 400);
    }

    const missingFields = requiredFields.filter(field => {
      return params[field] === undefined || params[field] === null || params[field] === '';
    });

    if (missingFields.length > 0) {
      throw new AppError(`Missing required fields: ${missingFields.join(', ')}`, 400);
    }
  }

  /**
   * Validate user ID format
   * @param {string|number} userId - User ID to validate
   * @returns {number} Validated numeric user ID
   * @throws {AppError} If user ID is invalid
   */
  validateUserId(userId) {
    if (!userId) {
      throw new AppError('User ID is required', 400);
    }

    const numericUserId = parseInt(userId);
    if (isNaN(numericUserId) || numericUserId <= 0) {
      throw new AppError('Invalid user ID format', 400);
    }

    return numericUserId;
  }

  /**
   * Handle service method execution with logging and error handling
   * @param {string} methodName - Name of the method
   * @param {Function} method - Method to execute
   * @param {Object} params - Parameters to pass to the method
   * @returns {Promise<any>} Method result
   */
  async executeMethod(methodName, method, params = {}) {
    try {
      this.logMethodEntry(methodName, params);
      const result = await method.call(this, params);
      this.logMethodSuccess(methodName, result);
      return result;
    } catch (error) {
      this.logMethodError(methodName, error);
      throw error;
    }
  }

  /**
   * Create a paginated response
   * @param {Array} data - Data array
   * @param {number} total - Total count
   * @param {number} limit - Page limit
   * @param {number} offset - Page offset
   * @returns {Object} Paginated response object
   */
  createPaginatedResponse(data, total, limit, offset) {
    return {
      data,
      pagination: {
        total,
        limit,
        offset,
        hasMore: (offset + limit) < total,
        totalPages: Math.ceil(total / limit),
        currentPage: Math.floor(offset / limit) + 1
      }
    };
  }

  /**
   * Transform database record to API response format
   * @param {Object} record - Database record
   * @param {Object} transformations - Field transformations
   * @returns {Object} Transformed record
   */
  transformRecord(record, transformations = {}) {
    if (!record) return null;

    const transformed = { ...record };

    // Apply field transformations
    Object.entries(transformations).forEach(([oldKey, newKey]) => {
      if (transformed[oldKey] !== undefined) {
        transformed[newKey] = transformed[oldKey];
        delete transformed[oldKey];
      }
    });

    return transformed;
  }

  /**
   * Transform array of database records
   * @param {Array} records - Array of database records
   * @param {Object} transformations - Field transformations
   * @returns {Array} Transformed records
   */
  transformRecords(records, transformations = {}) {
    if (!Array.isArray(records)) return [];
    return records.map(record => this.transformRecord(record, transformations));
  }

  /**
   * Check if user has permission to access resource
   * @param {string|number} userId - User ID
   * @param {string|number} resourceUserId - Resource owner's user ID
   * @param {boolean} isAdmin - Whether user is admin
   * @returns {boolean} Whether user has permission
   */
  hasPermission(userId, resourceUserId, isAdmin = false) {
    const numericUserId = this.validateUserId(userId);
    const numericResourceUserId = this.validateUserId(resourceUserId);

    // Admin can access any resource
    if (isAdmin) return true;

    // User can only access their own resources
    return numericUserId === numericResourceUserId;
  }

  /**
   * Validate and sanitize search criteria
   * @param {Object} criteria - Search criteria
   * @param {Array} allowedFields - Allowed field names
   * @returns {Object} Sanitized criteria
   */
  sanitizeSearchCriteria(criteria, allowedFields) {
    if (!criteria || typeof criteria !== 'object') {
      return {};
    }

    const sanitized = {};
    Object.keys(criteria).forEach(key => {
      if (allowedFields.includes(key) && criteria[key] !== undefined && criteria[key] !== null) {
        sanitized[key] = criteria[key];
      }
    });

    return sanitized;
  }

  /**
   * Validate pagination parameters
   * @param {Object} options - Pagination options
   * @param {number} maxLimit - Maximum allowed limit
   * @returns {Object} Validated pagination options
   */
  validatePaginationOptions(options = {}, maxLimit = 100) {
    const limit = Math.min(parseInt(options.limit) || 10, maxLimit);
    const offset = Math.max(parseInt(options.offset) || 0, 0);

    return { limit, offset };
  }
}

module.exports = BaseService;
````

## File: src/services/CanadianResumeService.js
````javascript
const BaseService = require('./BaseService');
const { GoogleGenerativeAI } = require('@google/generative-ai');
const { AppError } = require('../utils/errors');
const { 
  RESUME_GENERATION_PROMPT, 
  JOB_TARGETING_ANALYSIS_PROMPT, 
  ATS_OPTIMIZATION_PROMPT,
  SKILLS_TRANSLATION_PROMPT,
  CANADIAN_MARKET_INTELLIGENCE_PROMPT,
  createResumeGenerationPrompt,
  createJobTargetingAnalysisPrompt,
  createATSOptimizationPrompt,
  createSkillsTranslationPrompt,
  createCanadianMarketIntelligencePrompt
} = require('../prompts/resumeGenerator');

/**
 * Canadian Resume Service for AI-powered resume generation
 * Integrates with Gemini AI for Canadian job market optimization
 */
class CanadianResumeService extends BaseService {
  constructor(repositories) {
    super(repositories);
    this.generatedResumeRepository = this.getRepository('generatedResume');
    this.resumeRepository = this.getRepository('resume');
    this.userRepository = this.getRepository('user');
    
    // Initialize Gemini AI
    this.genAI = new GoogleGenerativeAI(process.env.GEMINI_API_KEY);
    this.model = this.genAI.getGenerativeModel({ 
      model: "gemini-1.5-flash",
      generationConfig: {
        temperature: 0.1, // Low temperature for consistent structured output
        topK: 1,
        topP: 1,
        maxOutputTokens: 8192,
      }
    });
    
    // Rate limiting
    this.requestCount = {
      minute: { count: 0, resetTime: Date.now() + 60000 },
      day: { count: 0, resetTime: Date.now() + 86400000 }
    };
    
    this.maxRequestsPerMinute = 1000;
    this.maxRequestsPerDay = 50000;
  }

  /**
   * Check and enforce rate limits
   * @throws {Error} If rate limit exceeded
   */
  checkRateLimit() {
    const now = Date.now();
    
    if (now > this.requestCount.minute.resetTime) {
      this.requestCount.minute = { count: 0, resetTime: now + 60000 };
    }
    
    if (now > this.requestCount.day.resetTime) {
      this.requestCount.day = { count: 0, resetTime: now + 86400000 };
    }
    
    if (this.requestCount.minute.count >= this.maxRequestsPerMinute) {
      throw new Error('Rate limit exceeded: too many requests per minute (1000/min limit)');
    }
    
    if (this.requestCount.day.count >= this.maxRequestsPerDay) {
      throw new Error('Rate limit exceeded: too many requests per day');
    }
    
    return true;
  }

  /**
   * Increment request count for rate limiting
   */
  incrementRequestCount() {
    this.requestCount.minute.count++;
    this.requestCount.day.count++;
  }

  /**
   * Generate a Canadian resume using AI
   * @param {string|number} userId - User ID
   * @param {string|number} originalAnalysisId - Original resume analysis ID
   * @param {Object} jobTargeting - Job targeting information
   * @returns {Promise<Object>} Generated resume with metadata
   */
  async generateCanadianResume(userId, originalAnalysisId, jobTargeting) {
    return this.executeMethod('generateCanadianResume', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      this.validateRequiredParams(params.jobTargeting, ['jobTitle', 'companyName']);
      
      // Verify user exists
      const user = await this.userRepository.findById(validatedUserId, true);
      if (!user) {
        throw new AppError('User not found', 404);
      }

      // Get original resume analysis
      const originalAnalysis = await this.resumeRepository.findById(params.originalAnalysisId, true);
      if (!originalAnalysis) {
        throw new AppError('Original resume analysis not found', 404);
      }

      // Check rate limits
      this.checkRateLimit();

      try {
        // Generate resume using AI
        const generatedResumeData = await this.generateResumeWithAI(originalAnalysis, params.jobTargeting);
        
        // Calculate ATS score
        const atsScore = await this.calculateATSScore(generatedResumeData, params.jobTargeting);
        
        // Generate AI suggestions
        const aiSuggestions = await this.generateAISuggestions(generatedResumeData, params.jobTargeting);
        
        // Save generated resume to database
        const generatedResume = await this.generatedResumeRepository.createGeneratedResume(
          generatedResumeData,
          validatedUserId,
          params.originalAnalysisId,
          params.jobTargeting
        );

        // Update with ATS score and suggestions
        await this.generatedResumeRepository.updateATSScore(generatedResume.id, atsScore, true);
        await this.generatedResumeRepository.updateAISuggestions(generatedResume.id, aiSuggestions, true);

        return {
          id: generatedResume.id,
          resumeData: generatedResumeData,
          atsScore,
          aiSuggestions,
          jobTargeting: params.jobTargeting,
          status: generatedResume.status,
          createdAt: generatedResume.created_at,
          template: params.jobTargeting.template || 'canadian_classic'
        };

      } catch (error) {
        this.logger.error('❌ Error generating Canadian resume:', error);
        throw new AppError(`Failed to generate resume: ${error.message}`, 500);
      }
    }, { userId, originalAnalysisId, jobTargeting });
  }

  /**
   * Generate resume content using AI
   * @param {Object} originalAnalysis - Original resume analysis
   * @param {Object} jobTargeting - Job targeting information
   * @returns {Promise<Object>} Generated resume data
   */
  async generateResumeWithAI(originalAnalysis, jobTargeting) {
    try {
      const prompt = createResumeGenerationPrompt(originalAnalysis, jobTargeting);
      
      const result = await this.model.generateContent(prompt);
      const response = await result.response;
      const generatedText = response.text();
      
      this.incrementRequestCount();
      
      // Parse JSON response
      let resumeData;
      try {
        resumeData = JSON.parse(generatedText);
      } catch (parseError) {
        // Try to extract JSON from response if it's wrapped in markdown
        const jsonMatch = generatedText.match(/```json\n([\s\S]*?)\n```/) || 
                         generatedText.match(/\{[\s\S]*\}/);
        if (jsonMatch) {
          resumeData = JSON.parse(jsonMatch[1] || jsonMatch[0]);
        } else {
          throw new Error('Failed to parse AI response as JSON');
        }
      }

      // Validate generated resume structure
      this.validateGeneratedResume(resumeData);
      
      return resumeData;
    } catch (error) {
      this.logger.error('❌ Error in AI resume generation:', error);
      throw new AppError(`AI resume generation failed: ${error.message}`, 500);
    }
  }

  /**
   * Calculate ATS score for generated resume
   * @param {Object} resumeData - Generated resume data
   * @param {Object} jobTargeting - Job targeting information
   * @returns {Promise<number>} ATS score (0-100)
   */
  async calculateATSScore(resumeData, jobTargeting) {
    try {
      const prompt = createATSOptimizationPrompt(resumeData, jobTargeting);
      
      const result = await this.model.generateContent(prompt);
      const response = await result.response;
      const scoreText = response.text();
      
      this.incrementRequestCount();
      
      // Extract score from response
      const scoreMatch = scoreText.match(/score["\s:]*(\d+)/i) || 
                        scoreText.match(/(\d+)/);
      
      if (scoreMatch) {
        const score = parseInt(scoreMatch[1]);
        return Math.min(Math.max(score, 0), 100); // Ensure score is between 0-100
      }
      
      // Default score if parsing fails
      return 75;
    } catch (error) {
      this.logger.error('❌ Error calculating ATS score:', error);
      return 75; // Default score on error
    }
  }

  /**
   * Generate AI suggestions for resume improvement
   * @param {Object} resumeData - Generated resume data
   * @param {Object} jobTargeting - Job targeting information
   * @returns {Promise<Array>} AI suggestions
   */
  async generateAISuggestions(resumeData, jobTargeting) {
    try {
      const prompt = createCanadianMarketIntelligencePrompt(resumeData, jobTargeting);
      
      const result = await this.model.generateContent(prompt);
      const response = await result.response;
      const suggestionsText = response.text();
      
      this.incrementRequestCount();
      
      // Parse suggestions from response
      let suggestions;
      try {
        suggestions = JSON.parse(suggestionsText);
      } catch (parseError) {
        // Try to extract JSON from response
        const jsonMatch = suggestionsText.match(/```json\n([\s\S]*?)\n```/) || 
                         suggestionsText.match(/\[[\s\S]*\]/);
        if (jsonMatch) {
          suggestions = JSON.parse(jsonMatch[1] || jsonMatch[0]);
        } else {
          // Fallback: create basic suggestions
          suggestions = [
            {
              category: 'general',
              suggestion: 'Consider adding more quantifiable achievements to your experience section.',
              priority: 'medium'
            }
          ];
        }
      }
      
      return Array.isArray(suggestions) ? suggestions : [];
    } catch (error) {
      this.logger.error('❌ Error generating AI suggestions:', error);
      return []; // Return empty array on error
    }
  }

  /**
   * Analyze job description for targeting
   * @param {string} jobDescription - Job description text
   * @param {Object} userProfile - User profile information
   * @returns {Promise<Object>} Job targeting analysis
   */
  async analyzeJobTargeting(jobDescription, userProfile) {
    return this.executeMethod('analyzeJobTargeting', async (params) => {
      this.validateRequiredParams(params, ['jobDescription']);
      
      this.checkRateLimit();

      try {
        const prompt = createJobTargetingAnalysisPrompt(params.jobDescription, params.userProfile);
        
        const result = await this.model.generateContent(prompt);
        const response = await result.response;
        const analysisText = response.text();
        
        this.incrementRequestCount();
        
        // Parse analysis from response
        let analysis;
        try {
          analysis = JSON.parse(analysisText);
        } catch (parseError) {
          const jsonMatch = analysisText.match(/```json\n([\s\S]*?)\n```/) || 
                           analysisText.match(/\{[\s\S]*\}/);
          if (jsonMatch) {
            analysis = JSON.parse(jsonMatch[1] || jsonMatch[0]);
          } else {
            throw new Error('Failed to parse job targeting analysis');
          }
        }
        
        return analysis;
      } catch (error) {
        this.logger.error('❌ Error analyzing job targeting:', error);
        throw new AppError(`Job targeting analysis failed: ${error.message}`, 500);
      }
    }, { jobDescription, userProfile });
  }

  /**
   * Translate skills for Canadian market
   * @param {Array} skills - User skills
   * @param {string} targetIndustry - Target industry
   * @returns {Promise<Array>} Translated skills
   */
  async translateSkillsForCanadianMarket(skills, targetIndustry) {
    return this.executeMethod('translateSkillsForCanadianMarket', async (params) => {
      this.validateRequiredParams(params, ['skills']);
      
      this.checkRateLimit();

      try {
        const prompt = createSkillsTranslationPrompt(params.skills, params.targetIndustry);
        
        const result = await this.model.generateContent(prompt);
        const response = await result.response;
        const translationText = response.text();
        
        this.incrementRequestCount();
        
        // Parse translation from response
        let translatedSkills;
        try {
          translatedSkills = JSON.parse(translationText);
        } catch (parseError) {
          const jsonMatch = translationText.match(/```json\n([\s\S]*?)\n```/) || 
                           translationText.match(/\[[\s\S]*\]/);
          if (jsonMatch) {
            translatedSkills = JSON.parse(jsonMatch[1] || jsonMatch[0]);
          } else {
            throw new Error('Failed to parse skills translation');
          }
        }
        
        return Array.isArray(translatedSkills) ? translatedSkills : params.skills;
      } catch (error) {
        this.logger.error('❌ Error translating skills:', error);
        return params.skills; // Return original skills on error
      }
    }, { skills, targetIndustry });
  }

  /**
   * Get generated resumes for a user
   * @param {string|number} userId - User ID
   * @param {Object} options - Query options
   * @returns {Promise<Object>} Generated resumes with pagination
   */
  async getUserGeneratedResumes(userId, options = {}) {
    return this.executeMethod('getUserGeneratedResumes', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      const paginationOptions = this.validatePaginationOptions(params.options, 50);

      const result = await this.generatedResumeRepository.getGeneratedResumesWithPagination(
        validatedUserId, 
        paginationOptions, 
        false
      );

      return this.createPaginatedResponse(
        result.resumes,
        result.pagination.total,
        result.pagination.limit,
        result.pagination.offset
      );
    }, { userId, options });
  }

  /**
   * Get generated resume by ID
   * @param {string|number} resumeId - Generated resume ID
   * @param {string|number} userId - User ID for permission check
   * @returns {Promise<Object>} Generated resume
   */
  async getGeneratedResumeById(resumeId, userId) {
    return this.executeMethod('getGeneratedResumeById', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      const resume = await this.generatedResumeRepository.getGeneratedResumeById(params.resumeId, false);
      if (!resume) {
        throw new AppError('Generated resume not found', 404);
      }

      // Check permissions
      if (!this.hasPermission(validatedUserId, resume.user_id)) {
        throw new AppError('Access denied', 403);
      }

      return this.transformRecord(resume, {
        user_id: 'userId',
        original_analysis_id: 'originalAnalysisId',
        job_title: 'jobTitle',
        job_description: 'jobDescription',
        company_name: 'companyName',
        industry: 'industry',
        location: 'location',
        resume_data: 'resumeData',
        user_edits: 'userEdits',
        ai_suggestions: 'aiSuggestions',
        ats_score: 'atsScore',
        status: 'status',
        pdf_downloaded_count: 'pdfDownloadedCount',
        template_used: 'templateUsed',
        generation_version: 'generationVersion',
        created_at: 'createdAt',
        last_updated: 'lastUpdated'
      });
    }, { resumeId, userId });
  }

  /**
   * Update generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {string|number} userId - User ID
   * @param {Object} updateData - Data to update
   * @returns {Promise<Object>} Updated resume
   */
  async updateGeneratedResume(resumeId, userId, updateData) {
    return this.executeMethod('updateGeneratedResume', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      // Get current resume for permission check
      const currentResume = await this.generatedResumeRepository.getGeneratedResumeById(params.resumeId, false);
      if (!currentResume) {
        throw new AppError('Generated resume not found', 404);
      }

      // Check permissions
      if (!this.hasPermission(validatedUserId, currentResume.user_id)) {
        throw new AppError('Access denied', 403);
      }

      const updatedResume = await this.generatedResumeRepository.updateGeneratedResume(
        params.resumeId, 
        params.updateData, 
        false
      );

      return this.transformRecord(updatedResume, {
        user_id: 'userId',
        original_analysis_id: 'originalAnalysisId',
        job_title: 'jobTitle',
        job_description: 'jobDescription',
        company_name: 'companyName',
        industry: 'industry',
        location: 'location',
        resume_data: 'resumeData',
        user_edits: 'userEdits',
        ai_suggestions: 'aiSuggestions',
        ats_score: 'atsScore',
        status: 'status',
        pdf_downloaded_count: 'pdfDownloadedCount',
        template_used: 'templateUsed',
        generation_version: 'generationVersion',
        created_at: 'createdAt',
        last_updated: 'lastUpdated'
      });
    }, { resumeId, userId, updateData });
  }

  /**
   * Auto-save user edits
   * @param {string|number} resumeId - Generated resume ID
   * @param {string|number} userId - User ID
   * @param {Object} userEdits - User edits data
   * @returns {Promise<Object>} Updated resume
   */
  async autoSaveUserEdits(resumeId, userId, userEdits) {
    return this.executeMethod('autoSaveUserEdits', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      // Get current resume for permission check
      const currentResume = await this.generatedResumeRepository.getGeneratedResumeById(params.resumeId, false);
      if (!currentResume) {
        throw new AppError('Generated resume not found', 404);
      }

      // Check permissions
      if (!this.hasPermission(validatedUserId, currentResume.user_id)) {
        throw new AppError('Access denied', 403);
      }

      const updatedResume = await this.generatedResumeRepository.autoSaveUserEdits(
        params.resumeId, 
        params.userEdits, 
        false
      );

      return this.transformRecord(updatedResume, {
        user_id: 'userId',
        original_analysis_id: 'originalAnalysisId',
        job_title: 'jobTitle',
        job_description: 'jobDescription',
        company_name: 'companyName',
        industry: 'industry',
        location: 'location',
        resume_data: 'resumeData',
        user_edits: 'userEdits',
        ai_suggestions: 'aiSuggestions',
        ats_score: 'atsScore',
        status: 'status',
        pdf_downloaded_count: 'pdfDownloadedCount',
        template_used: 'templateUsed',
        generation_version: 'generationVersion',
        created_at: 'createdAt',
        last_updated: 'lastUpdated'
      });
    }, { resumeId, userId, userEdits });
  }

  /**
   * Track PDF download
   * @param {string|number} resumeId - Generated resume ID
   * @param {string|number} userId - User ID
   * @returns {Promise<Object>} Updated resume
   */
  async trackPDFDownload(resumeId, userId) {
    return this.executeMethod('trackPDFDownload', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      // Get current resume for permission check
      const currentResume = await this.generatedResumeRepository.getGeneratedResumeById(params.resumeId, false);
      if (!currentResume) {
        throw new AppError('Generated resume not found', 404);
      }

      // Check permissions
      if (!this.hasPermission(validatedUserId, currentResume.user_id)) {
        throw new AppError('Access denied', 403);
      }

      const updatedResume = await this.generatedResumeRepository.trackPDFDownload(params.resumeId, false);

      return this.transformRecord(updatedResume, {
        user_id: 'userId',
        original_analysis_id: 'originalAnalysisId',
        job_title: 'jobTitle',
        job_description: 'jobDescription',
        company_name: 'companyName',
        industry: 'industry',
        location: 'location',
        resume_data: 'resumeData',
        user_edits: 'userEdits',
        ai_suggestions: 'aiSuggestions',
        ats_score: 'atsScore',
        status: 'status',
        pdf_downloaded_count: 'pdfDownloadedCount',
        template_used: 'templateUsed',
        generation_version: 'generationVersion',
        created_at: 'createdAt',
        last_updated: 'lastUpdated'
      });
    }, { resumeId, userId });
  }

  /**
   * Delete generated resume
   * @param {string|number} resumeId - Generated resume ID
   * @param {string|number} userId - User ID
   * @returns {Promise<boolean>} Success status
   */
  async deleteGeneratedResume(resumeId, userId) {
    return this.executeMethod('deleteGeneratedResume', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      // Get current resume for permission check
      const currentResume = await this.generatedResumeRepository.getGeneratedResumeById(params.resumeId, false);
      if (!currentResume) {
        throw new AppError('Generated resume not found', 404);
      }

      // Check permissions
      if (!this.hasPermission(validatedUserId, currentResume.user_id)) {
        throw new AppError('Access denied', 403);
      }

      return await this.generatedResumeRepository.deleteGeneratedResume(params.resumeId, false);
    }, { resumeId, userId });
  }

  /**
   * Search generated resumes
   * @param {string|number} userId - User ID
   * @param {Object} criteria - Search criteria
   * @param {Object} options - Query options
   * @returns {Promise<Array>} Matching resumes
   */
  async searchGeneratedResumes(userId, criteria = {}, options = {}) {
    return this.executeMethod('searchGeneratedResumes', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      // Add user ID to search criteria
      const searchCriteria = { ...params.criteria, userId: validatedUserId };
      
      const resumes = await this.generatedResumeRepository.searchGeneratedResumes(
        searchCriteria, 
        params.options, 
        false
      );

      return this.transformRecords(resumes, {
        user_id: 'userId',
        original_analysis_id: 'originalAnalysisId',
        job_title: 'jobTitle',
        job_description: 'jobDescription',
        company_name: 'companyName',
        industry: 'industry',
        location: 'location',
        resume_data: 'resumeData',
        user_edits: 'userEdits',
        ai_suggestions: 'aiSuggestions',
        ats_score: 'atsScore',
        status: 'status',
        pdf_downloaded_count: 'pdfDownloadedCount',
        template_used: 'templateUsed',
        generation_version: 'generationVersion',
        created_at: 'createdAt',
        last_updated: 'lastUpdated'
      });
    }, { userId, criteria, options });
  }

  /**
   * Get generated resume statistics
   * @param {string|number} userId - User ID
   * @returns {Promise<Object>} Statistics
   */
  async getGeneratedResumeStatistics(userId) {
    return this.executeMethod('getGeneratedResumeStatistics', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      const statistics = await this.generatedResumeRepository.getGeneratedResumeStatistics(false);
      
      // Filter statistics for specific user if needed
      const userResumes = await this.generatedResumeRepository.getGeneratedResumes(validatedUserId, false);
      
      return {
        global: statistics,
        user: {
          totalResumes: userResumes.length,
          byStatus: userResumes.reduce((acc, resume) => {
            const status = resume.status || 'draft';
            acc[status] = (acc[status] || 0) + 1;
            return acc;
          }, {}),
          byTemplate: userResumes.reduce((acc, resume) => {
            const template = resume.template_used || 'canadian_classic';
            acc[template] = (acc[template] || 0) + 1;
            return acc;
          }, {})
        }
      };
    }, { userId });
  }

  /**
   * Validate generated resume structure
   * @param {Object} resumeData - Generated resume data
   * @throws {AppError} If validation fails
   */
  validateGeneratedResume(resumeData) {
    if (!resumeData || typeof resumeData !== 'object') {
      throw new AppError('Invalid resume data structure', 400);
    }

    const requiredSections = ['personalInfo', 'professionalSummary', 'workExperience', 'education', 'skills'];
    const missingSections = requiredSections.filter(section => !resumeData[section]);

    if (missingSections.length > 0) {
      throw new AppError(`Missing required resume sections: ${missingSections.join(', ')}`, 400);
    }

    // Validate personal info
    if (!resumeData.personalInfo.name || !resumeData.personalInfo.email) {
      throw new AppError('Personal info must include name and email', 400);
    }

    // Validate work experience
    if (!Array.isArray(resumeData.workExperience) || resumeData.workExperience.length === 0) {
      throw new AppError('Work experience must be a non-empty array', 400);
    }

    // Validate skills
    if (!Array.isArray(resumeData.skills) || resumeData.skills.length === 0) {
      throw new AppError('Skills must be a non-empty array', 400);
    }
  }
}

module.exports = CanadianResumeService;
````

## File: src/services/CareerProfileService.js
````javascript
const { GoogleGenerativeAI } = require('@google/generative-ai');
const GeminiResumeService = require('./GeminiResumeService');
const SupabaseDatabase = require('./supabaseDatabase');
const { 
  POSITION_RECOMMENDATION_PROMPT, 
  ENHANCED_PROFILE_PROMPT, 
  SKILL_GAP_ANALYSIS_PROMPT, 
  RESUME_GENERATION_PROMPT 
} = require('../prompts/career');

class CareerProfileService extends GeminiResumeService {
  constructor() {
    super();
    this.supabaseDb = new SupabaseDatabase();
    
    // Use Gemini 1.5 Pro for complex career analysis
    this.proModel = this.genAI.getGenerativeModel({ 
      model: "gemini-1.5-pro",
      generationConfig: {
        temperature: 0.2, // Slightly higher for creative recommendations
        topK: 40,
        topP: 0.95,
        maxOutputTokens: 8192,
      }
    });
  }

  /**
   * Generate position recommendations based on resume analysis
   * @param {Object} resumeAnalysis - Analyzed resume data
   * @param {Object} userProfile - User's career profile data
   * @returns {Array} Array of position recommendations with success probabilities
   */
  async generatePositionRecommendations(resumeAnalysis, userProfile = {}) {
    this.checkRateLimit();
    
    try {
      console.log('🎯 Generating position recommendations...');
      
      const prompt = POSITION_RECOMMENDATION_PROMPT(resumeAnalysis, userProfile);
      
      const result = await this.proModel.generateContent(prompt);
      const response = await result.response;
      const recommendationsText = response.text();
      
      this.incrementRequestCount();
      
      // Parse JSON response
      let recommendations;
      try {
        recommendations = JSON.parse(recommendationsText);
      } catch (parseError) {
        const jsonMatch = recommendationsText.match(/```json\n([\s\S]*?)\n```/) || 
                         recommendationsText.match(/\{[\s\S]*\}/);
        if (jsonMatch) {
          recommendations = JSON.parse(jsonMatch[1] || jsonMatch[0]);
        } else {
          throw new Error('Failed to parse AI response as JSON');
        }
      }
      
      // Validate and sort recommendations by success probability
      recommendations = this.validateRecommendations(recommendations);
      
      console.log(`✅ Generated ${recommendations.positions.length} position recommendations`);
      return recommendations;
      
    } catch (error) {
      console.error('❌ Position recommendation error:', error);
      throw new Error(`Position recommendation failed: ${error.message}`);
    }
  }

  /**
   * Generate enhanced profile for a specific position
   * @param {Object} resumeAnalysis - Analyzed resume data
   * @param {Object} targetPosition - Selected position details
   * @param {Object} userPreferences - User's career preferences
   * @returns {Object} Enhanced career profile for the position
   */
  async generateEnhancedProfile(resumeAnalysis, targetPosition, userPreferences = {}) {
    this.checkRateLimit();
    
    try {
      console.log(`🚀 Generating enhanced profile for: ${targetPosition.title}`);
      
      const prompt = ENHANCED_PROFILE_PROMPT(resumeAnalysis, targetPosition, userPreferences);
      
      const result = await this.proModel.generateContent(prompt);
      const response = await result.response;
      const profileText = response.text();
      
      this.incrementRequestCount();
      
      // Parse JSON response
      let enhancedProfile;
      try {
        enhancedProfile = JSON.parse(profileText);
      } catch (parseError) {
        const jsonMatch = profileText.match(/```json\n([\s\S]*?)\n```/) || 
                         profileText.match(/\{[\s\S]*\}/);
        if (jsonMatch) {
          enhancedProfile = JSON.parse(jsonMatch[1] || jsonMatch[0]);
        } else {
          throw new Error('Failed to parse AI response as JSON');
        }
      }
      
      // Validate and enhance the profile
      enhancedProfile = this.validateEnhancedProfile(enhancedProfile, targetPosition);
      
      console.log('✅ Enhanced profile generated successfully');
      return enhancedProfile;
      
    } catch (error) {
      console.error('❌ Enhanced profile generation error:', error);
      throw new Error(`Enhanced profile generation failed: ${error.message}`);
    }
  }

  /**
   * Generate detailed skill gap analysis for a target position
   * @param {Object} resumeAnalysis - Analyzed resume data
   * @param {Object} targetPosition - Target position requirements
   * @returns {Object} Detailed skill gap analysis
   */
  async generateSkillGapAnalysis(resumeAnalysis, targetPosition) {
    this.checkRateLimit();
    
    try {
      console.log(`📊 Analyzing skill gaps for: ${targetPosition.title}`);
      
      const prompt = SKILL_GAP_ANALYSIS_PROMPT(resumeAnalysis, targetPosition);
      
      const result = await this.proModel.generateContent(prompt);
      const response = await result.response;
      const analysisText = response.text();
      
      this.incrementRequestCount();
      
      // Parse JSON response
      let skillGapAnalysis;
      try {
        skillGapAnalysis = JSON.parse(analysisText);
      } catch (parseError) {
        const jsonMatch = analysisText.match(/```json\n([\s\S]*?)\n```/) || 
                         analysisText.match(/\{[\s\S]*\}/);
        if (jsonMatch) {
          skillGapAnalysis = JSON.parse(jsonMatch[1] || jsonMatch[0]);
        } else {
          throw new Error('Failed to parse AI response as JSON');
        }
      }
      
      console.log('✅ Skill gap analysis completed');
      return skillGapAnalysis;
      
    } catch (error) {
      console.error('❌ Skill gap analysis error:', error);
      throw new Error(`Skill gap analysis failed: ${error.message}`);
    }
  }

  /**
   * Generate an optimized resume for a specific career path
   * @param {Object} userProfile - User's career profile and preferences
   * @param {Object} targetPosition - Selected career path/position
   * @param {Object} existingAnalysis - Optional existing resume analysis for reference
   * @returns {Object} Generated resume in structured JSON format
   */
  async generateOptimizedResume(userProfile, targetPosition, existingAnalysis = null) {
    this.checkRateLimit();
    
    try {
      console.log(`🎯 Generating optimized resume for: ${targetPosition.title}`);
      
      const prompt = RESUME_GENERATION_PROMPT(userProfile, targetPosition, existingAnalysis);
      
      const result = await this.proModel.generateContent(prompt);
      const response = await result.response;
      const resumeText = response.text();
      
      this.incrementRequestCount();
      
      // Parse JSON response
      let generatedResume;
      try {
        generatedResume = JSON.parse(resumeText);
      } catch (parseError) {
        const jsonMatch = resumeText.match(/```json\n([\s\S]*?)\n```/) || 
                         resumeText.match(/\{[\s\S]*\}/);
        if (jsonMatch) {
          generatedResume = JSON.parse(jsonMatch[1] || jsonMatch[0]);
        } else {
          throw new Error('Failed to parse AI response as JSON');
        }
      }
      
      // Validate and enhance the generated resume
      generatedResume = this.validateGeneratedResume(generatedResume, targetPosition);
      
      console.log('✅ Optimized resume generated successfully');
      return generatedResume;
      
    } catch (error) {
      console.error('❌ Resume generation error:', error);
      throw new Error(`Resume generation failed: ${error.message}`);
    }
  }









  // Validate position recommendations
  validateRecommendations(recommendations) {
    // Ensure required structure
    if (!recommendations.positions || !Array.isArray(recommendations.positions)) {
      recommendations.positions = [];
    }
    
    // Sort by success probability (highest first)
    recommendations.positions.sort((a, b) => (b.successProbability || 0) - (a.successProbability || 0));
    
    // Validate each position
    recommendations.positions = recommendations.positions.map(position => ({
      title: position.title || 'Unknown Position',
      industry: position.industry || 'Various',
      level: position.level || 'Mid',
      successProbability: Math.min(1.0, Math.max(0.0, position.successProbability || 0)),
      matchScore: Math.min(1.0, Math.max(0.0, position.matchScore || 0)),
      salaryRange: position.salaryRange || { min: 40000, max: 60000, currency: 'CAD' },
      ...position
    }));
    
    return recommendations;
  }

  // Validate enhanced profile
  validateEnhancedProfile(profile, targetPosition) {
    // Ensure required structure exists
    const defaults = {
      enhancedProfile: {
        optimizedSummary: '',
        keyStrengths: [],
        skillsPresentation: { technical: {}, soft: {} },
        experienceRepositioning: []
      },
      applicationStrategy: {
        coverLetterTemplate: '',
        resumeOptimizations: {},
        interviewPreparation: {}
      },
      skillDevelopment: {
        immediateActions: [],
        mediumTermGoals: [],
        certificationRoadmap: []
      }
    };
    
    // Deep merge with defaults
    profile = { ...defaults, ...profile };
    
    // Add metadata
    profile.metadata = {
      targetPosition: targetPosition.title,
      generatedAt: new Date().toISOString(),
      apiVersion: 'gemini-1.5-pro'
    };
    
    return profile;
  }

  // Validate generated resume
  validateGeneratedResume(resume, targetPosition) {
    // Ensure required fields are present
    if (!resume.personalInfo || !resume.professionalSummary || !resume.workExperience) {
      throw new Error('Generated resume missing required sections');
    }

    // Validate professional summary targets the position
    if (!resume.professionalSummary.summary.toLowerCase().includes(targetPosition.title.toLowerCase().split(' ')[0])) {
      console.warn('Generated summary may not be well-targeted to position');
    }

    // Ensure skills include required skills
    const allSkills = [
      ...(resume.skills.technical || []),
      ...(resume.skills.soft || [])
    ].map(skill => skill.toLowerCase());
    
    const requiredSkillsLower = targetPosition.requiredSkills.map(skill => skill.toLowerCase());
    const missingSkills = requiredSkillsLower.filter(skill => 
      !allSkills.some(userSkill => userSkill.includes(skill) || skill.includes(userSkill))
    );
    
    if (missingSkills.length > 0) {
      console.warn(`Generated resume missing some required skills: ${missingSkills.join(', ')}`);
    }

    // Add generation metadata
    resume.metadata = {
      ...resume.metadata,
      generatedFor: targetPosition.title,
      targetIndustry: targetPosition.industry,
      optimizationLevel: targetPosition.level,
      canadianMarketFocus: true,
      generatedAt: new Date().toISOString(),
      aiModel: 'gemini-1.5-pro'
    };

    return resume;
  }

  // Save career profile to database
  async saveCareerProfile(userId, profileData) {
    try {
      const existingProfile = await this.supabaseDb.fetchUserCareerProfile(userId);
      
      if (existingProfile) {
        return await this.supabaseDb.updateUserCareerProfile(userId, {
          professionalSummary: profileData.enhancedProfile?.optimizedSummary,
          skillsCategories: profileData.enhancedProfile?.skillsPresentation,
          careerObjectives: profileData.applicationStrategy?.coverLetterTemplate,
          targetIndustries: profileData.targetIndustries || [],
          marketAlignmentScore: Math.round((profileData.overallMatchScore || 0) * 100),
          skillGaps: profileData.skillDevelopment,
          improvementRoadmap: profileData.careerProjection,
          lastUpdated: new Date()
        });
      } else {
        return await this.supabaseDb.createUserCareerProfile({
          userId,
          professionalSummary: profileData.enhancedProfile?.optimizedSummary,
          skillsCategories: profileData.enhancedProfile?.skillsPresentation,
          careerObjectives: profileData.applicationStrategy?.coverLetterTemplate,
          targetIndustries: profileData.targetIndustries || [],
          marketAlignmentScore: Math.round((profileData.overallMatchScore || 0) * 100),
          skillGaps: profileData.skillDevelopment,
          improvementRoadmap: profileData.careerProjection
        });
      }
    } catch (error) {
      console.error('❌ Error saving career profile:', error);
      throw new Error(`Failed to save career profile: ${error.message}`);
    }
  }

  // Save job matches to database
  async saveJobMatches(userId, jobMatches) {
    try {
      const savedMatches = [];
      
      for (const match of jobMatches) {
        // Create or find job opportunity
        let jobOpportunity = await this.supabaseDb.fetchJobOpportunity(match.title, match.company || 'Various Companies');
        
        if (!jobOpportunity) {
          jobOpportunity = await this.supabaseDb.createJobOpportunity({
            title: match.title,
            company: match.company || 'Various Companies',
            location: match.location || 'Canada',
            description: match.description || '',
            requirements: match.requiredSkills || [],
            salaryRange: match.salaryRange,
            isNewcomerFriendly: match.newcomerFriendly || false
          });
        }
        
        // Create job match
        const jobMatch = await this.supabaseDb.createJobMatch({
          userId,
          jobId: jobOpportunity.id,
          matchScore: Math.round((match.matchScore || 0) * 100),
          matchAnalysis: {
            successProbability: match.successProbability,
            skillsMatch: match.skillsMatch,
            applicationStrategy: match.applicationStrategy
          },
          skillsGaps: match.skillsMatch?.missing || []
        });
        
        savedMatches.push(jobMatch);
      }
      
      return savedMatches;
    } catch (error) {
      console.error('❌ Error saving job matches:', error);
      throw new Error(`Failed to save job matches: ${error.message}`);
    }
  }

  /**
   * Save generated resume to database
   * @param {number} userId - User ID
   * @param {Object} generatedResume - Generated resume data
   * @param {Object} targetPosition - Target position details
   * @returns {Object} Saved resume analysis record
   */
  async saveGeneratedResume(userId, generatedResume, targetPosition) {
    try {
      const savedAnalysis = await this.supabaseDb.createResumeAnalysis({
        userId: userId,
        originalFileName: `AI_Generated_Resume_${targetPosition.title}_${Date.now()}.json`,
        structuredData: generatedResume,
        personalInfo: generatedResume.personalInfo,
        professionalSummary: generatedResume.professionalSummary?.summary,
        skills: generatedResume.skills,
        workExperience: generatedResume.workExperience,
        education: generatedResume.education,
        certifications: generatedResume.certifications,
        projects: generatedResume.projects,
        canadianMarketAnalysis: generatedResume.canadianMarketAnalysis,
        confidenceScores: { overall: 1.0 },
        metadata: generatedResume.metadata,
        processingMethod: 'ai_generated'
      });

      return savedAnalysis;
    } catch (error) {
      console.error('❌ Error saving generated resume:', error);
      throw new Error(`Failed to save generated resume: ${error.message}`);
    }
  }
}

module.exports = CareerProfileService;
````

## File: src/services/documentProcessor.js
````javascript
const fs = require('fs').promises;
const path = require('path');
const pdf = require('pdf-parse');
const mammoth = require('mammoth');
const Tesseract = require('tesseract.js');
const sharp = require('sharp');

class DocumentProcessor {
  constructor() {
    this.supportedFormats = ['.pdf', '.docx', '.jpg', '.jpeg', '.png'];
  }

  // Main document processing method
  async processDocument(filePath, originalName) {
    try {
      const ext = path.extname(originalName).toLowerCase();
      
      if (!this.supportedFormats.includes(ext)) {
        throw new Error(`Unsupported file format: ${ext}`);
      }

      let extractedText = '';
      
      switch (ext) {
        case '.pdf':
          extractedText = await this.processPDF(filePath);
          break;
        case '.docx':
          extractedText = await this.processDocx(filePath);
          break;
        case '.jpg':
        case '.jpeg':
        case '.png':
          extractedText = await this.processImage(filePath);
          break;
        default:
          throw new Error(`Unsupported file format: ${ext}`);
      }

      return {
        extractedText: extractedText.trim(),
        originalFileName: originalName,
        fileSize: (await fs.stat(filePath)).size,
        processedAt: new Date().toISOString()
      };

    } catch (error) {
      console.error('Document processing error:', error);
      throw new Error(`Failed to process document: ${error.message}`);
    }
  }

  // Process PDF files
  async processPDF(filePath) {
    try {
      const dataBuffer = await fs.readFile(filePath);
      const data = await pdf(dataBuffer);
      return data.text;
    } catch (error) {
      console.error('PDF processing error:', error);
      throw new Error('Failed to process PDF file');
    }
  }

  // Process DOCX files
  async processDocx(filePath) {
    try {
      const result = await mammoth.extractRawText({ path: filePath });
      return result.value;
    } catch (error) {
      console.error('DOCX processing error:', error);
      throw new Error('Failed to process DOCX file');
    }
  }

  // Process image files using OCR
  async processImage(filePath) {
    try {
      // Optimize image for better OCR results
      const optimizedBuffer = await sharp(filePath)
        .resize(null, 2000, { 
          withoutEnlargement: true,
          fit: 'inside'
        })
        .grayscale()
        .normalize()
        .sharpen()
        .toBuffer();

      // Perform OCR
      const { data: { text } } = await Tesseract.recognize(optimizedBuffer, 'eng', {
        logger: m => console.log(m)
      });

      return text;
    } catch (error) {
      console.error('Image OCR processing error:', error);
      throw new Error('Failed to process image file');
    }
  }

  // Validate file before processing
  validateFile(file) {
    const errors = [];

    // Check file size (5MB limit)
    if (file.size > 5 * 1024 * 1024) {
      errors.push('File size must be less than 5MB');
    }

    // Check file format
    const ext = path.extname(file.originalname).toLowerCase();
    if (!this.supportedFormats.includes(ext)) {
      errors.push(`Unsupported file format. Supported formats: ${this.supportedFormats.join(', ')}`);
    }

    // Check file name
    if (!file.originalname || file.originalname.trim().length === 0) {
      errors.push('Invalid file name');
    }

    return {
      isValid: errors.length === 0,
      errors
    };
  }

  // Clean up temporary files
  async cleanupFile(filePath) {
    try {
      await fs.unlink(filePath);
    } catch (error) {
      console.error('File cleanup error:', error);
      // Don't throw error for cleanup failures
    }
  }

  // Extract structured data from raw text
  extractBasicInfo(text) {
    const info = {
      emails: [],
      phones: [],
      urls: []
    };

    // Extract emails
    const emailRegex = /\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b/g;
    info.emails = [...new Set(text.match(emailRegex) || [])];

    // Extract phone numbers (various formats)
    const phoneRegex = /(\+?1?[-.\s]?)?\(?([0-9]{3})\)?[-.\s]?([0-9]{3})[-.\s]?([0-9]{4})/g;
    const phoneMatches = text.match(phoneRegex) || [];
    info.phones = [...new Set(phoneMatches.map(phone => phone.replace(/\D/g, '')))];

    // Extract URLs
    const urlRegex = /https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)/g;
    info.urls = [...new Set(text.match(urlRegex) || [])];

    return info;
  }

  // Data quality validation
  validateExtractedData(data) {
    const quality = {
      score: 0,
      issues: [],
      suggestions: []
    };

    let score = 0;

    // Check personal info completeness
    if (data.personalInfo) {
      if (data.personalInfo.name) score += 20;
      else quality.issues.push('Missing name information');
      
      if (data.personalInfo.email) score += 15;
      else quality.issues.push('Missing email information');
      
      if (data.personalInfo.phone) score += 10;
      else quality.suggestions.push('Consider adding phone number');
    }

    // Check education section
    if (data.education && data.education.length > 0) {
      score += 20;
    } else {
      quality.issues.push('Missing education information');
    }

    // Check work experience
    if (data.workExperience && data.workExperience.length > 0) {
      score += 25;
      
      // Check if experience has details
      const hasDetailedExperience = data.workExperience.some(exp => 
        exp.responsibilities && exp.responsibilities.length > 0
      );
      
      if (!hasDetailedExperience) {
        quality.suggestions.push('Add more detailed job responsibilities');
      }
    } else {
      quality.issues.push('Missing work experience information');
    }

    // Check skills
    if (data.skills && (data.skills.technical?.length > 0 || data.skills.soft?.length > 0)) {
      score += 10;
    } else {
      quality.suggestions.push('Add skills section for better matching');
    }

    quality.score = score;
    
    if (score >= 80) quality.level = 'Excellent';
    else if (score >= 60) quality.level = 'Good';
    else if (score >= 40) quality.level = 'Fair';
    else quality.level = 'Needs Improvement';

    return quality;
  }
}

module.exports = DocumentProcessor;
````

## File: src/services/GeminiResumeService.js
````javascript
const { GoogleGenerativeAI } = require('@google/generative-ai');
const fs = require('fs');
const path = require('path');
const { ANALYSIS_PROMPT, TEXT_ANALYSIS_PROMPT, createBasicAnalysis } = require('../prompts/resume');

class GeminiResumeService {
  constructor() {
    this.genAI = new GoogleGenerativeAI(process.env.GEMINI_API_KEY);
    
    // Use Gemini 1.5 Flash for faster, cost-effective processing
    // Rate limit: 1000 requests/minute (vs 15 with AI Studio)
    this.model = this.genAI.getGenerativeModel({ 
      model: "gemini-1.5-flash",
      generationConfig: {
        temperature: 0.1, // Low temperature for consistent structured output
        topK: 1,
        topP: 1,
        maxOutputTokens: 8192,
      }
    });
    
    // Rate limiting (much higher limits with Developer API)
    this.requestCount = {
      minute: { count: 0, resetTime: Date.now() + 60000 },
      day: { count: 0, resetTime: Date.now() + 86400000 }
    };
    
    this.maxRequestsPerMinute = 1000; // Increased from 15
    this.maxRequestsPerDay = 50000;   // Much higher daily limit
  }

  // Enhanced rate limiting check
  checkRateLimit() {
    const now = Date.now();
    
    if (now > this.requestCount.minute.resetTime) {
      this.requestCount.minute = { count: 0, resetTime: now + 60000 };
    }
    
    if (now > this.requestCount.day.resetTime) {
      this.requestCount.day = { count: 0, resetTime: now + 86400000 };
    }
    
    if (this.requestCount.minute.count >= this.maxRequestsPerMinute) {
      throw new Error('Rate limit exceeded: too many requests per minute (1000/min limit)');
    }
    
    if (this.requestCount.day.count >= this.maxRequestsPerDay) {
      throw new Error('Rate limit exceeded: too many requests per day');
    }
    
    return true;
  }

  incrementRequestCount() {
    this.requestCount.minute.count++;
    this.requestCount.day.count++;
  }

  // Direct PDF processing with Gemini (no need for text extraction)
  async analyzeResumePDF(filePath, originalFileName, retryCount = 0) {
    this.checkRateLimit();
    
    try {
      console.log('🔍 Processing PDF directly with Gemini API...');
      
      // Read PDF file as base64
      const fileBuffer = fs.readFileSync(filePath);
      const mimeType = 'application/pdf';
      
      const prompt = ANALYSIS_PROMPT;
      
      const result = await this.model.generateContent([
        {
          inlineData: {
            data: fileBuffer.toString('base64'),
            mimeType: mimeType
          }
        },
        { text: prompt }
      ]);

      const response = await result.response;
      const analysisText = response.text();
      
      this.incrementRequestCount();
      
      // Parse JSON response
      let analysis;
      try {
        analysis = JSON.parse(analysisText);
      } catch (parseError) {
        console.error('JSON parsing error:', parseError);
        // Try to extract JSON from response if it's wrapped in markdown
        const jsonMatch = analysisText.match(/```json\n([\s\S]*?)\n```/) || 
                         analysisText.match(/\{[\s\S]*\}/);
        if (jsonMatch) {
          analysis = JSON.parse(jsonMatch[1] || jsonMatch[0]);
        } else {
          throw new Error('Failed to parse AI response as JSON');
        }
      }
      
      // Validate and enhance analysis
      analysis = this.validateAndEnhanceAnalysis(analysis, originalFileName);
      
      console.log('✅ PDF analysis completed successfully');
      return analysis;
      
    } catch (error) {
      console.error('❌ PDF analysis error:', error);
      
      // Check if it's a service overload error (503)
      if (error.status === 503 || error.message.includes('Service Unavailable') || error.message.includes('overloaded')) {
        console.log('🔄 Gemini API is overloaded, attempting retry...');
        
        if (retryCount < 3) {
          // Exponential backoff: wait 2^retryCount seconds
          const waitTime = Math.pow(2, retryCount) * 1000;
          console.log(`⏳ Waiting ${waitTime/1000} seconds before retry ${retryCount + 1}/3...`);
          
          await new Promise(resolve => setTimeout(resolve, waitTime));
          
          return this.analyzeResumePDF(filePath, originalFileName, retryCount + 1);
        } else {
          console.log('⚠️ Max retries reached, falling back to text extraction...');
          return this.fallbackToTextExtraction(filePath, originalFileName);
        }
      }
      
      throw new Error(`Resume analysis failed: ${error.message}`);
    }
  }

  // Fallback method using text extraction when Gemini API is overloaded
  async fallbackToTextExtraction(filePath, originalFileName) {
    console.log('📄 Falling back to text extraction method...');
    
    try {
      // Use a simple text extraction library or basic PDF parsing
      const DocumentProcessor = require('./documentProcessor');
      const documentProcessor = new DocumentProcessor();
      
      const documentData = await documentProcessor.processDocument(filePath, originalFileName);
      const extractedText = documentData.extractedText;
      
      if (!extractedText || extractedText.trim().length === 0) {
        throw new Error('Could not extract text from PDF for fallback analysis');
      }
      
      console.log('✅ Text extracted successfully for fallback analysis');
      
      // Use the text-based analysis method
      return this.analyzeResumeText(extractedText, originalFileName);
      
    } catch (fallbackError) {
      console.error('❌ Fallback analysis also failed:', fallbackError);
      
      // Return a basic analysis structure as last resort
      return this.createBasicAnalysis(originalFileName);
    }
  }

  // Create a basic analysis structure when all methods fail
  createBasicAnalysis(originalFileName) {
    console.log('🛠️ Creating basic analysis structure as last resort...');
    return createBasicAnalysis(originalFileName);
  }



  // Analyze text-based resume (fallback for non-PDF files)
  async analyzeResumeText(extractedText, originalFileName, retryCount = 0) {
    this.checkRateLimit();
    
    try {
      console.log('🔍 Processing text-based resume with Gemini...');
      
      const prompt = TEXT_ANALYSIS_PROMPT(extractedText, originalFileName);
      
      const result = await this.model.generateContent(prompt);
      const response = await result.response;
      const analysisText = response.text();
      
      this.incrementRequestCount();
      
      // Parse and validate response
      let analysis;
      try {
        analysis = JSON.parse(analysisText);
      } catch (parseError) {
        const jsonMatch = analysisText.match(/```json\n([\s\S]*?)\n```/) || 
                         analysisText.match(/\{[\s\S]*\}/);
        if (jsonMatch) {
          analysis = JSON.parse(jsonMatch[1] || jsonMatch[0]);
        } else {
          throw new Error('Failed to parse AI response as JSON');
        }
      }
      
      analysis = this.validateAndEnhanceAnalysis(analysis, originalFileName);
      
      console.log('✅ Text analysis completed successfully');
      return analysis;
      
    } catch (error) {
      console.error('❌ Text analysis error:', error);
      
      // Check if it's a service overload error (503)
      if (error.status === 503 || error.message.includes('Service Unavailable') || error.message.includes('overloaded')) {
        console.log('🔄 Gemini API is overloaded, attempting retry for text analysis...');
        
        if (retryCount < 3) {
          // Exponential backoff: wait 2^retryCount seconds
          const waitTime = Math.pow(2, retryCount) * 1000;
          console.log(`⏳ Waiting ${waitTime/1000} seconds before retry ${retryCount + 1}/3...`);
          
          await new Promise(resolve => setTimeout(resolve, waitTime));
          
          return this.analyzeResumeText(extractedText, originalFileName, retryCount + 1);
        } else {
          console.log('⚠️ Max retries reached for text analysis, creating basic analysis...');
          return this.createBasicAnalysis(originalFileName);
        }
      }
      
      throw new Error(`Resume analysis failed: ${error.message}`);
    }
  }

  // Validate and enhance analysis results
  validateAndEnhanceAnalysis(analysis, originalFileName) {
    // Ensure all required fields exist
    const defaults = {
      personalInfo: { confidence: 0 },
      professionalSummary: { confidence: 0 },
      education: [],
      workExperience: [],
      skills: { technical: [], soft: [], languages: [], confidence: 0 },
      certifications: [],
      projects: [],
      canadianMarketAnalysis: { confidence: 0 },
      confidenceScores: { overall: 0, dataExtraction: 0, marketAnalysis: 0 }
    };

    // Deep merge with defaults
    analysis = { ...defaults, ...analysis };
    
    // Calculate overall confidence if not provided
    if (!analysis.confidenceScores.overall) {
      const confidences = [
        analysis.personalInfo.confidence || 0,
        analysis.professionalSummary.confidence || 0,
        analysis.skills.confidence || 0,
        analysis.canadianMarketAnalysis.confidence || 0
      ];
      analysis.confidenceScores.overall = 
        confidences.reduce((a, b) => a + b, 0) / confidences.length;
    }

    // Add metadata
    analysis.metadata = {
      processedAt: new Date().toISOString(),
      originalFileName: originalFileName,
      processingMethod: originalFileName.toLowerCase().endsWith('.pdf') ? 'direct_pdf' : 'text_extraction',
      apiVersion: 'gemini-1.5-flash'
    };

    return analysis;
  }

  // Get rate limit status
  getRateLimitStatus() {
    const now = Date.now();
    return {
      minute: {
        used: this.requestCount.minute.count,
        limit: this.maxRequestsPerMinute,
        resetIn: Math.max(0, this.requestCount.minute.resetTime - now)
      },
      day: {
        used: this.requestCount.day.count,
        limit: this.maxRequestsPerDay,
        resetIn: Math.max(0, this.requestCount.day.resetTime - now)
      }
    };
  }
}

module.exports = GeminiResumeService;
````

## File: src/services/googleAiService.js
````javascript
const { GoogleGenerativeAI } = require('@google/generative-ai');
const aiConfig = require('./aiConfig');
const {
  RESUME_ANALYSIS_PROMPT,
  CAREER_PROFILE_PROMPT,
  MENTOR_COMPATIBILITY_PROMPT,
  COACHING_QUERY_PROMPT,
  JOB_COMPATIBILITY_PROMPT,
  SKILL_GAP_ANALYSIS_PROMPT,
  CULTURAL_GUIDANCE_PROMPT,
  CAREER_PROFILE_WITH_GEMINI_PROMPT,
  POSITION_RECOMMENDATIONS_WITH_GEMINI_PROMPT,
  ENHANCED_PROFILE_WITH_GEMINI_PROMPT
} = require('../prompts/jobs');

class GoogleAIService {
  constructor() {
    this.genAI = new GoogleGenerativeAI(aiConfig.googleAI.apiKey);
    this.flashModel = this.genAI.getGenerativeModel({ model: aiConfig.googleAI.models.flash });
    this.proModel = this.genAI.getGenerativeModel({ model: aiConfig.googleAI.models.pro });
    
    // Rate limiting tracking
    this.requestCount = {
      minute: { count: 0, resetTime: Date.now() + 60000 },
      day: { count: 0, resetTime: Date.now() + 86400000 }
    };
  }

  // Rate limiting check
  checkRateLimit() {
    const now = Date.now();
    
    // Reset minute counter if needed
    if (now > this.requestCount.minute.resetTime) {
      this.requestCount.minute = { count: 0, resetTime: now + 60000 };
    }
    
    // Reset day counter if needed
    if (now > this.requestCount.day.resetTime) {
      this.requestCount.day = { count: 0, resetTime: now + 86400000 };
    }
    
    // Check limits
    if (this.requestCount.minute.count >= aiConfig.rateLimits.maxRequestsPerMinute) {
      throw new Error('Rate limit exceeded: too many requests per minute');
    }
    
    if (this.requestCount.day.count >= aiConfig.rateLimits.maxRequestsPerDay) {
      throw new Error('Rate limit exceeded: too many requests per day');
    }
    
    return true;
  }

  // Increment request counters
  incrementRequestCount() {
    this.requestCount.minute.count++;
    this.requestCount.day.count++;
  }

  // Generic AI request method
  async makeAIRequest(prompt, useProModel = false, retries = 3) {
    this.checkRateLimit();
    
    try {
      const model = useProModel ? this.proModel : this.flashModel;
      const result = await model.generateContent(prompt);
      const response = await result.response;
      
      this.incrementRequestCount();
      return response.text();
    } catch (error) {
      if (retries > 0 && error.message.includes('rate limit')) {
        console.log(`Rate limit hit, retrying in 2 seconds... (${retries} retries left)`);
        await new Promise(resolve => setTimeout(resolve, 2000));
        return this.makeAIRequest(prompt, useProModel, retries - 1);
      }
      throw error;
    }
  }

  // Resume Analysis Feature
  async analyzeResume(extractedText, userProfile = {}) {
    const prompt = RESUME_ANALYSIS_PROMPT(extractedText, userProfile);

    try {
      const response = await this.makeAIRequest(prompt, false);
      return JSON.parse(response);
    } catch (error) {
      console.error('Resume analysis error:', error);
      throw new Error('Failed to analyze resume');
    }
  }

  // Career Profile Generation Feature
  async generateCareerProfile(resumeData, userObjectives = {}) {
    const prompt = CAREER_PROFILE_PROMPT(resumeData, userObjectives);

    try {
      const response = await this.makeAIRequest(prompt, true);
      return JSON.parse(response);
    } catch (error) {
      console.error('Career profile generation error:', error);
      throw new Error('Failed to generate career profile');
    }
  }

  // Mentor Matching Feature
  async calculateMentorCompatibility(menteeProfile, mentorProfile) {
    const prompt = MENTOR_COMPATIBILITY_PROMPT(menteeProfile, mentorProfile);

    try {
      const response = await this.makeAIRequest(prompt, true);
      return JSON.parse(response);
    } catch (error) {
      console.error('Mentor compatibility calculation error:', error);
      throw new Error('Failed to calculate mentor compatibility');
    }
  }

  // AI Career Coaching Feature
  async processCoachingQuery(query, userProfile, sessionHistory = []) {
    const prompt = COACHING_QUERY_PROMPT(query, userProfile, sessionHistory);

    try {
      const response = await this.makeAIRequest(prompt, true);
      return JSON.parse(response);
    } catch (error) {
      console.error('Coaching query processing error:', error);
      throw new Error('Failed to process coaching query');
    }
  }

  // Job Opportunity Analysis Feature
  async analyzeJobCompatibility(userProfile, jobDescription) {
    const prompt = JOB_COMPATIBILITY_PROMPT(userProfile, jobDescription);

    try {
      const response = await this.makeAIRequest(prompt, true);
      return JSON.parse(response);
    } catch (error) {
      console.error('Job compatibility analysis error:', error);
      throw new Error('Failed to analyze job compatibility');
    }
  }

  // Skill Gap Analysis Feature
  async analyzeSkillGaps(currentSkills, targetRole, marketData = {}) {
    const prompt = SKILL_GAP_ANALYSIS_PROMPT(currentSkills, targetRole, marketData);

    try {
      const response = await this.makeAIRequest(prompt, true);
      return JSON.parse(response);
    } catch (error) {
      console.error('Skill gap analysis error:', error);
      throw new Error('Failed to analyze skill gaps');
    }
  }

  // Cultural Integration Support Feature
  async generateCulturalGuidance(userBackground, targetWorkplace = {}) {
    const prompt = CULTURAL_GUIDANCE_PROMPT(userBackground, targetWorkplace);

    try {
      const response = await this.makeAIRequest(prompt, false);
      return JSON.parse(response);
    } catch (error) {
      console.error('Cultural guidance generation error:', error);
      throw new Error('Failed to generate cultural guidance');
    }
  }

  // Career Profile Generation for the Resume Page
  async generateCareerProfileWithGemini(data) {
    const prompt = CAREER_PROFILE_WITH_GEMINI_PROMPT(data);

    try {
      const response = await this.makeAIRequest(prompt, true);
      return JSON.parse(response);
    } catch (error) {
      console.error('Career profile generation error:', error);
      throw new Error('Failed to generate career profile');
    }
  }

  // Position Recommendations Generation
  async generatePositionRecommendationsWithGemini(resumeAnalysis) {
    const prompt = POSITION_RECOMMENDATIONS_WITH_GEMINI_PROMPT(resumeAnalysis);

    try {
      const response = await this.makeAIRequest(prompt, true);
      return JSON.parse(response);
    } catch (error) {
      console.error('Position recommendations generation error:', error);
      throw new Error('Failed to generate position recommendations');
    }
  }

  // Enhanced Profile Generation for Specific Position
  async generateEnhancedProfileWithGemini(targetPosition, resumeAnalysis) {
    const prompt = ENHANCED_PROFILE_WITH_GEMINI_PROMPT(targetPosition, resumeAnalysis);

    try {
      const response = await this.makeAIRequest(prompt, true);
      return JSON.parse(response);
    } catch (error) {
      console.error('Enhanced profile generation error:', error);
      throw new Error('Failed to generate enhanced profile');
    }
  }
}

// Export the class and standalone functions for backwards compatibility
const googleAIService = new GoogleAIService();

// Export individual functions for direct use
const generateCareerProfileWithGemini = (data) => googleAIService.generateCareerProfileWithGemini(data);
const generatePositionRecommendationsWithGemini = (resumeAnalysis) => googleAIService.generatePositionRecommendationsWithGemini(resumeAnalysis);
const generateEnhancedProfileWithGemini = (targetPosition, resumeAnalysis) => googleAIService.generateEnhancedProfileWithGemini(targetPosition, resumeAnalysis);

module.exports = {
  GoogleAIService,
  generateCareerProfileWithGemini,
  generatePositionRecommendationsWithGemini, 
  generateEnhancedProfileWithGemini,
  default: googleAIService
};
````

## File: src/services/GoogleJobsService.js
````javascript
const { JobServiceClient } = require('@google-cloud/talent');

class GoogleJobsService {
  constructor() {
    // Check if Google Cloud credentials are configured
    if (process.env.GOOGLE_CLOUD_PROJECT_ID && process.env.GOOGLE_APPLICATION_CREDENTIALS) {
      try {
        // Initialize Google Cloud Talent Solution client
        this.client = new JobServiceClient({
          projectId: process.env.GOOGLE_CLOUD_PROJECT_ID,
          keyFilename: process.env.GOOGLE_APPLICATION_CREDENTIALS
        });
        
        this.projectPath = this.client.projectPath(process.env.GOOGLE_CLOUD_PROJECT_ID);
        this.isConfigured = true;
        console.log('✅ Google Cloud Talent API configured successfully');
      } catch (error) {
        console.log('⚠️ Google Cloud Talent API configuration failed:', error.message);
        this.isConfigured = false;
      }
    } else {
      console.log('⚠️ Google Cloud Talent API not configured - missing environment variables');
      this.isConfigured = false;
    }
  }

  /**
   * Search for jobs using Google for Jobs API
   * @param {Object} careerPath - Career path object with title and industry
   * @param {string} location - Location to search jobs (default: 'Canada')
   * @param {Object} filters - Additional search filters
   * @returns {Array} Array of job results
   */
  async searchJobs(careerPath, location = 'Canada', filters = {}) {
    // If Google Cloud API is not configured, return mock data
    if (!this.isConfigured) {
      return this.getMockJobData(careerPath, location);
    }

    try {
      console.log(`🔍 Searching jobs for: ${careerPath.title} in ${location}`);
      
      const request = {
        parent: this.projectPath,
        requestMetadata: {
          userId: filters.userId || 'anonymous',
          sessionId: filters.sessionId || this.generateSessionId(),
          domain: 'immigrowai.com'
        },
        jobQuery: {
          query: this.buildJobQuery(careerPath, location),
          jobTitleFilters: [{
            jobTitle: careerPath.title,
            negated: false
          }],
          locationFilters: [{
            address: location
          }],
          languageCodes: ['en-CA', 'fr-CA'],
          publishTimeRange: {
            startTime: {
              seconds: Math.floor((Date.now() - 30 * 24 * 60 * 60 * 1000) / 1000) // Last 30 days
            },
            endTime: {
              seconds: Math.floor(Date.now() / 1000)
            }
          }
        },
        histogramQueries: [{
          histogramQuery: 'COMPANY_SIZE'
        }],
        jobView: 'JOB_VIEW_FULL',
        maxResults: 20,
        orderBy: 'relevance desc'
      };

      const [response] = await this.client.searchJobs(request);
      
      const jobs = this.parseJobResults(response.jobs || []);
      console.log(`✅ Found ${jobs.length} jobs for ${careerPath.title}`);
      
      return {
        jobs,
        totalCount: response.totalSize || 0,
        nextPageToken: response.nextPageToken,
        metadata: {
          searchQuery: careerPath.title,
          location: location,
          searchedAt: new Date().toISOString()
        }
      };

    } catch (error) {
      console.error('❌ Google Jobs API error:', error);
      
      // Fallback to mock data if Google Jobs API fails
      return this.getMockJobData(careerPath, location);
    }
  }

  /**
   * Build search query string for job search
   */
  buildJobQuery(careerPath, location) {
    const queryParts = [
      careerPath.title,
      careerPath.industry || '',
      location
    ].filter(Boolean);
    
    return queryParts.join(' ');
  }

  /**
   * Parse job results from Google Jobs API response
   */
  parseJobResults(jobs) {
    return jobs.map(job => ({
      id: job.name,
      title: job.title,
      company: job.companyDisplayName || job.companyName,
      location: this.formatLocation(job.addresses),
      description: this.cleanDescription(job.description),
      salaryInfo: this.formatSalary(job.compensationInfo),
      jobLevel: job.jobLevel,
      employmentTypes: job.employmentTypes || [],
      applicationInfo: {
        applicationUrls: job.applicationInfo?.uris || [],
        applicationEmails: job.applicationInfo?.emails || [],
        instruction: job.applicationInfo?.instruction || ''
      },
      postingPublishTime: job.postingPublishTime,
      postingExpireTime: job.postingExpireTime,
      jobBenefits: job.jobBenefits || [],
      qualifications: job.qualifications,
      responsibilities: job.responsibilities,
      companySize: job.companySize,
      jobCategory: job.jobCategory,
      languageCode: job.languageCode,
      promotionValue: job.promotionValue || 0,
      customAttributes: job.customAttributes || {}
    }));
  }

  /**
   * Format location information
   */
  formatLocation(addresses) {
    if (!addresses || addresses.length === 0) return 'Location not specified';
    
    const address = addresses[0];
    const parts = [];
    
    if (address.locality) parts.push(address.locality);
    if (address.administrativeArea) parts.push(address.administrativeArea);
    if (address.country) parts.push(address.country);
    
    return parts.join(', ') || 'Remote';
  }

  /**
   * Clean and truncate job description
   */
  cleanDescription(description) {
    if (!description) return 'No description available';
    
    // Remove HTML tags and extra whitespace
    const cleaned = description
      .replace(/<[^>]*>/g, '')
      .replace(/\s+/g, ' ')
      .trim();
    
    // Truncate to 300 characters
    return cleaned.length > 300 ? cleaned.substring(0, 300) + '...' : cleaned;
  }

  /**
   * Format salary information
   */
  formatSalary(compensationInfo) {
    if (!compensationInfo || !compensationInfo.entries) {
      return null;
    }

    const salaryEntry = compensationInfo.entries.find(entry => 
      entry.type === 'BASE' || entry.type === 'SALARY'
    );

    if (!salaryEntry || !salaryEntry.range) {
      return null;
    }

    const range = salaryEntry.range;
    const currency = range.currencyCode || 'CAD';
    
    return {
      min: range.min?.currencyCode ? range.min.units || 0 : 0,
      max: range.max?.currencyCode ? range.max.units || 0 : 0,
      currency: currency,
      period: salaryEntry.unit || 'YEAR',
      formatted: this.formatSalaryRange(range, currency)
    };
  }

  /**
   * Format salary range for display
   */
  formatSalaryRange(range, currency) {
    if (!range.min && !range.max) return null;
    
    const formatAmount = (amount) => {
      if (!amount || !amount.units) return null;
      return new Intl.NumberFormat('en-CA', {
        style: 'currency',
        currency: currency,
        minimumFractionDigits: 0
      }).format(amount.units);
    };

    const minFormatted = formatAmount(range.min);
    const maxFormatted = formatAmount(range.max);

    if (minFormatted && maxFormatted) {
      return `${minFormatted} - ${maxFormatted}`;
    } else if (minFormatted) {
      return `From ${minFormatted}`;
    } else if (maxFormatted) {
      return `Up to ${maxFormatted}`;
    }
    
    return null;
  }

  /**
   * Returns mock job data when Google Cloud API is not configured
   * This allows the feature to work during development/testing
   */
  getMockJobData(careerPath, location) {
    console.log(`📋 Returning mock job data for: ${careerPath.title} in ${location}`);
    
    const mockJobs = [
      {
        id: 'mock-job-1',
        title: `${careerPath.title}`,
        company: 'TechCorp Canada',
        location: `${location}`,
        description: `We are looking for an experienced ${careerPath.title} to join our growing team. This role offers exciting opportunities for professional growth and development.`,
        salaryInfo: {
          formatted: 'CAD $70,000 - $90,000 per year',
          currency: 'CAD'
        },
        jobLevel: 'Mid-level',
        employmentTypes: ['Full-time'],
        applicationInfo: {
          applicationUrls: ['https://indeed.ca'],
          applicationEmails: [],
          instruction: 'Apply through company website'
        },
        postingDate: new Date().toISOString()
      },
      {
        id: 'mock-job-2',
        title: `Senior ${careerPath.title}`,
        company: 'InnovateTech Solutions',
        location: `${location}`,
        description: `Join our dynamic team as a Senior ${careerPath.title}. We offer competitive salary, excellent benefits, and a collaborative work environment.`,
        salaryInfo: {
          formatted: 'CAD $80,000 - $100,000 per year',
          currency: 'CAD'
        },
        jobLevel: 'Senior-level',
        employmentTypes: ['Full-time'],
        applicationInfo: {
          applicationUrls: ['https://linkedin.com/jobs'],
          applicationEmails: [],
          instruction: 'Apply through LinkedIn'
        },
        postingDate: new Date().toISOString()
      },
      {
        id: 'mock-job-3',
        title: `${careerPath.title} - Remote`,
        company: 'Global Remote Solutions',
        location: `Remote, ${location}`,
        description: `Remote opportunity for a skilled ${careerPath.title}. Work from anywhere in Canada with flexible hours and modern technology stack.`,
        salaryInfo: {
          formatted: 'CAD $75,000 - $95,000 per year',
          currency: 'CAD'
        },
        jobLevel: 'Mid-level',
        employmentTypes: ['Full-time', 'Remote'],
        applicationInfo: {
          applicationUrls: ['https://workopolis.com'],
          applicationEmails: [],
          instruction: 'Apply through Workopolis'
        },
        postingDate: new Date().toISOString()
      }
    ];

    return {
      jobs: mockJobs,
      totalCount: mockJobs.length,
      searchQuery: careerPath.title,
      location: location,
      nextPageToken: null,
      source: 'mock',
      message: 'These are sample job listings. Configure Google Cloud Talent API for real job data.'
    };
  }

  /**
   * Generate unique session ID for tracking
   */
  generateSessionId() {
    return `session_${Date.now()}_${Math.random().toString(36).substr(2, 9)}`;
  }

  /**
   * Map industry to Google Jobs category
   */
  mapIndustryToCategory(industry) {
    const industryMap = {
      'Technology': 'COMPUTER_AND_IT',
      'Healthcare': 'HEALTHCARE',
      'Finance': 'ACCOUNTING_AND_FINANCE',
      'Education': 'EDUCATION',
      'Engineering': 'ARCHITECTURE_AND_ENGINEERING',
      'Marketing': 'SALES_AND_RETAIL',
      'Sales': 'SALES_AND_RETAIL',
      'Manufacturing': 'MANUFACTURING_AND_WAREHOUSE',
      'Legal': 'LEGAL',
      'Construction': 'CONSTRUCTION_AND_MINING',
      'Transportation': 'TRANSPORTATION_AND_LOGISTICS',
      'Hospitality': 'RESTAURANT_AND_HOSPITALITY',
      'Real Estate': 'REAL_ESTATE',
      'Media': 'ARTS_ENTERTAINMENT_AND_MEDIA'
    };

    return industryMap[industry] || 'OTHER';
  }

  /**
   * Get available job categories
   */
  getJobCategories() {
    return [
      'ACCOUNTING_AND_FINANCE',
      'ADMINISTRATIVE_AND_OFFICE',
      'ADVERTISING_AND_MARKETING',
      'ANIMAL_CARE',
      'ART_FASHION_AND_DESIGN',
      'BUSINESS_OPERATIONS',
      'CLEANING_AND_FACILITIES',
      'COMPUTER_AND_IT',
      'CONSTRUCTION_AND_MINING',
      'EDUCATION',
      'ENTERTAINMENT_AND_TRAVEL',
      'FARMING_AND_OUTDOORS',
      'HEALTHCARE',
      'HUMAN_RESOURCES',
      'INSTALLATION_MAINTENANCE_AND_REPAIR',
      'LEGAL',
      'MANAGEMENT',
      'MANUFACTURING_AND_WAREHOUSE',
      'MEDIA_COMMUNICATIONS_AND_WRITING',
      'OIL_GAS_AND_MINING',
      'PERSONAL_CARE_AND_SERVICES',
      'PROTECTIVE_SERVICES',
      'REAL_ESTATE',
      'RESTAURANT_AND_HOSPITALITY',
      'SALES_AND_RETAIL',
      'SCIENCE_AND_ENGINEERING',
      'SOCIAL_SERVICES_AND_NON_PROFIT',
      'SPORTS_FITNESS_AND_RECREATION',
      'TRANSPORTATION_AND_LOGISTICS'
    ];
  }
}

module.exports = GoogleJobsService;
````

## File: src/services/index.js
````javascript
/**
 * Service exports
 * This file exports all service classes and the ServiceFactory for easy importing
 */

const BaseService = require('./BaseService');
const UserService = require('./UserService');
const ResumeService = require('./ResumeService');
const CanadianResumeService = require('./CanadianResumeService');
const ServiceFactory = require('./ServiceFactory');

module.exports = {
  BaseService,
  UserService,
  ResumeService,
  CanadianResumeService,
  ServiceFactory
};
````

## File: src/services/ResumeService.js
````javascript
const BaseService = require('./BaseService');
const { AppError } = require('../utils/errors');

/**
 * Resume Service for resume analysis-related business logic
 */
class ResumeService extends BaseService {
  constructor(repositories) {
    super(repositories);
    this.resumeRepository = this.getRepository('resume');
    this.userRepository = this.getRepository('user');
  }

  /**
   * Save resume analysis
   * @param {string|number} userId - User ID
   * @param {Object} analysisData - Resume analysis data
   * @returns {Promise<Object>} Saved analysis record
   */
  async saveResumeAnalysis(userId, analysisData) {
    return this.executeMethod('saveResumeAnalysis', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      this.validateRequiredParams(params.analysisData, ['originalFileName']);

      // Verify user exists
      const user = await this.userRepository.findById(validatedUserId, true);
      if (!user) {
        throw new AppError('User not found', 404);
      }

      const analysis = await this.resumeRepository.saveResumeAnalysis(validatedUserId, params.analysisData);
      return this.transformRecord(analysis, {
        user_id: 'userId',
        original_file_name: 'originalFileName',
        extracted_text: 'extractedText',
        structured_data: 'structuredData',
        confidence_scores: 'confidenceScores',
        canadian_market_analysis: 'canadianMarketAnalysis',
        personal_info: 'personalInfo',
        professional_summary: 'professionalSummary',
        work_experience: 'workExperience',
        processing_method: 'processingMethod',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { userId, analysisData });
  }

  /**
   * Get resume analyses for a user
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Resume analyses for the user
   */
  async getResumeAnalyses(userId, useServiceRole = false) {
    return this.executeMethod('getResumeAnalyses', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);

      const analyses = await this.resumeRepository.getResumeAnalyses(validatedUserId, params.useServiceRole);
      return this.transformRecords(analyses, {
        user_id: 'userId',
        original_file_name: 'originalFileName',
        extracted_text: 'extractedText',
        structured_data: 'structuredData',
        confidence_scores: 'confidenceScores',
        canadian_market_analysis: 'canadianMarketAnalysis',
        personal_info: 'personalInfo',
        professional_summary: 'professionalSummary',
        work_experience: 'workExperience',
        processing_method: 'processingMethod',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { userId, useServiceRole });
  }

  /**
   * Get resume analyses for a user with ordering
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Resume analyses for the user ordered by creation date
   */
  async getUserResumeAnalyses(userId, useServiceRole = false) {
    return this.executeMethod('getUserResumeAnalyses', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);

      const analyses = await this.resumeRepository.getUserResumeAnalyses(validatedUserId, params.useServiceRole);
      return this.transformRecords(analyses, {
        user_id: 'userId',
        original_file_name: 'originalFileName',
        extracted_text: 'extractedText',
        structured_data: 'structuredData',
        confidence_scores: 'confidenceScores',
        canadian_market_analysis: 'canadianMarketAnalysis',
        personal_info: 'personalInfo',
        professional_summary: 'professionalSummary',
        work_experience: 'workExperience',
        processing_method: 'processingMethod',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { userId, useServiceRole });
  }

  /**
   * Get resume analysis by ID
   * @param {string|number} analysisId - Analysis ID
   * @param {string|number} userId - User ID for permission check
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} Resume analysis record or null
   */
  async getResumeAnalysisById(analysisId, userId = null, useServiceRole = false) {
    return this.executeMethod('getResumeAnalysisById', async (params) => {
      if (!params.analysisId || isNaN(parseInt(params.analysisId))) {
        throw new AppError('Valid analysis ID is required', 400);
      }

      const analysis = await this.resumeRepository.getResumeAnalysisById(parseInt(params.analysisId), params.useServiceRole);
      if (!analysis) return null;

      // Check permission if userId is provided
      if (params.userId && !params.useServiceRole) {
        const validatedUserId = this.validateUserId(params.userId);
        if (!this.hasPermission(validatedUserId, analysis.user_id)) {
          throw new AppError('Access denied', 403);
        }
      }

      return this.transformRecord(analysis, {
        user_id: 'userId',
        original_file_name: 'originalFileName',
        extracted_text: 'extractedText',
        structured_data: 'structuredData',
        confidence_scores: 'confidenceScores',
        canadian_market_analysis: 'canadianMarketAnalysis',
        personal_info: 'personalInfo',
        professional_summary: 'professionalSummary',
        work_experience: 'workExperience',
        processing_method: 'processingMethod',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { analysisId, userId, useServiceRole });
  }

  /**
   * Update resume analysis
   * @param {string|number} analysisId - Analysis ID
   * @param {string|number} userId - User ID for permission check
   * @param {Object} updateData - Data to update
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Updated analysis record
   */
  async updateResumeAnalysis(analysisId, userId, updateData, useServiceRole = false) {
    return this.executeMethod('updateResumeAnalysis', async (params) => {
      if (!params.analysisId || isNaN(parseInt(params.analysisId))) {
        throw new AppError('Valid analysis ID is required', 400);
      }

      const validatedUserId = this.validateUserId(params.userId);

      // Get existing analysis to check permission
      const existingAnalysis = await this.resumeRepository.getResumeAnalysisById(parseInt(params.analysisId), params.useServiceRole);
      if (!existingAnalysis) {
        throw new AppError('Resume analysis not found', 404);
      }

      // Check permission if not using service role
      if (!params.useServiceRole && !this.hasPermission(validatedUserId, existingAnalysis.user_id)) {
        throw new AppError('Access denied', 403);
      }

      const updatedAnalysis = await this.resumeRepository.updateResumeAnalysis(parseInt(params.analysisId), params.updateData, params.useServiceRole);
      return this.transformRecord(updatedAnalysis, {
        user_id: 'userId',
        original_file_name: 'originalFileName',
        extracted_text: 'extractedText',
        structured_data: 'structuredData',
        confidence_scores: 'confidenceScores',
        canadian_market_analysis: 'canadianMarketAnalysis',
        personal_info: 'personalInfo',
        professional_summary: 'professionalSummary',
        work_experience: 'workExperience',
        processing_method: 'processingMethod',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { analysisId, userId, updateData, useServiceRole });
  }

  /**
   * Delete resume analysis
   * @param {string|number} analysisId - Analysis ID
   * @param {string|number} userId - User ID for permission check
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<boolean>} Success status
   */
  async deleteResumeAnalysis(analysisId, userId, useServiceRole = false) {
    return this.executeMethod('deleteResumeAnalysis', async (params) => {
      if (!params.analysisId || isNaN(parseInt(params.analysisId))) {
        throw new AppError('Valid analysis ID is required', 400);
      }

      const validatedUserId = this.validateUserId(params.userId);

      // Get existing analysis to check permission
      const existingAnalysis = await this.resumeRepository.getResumeAnalysisById(parseInt(params.analysisId), params.useServiceRole);
      if (!existingAnalysis) {
        throw new AppError('Resume analysis not found', 404);
      }

      // Check permission if not using service role
      if (!params.useServiceRole && !this.hasPermission(validatedUserId, existingAnalysis.user_id)) {
        throw new AppError('Access denied', 403);
      }

      return await this.resumeRepository.deleteResumeAnalysis(parseInt(params.analysisId), params.useServiceRole);
    }, { analysisId, userId, useServiceRole });
  }

  /**
   * Search resume analyses with criteria
   * @param {Object} criteria - Search criteria
   * @param {Object} options - Query options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Matching resume analyses
   */
  async searchResumeAnalyses(criteria = {}, options = {}, useServiceRole = false) {
    return this.executeMethod('searchResumeAnalyses', async (params) => {
      const allowedFields = ['userId', 'fileName', 'processingMethod', 'createdAfter', 'createdBefore'];
      const sanitizedCriteria = this.sanitizeSearchCriteria(params.criteria, allowedFields);
      const paginationOptions = this.validatePaginationOptions(params.options);

      const analyses = await this.resumeRepository.searchResumeAnalyses(sanitizedCriteria, paginationOptions, params.useServiceRole);
      return this.transformRecords(analyses, {
        user_id: 'userId',
        original_file_name: 'originalFileName',
        extracted_text: 'extractedText',
        structured_data: 'structuredData',
        confidence_scores: 'confidenceScores',
        canadian_market_analysis: 'canadianMarketAnalysis',
        personal_info: 'personalInfo',
        professional_summary: 'professionalSummary',
        work_experience: 'workExperience',
        processing_method: 'processingMethod',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { criteria, options, useServiceRole });
  }

  /**
   * Get resume analyses with pagination
   * @param {string|number} userId - User ID
   * @param {Object} options - Pagination options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Resume analyses with pagination info
   */
  async getResumeAnalysesWithPagination(userId, options = {}, useServiceRole = false) {
    return this.executeMethod('getResumeAnalysesWithPagination', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      const paginationOptions = this.validatePaginationOptions(params.options);

      const result = await this.resumeRepository.getResumeAnalysesWithPagination(validatedUserId, paginationOptions, params.useServiceRole);
      
      const transformedAnalyses = this.transformRecords(result.analyses, {
        user_id: 'userId',
        original_file_name: 'originalFileName',
        extracted_text: 'extractedText',
        structured_data: 'structuredData',
        confidence_scores: 'confidenceScores',
        canadian_market_analysis: 'canadianMarketAnalysis',
        personal_info: 'personalInfo',
        professional_summary: 'professionalSummary',
        work_experience: 'workExperience',
        processing_method: 'processingMethod',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });

      return {
        analyses: transformedAnalyses,
        pagination: result.pagination
      };
    }, { userId, options, useServiceRole });
  }

  /**
   * Get resume analysis statistics
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Resume analysis statistics
   */
  async getResumeAnalysisStatistics(useServiceRole = false) {
    return this.executeMethod('getResumeAnalysisStatistics', async (params) => {
      return await this.resumeRepository.getResumeAnalysisStatistics(params.useServiceRole);
    }, { useServiceRole });
  }

  /**
   * Get resume analysis count for a user
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<number>} Analysis count
   */
  async getResumeAnalysisCount(userId, useServiceRole = false) {
    return this.executeMethod('getResumeAnalysisCount', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      return await this.resumeRepository.count({ user_id: validatedUserId }, params.useServiceRole);
    }, { userId, useServiceRole });
  }

  /**
   * Get latest resume analysis for a user
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} Latest analysis record or null
   */
  async getLatestResumeAnalysis(userId, useServiceRole = false) {
    return this.executeMethod('getLatestResumeAnalysis', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);

      const analyses = await this.resumeRepository.getUserResumeAnalyses(validatedUserId, params.useServiceRole);
      if (analyses.length === 0) return null;

      const latestAnalysis = analyses[0]; // Already ordered by created_at desc
      return this.transformRecord(latestAnalysis, {
        user_id: 'userId',
        original_file_name: 'originalFileName',
        extracted_text: 'extractedText',
        structured_data: 'structuredData',
        confidence_scores: 'confidenceScores',
        canadian_market_analysis: 'canadianMarketAnalysis',
        personal_info: 'personalInfo',
        professional_summary: 'professionalSummary',
        work_experience: 'workExperience',
        processing_method: 'processingMethod',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { userId, useServiceRole });
  }

  /**
   * Parse JSON fields in analysis data
   * @param {Object} analysis - Analysis record
   * @returns {Object} Analysis with parsed JSON fields
   */
  parseAnalysisData(analysis) {
    if (!analysis) return null;

    const parsed = { ...analysis };

    // Parse JSON fields
    const jsonFields = ['confidence_scores', 'canadian_market_analysis', 'personal_info', 'skills', 'work_experience', 'education', 'certifications', 'projects', 'metadata'];
    
    jsonFields.forEach(field => {
      if (parsed[field] && typeof parsed[field] === 'string') {
        try {
          parsed[field] = JSON.parse(parsed[field]);
        } catch (error) {
          this.logger.warn(`Failed to parse JSON field ${field}:`, error);
          parsed[field] = null;
        }
      }
    });

    return parsed;
  }

  /**
   * Get resume analysis with parsed data
   * @param {string|number} analysisId - Analysis ID
   * @param {string|number} userId - User ID for permission check
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} Resume analysis with parsed data or null
   */
  async getResumeAnalysisWithParsedData(analysisId, userId = null, useServiceRole = false) {
    return this.executeMethod('getResumeAnalysisWithParsedData', async (params) => {
      const analysis = await this.getResumeAnalysisById(params.analysisId, params.userId, params.useServiceRole);
      if (!analysis) return null;

      return this.parseAnalysisData(analysis);
    }, { analysisId, userId, useServiceRole });
  }
}

module.exports = ResumeService;
````

## File: src/services/ServiceFactory.js
````javascript
const { createSupabaseClient, createSupabaseAdminClient } = require('../config/database');
const { UserRepository, ResumeRepository, CareerProfileRepository, GeneratedResumeRepository } = require('../repositories');
const { UserService, ResumeService, CanadianResumeService } = require('./');

/**
 * Service Factory for creating and managing service instances
 * This factory ensures proper dependency injection and singleton patterns
 */
class ServiceFactory {
  constructor() {
    this.services = new Map();
    this.repositories = new Map();
    this.initialized = false;
  }

  /**
   * Initialize the service factory with database connections
   */
  async initialize() {
    if (this.initialized) {
      return;
    }

    try {
      // Create database clients
      const supabase = createSupabaseClient();
      const supabaseService = createSupabaseAdminClient();
      
      // Initialize repositories
      await this.initializeRepositories(supabase, supabaseService);
      
      // Initialize services
      await this.initializeServices();
      
      this.initialized = true;
    } catch (error) {
      throw new Error(`Failed to initialize ServiceFactory: ${error.message}`);
    }
  }

  /**
   * Initialize all repositories with database connections
   * @param {Object} supabase - Supabase client
   * @param {Object} supabaseService - Supabase service role client
   */
  async initializeRepositories(supabase, supabaseService) {
    // Create repository instances
    const userRepository = new UserRepository(supabase, supabaseService);
    const resumeRepository = new ResumeRepository(supabase, supabaseService);
    const careerProfileRepository = new CareerProfileRepository(supabase, supabaseService);
    const generatedResumeRepository = new GeneratedResumeRepository(supabase, supabaseService);

    // Store repositories
    this.repositories.set('user', userRepository);
    this.repositories.set('resume', resumeRepository);
    this.repositories.set('careerProfile', careerProfileRepository);
    this.repositories.set('generatedResume', generatedResumeRepository);
  }

  /**
   * Initialize all services with their required repositories
   */
  async initializeServices() {
    // Create service instances with repositories
    const userService = new UserService({
      user: this.repositories.get('user')
    });

    const resumeService = new ResumeService({
      resume: this.repositories.get('resume'),
      user: this.repositories.get('user')
    });

    const canadianResumeService = new CanadianResumeService({
      resume: this.repositories.get('resume'),
      user: this.repositories.get('user'),
      careerProfile: this.repositories.get('careerProfile'),
      generatedResume: this.repositories.get('generatedResume')
    });

    // Store services
    this.services.set('user', userService);
    this.services.set('resume', resumeService);
    this.services.set('canadianResume', canadianResumeService);
  }

  /**
   * Get a service by name
   * @param {string} serviceName - Name of the service
   * @returns {Object} Service instance
   */
  getService(serviceName) {
    if (!this.initialized) {
      throw new Error('ServiceFactory not initialized. Call initialize() first.');
    }

    const service = this.services.get(serviceName);
    if (!service) {
      throw new Error(`Service '${serviceName}' not found`);
    }

    return service;
  }

  /**
   * Get a repository by name
   * @param {string} repositoryName - Name of the repository
   * @returns {Object} Repository instance
   */
  getRepository(repositoryName) {
    if (!this.initialized) {
      throw new Error('ServiceFactory not initialized. Call initialize() first.');
    }

    const repository = this.repositories.get(repositoryName);
    if (!repository) {
      throw new Error(`Repository '${repositoryName}' not found`);
    }

    return repository;
  }

  /**
   * Get all services as an object
   * @returns {Object} All services
   */
  getAllServices() {
    if (!this.initialized) {
      throw new Error('ServiceFactory not initialized. Call initialize() first.');
    }

    const services = {};
    for (const [name, service] of this.services) {
      services[name] = service;
    }

    return services;
  }

  /**
   * Get all repositories as an object
   * @returns {Object} All repositories
   */
  getAllRepositories() {
    if (!this.initialized) {
      throw new Error('ServiceFactory not initialized. Call initialize() first.');
    }

    const repositories = {};
    for (const [name, repository] of this.repositories) {
      repositories[name] = repository;
    }

    return repositories;
  }

  /**
   * Check if a service exists
   * @param {string} serviceName - Name of the service
   * @returns {boolean} Whether the service exists
   */
  hasService(serviceName) {
    return this.services.has(serviceName);
  }

  /**
   * Check if a repository exists
   * @param {string} repositoryName - Name of the repository
   * @returns {boolean} Whether the repository exists
   */
  hasRepository(repositoryName) {
    return this.repositories.has(repositoryName);
  }

  /**
   * Get list of available service names
   * @returns {Array} Array of service names
   */
  getAvailableServices() {
    return Array.from(this.services.keys());
  }

  /**
   * Get list of available repository names
   * @returns {Array} Array of repository names
   */
  getAvailableRepositories() {
    return Array.from(this.repositories.keys());
  }

  /**
   * Reset the factory (useful for testing)
   */
  reset() {
    this.services.clear();
    this.repositories.clear();
    this.initialized = false;
  }

  /**
   * Health check for all services
   * @returns {Object} Health status
   */
  async healthCheck() {
    if (!this.initialized) {
      return {
        status: 'error',
        message: 'ServiceFactory not initialized',
        services: {},
        repositories: {}
      };
    }

    const health = {
      status: 'healthy',
      message: 'All services and repositories are healthy',
      services: {},
      repositories: {},
      timestamp: new Date().toISOString()
    };

    // Check repositories
    for (const [name, repository] of this.repositories) {
      try {
        // Simple health check - try to count records
        await repository.count({}, false);
        health.repositories[name] = { status: 'healthy' };
      } catch (error) {
        health.repositories[name] = { 
          status: 'error', 
          error: error.message 
        };
        health.status = 'error';
        health.message = 'Some repositories are unhealthy';
      }
    }

    // Check services
    for (const [name, service] of this.services) {
      try {
        // Simple health check - check if service has required repositories
        const hasRepositories = service.repositories && Object.keys(service.repositories).length > 0;
        health.services[name] = { 
          status: hasRepositories ? 'healthy' : 'warning',
          message: hasRepositories ? 'Service is healthy' : 'Service has no repositories'
        };
        
        if (!hasRepositories) {
          health.status = 'warning';
          health.message = 'Some services have warnings';
        }
      } catch (error) {
        health.services[name] = { 
          status: 'error', 
          error: error.message 
        };
        health.status = 'error';
        health.message = 'Some services are unhealthy';
      }
    }

    return health;
  }
}

// Create singleton instance
const serviceFactory = new ServiceFactory();

module.exports = serviceFactory;
````

## File: src/services/supabaseDatabase.js
````javascript
const { createClient } = require('@supabase/supabase-js');

class SupabaseDatabase {
  constructor() {
    this.supabase = createClient(
      process.env.SUPABASE_URL,
      process.env.SUPABASE_ANON_KEY
    );
    
    // Create service role client for operations that need to bypass RLS
    this.supabaseService = createClient(
      process.env.SUPABASE_URL,
      process.env.SUPABASE_SERVICE_ROLE_KEY
    );
  }

  async connect() {
    try {
      // Test the connection
      const { data, error } = await this.supabase.from('users').select('count').limit(1);
      if (error) {
        console.error('❌ Supabase connection failed:', error);
        throw error;
      }
      console.log('✅ Supabase Database connected successfully');
    } catch (error) {
      console.error('❌ Supabase Database connection failed:', error);
      throw error;
    }
  }

  async disconnect() {
    // Supabase client doesn't need explicit disconnection
    console.log('✅ Supabase connection closed');
  }

  // User management for AI features
  async findOrCreateUser(userData) {
    console.log('🔍 Starting findOrCreateUser with:', JSON.stringify(userData, null, 2));
    
    try {
      console.log('🔍 Searching for user by email:', userData.email);
      
      // Try to find existing user by email using service role to bypass RLS
      const { data: existingUser, error: findError } = await this.supabaseService
        .from('users')
        .select('*')
        .eq('email', userData.email)
        .single();

      if (findError && findError.code !== 'PGRST116') {
        console.error('❌ Error finding user:', findError);
        throw findError;
      }

      if (existingUser) {
        console.log('✅ Found existing AI user by email:', existingUser.email, 'with ID:', existingUser.id);
        console.log('✅ User details:', JSON.stringify(existingUser, null, 2));
        return existingUser;
      }

      // If user doesn't exist, create them using service role to bypass RLS
      const { data: newUser, error: createError } = await this.supabaseService
        .from('users')
        .insert({
          email: userData.email,
          full_name: userData.fullName || 'User',
          phone_no: userData.phoneNo,
          status_in_canada: userData.statusInCanada,
          country_of_origin: userData.countryOfOrigin,
          current_location: userData.currentLocation,
          role_id: 3, // Immigrant role (ID 3 based on database)
          created_at: new Date().toISOString()
        })
        .select()
        .single();

      if (createError) {
        console.error('❌ Error creating user:', createError);
        throw createError;
      }

      console.log('✅ New AI user created:', newUser.id);
      return newUser;

    } catch (error) {
      console.error('❌ Error finding/creating AI user:', error);
      throw error;
    }
  }

  // Update user profile
  async updateUser(userId, userData) {
    console.log('🔍 Starting updateUser for ID:', userId, 'with data:', JSON.stringify(userData, null, 2));
    
    try {
      const updateData = {};
      
      if (userData.fullName) updateData.full_name = userData.fullName;
      if (userData.phoneNo) updateData.phone_no = userData.phoneNo;
      if (userData.statusInCanada) updateData.status_in_canada = userData.statusInCanada;
      if (userData.countryOfOrigin) updateData.country_of_origin = userData.countryOfOrigin;
      if (userData.currentLocation) updateData.current_location = userData.currentLocation;
      
      updateData.updated_at = new Date().toISOString();

      const { data: updatedUser, error } = await this.supabaseService
        .from('users')
        .update(updateData)
        .eq('id', userId)
        .select()
        .single();

      if (error) {
        console.error('❌ Error updating user:', error);
        throw error;
      }

      console.log('✅ User updated successfully:', updatedUser.id);
      return updatedUser;

    } catch (error) {
      console.error('❌ Error updating user:', error);
      throw error;
    }
  }

  // Resume Analysis methods
  async saveResumeAnalysis(userId, analysisData) {
    console.log('💾 Starting saveResumeAnalysis for user:', userId);
    console.log('💾 Analysis data keys:', Object.keys(analysisData));
    
    try {
      // Ensure userId is a valid number (database serial ID)
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      // Use service role client to bypass RLS policies
      const { data: analysis, error } = await this.supabaseService
        .from('resume_analyses')
        .insert({
          user_id: numericUserId,
          original_file_name: analysisData.originalFileName,
          extracted_text: analysisData.rawText || analysisData.extractedText || 'Text extracted from resume',
          structured_data: analysisData.structuredData || null,
          confidence_scores: JSON.stringify(analysisData.confidenceScores || {}),
          canadian_market_analysis: JSON.stringify(analysisData.canadianMarketAnalysis || {}),
          personal_info: JSON.stringify(analysisData.personalInfo || {}),
          professional_summary: analysisData.professionalSummary || '',
          skills: JSON.stringify(analysisData.skills || {}),
          work_experience: JSON.stringify(analysisData.workExperience || []),
          education: JSON.stringify(analysisData.education || []),
          certifications: JSON.stringify(analysisData.certifications || []),
          projects: JSON.stringify(analysisData.projects || []),
          metadata: JSON.stringify(analysisData.metadata || {}),
          processing_method: analysisData.processingMethod || 'unknown',
          created_at: new Date().toISOString()
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error saving resume analysis:', error);
        console.error('❌ Error details:', {
          code: error.code,
          message: error.message,
          details: error.details,
          hint: error.hint
        });
        throw error;
      }

      console.log('✅ Resume analysis saved successfully with ID:', analysis.id);
      console.log('✅ Saved analysis data:', {
        id: analysis.id,
        userId: analysis.user_id,
        fileName: analysis.original_file_name,
        createdAt: analysis.created_at
      });

      return analysis;
    } catch (error) {
      console.error('❌ Error saving resume analysis:', error);
      console.error('❌ Error stack:', error.stack);
      throw error;
    }
  }

  async getResumeAnalyses(userId) {
    try {
      // Ensure userId is a valid number (database serial ID)
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      const { data: analyses, error } = await this.supabase
        .from('resume_analyses')
        .select('*')
        .eq('user_id', numericUserId)
        .order('created_at', { ascending: false });

      if (error) {
        console.error('❌ Error fetching resume analyses:', error);
        throw error;
      }

      return analyses;
    } catch (error) {
      console.error('❌ Error fetching resume analyses:', error);
      throw error;
    }
  }

  // Alias for getUserResumeAnalyses to maintain compatibility
  async getUserResumeAnalyses(userId) {
    console.log('🔍 Starting getUserResumeAnalyses for user:', userId);
    
    try {
      // Ensure userId is a valid number (database serial ID)
      const numericUserId = parseInt(userId);
      if (isNaN(numericUserId)) {
        throw new Error(`Invalid user ID: ${userId}. Expected a numeric database user ID.`);
      }
      
      // Use service role client to bypass RLS policies
      const { data: analyses, error } = await this.supabaseService
        .from('resume_analyses')
        .select('*')
        .eq('user_id', numericUserId)
        .order('created_at', { ascending: false });

      if (error) {
        console.error('❌ Error fetching resume analyses:', error);
        console.error('❌ Error details:', {
          code: error.code,
          message: error.message,
          details: error.details,
          hint: error.hint
        });
        throw error;
      }

      console.log('✅ Retrieved', analyses.length, 'resume analyses for user:', userId);
      if (analyses.length > 0) {
        console.log('✅ Sample analysis:', {
          id: analyses[0].id,
          fileName: analyses[0].original_file_name,
          createdAt: analyses[0].created_at
        });
      }

      return analyses;
    } catch (error) {
      console.error('❌ Error fetching resume analyses:', error);
      console.error('❌ Error stack:', error.stack);
      throw error;
    }
  }

  async getResumeAnalysisById(analysisId) {
    try {
      const { data: analysis, error } = await this.supabase
        .from('resume_analyses')
        .select('*')
        .eq('id', analysisId)
        .single();

      if (error) {
        console.error('❌ Error fetching resume analysis:', error);
        throw error;
      }

      return analysis;
    } catch (error) {
      console.error('❌ Error fetching resume analysis:', error);
      throw error;
    }
  }

  // Career Profile methods
  async saveCareerProfile(userId, profileData) {
    try {
      const { data: profile, error } = await this.supabase
        .from('user_career_profiles')
        .upsert({
          user_id: parseInt(userId),
          professional_summary: profileData.professionalSummary,
          skills_categories: profileData.skillsCategories,
          career_objectives: profileData.careerObjectives,
          target_industries: profileData.targetIndustries,
          market_alignment_score: profileData.marketAlignmentScore,
          skill_gaps: profileData.skillGaps,
          improvement_roadmap: profileData.improvementRoadmap,
          last_updated: new Date().toISOString()
        }, {
          onConflict: 'user_id'
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error saving career profile:', error);
        throw error;
      }

      return profile;
    } catch (error) {
      console.error('❌ Error saving career profile:', error);
      throw error;
    }
  }

  async getCareerProfile(userId) {
    try {
      const { data: profile, error } = await this.supabase
        .from('user_career_profiles')
        .select('*')
        .eq('user_id', userId)
        .single();

      if (error && error.code !== 'PGRST116') {
        console.error('❌ Error fetching career profile:', error);
        throw error;
      }

      return profile;
    } catch (error) {
      console.error('❌ Error fetching career profile:', error);
      throw error;
    }
  }

  // Job Opportunities methods
  async saveJobOpportunity(jobData) {
    try {
      const { data: job, error } = await this.supabase
        .from('job_opportunities')
        .insert({
          title: jobData.title,
          company: jobData.company,
          location: jobData.location,
          description: jobData.description,
          requirements: jobData.requirements,
          salary_range: jobData.salaryRange,
          job_url: jobData.jobUrl,
          is_newcomer_friendly: jobData.isNewcomerFriendly,
          discovered_at: new Date().toISOString(),
          is_active: true
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error saving job opportunity:', error);
        throw error;
      }

      return job;
    } catch (error) {
      console.error('❌ Error saving job opportunity:', error);
      throw error;
    }
  }

  async getJobOpportunities(filters = {}) {
    try {
      let query = this.supabase
        .from('job_opportunities')
        .select('*')
        .eq('is_active', true);

      if (filters.location) {
        query = query.ilike('location', `%${filters.location}%`);
      }

      if (filters.title) {
        query = query.ilike('title', `%${filters.title}%`);
      }

      if (filters.isNewcomerFriendly !== undefined) {
        query = query.eq('is_newcomer_friendly', filters.isNewcomerFriendly);
      }

      const { data: jobs, error } = await query.order('discovered_at', { ascending: false });

      if (error) {
        console.error('❌ Error fetching job opportunities:', error);
        throw error;
      }

      return jobs;
    } catch (error) {
      console.error('❌ Error fetching job opportunities:', error);
      throw error;
    }
  }

  // Job Matches methods
  async saveJobMatch(matchData) {
    try {
      const { data: match, error } = await this.supabase
        .from('job_matches')
        .insert({
          user_id: parseInt(matchData.userId),
          job_id: parseInt(matchData.jobId),
          match_score: matchData.matchScore,
          match_analysis: matchData.matchAnalysis,
          skills_gaps: matchData.skillsGaps,
          application_status: matchData.applicationStatus || 'not_applied',
          created_at: new Date().toISOString()
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error saving job match:', error);
        throw error;
      }

      return match;
    } catch (error) {
      console.error('❌ Error saving job match:', error);
      throw error;
    }
  }

  async getJobMatches(userId) {
    try {
      const { data: matches, error } = await this.supabase
        .from('job_matches')
        .select(`
          *,
          job_opportunities (
            id,
            title,
            company,
            location,
            description,
            requirements,
            salary_range,
            job_url,
            is_newcomer_friendly
          )
        `)
        .eq('user_id', userId)
        .order('created_at', { ascending: false });

      if (error) {
        console.error('❌ Error fetching job matches:', error);
        throw error;
      }

      return matches;
    } catch (error) {
      console.error('❌ Error fetching job matches:', error);
      throw error;
    }
  }

  // Skill Gap Analysis methods
  async saveSkillGapAnalysis(userId, analysisData) {
    try {
      const { data: analysis, error } = await this.supabase
        .from('skill_gap_analyses')
        .insert({
          user_id: parseInt(userId),
          current_skills: analysisData.currentSkills,
          target_skills: analysisData.targetSkills,
          identified_gaps: analysisData.identifiedGaps,
          learning_path: analysisData.learningPath,
          progress_tracking: analysisData.progressTracking,
          last_updated: new Date().toISOString()
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error saving skill gap analysis:', error);
        throw error;
      }

      return analysis;
    } catch (error) {
      console.error('❌ Error saving skill gap analysis:', error);
      throw error;
    }
  }

  async getSkillGapAnalysis(userId) {
    try {
      const { data: analysis, error } = await this.supabase
        .from('skill_gap_analyses')
        .select('*')
        .eq('user_id', userId)
        .order('last_updated', { ascending: false })
        .limit(1)
        .single();

      if (error && error.code !== 'PGRST116') {
        console.error('❌ Error fetching skill gap analysis:', error);
        throw error;
      }

      return analysis;
    } catch (error) {
      console.error('❌ Error fetching skill gap analysis:', error);
      throw error;
    }
  }

  // User Documents methods
  async saveUserDocument(userId, documentData) {
    try {
      const { data: document, error } = await this.supabase
        .from('user_documents')
        .insert({
          user_id: parseInt(userId),
          file_name: documentData.fileName,
          file_type: documentData.fileType,
          file_path: documentData.filePath,
          created_at: new Date().toISOString()
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error saving user document:', error);
        throw error;
      }

      return document;
    } catch (error) {
      console.error('❌ Error saving user document:', error);
      throw error;
    }
  }

  async getUserDocuments(userId) {
    try {
      const { data: documents, error } = await this.supabase
        .from('user_documents')
        .select('*')
        .eq('user_id', userId)
        .order('created_at', { ascending: false });

      if (error) {
        console.error('❌ Error fetching user documents:', error);
        throw error;
      }

      return documents;
    } catch (error) {
      console.error('❌ Error fetching user documents:', error);
      throw error;
    }
  }

  // Additional methods for CareerProfileService
  async fetchUserCareerProfile(userId) {
    try {
      const { data: profile, error } = await this.supabase
        .from('user_career_profiles')
        .select('*')
        .eq('user_id', userId)
        .single();

      if (error && error.code !== 'PGRST116') {
        console.error('❌ Error fetching user career profile:', error);
        throw error;
      }

      return profile;
    } catch (error) {
      console.error('❌ Error fetching user career profile:', error);
      throw error;
    }
  }

  async updateUserCareerProfile(userId, profileData) {
    try {
      const { data: profile, error } = await this.supabase
        .from('user_career_profiles')
        .update({
          professional_summary: profileData.professionalSummary,
          skills_categories: profileData.skillsCategories,
          career_objectives: profileData.careerObjectives,
          target_industries: profileData.targetIndustries,
          market_alignment_score: profileData.marketAlignmentScore,
          skill_gaps: profileData.skillGaps,
          improvement_roadmap: profileData.improvementRoadmap,
          last_updated: new Date().toISOString()
        })
        .eq('user_id', userId)
        .select()
        .single();

      if (error) {
        console.error('❌ Error updating user career profile:', error);
        throw error;
      }

      return profile;
    } catch (error) {
      console.error('❌ Error updating user career profile:', error);
      throw error;
    }
  }

  async createUserCareerProfile(profileData) {
    try {
      const { data: profile, error } = await this.supabase
        .from('user_career_profiles')
        .insert({
          user_id: parseInt(profileData.userId),
          professional_summary: profileData.professionalSummary,
          skills_categories: profileData.skillsCategories,
          career_objectives: profileData.careerObjectives,
          target_industries: profileData.targetIndustries,
          market_alignment_score: profileData.marketAlignmentScore,
          skill_gaps: profileData.skillGaps,
          improvement_roadmap: profileData.improvementRoadmap,
          created_at: new Date().toISOString(),
          last_updated: new Date().toISOString()
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error creating user career profile:', error);
        throw error;
      }

      return profile;
    } catch (error) {
      console.error('❌ Error creating user career profile:', error);
      throw error;
    }
  }

  async fetchJobOpportunity(title, company) {
    try {
      const { data: job, error } = await this.supabase
        .from('job_opportunities')
        .select('*')
        .eq('title', title)
        .eq('company', company)
        .single();

      if (error && error.code !== 'PGRST116') {
        console.error('❌ Error fetching job opportunity:', error);
        throw error;
      }

      return job;
    } catch (error) {
      console.error('❌ Error fetching job opportunity:', error);
      throw error;
    }
  }

  async createJobOpportunity(jobData) {
    try {
      const { data: job, error } = await this.supabase
        .from('job_opportunities')
        .insert({
          title: jobData.title,
          company: jobData.company,
          location: jobData.location,
          description: jobData.description,
          requirements: jobData.requirements,
          salary_range: jobData.salaryRange,
          job_url: jobData.jobUrl,
          is_newcomer_friendly: jobData.isNewcomerFriendly,
          discovered_at: new Date().toISOString(),
          is_active: true
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error creating job opportunity:', error);
        throw error;
      }

      return job;
    } catch (error) {
      console.error('❌ Error creating job opportunity:', error);
      throw error;
    }
  }

  async createJobMatch(matchData) {
    try {
      const { data: match, error } = await this.supabase
        .from('job_matches')
        .insert({
          user_id: parseInt(matchData.userId),
          job_id: parseInt(matchData.jobId),
          match_score: matchData.matchScore,
          match_analysis: matchData.matchAnalysis,
          skills_gaps: matchData.skillsGaps,
          application_status: matchData.applicationStatus || 'not_applied',
          created_at: new Date().toISOString()
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error creating job match:', error);
        throw error;
      }

      return match;
    } catch (error) {
      console.error('❌ Error creating job match:', error);
      throw error;
    }
  }

  async createResumeAnalysis(analysisData) {
    try {
      const { data: analysis, error } = await this.supabase
        .from('resume_analyses')
        .insert({
          user_id: parseInt(analysisData.userId),
          original_file_name: analysisData.originalFileName,
          extracted_text: analysisData.extractedText,
          structured_data: analysisData.structuredData,
          confidence_scores: analysisData.confidenceScores,
          canadian_market_analysis: analysisData.canadianMarketAnalysis,
          personal_info: analysisData.personalInfo,
          professional_summary: analysisData.professionalSummary,
          skills: analysisData.skills,
          work_experience: analysisData.workExperience,
          education: analysisData.education,
          certifications: analysisData.certifications,
          projects: analysisData.projects,
          metadata: analysisData.metadata,
          processing_method: analysisData.processingMethod,
          created_at: new Date().toISOString()
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error creating resume analysis:', error);
        throw error;
      }

      return analysis;
    } catch (error) {
      console.error('❌ Error creating resume analysis:', error);
      throw error;
    }
  }

  async getUserCareerProfile(userId) {
    try {
      const { data: profile, error } = await this.supabase
        .from('user_career_profiles')
        .select('*')
        .eq('user_id', userId)
        .single();

      if (error && error.code !== 'PGRST116') {
        console.error('❌ Error fetching user career profile:', error);
        throw error;
      }

      return profile;
    } catch (error) {
      console.error('❌ Error fetching user career profile:', error);
      throw error;
    }
  }

  async createSkillGapAnalysis(analysisData) {
    try {
      const { data: analysis, error } = await this.supabase
        .from('skill_gap_analyses')
        .insert({
          user_id: parseInt(analysisData.userId),
          current_skills: analysisData.currentSkills,
          target_skills: analysisData.targetSkills,
          identified_gaps: analysisData.identifiedGaps,
          learning_path: analysisData.learningPath,
          progress_tracking: analysisData.progressTracking,
          last_updated: new Date().toISOString()
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error creating skill gap analysis:', error);
        throw error;
      }

      return analysis;
    } catch (error) {
      console.error('❌ Error creating skill gap analysis:', error);
      throw error;
    }
  }

  async getSkillGapAnalyses(userId) {
    try {
      const { data: analyses, error } = await this.supabase
        .from('skill_gap_analyses')
        .select('*')
        .eq('user_id', userId)
        .order('last_updated', { ascending: false })
        .limit(5);

      if (error) {
        console.error('❌ Error fetching skill gap analyses:', error);
        throw error;
      }

      return analyses;
    } catch (error) {
      console.error('❌ Error fetching skill gap analyses:', error);
      throw error;
    }
  }

  async updateJobMatchStatus(jobMatchId, status) {
    try {
      const { data: match, error } = await this.supabase
        .from('job_matches')
        .update({
          application_status: status
        })
        .eq('id', jobMatchId)
        .select()
        .single();

      if (error) {
        console.error('❌ Error updating job match status:', error);
        throw error;
      }

      return { count: 1, data: match };
    } catch (error) {
      console.error('❌ Error updating job match status:', error);
      throw error;
    }
  }

  // Enhanced career profile methods
  async saveEnhancedCareerProfile(userId, profileData) {
    try {
      const { data: profile, error } = await this.supabase
        .from('enhanced_career_profiles')
        .upsert({
          user_id: parseInt(userId),
          target_position: profileData.targetPosition,
          enhanced_profile: profileData.enhancedProfile,
          resume_analysis_id: profileData.resumeAnalysisId,
          created_at: new Date().toISOString(),
          last_updated: new Date().toISOString()
        }, {
          onConflict: 'user_id'
        })
        .select()
        .single();

      if (error) {
        console.error('❌ Error saving enhanced career profile:', error);
        throw error;
      }

      return profile;
    } catch (error) {
      console.error('❌ Error saving enhanced career profile:', error);
      throw error;
    }
  }

  async getEnhancedCareerProfile(userId) {
    try {
      const { data: profile, error } = await this.supabase
        .from('enhanced_career_profiles')
        .select('*')
        .eq('user_id', userId)
        .order('last_updated', { ascending: false })
        .limit(1)
        .single();

      if (error && error.code !== 'PGRST116') {
        console.error('❌ Error fetching enhanced career profile:', error);
        throw error;
      }

      return profile;
    } catch (error) {
      console.error('❌ Error fetching enhanced career profile:', error);
      throw error;
    }
  }
}

module.exports = SupabaseDatabase;
````

## File: src/services/UserService.js
````javascript
const BaseService = require('./BaseService');
const { AppError } = require('../utils/errors');

/**
 * User Service for user-related business logic
 */
class UserService extends BaseService {
  constructor(repositories) {
    super(repositories);
    this.userRepository = this.getRepository('user');
  }

  /**
   * Find or create a user
   * @param {Object} userData - User data
   * @returns {Promise<Object>} User record
   */
  async findOrCreateUser(userData) {
    return this.executeMethod('findOrCreateUser', async (params) => {
      this.validateRequiredParams(params, ['email']);
      
      const user = await this.userRepository.findOrCreateUser(params);
      return this.transformRecord(user, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, userData);
  }

  /**
   * Update user profile
   * @param {string|number} userId - User ID
   * @param {Object} userData - User data to update
   * @returns {Promise<Object>} Updated user record
   */
  async updateUser(userId, userData) {
    return this.executeMethod('updateUser', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      const user = await this.userRepository.updateUser(validatedUserId, params.userData);
      return this.transformRecord(user, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { userId, userData });
  }

  /**
   * Get user by ID
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} User record or null
   */
  async getUserById(userId, useServiceRole = false) {
    return this.executeMethod('getUserById', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      const user = await this.userRepository.findById(validatedUserId, params.useServiceRole);
      if (!user) return null;

      return this.transformRecord(user, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { userId, useServiceRole });
  }

  /**
   * Get user by email
   * @param {string} email - User email
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object|null>} User record or null
   */
  async getUserByEmail(email, useServiceRole = false) {
    return this.executeMethod('getUserByEmail', async (params) => {
      if (!params.email) {
        throw new AppError('Email is required', 400);
      }

      const user = await this.userRepository.findByEmail(params.email, params.useServiceRole);
      if (!user) return null;

      return this.transformRecord(user, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { email, useServiceRole });
  }

  /**
   * Search users with criteria
   * @param {Object} criteria - Search criteria
   * @param {Object} options - Query options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Matching users
   */
  async searchUsers(criteria = {}, options = {}, useServiceRole = false) {
    return this.executeMethod('searchUsers', async (params) => {
      const allowedFields = ['email', 'fullName', 'roleId', 'statusInCanada', 'countryOfOrigin', 'currentLocation'];
      const sanitizedCriteria = this.sanitizeSearchCriteria(params.criteria, allowedFields);
      const paginationOptions = this.validatePaginationOptions(params.options);

      const users = await this.userRepository.searchUsers(sanitizedCriteria, paginationOptions, params.useServiceRole);
      return this.transformRecords(users, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { criteria, options, useServiceRole });
  }

  /**
   * Get users with pagination
   * @param {Object} options - Pagination options
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} Users with pagination info
   */
  async getUsersWithPagination(options = {}, useServiceRole = false) {
    return this.executeMethod('getUsersWithPagination', async (params) => {
      const paginationOptions = this.validatePaginationOptions(params.options);

      const users = await this.userRepository.findAll(paginationOptions, params.useServiceRole);
      const total = await this.userRepository.count({}, params.useServiceRole);

      const transformedUsers = this.transformRecords(users, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });

      return this.createPaginatedResponse(
        transformedUsers,
        total,
        paginationOptions.limit,
        paginationOptions.offset
      );
    }, { options, useServiceRole });
  }

  /**
   * Get users by role
   * @param {number} roleId - Role ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Users with the specified role
   */
  async getUsersByRole(roleId, useServiceRole = false) {
    return this.executeMethod('getUsersByRole', async (params) => {
      if (!params.roleId || isNaN(parseInt(params.roleId))) {
        throw new AppError('Valid role ID is required', 400);
      }

      const users = await this.userRepository.findByRole(parseInt(params.roleId), params.useServiceRole);
      return this.transformRecords(users, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { roleId, useServiceRole });
  }

  /**
   * Get users by status in Canada
   * @param {string} status - Status in Canada
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Users with the specified status
   */
  async getUsersByStatusInCanada(status, useServiceRole = false) {
    return this.executeMethod('getUsersByStatusInCanada', async (params) => {
      if (!params.status) {
        throw new AppError('Status is required', 400);
      }

      const users = await this.userRepository.findByStatusInCanada(params.status, params.useServiceRole);
      return this.transformRecords(users, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { status, useServiceRole });
  }

  /**
   * Get users by country of origin
   * @param {string} country - Country of origin
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Users from the specified country
   */
  async getUsersByCountryOfOrigin(country, useServiceRole = false) {
    return this.executeMethod('getUsersByCountryOfOrigin', async (params) => {
      if (!params.country) {
        throw new AppError('Country is required', 400);
      }

      const users = await this.userRepository.findByCountryOfOrigin(params.country, params.useServiceRole);
      return this.transformRecords(users, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { country, useServiceRole });
  }

  /**
   * Get users by current location
   * @param {string} location - Current location
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Array>} Users in the specified location
   */
  async getUsersByCurrentLocation(location, useServiceRole = false) {
    return this.executeMethod('getUsersByCurrentLocation', async (params) => {
      if (!params.location) {
        throw new AppError('Location is required', 400);
      }

      const users = await this.userRepository.findByCurrentLocation(params.location, params.useServiceRole);
      return this.transformRecords(users, {
        full_name: 'fullName',
        phone_no: 'phoneNo',
        status_in_canada: 'statusInCanada',
        country_of_origin: 'countryOfOrigin',
        current_location: 'currentLocation',
        role_id: 'roleId',
        created_at: 'createdAt',
        updated_at: 'updatedAt'
      });
    }, { location, useServiceRole });
  }

  /**
   * Get user statistics
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<Object>} User statistics
   */
  async getUserStatistics(useServiceRole = false) {
    return this.executeMethod('getUserStatistics', async (params) => {
      return await this.userRepository.getUserStatistics(params.useServiceRole);
    }, { useServiceRole });
  }

  /**
   * Delete user
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<boolean>} Success status
   */
  async deleteUser(userId, useServiceRole = false) {
    return this.executeMethod('deleteUser', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      return await this.userRepository.deleteById(validatedUserId, params.useServiceRole);
    }, { userId, useServiceRole });
  }

  /**
   * Check if user exists
   * @param {string|number} userId - User ID
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<boolean>} Whether user exists
   */
  async userExists(userId, useServiceRole = false) {
    return this.executeMethod('userExists', async (params) => {
      const validatedUserId = this.validateUserId(params.userId);
      
      const user = await this.userRepository.findById(validatedUserId, params.useServiceRole);
      return !!user;
    }, { userId, useServiceRole });
  }

  /**
   * Get user count
   * @param {Object} filter - Filter conditions
   * @param {boolean} useServiceRole - Whether to use service role client
   * @returns {Promise<number>} User count
   */
  async getUserCount(filter = {}, useServiceRole = false) {
    return this.executeMethod('getUserCount', async (params) => {
      return await this.userRepository.count(params.filter, params.useServiceRole);
    }, { filter, useServiceRole });
  }
}

module.exports = UserService;
````

## File: src/utils/databaseOptimization.js
````javascript
/**
 * Database Query Optimization Utilities
 * Provides query caching, connection pooling, and performance monitoring
 */

const { logger } = require('../config/logger');
const { cacheConfig } = require('../config/cache');

class DatabaseOptimizer {
  constructor() {
    this.queryStats = new Map();
    this.slowQueryThreshold = 1000; // 1 second
    this.queryCache = new Map();
    this.connectionPool = new Map();
    this.performanceMetrics = {
      totalQueries: 0,
      cachedQueries: 0,
      slowQueries: 0,
      failedQueries: 0,
      averageResponseTime: 0,
      totalResponseTime: 0
    };
  }

  /**
   * Query caching wrapper
   * @param {string} cacheKey - Unique key for the query
   * @param {Function} queryFunction - The actual query function
   * @param {string} cacheType - Type of cache strategy
   * @param {number} ttl - Time to live in seconds
   * @returns {Promise} Query result
   */
  async cachedQuery(cacheKey, queryFunction, cacheType = 'static', ttl = null) {
    const startTime = Date.now();
    
    try {
      // Check cache first
      if (cacheConfig.isConnected) {
        const cachedResult = await cacheConfig.get(cacheType, cacheKey);
        if (cachedResult) {
          this.performanceMetrics.cachedQueries++;
          this.logQueryPerformance(cacheKey, Date.now() - startTime, true);
          return cachedResult;
        }
      }

      // Execute query
      const result = await queryFunction();
      
      // Cache the result
      if (cacheConfig.isConnected && result) {
        const strategy = cacheConfig.getStrategy(cacheType);
        const cacheTTL = ttl || strategy.ttl;
        await cacheConfig.set(cacheType, cacheKey, result);
      }

      this.performanceMetrics.totalQueries++;
      this.logQueryPerformance(cacheKey, Date.now() - startTime, false);
      
      return result;
    } catch (error) {
      this.performanceMetrics.failedQueries++;
      logger.error('Cached query failed:', { cacheKey, error: error.message });
      throw error;
    }
  }

  /**
   * Query performance monitoring wrapper
   * @param {string} queryName - Name/identifier for the query
   * @param {Function} queryFunction - The actual query function
   * @returns {Promise} Query result
   */
  async monitoredQuery(queryName, queryFunction) {
    const startTime = Date.now();
    
    try {
      const result = await queryFunction();
      const duration = Date.now() - startTime;
      
      // Update performance metrics
      this.performanceMetrics.totalQueries++;
      this.performanceMetrics.totalResponseTime += duration;
      this.performanceMetrics.averageResponseTime = 
        this.performanceMetrics.totalResponseTime / this.performanceMetrics.totalQueries;

      // Check for slow queries
      if (duration > this.slowQueryThreshold) {
        this.performanceMetrics.slowQueries++;
        logger.warn('Slow query detected', {
          queryName,
          duration,
          threshold: this.slowQueryThreshold
        });
      }

      // Store query statistics
      this.updateQueryStats(queryName, duration, true);
      
      return result;
    } catch (error) {
      this.performanceMetrics.failedQueries++;
      this.updateQueryStats(queryName, Date.now() - startTime, false);
      logger.error('Query failed:', { queryName, error: error.message });
      throw error;
    }
  }

  /**
   * Update query statistics
   */
  updateQueryStats(queryName, duration, success) {
    if (!this.queryStats.has(queryName)) {
      this.queryStats.set(queryName, {
        count: 0,
        totalTime: 0,
        averageTime: 0,
        minTime: Infinity,
        maxTime: 0,
        successCount: 0,
        failureCount: 0,
        lastExecuted: null
      });
    }

    const stats = this.queryStats.get(queryName);
    stats.count++;
    stats.totalTime += duration;
    stats.averageTime = stats.totalTime / stats.count;
    stats.minTime = Math.min(stats.minTime, duration);
    stats.maxTime = Math.max(stats.maxTime, duration);
    stats.lastExecuted = new Date().toISOString();

    if (success) {
      stats.successCount++;
    } else {
      stats.failureCount++;
    }
  }

  /**
   * Log query performance
   */
  logQueryPerformance(queryName, duration, cached) {
    const logData = {
      queryName,
      duration,
      cached,
      timestamp: new Date().toISOString()
    };

    if (duration > this.slowQueryThreshold) {
      logger.warn('Slow query performance', logData);
    } else if (duration > 500) { // Medium performance
      logger.info('Medium query performance', logData);
    } else {
      logger.debug('Fast query performance', logData);
    }
  }

  /**
   * Get query performance statistics
   */
  getQueryStats(queryName = null) {
    if (queryName) {
      return this.queryStats.get(queryName) || null;
    }
    
    return {
      overall: this.performanceMetrics,
      queries: Object.fromEntries(this.queryStats),
      summary: this.getPerformanceSummary()
    };
  }

  /**
   * Get performance summary
   */
  getPerformanceSummary() {
    const queries = Array.from(this.queryStats.values());
    const totalQueries = queries.reduce((sum, q) => sum + q.count, 0);
    const totalTime = queries.reduce((sum, q) => sum + q.totalTime, 0);
    const successRate = totalQueries > 0 
      ? (queries.reduce((sum, q) => sum + q.successCount, 0) / totalQueries) * 100 
      : 0;

    return {
      totalQueries,
      totalTime,
      averageTime: totalQueries > 0 ? totalTime / totalQueries : 0,
      successRate: `${successRate.toFixed(2)}%`,
      slowQueries: this.performanceMetrics.slowQueries,
      failedQueries: this.performanceMetrics.failedQueries,
      cacheHitRate: this.performanceMetrics.totalQueries > 0 
        ? `${((this.performanceMetrics.cachedQueries / this.performanceMetrics.totalQueries) * 100).toFixed(2)}%`
        : '0%'
    };
  }

  /**
   * Reset performance metrics
   */
  resetMetrics() {
    this.queryStats.clear();
    this.performanceMetrics = {
      totalQueries: 0,
      cachedQueries: 0,
      slowQueries: 0,
      failedQueries: 0,
      averageResponseTime: 0,
      totalResponseTime: 0
    };
    logger.info('Database performance metrics reset');
  }

  /**
   * Set slow query threshold
   */
  setSlowQueryThreshold(threshold) {
    this.slowQueryThreshold = threshold;
    logger.info(`Slow query threshold set to ${threshold}ms`);
  }

  /**
   * Generate optimized cache key
   */
  generateCacheKey(prefix, params) {
    const sortedParams = Object.keys(params || {})
      .sort()
      .map(key => `${key}:${params[key]}`)
      .join(':');
    
    return `${prefix}:${sortedParams}`;
  }

  /**
   * Batch query execution
   * @param {Array} queries - Array of query objects
   * @returns {Promise<Array>} Results array
   */
  async batchQueries(queries) {
    const startTime = Date.now();
    const results = [];
    const errors = [];

    try {
      // Execute queries in parallel with concurrency limit
      const concurrencyLimit = 5;
      const chunks = this.chunkArray(queries, concurrencyLimit);

      for (const chunk of chunks) {
        const chunkPromises = chunk.map(async (query) => {
          try {
            const result = await this.monitoredQuery(
              query.name || 'batch-query',
              query.function
            );
            return { success: true, result };
          } catch (error) {
            return { success: false, error: error.message };
          }
        });

        const chunkResults = await Promise.all(chunkPromises);
        results.push(...chunkResults);
      }

      const duration = Date.now() - startTime;
      logger.info('Batch queries completed', {
        totalQueries: queries.length,
        duration,
        successCount: results.filter(r => r.success).length,
        errorCount: results.filter(r => !r.success).length
      });

      return results;
    } catch (error) {
      logger.error('Batch queries failed:', error);
      throw error;
    }
  }

  /**
   * Split array into chunks
   */
  chunkArray(array, size) {
    const chunks = [];
    for (let i = 0; i < array.length; i += size) {
      chunks.push(array.slice(i, i + size));
    }
    return chunks;
  }

  /**
   * Connection pool management
   */
  async getConnection(poolName = 'default') {
    if (!this.connectionPool.has(poolName)) {
      this.connectionPool.set(poolName, {
        connections: [],
        maxConnections: 10,
        activeConnections: 0
      });
    }

    const pool = this.connectionPool.get(poolName);
    
    if (pool.activeConnections < pool.maxConnections) {
      pool.activeConnections++;
      return { poolName, connectionId: Date.now() };
    } else {
      throw new Error(`Connection pool '${poolName}' is full`);
    }
  }

  /**
   * Release connection
   */
  releaseConnection(poolName = 'default') {
    const pool = this.connectionPool.get(poolName);
    if (pool && pool.activeConnections > 0) {
      pool.activeConnections--;
    }
  }

  /**
   * Get connection pool status
   */
  getConnectionPoolStatus() {
    const status = {};
    for (const [poolName, pool] of this.connectionPool.entries()) {
      status[poolName] = {
        activeConnections: pool.activeConnections,
        maxConnections: pool.maxConnections,
        availableConnections: pool.maxConnections - pool.activeConnections
      };
    }
    return status;
  }
}

// Create singleton instance
const databaseOptimizer = new DatabaseOptimizer();

/**
 * Query optimization decorators
 */

/**
 * Cache decorator for database queries
 */
function cached(cacheType = 'static', ttl = null) {
  return function(target, propertyName, descriptor) {
    const method = descriptor.value;
    
    descriptor.value = async function(...args) {
      const cacheKey = `${target.constructor.name}:${propertyName}:${JSON.stringify(args)}`;
      return await databaseOptimizer.cachedQuery(cacheKey, () => method.apply(this, args), cacheType, ttl);
    };
    
    return descriptor;
  };
}

/**
 * Monitor decorator for database queries
 */
function monitored(queryName = null) {
  return function(target, propertyName, descriptor) {
    const method = descriptor.value;
    const name = queryName || `${target.constructor.name}.${propertyName}`;
    
    descriptor.value = async function(...args) {
      return await databaseOptimizer.monitoredQuery(name, () => method.apply(this, args));
    };
    
    return descriptor;
  };
}

module.exports = {
  databaseOptimizer,
  cached,
  monitored,
  DatabaseOptimizer
};
````

## File: src/utils/errors/AppError.js
````javascript
/**
 * Base Application Error Class
 * All custom errors should extend this class
 */

class AppError extends Error {
  constructor(message, statusCode = 500, isOperational = true, code = null) {
    super(message);
    
    this.name = this.constructor.name;
    this.statusCode = statusCode;
    this.isOperational = isOperational;
    this.code = code;
    this.timestamp = new Date().toISOString();
    
    // Capture stack trace, excluding constructor call from it
    Error.captureStackTrace(this, this.constructor);
  }
  
  /**
   * Get error response object
   */
  toResponse() {
    return {
      error: {
        message: this.message,
        code: this.code,
        statusCode: this.statusCode,
        timestamp: this.timestamp
      }
    };
  }
  
  /**
   * Get error for logging
   */
  toLog() {
    return {
      name: this.name,
      message: this.message,
      statusCode: this.statusCode,
      code: this.code,
      stack: this.stack,
      timestamp: this.timestamp,
      isOperational: this.isOperational
    };
  }
  
  /**
   * Check if error is operational
   */
  isOperationalError() {
    return this.isOperational;
  }
  
  /**
   * Get HTTP status code
   */
  getStatusCode() {
    return this.statusCode;
  }
}

module.exports = AppError;
````

## File: src/utils/errors/AuthenticationError.js
````javascript
/**
 * Authentication Error Class
 * Used for authentication and authorization errors
 */

const AppError = require('./AppError');

class AuthenticationError extends AppError {
  constructor(message, authType = null, userId = null) {
    super(message, 401, true, 'AUTHENTICATION_ERROR');
    
    this.authType = authType;
    this.userId = userId;
  }
  
  /**
   * Get error response object
   */
  toResponse() {
    const response = super.toResponse();
    
    response.error.authType = this.authType;
    
    return response;
  }
  
  /**
   * Get error for logging
   */
  toLog() {
    const log = super.toLog();
    
    log.authType = this.authType;
    log.userId = this.userId;
    
    return log;
  }
  
  /**
   * Create authentication error for invalid credentials
   */
  static invalidCredentials() {
    return new AuthenticationError(
      'Invalid email or password',
      'CREDENTIALS'
    );
  }
  
  /**
   * Create authentication error for missing token
   */
  static missingToken() {
    return new AuthenticationError(
      'Authentication token is required',
      'TOKEN_MISSING'
    );
  }
  
  /**
   * Create authentication error for invalid token
   */
  static invalidToken(token = null) {
    return new AuthenticationError(
      'Invalid or expired authentication token',
      'TOKEN_INVALID',
      token
    );
  }
  
  /**
   * Create authentication error for expired token
   */
  static expiredToken() {
    return new AuthenticationError(
      'Authentication token has expired',
      'TOKEN_EXPIRED'
    );
  }
  
  /**
   * Create authentication error for insufficient permissions
   */
  static insufficientPermissions(requiredRole = null) {
    return new AuthenticationError(
      'Insufficient permissions to access this resource',
      'INSUFFICIENT_PERMISSIONS',
      requiredRole
    );
  }
  
  /**
   * Create authentication error for account not verified
   */
  static accountNotVerified() {
    return new AuthenticationError(
      'Account is not verified. Please verify your email address',
      'ACCOUNT_NOT_VERIFIED'
    );
  }
  
  /**
   * Create authentication error for account locked
   */
  static accountLocked() {
    return new AuthenticationError(
      'Account is locked. Please contact support',
      'ACCOUNT_LOCKED'
    );
  }
  
  /**
   * Create authentication error for too many failed attempts
   */
  static tooManyFailedAttempts() {
    return new AuthenticationError(
      'Too many failed login attempts. Please try again later',
      'TOO_MANY_ATTEMPTS'
    );
  }
}

module.exports = AuthenticationError;
````

## File: src/utils/errors/DatabaseError.js
````javascript
/**
 * Database Error Class
 * Used for database operation errors
 */

const AppError = require('./AppError');

class DatabaseError extends AppError {
  constructor(message, operation = null, table = null, query = null, originalError = null) {
    super(message, 500, true, 'DATABASE_ERROR');
    
    this.operation = operation;
    this.table = table;
    this.query = query;
    this.originalError = originalError;
  }
  
  /**
   * Get error response object
   */
  toResponse() {
    const response = super.toResponse();
    
    // Don't expose sensitive database information in response
    response.error.operation = this.operation;
    
    return response;
  }
  
  /**
   * Get error for logging
   */
  toLog() {
    const log = super.toLog();
    
    log.operation = this.operation;
    log.table = this.table;
    log.query = this.query;
    log.originalError = this.originalError;
    
    return log;
  }
  
  /**
   * Create database error for connection failure
   */
  static connectionFailed(originalError = null) {
    return new DatabaseError(
      'Database connection failed',
      'CONNECT',
      null,
      null,
      originalError
    );
  }
  
  /**
   * Create database error for query failure
   */
  static queryFailed(operation, table, query, originalError = null) {
    return new DatabaseError(
      `Database query failed: ${operation}`,
      operation,
      table,
      query,
      originalError
    );
  }
  
  /**
   * Create database error for record not found
   */
  static recordNotFound(table, id) {
    return new DatabaseError(
      `Record not found in ${table}`,
      'SELECT',
      table,
      `id = ${id}`,
      null
    );
  }
  
  /**
   * Create database error for duplicate key
   */
  static duplicateKey(table, field, value, originalError = null) {
    return new DatabaseError(
      `Duplicate key violation in ${table} for field ${field}`,
      'INSERT',
      table,
      `${field} = ${value}`,
      originalError
    );
  }
  
  /**
   * Create database error for foreign key constraint
   */
  static foreignKeyConstraint(table, field, referencedTable, originalError = null) {
    return new DatabaseError(
      `Foreign key constraint violation in ${table} for field ${field}`,
      'INSERT/UPDATE',
      table,
      `foreign key: ${field} -> ${referencedTable}`,
      originalError
    );
  }
  
  /**
   * Create database error for transaction failure
   */
  static transactionFailed(operation, originalError = null) {
    return new DatabaseError(
      `Database transaction failed: ${operation}`,
      'TRANSACTION',
      null,
      operation,
      originalError
    );
  }
  
  /**
   * Create database error for timeout
   */
  static timeout(operation, table, query, originalError = null) {
    return new DatabaseError(
      `Database operation timed out: ${operation}`,
      operation,
      table,
      query,
      originalError
    );
  }
  
  /**
   * Create database error for constraint violation
   */
  static constraintViolation(table, constraint, originalError = null) {
    return new DatabaseError(
      `Database constraint violation in ${table}: ${constraint}`,
      'INSERT/UPDATE',
      table,
      constraint,
      originalError
    );
  }
}

module.exports = DatabaseError;
````

## File: src/utils/errors/index.js
````javascript
/**
 * Error Classes Index
 * Exports all custom error classes
 */

const AppError = require('./AppError');
const ValidationError = require('./ValidationError');
const AuthenticationError = require('./AuthenticationError');
const DatabaseError = require('./DatabaseError');

module.exports = {
  AppError,
  ValidationError,
  AuthenticationError,
  DatabaseError
};
````

## File: src/utils/errors/ValidationError.js
````javascript
/**
 * Validation Error Class
 * Used for input validation errors
 */

const AppError = require('./AppError');

class ValidationError extends AppError {
  constructor(message, field = null, value = null, validationType = null) {
    super(message, 400, true, 'VALIDATION_ERROR');
    
    this.field = field;
    this.value = value;
    this.validationType = validationType;
    this.details = [];
  }
  
  /**
   * Add validation detail
   */
  addDetail(field, message, value = null, validationType = null) {
    this.details.push({
      field,
      message,
      value,
      validationType
    });
  }
  
  /**
   * Get error response object with validation details
   */
  toResponse() {
    const response = super.toResponse();
    
    response.error.field = this.field;
    response.error.validationType = this.validationType;
    
    if (this.details.length > 0) {
      response.error.details = this.details;
    }
    
    return response;
  }
  
  /**
   * Get error for logging
   */
  toLog() {
    const log = super.toLog();
    
    log.field = this.field;
    log.validationType = this.validationType;
    log.details = this.details;
    
    return log;
  }
  
  /**
   * Create validation error for missing required field
   */
  static missingField(fieldName) {
    return new ValidationError(
      `Missing required field: ${fieldName}`,
      fieldName,
      null,
      'MISSING_FIELD'
    );
  }
  
  /**
   * Create validation error for invalid field type
   */
  static invalidType(fieldName, expectedType, actualValue) {
    return new ValidationError(
      `Field ${fieldName} must be of type ${expectedType}`,
      fieldName,
      actualValue,
      'INVALID_TYPE'
    );
  }
  
  /**
   * Create validation error for field length
   */
  static invalidLength(fieldName, minLength, maxLength, actualValue) {
    const message = maxLength 
      ? `Field ${fieldName} must be between ${minLength} and ${maxLength} characters`
      : `Field ${fieldName} must be at least ${minLength} characters`;
      
    return new ValidationError(
      message,
      fieldName,
      actualValue,
      'INVALID_LENGTH'
    );
  }
  
  /**
   * Create validation error for invalid email
   */
  static invalidEmail(email) {
    return new ValidationError(
      'Invalid email format',
      'email',
      email,
      'INVALID_EMAIL'
    );
  }
  
  /**
   * Create validation error for invalid file type
   */
  static invalidFileType(fileName, allowedTypes, actualType) {
    return new ValidationError(
      `File type not allowed. Allowed types: ${allowedTypes.join(', ')}`,
      'file',
      fileName,
      'INVALID_FILE_TYPE'
    );
  }
  
  /**
   * Create validation error for file size
   */
  static fileTooLarge(fileName, maxSize, actualSize) {
    return new ValidationError(
      `File size exceeds maximum allowed size of ${maxSize} bytes`,
      'file',
      fileName,
      'FILE_TOO_LARGE'
    );
  }
}

module.exports = ValidationError;
````

## File: src/utils/performanceTest.js
````javascript
/**
 * Performance Testing Utility
 * Tests application performance under load and measures response times
 */

const axios = require('axios');
const { performance } = require('perf_hooks');
const { logger } = require('../config/logger');

class PerformanceTester {
  constructor(baseUrl = 'http://localhost:3000') {
    this.baseUrl = baseUrl;
    this.results = [];
    this.config = {
      concurrent: 10,
      duration: 60000, // 1 minute
      rampUp: 10000, // 10 seconds
      endpoints: [
        { path: '/health', method: 'GET', weight: 1 },
        { path: '/api/versions', method: 'GET', weight: 1 },
        { path: '/api/v1/auth/current-user', method: 'GET', weight: 2 },
        { path: '/api/v1/career/profile', method: 'GET', weight: 3 },
        { path: '/api/v1/ai/analyze-resume', method: 'POST', weight: 1 }
      ]
    };
  }

  /**
   * Run performance test
   */
  async runTest(options = {}) {
    const config = { ...this.config, ...options };
    logger.info('Starting performance test', config);

    const startTime = performance.now();
    const promises = [];

    // Create concurrent requests
    for (let i = 0; i < config.concurrent; i++) {
      promises.push(this.runConcurrentRequests(config));
    }

    // Wait for all requests to complete
    const results = await Promise.all(promises);
    const endTime = performance.now();
    const totalDuration = endTime - startTime;

    // Flatten results
    const allResults = results.flat();
    
    // Analyze results
    const analysis = this.analyzeResults(allResults, totalDuration);
    
    // Log results
    this.logResults(analysis);
    
    return analysis;
  }

  /**
   * Run concurrent requests
   */
  async runConcurrentRequests(config) {
    const results = [];
    const startTime = performance.now();
    const endTime = startTime + config.duration;

    while (performance.now() < endTime) {
      const endpoint = this.selectRandomEndpoint(config.endpoints);
      const result = await this.makeRequest(endpoint);
      results.push(result);
      
      // Add small delay between requests
      await this.sleep(100);
    }

    return results;
  }

  /**
   * Select random endpoint based on weights
   */
  selectRandomEndpoint(endpoints) {
    const totalWeight = endpoints.reduce((sum, ep) => sum + ep.weight, 0);
    let random = Math.random() * totalWeight;
    
    for (const endpoint of endpoints) {
      random -= endpoint.weight;
      if (random <= 0) {
        return endpoint;
      }
    }
    
    return endpoints[0];
  }

  /**
   * Make HTTP request
   */
  async makeRequest(endpoint) {
    const startTime = performance.now();
    
    try {
      const url = `${this.baseUrl}${endpoint.path}`;
      const config = {
        method: endpoint.method,
        url,
        timeout: 10000,
        headers: {
          'Content-Type': 'application/json',
          'User-Agent': 'PerformanceTester/1.0'
        }
      };

      // Add sample data for POST requests
      if (endpoint.method === 'POST') {
        config.data = this.getSampleData(endpoint.path);
      }

      const response = await axios(config);
      const endTime = performance.now();
      
      return {
        endpoint: endpoint.path,
        method: endpoint.method,
        statusCode: response.status,
        responseTime: endTime - startTime,
        success: true,
        timestamp: new Date().toISOString()
      };
    } catch (error) {
      const endTime = performance.now();
      
      return {
        endpoint: endpoint.path,
        method: endpoint.method,
        statusCode: error.response?.status || 0,
        responseTime: endTime - startTime,
        success: false,
        error: error.message,
        timestamp: new Date().toISOString()
      };
    }
  }

  /**
   * Get sample data for POST requests
   */
  getSampleData(path) {
    switch (path) {
      case '/api/v1/ai/analyze-resume':
        return {
          resumeText: 'Sample resume text for performance testing...',
          analysisType: 'general'
        };
      case '/api/v1/career/profile':
        return {
          skills: ['JavaScript', 'Node.js', 'React'],
          experience: '5 years',
          education: 'Bachelor\'s Degree'
        };
      default:
        return {};
    }
  }

  /**
   * Analyze test results
   */
  analyzeResults(results, totalDuration) {
    const successful = results.filter(r => r.success);
    const failed = results.filter(r => !r.success);
    
    const responseTimes = successful.map(r => r.responseTime);
    const sortedTimes = responseTimes.sort((a, b) => a - b);
    
    const analysis = {
      summary: {
        totalRequests: results.length,
        successfulRequests: successful.length,
        failedRequests: failed.length,
        successRate: (successful.length / results.length) * 100,
        totalDuration: totalDuration,
        requestsPerSecond: results.length / (totalDuration / 1000)
      },
      responseTimes: {
        min: Math.min(...responseTimes),
        max: Math.max(...responseTimes),
        average: responseTimes.reduce((sum, time) => sum + time, 0) / responseTimes.length,
        median: sortedTimes[Math.floor(sortedTimes.length / 2)],
        p95: sortedTimes[Math.floor(sortedTimes.length * 0.95)],
        p99: sortedTimes[Math.floor(sortedTimes.length * 0.99)]
      },
      statusCodes: this.analyzeStatusCodes(results),
      endpoints: this.analyzeEndpoints(results),
      errors: failed.map(r => ({
        endpoint: r.endpoint,
        error: r.error,
        statusCode: r.statusCode
      }))
    };

    return analysis;
  }

  /**
   * Analyze status codes
   */
  analyzeStatusCodes(results) {
    const statusCodes = {};
    results.forEach(result => {
      const code = result.statusCode;
      statusCodes[code] = (statusCodes[code] || 0) + 1;
    });
    return statusCodes;
  }

  /**
   * Analyze endpoint performance
   */
  analyzeEndpoints(results) {
    const endpoints = {};
    
    results.forEach(result => {
      if (!endpoints[result.endpoint]) {
        endpoints[result.endpoint] = {
          total: 0,
          successful: 0,
          failed: 0,
          responseTimes: []
        };
      }
      
      endpoints[result.endpoint].total++;
      if (result.success) {
        endpoints[result.endpoint].successful++;
        endpoints[result.endpoint].responseTimes.push(result.responseTime);
      } else {
        endpoints[result.endpoint].failed++;
      }
    });

    // Calculate averages for each endpoint
    Object.keys(endpoints).forEach(endpoint => {
      const times = endpoints[endpoint].responseTimes;
      endpoints[endpoint].averageResponseTime = times.length > 0 
        ? times.reduce((sum, time) => sum + time, 0) / times.length 
        : 0;
      endpoints[endpoint].successRate = (endpoints[endpoint].successful / endpoints[endpoint].total) * 100;
    });

    return endpoints;
  }

  /**
   * Log test results
   */
  logResults(analysis) {
    logger.info('Performance Test Results:', {
      summary: analysis.summary,
      responseTimes: analysis.responseTimes,
      statusCodes: analysis.statusCodes
    });

    logger.info('Endpoint Performance:', analysis.endpoints);
    
    if (analysis.errors.length > 0) {
      logger.warn('Test Errors:', analysis.errors);
    }

    // Log recommendations
    this.logRecommendations(analysis);
  }

  /**
   * Log performance recommendations
   */
  logRecommendations(analysis) {
    const recommendations = [];

    if (analysis.summary.successRate < 95) {
      recommendations.push('Success rate is below 95%. Investigate failed requests.');
    }

    if (analysis.responseTimes.p95 > 2000) {
      recommendations.push('95th percentile response time is above 2 seconds. Consider optimization.');
    }

    if (analysis.responseTimes.average > 1000) {
      recommendations.push('Average response time is above 1 second. Consider caching or optimization.');
    }

    if (analysis.summary.requestsPerSecond < 10) {
      recommendations.push('Throughput is low. Consider scaling or optimization.');
    }

    if (recommendations.length > 0) {
      logger.info('Performance Recommendations:', recommendations);
    } else {
      logger.info('Performance is within acceptable ranges.');
    }
  }

  /**
   * Sleep utility
   */
  sleep(ms) {
    return new Promise(resolve => setTimeout(resolve, ms));
  }

  /**
   * Load test specific endpoint
   */
  async loadTestEndpoint(path, method = 'GET', data = null, options = {}) {
    const config = {
      concurrent: options.concurrent || 5,
      requests: options.requests || 100,
      delay: options.delay || 100,
      ...options
    };

    logger.info(`Starting load test for ${method} ${path}`, config);

    const results = [];
    const promises = [];

    for (let i = 0; i < config.requests; i++) {
      promises.push(this.makeRequest({ path, method, data }));
      
      if (i % config.concurrent === 0) {
        await this.sleep(config.delay);
      }
    }

    const responses = await Promise.all(promises);
    const analysis = this.analyzeResults(responses, 0);
    
    logger.info(`Load test completed for ${path}:`, analysis.summary);
    return analysis;
  }

  /**
   * Stress test
   */
  async stressTest(options = {}) {
    const config = {
      maxConcurrent: 50,
      duration: 300000, // 5 minutes
      rampUpTime: 60000, // 1 minute
      ...options
    };

    logger.info('Starting stress test', config);

    const results = [];
    const startTime = performance.now();
    const endTime = startTime + config.duration;

    let currentConcurrent = 1;
    const rampUpInterval = config.rampUpTime / (config.maxConcurrent - 1);

    while (performance.now() < endTime) {
      const promises = [];
      
      for (let i = 0; i < currentConcurrent; i++) {
        const endpoint = this.selectRandomEndpoint(this.config.endpoints);
        promises.push(this.makeRequest(endpoint));
      }

      const batchResults = await Promise.all(promises);
      results.push(...batchResults);

      // Ramp up concurrency
      if (currentConcurrent < config.maxConcurrent) {
        currentConcurrent++;
        await this.sleep(rampUpInterval);
      } else {
        await this.sleep(1000);
      }
    }

    const analysis = this.analyzeResults(results, config.duration);
    logger.info('Stress test completed:', analysis.summary);
    return analysis;
  }
}

// CLI interface
if (require.main === module) {
  const tester = new PerformanceTester();
  
  const args = process.argv.slice(2);
  const command = args[0];

  switch (command) {
    case 'load':
      const path = args[1] || '/health';
      const method = args[2] || 'GET';
      const requests = parseInt(args[3]) || 100;
      const concurrent = parseInt(args[4]) || 10;
      
      tester.loadTestEndpoint(path, method, null, { requests, concurrent })
        .then(() => process.exit(0))
        .catch(err => {
          logger.error('Load test failed:', err);
          process.exit(1);
        });
      break;

    case 'stress':
      tester.stressTest()
        .then(() => process.exit(0))
        .catch(err => {
          logger.error('Stress test failed:', err);
          process.exit(1);
        });
      break;

    case 'full':
      tester.runTest()
        .then(() => process.exit(0))
        .catch(err => {
          logger.error('Performance test failed:', err);
          process.exit(1);
        });
      break;

    default:
      console.log(`
Performance Testing Utility

Usage:
  node performanceTest.js load [path] [method] [requests] [concurrent]
  node performanceTest.js stress
  node performanceTest.js full

Examples:
  node performanceTest.js load /health GET 100 10
  node performanceTest.js load /api/v1/auth/current-user GET 50 5
  node performanceTest.js stress
  node performanceTest.js full
      `);
      process.exit(0);
  }
}

module.exports = {
  PerformanceTester,
  PerformanceTester: PerformanceTester
};
````

## File: src/utils/responseFormatter.js
````javascript
/**
 * Response Formatter
 * Handles different response formats for different API versions
 */

const { getApiVersionConfig } = require('../config/apiVersioning');

/**
 * Response formatter class
 */
class ResponseFormatter {
  /**
   * Format success response based on API version
   * @param {Object} data - Response data
   * @param {string} version - API version
   * @param {Object} options - Formatting options
   * @returns {Object} Formatted response
   */
  static formatSuccess(data, version = 'v1', options = {}) {
    const {
      message = 'Success',
      meta = {},
      pagination = null
    } = options;

    const versionConfig = getApiVersionConfig(version);
    
    // Version-specific formatting
    switch (version) {
      case 'v1':
        return this.formatV1Success(data, message, meta, pagination);
      case 'v2':
        return this.formatV2Success(data, message, meta, pagination);
      default:
        return this.formatV1Success(data, message, meta, pagination);
    }
  }

  /**
   * Format error response based on API version
   * @param {Error} error - Error object
   * @param {string} version - API version
   * @param {Object} options - Formatting options
   * @returns {Object} Formatted error response
   */
  static formatError(error, version = 'v1', options = {}) {
    const {
      statusCode = 500,
      includeStack = false
    } = options;

    const versionConfig = getApiVersionConfig(version);
    
    // Version-specific error formatting
    switch (version) {
      case 'v1':
        return this.formatV1Error(error, statusCode, includeStack);
      case 'v2':
        return this.formatV2Error(error, statusCode, includeStack);
      default:
        return this.formatV1Error(error, statusCode, includeStack);
    }
  }

  /**
   * Format pagination response based on API version
   * @param {Array} data - Data array
   * @param {Object} pagination - Pagination info
   * @param {string} version - API version
   * @returns {Object} Formatted paginated response
   */
  static formatPagination(data, pagination, version = 'v1') {
    switch (version) {
      case 'v1':
        return this.formatV1Pagination(data, pagination);
      case 'v2':
        return this.formatV2Pagination(data, pagination);
      default:
        return this.formatV1Pagination(data, pagination);
    }
  }

  /**
   * V1 Success Response Format
   * @param {Object} data - Response data
   * @param {string} message - Success message
   * @param {Object} meta - Additional metadata
   * @param {Object} pagination - Pagination info
   * @returns {Object} V1 formatted response
   */
  static formatV1Success(data, message, meta, pagination) {
    const response = {
      success: true,
      message,
      data,
      timestamp: new Date().toISOString()
    };

    if (meta && Object.keys(meta).length > 0) {
      response.meta = meta;
    }

    if (pagination) {
      response.pagination = {
        page: pagination.page,
        limit: pagination.limit,
        total: pagination.total,
        pages: pagination.pages
      };
    }

    return response;
  }

  /**
   * V2 Success Response Format
   * @param {Object} data - Response data
   * @param {string} message - Success message
   * @param {Object} meta - Additional metadata
   * @param {Object} pagination - Pagination info
   * @returns {Object} V2 formatted response
   */
  static formatV2Success(data, message, meta, pagination) {
    const response = {
      status: 'success',
      message,
      data,
      timestamp: new Date().toISOString(),
      version: '2.0.0'
    };

    if (meta && Object.keys(meta).length > 0) {
      response.meta = meta;
    }

    if (pagination) {
      response.pagination = {
        current_page: pagination.page,
        per_page: pagination.limit,
        total: pagination.total,
        total_pages: pagination.pages,
        has_next: pagination.page < pagination.pages,
        has_prev: pagination.page > 1
      };
    }

    return response;
  }

  /**
   * V1 Error Response Format
   * @param {Error} error - Error object
   * @param {number} statusCode - HTTP status code
   * @param {boolean} includeStack - Whether to include stack trace
   * @returns {Object} V1 formatted error response
   */
  static formatV1Error(error, statusCode, includeStack) {
    const response = {
      success: false,
      error: {
        message: error.message || 'An error occurred',
        code: error.code || 'INTERNAL_ERROR',
        status: statusCode
      },
      timestamp: new Date().toISOString()
    };

    if (includeStack && error.stack) {
      response.error.stack = error.stack;
    }

    if (error.details) {
      response.error.details = error.details;
    }

    return response;
  }

  /**
   * V2 Error Response Format
   * @param {Error} error - Error object
   * @param {number} statusCode - HTTP status code
   * @param {boolean} includeStack - Whether to include stack trace
   * @returns {Object} V2 formatted error response
   */
  static formatV2Error(error, statusCode, includeStack) {
    const response = {
      status: 'error',
      error: {
        type: error.constructor.name,
        message: error.message || 'An error occurred',
        code: error.code || 'INTERNAL_ERROR',
        status_code: statusCode,
        request_id: error.requestId || null
      },
      timestamp: new Date().toISOString(),
      version: '2.0.0'
    };

    if (includeStack && error.stack) {
      response.error.stack_trace = error.stack;
    }

    if (error.details) {
      response.error.details = error.details;
    }

    if (error.validationErrors) {
      response.error.validation_errors = error.validationErrors;
    }

    return response;
  }

  /**
   * V1 Pagination Format
   * @param {Array} data - Data array
   * @param {Object} pagination - Pagination info
   * @returns {Object} V1 paginated response
   */
  static formatV1Pagination(data, pagination) {
    return {
      success: true,
      data,
      pagination: {
        page: pagination.page,
        limit: pagination.limit,
        total: pagination.total,
        pages: pagination.pages
      },
      timestamp: new Date().toISOString()
    };
  }

  /**
   * V2 Pagination Format
   * @param {Array} data - Data array
   * @param {Object} pagination - Pagination info
   * @returns {Object} V2 paginated response
   */
  static formatV2Pagination(data, pagination) {
    return {
      status: 'success',
      data,
      pagination: {
        current_page: pagination.page,
        per_page: pagination.limit,
        total: pagination.total,
        total_pages: pagination.pages,
        has_next: pagination.page < pagination.pages,
        has_prev: pagination.page > 1,
        next_page: pagination.page < pagination.pages ? pagination.page + 1 : null,
        prev_page: pagination.page > 1 ? pagination.page - 1 : null
      },
      timestamp: new Date().toISOString(),
      version: '2.0.0'
    };
  }

  /**
   * Format validation error response
   * @param {Array} validationErrors - Validation errors array
   * @param {string} version - API version
   * @returns {Object} Formatted validation error response
   */
  static formatValidationError(validationErrors, version = 'v1') {
    const error = new Error('Validation failed');
    error.validationErrors = validationErrors;
    error.code = 'VALIDATION_ERROR';
    
    return this.formatError(error, version, {
      statusCode: 400,
      includeStack: false
    });
  }

  /**
   * Format not found error response
   * @param {string} resource - Resource name
   * @param {string} version - API version
   * @returns {Object} Formatted not found error response
   */
  static formatNotFoundError(resource, version = 'v1') {
    const error = new Error(`${resource} not found`);
    error.code = 'NOT_FOUND';
    
    return this.formatError(error, version, {
      statusCode: 404,
      includeStack: false
    });
  }

  /**
   * Format unauthorized error response
   * @param {string} message - Error message
   * @param {string} version - API version
   * @returns {Object} Formatted unauthorized error response
   */
  static formatUnauthorizedError(message = 'Unauthorized', version = 'v1') {
    const error = new Error(message);
    error.code = 'UNAUTHORIZED';
    
    return this.formatError(error, version, {
      statusCode: 401,
      includeStack: false
    });
  }

  /**
   * Format forbidden error response
   * @param {string} message - Error message
   * @param {string} version - API version
   * @returns {Object} Formatted forbidden error response
   */
  static formatForbiddenError(message = 'Forbidden', version = 'v1') {
    const error = new Error(message);
    error.code = 'FORBIDDEN';
    
    return this.formatError(error, version, {
      statusCode: 403,
      includeStack: false
    });
  }

  /**
   * Format rate limit error response
   * @param {string} message - Error message
   * @param {string} version - API version
   * @returns {Object} Formatted rate limit error response
   */
  static formatRateLimitError(message = 'Rate limit exceeded', version = 'v1') {
    const error = new Error(message);
    error.code = 'RATE_LIMIT_EXCEEDED';
    
    return this.formatError(error, version, {
      statusCode: 429,
      includeStack: false
    });
  }

  /**
   * Add response headers based on version
   * @param {Object} res - Express response object
   * @param {string} version - API version
   * @param {Object} options - Additional options
   */
  static addResponseHeaders(res, version, options = {}) {
    const {
      cacheControl = 'no-cache',
      contentType = 'application/json'
    } = options;

    res.setHeader('Content-Type', contentType);
    res.setHeader('Cache-Control', cacheControl);
    res.setHeader('X-API-Version', version);
    res.setHeader('X-Response-Format', version);

    // Version-specific headers
    if (version === 'v2') {
      res.setHeader('X-API-Status', 'stable');
      res.setHeader('X-Response-Time', Date.now());
    }
  }
}

module.exports = ResponseFormatter;
````

## File: supabase_tables.sql
````sql
-- Supabase Database Schema for ImmiGrowAI
-- Run these queries in your Supabase SQL Editor

-- Enable UUID extension
CREATE EXTENSION IF NOT EXISTS "uuid-ossp";

-- Create roles table
CREATE TABLE IF NOT EXISTS roles (
    id SERIAL PRIMARY KEY,
    name VARCHAR(255) UNIQUE NOT NULL,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Create users table
CREATE TABLE IF NOT EXISTS users (
    id SERIAL PRIMARY KEY,
    email VARCHAR(255) UNIQUE NOT NULL,
    full_name VARCHAR(255) NOT NULL,
    phone_no VARCHAR(50) UNIQUE,
    dob DATE,
    user_verified BOOLEAN DEFAULT FALSE,
    background_verification BOOLEAN DEFAULT FALSE,
    terms_condition_check BOOLEAN DEFAULT FALSE,
    status_in_canada VARCHAR(100),
    google_refresh_token TEXT,
    already_in_canada BOOLEAN,
    country_of_origin VARCHAR(100),
    current_location VARCHAR(255),
    role_id INTEGER REFERENCES roles(id),
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Create user_documents table
CREATE TABLE IF NOT EXISTS user_documents (
    id SERIAL PRIMARY KEY,
    user_id INTEGER REFERENCES users(id) ON DELETE CASCADE,
    file_name VARCHAR(255) NOT NULL,
    file_type VARCHAR(50) NOT NULL,
    file_path TEXT NOT NULL,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Create user_career_profiles table
CREATE TABLE IF NOT EXISTS user_career_profiles (
    id SERIAL PRIMARY KEY,
    user_id INTEGER REFERENCES users(id) ON DELETE CASCADE UNIQUE,
    professional_summary TEXT,
    skills_categories JSONB,
    career_objectives TEXT,
    target_industries TEXT[],
    market_alignment_score INTEGER,
    skill_gaps JSONB,
    improvement_roadmap JSONB,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW(),
    last_updated TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Create resume_analyses table
CREATE TABLE IF NOT EXISTS resume_analyses (
    id SERIAL PRIMARY KEY,
    user_id INTEGER REFERENCES users(id) ON DELETE CASCADE,
    original_file_name VARCHAR(255) NOT NULL,
    file_data BYTEA,
    extracted_text TEXT,
    structured_data JSONB,
    confidence_scores JSONB,
    user_corrections JSONB,
    canadian_market_analysis JSONB,
    certifications JSONB,
    education JSONB,
    metadata JSONB,
    personal_info JSONB,
    processing_method VARCHAR(100),
    professional_summary TEXT,
    projects JSONB,
    skills JSONB,
    work_experience JSONB,
    position_recommendations JSONB,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Create job_opportunities table
CREATE TABLE IF NOT EXISTS job_opportunities (
    id SERIAL PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    company VARCHAR(255) NOT NULL,
    location VARCHAR(255) NOT NULL,
    description TEXT,
    requirements TEXT[],
    salary_range JSONB,
    job_url TEXT,
    is_newcomer_friendly BOOLEAN DEFAULT FALSE,
    discovered_at TIMESTAMP WITH TIME ZONE DEFAULT NOW(),
    is_active BOOLEAN DEFAULT TRUE
);

-- Create job_matches table
CREATE TABLE IF NOT EXISTS job_matches (
    id SERIAL PRIMARY KEY,
    user_id INTEGER REFERENCES users(id) ON DELETE CASCADE,
    job_opportunity_id INTEGER REFERENCES job_opportunities(id) ON DELETE CASCADE,
    match_score DECIMAL(5,2),
    match_reasons JSONB,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Create skill_gap_analyses table
CREATE TABLE IF NOT EXISTS skill_gap_analyses (
    id SERIAL PRIMARY KEY,
    user_id INTEGER REFERENCES users(id) ON DELETE CASCADE,
    target_position VARCHAR(255) NOT NULL,
    current_skills JSONB,
    required_skills JSONB,
    skill_gaps JSONB,
    improvement_plan JSONB,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Create enhanced_career_profiles table
CREATE TABLE IF NOT EXISTS enhanced_career_profiles (
    id SERIAL PRIMARY KEY,
    user_id INTEGER REFERENCES users(id) ON DELETE CASCADE UNIQUE,
    target_position JSONB,
    enhanced_profile JSONB,
    resume_analysis_id INTEGER REFERENCES resume_analyses(id) ON DELETE SET NULL,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW(),
    last_updated TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Insert default roles
INSERT INTO roles (name) VALUES 
    ('admin'),
    ('employer'),
    ('immigration_consultant'),
    ('immigrant')
ON CONFLICT (name) DO NOTHING;

-- Create indexes for better performance
CREATE INDEX IF NOT EXISTS idx_users_email ON users(email);
CREATE INDEX IF NOT EXISTS idx_users_role_id ON users(role_id);
CREATE INDEX IF NOT EXISTS idx_user_documents_user_id ON user_documents(user_id);
CREATE INDEX IF NOT EXISTS idx_resume_analyses_user_id ON resume_analyses(user_id);
CREATE INDEX IF NOT EXISTS idx_job_matches_user_id ON job_matches(user_id);
CREATE INDEX IF NOT EXISTS idx_job_matches_job_opportunity_id ON job_matches(job_opportunity_id);
CREATE INDEX IF NOT EXISTS idx_user_career_profiles_user_id ON user_career_profiles(user_id);
CREATE INDEX IF NOT EXISTS idx_skill_gap_analyses_user_id ON skill_gap_analyses(user_id);
CREATE INDEX IF NOT EXISTS idx_enhanced_career_profiles_user_id ON enhanced_career_profiles(user_id);

-- Enable Row Level Security (RLS)
ALTER TABLE users ENABLE ROW LEVEL SECURITY;
ALTER TABLE user_documents ENABLE ROW LEVEL SECURITY;
ALTER TABLE user_career_profiles ENABLE ROW LEVEL SECURITY;
ALTER TABLE resume_analyses ENABLE ROW LEVEL SECURITY;
ALTER TABLE job_opportunities ENABLE ROW LEVEL SECURITY;
ALTER TABLE job_matches ENABLE ROW LEVEL SECURITY;
ALTER TABLE skill_gap_analyses ENABLE ROW LEVEL SECURITY;
ALTER TABLE enhanced_career_profiles ENABLE ROW LEVEL SECURITY;

-- Drop existing policies if they exist
DROP POLICY IF EXISTS "Users can view their own data" ON users;
DROP POLICY IF EXISTS "Users can update their own data" ON users;
DROP POLICY IF EXISTS "Users can insert their own data" ON users;
DROP POLICY IF EXISTS "Users can view their own documents" ON user_documents;
DROP POLICY IF EXISTS "Users can insert their own documents" ON user_documents;
DROP POLICY IF EXISTS "Users can update their own documents" ON user_documents;
DROP POLICY IF EXISTS "Users can delete their own documents" ON user_documents;
DROP POLICY IF EXISTS "Users can view their own career profiles" ON user_career_profiles;
DROP POLICY IF EXISTS "Users can insert their own career profiles" ON user_career_profiles;
DROP POLICY IF EXISTS "Users can update their own career profiles" ON user_career_profiles;
DROP POLICY IF EXISTS "Users can view their own resume analyses" ON resume_analyses;
DROP POLICY IF EXISTS "Users can insert their own resume analyses" ON resume_analyses;
DROP POLICY IF EXISTS "Users can update their own resume analyses" ON resume_analyses;
DROP POLICY IF EXISTS "Anyone can view job opportunities" ON job_opportunities;
DROP POLICY IF EXISTS "Authenticated users can insert job opportunities" ON job_opportunities;
DROP POLICY IF EXISTS "Users can view their own job matches" ON job_matches;
DROP POLICY IF EXISTS "Users can insert their own job matches" ON job_matches;
DROP POLICY IF EXISTS "Users can update their own job matches" ON job_matches;
DROP POLICY IF EXISTS "Users can view their own skill gap analyses" ON skill_gap_analyses;
DROP POLICY IF EXISTS "Users can insert their own skill gap analyses" ON skill_gap_analyses;
DROP POLICY IF EXISTS "Users can update their own skill gap analyses" ON skill_gap_analyses;
DROP POLICY IF EXISTS "Users can view their own enhanced career profiles" ON enhanced_career_profiles;
DROP POLICY IF EXISTS "Users can insert their own enhanced career profiles" ON enhanced_career_profiles;
DROP POLICY IF EXISTS "Users can update their own enhanced career profiles" ON enhanced_career_profiles;

-- Create RLS policies for users table (allow service role and authenticated users)
CREATE POLICY "Service role can manage all users" ON users
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Users can view their own data" ON users
    FOR SELECT USING (auth.uid()::text = id::text);

CREATE POLICY "Users can update their own data" ON users
    FOR UPDATE USING (auth.uid()::text = id::text);

CREATE POLICY "Users can insert their own data" ON users
    FOR INSERT WITH CHECK (auth.uid()::text = id::text);

-- Create RLS policies for user_documents table
CREATE POLICY "Service role can manage all documents" ON user_documents
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Users can view their own documents" ON user_documents
    FOR SELECT USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can insert their own documents" ON user_documents
    FOR INSERT WITH CHECK (auth.uid()::text = user_id::text);

CREATE POLICY "Users can update their own documents" ON user_documents
    FOR UPDATE USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can delete their own documents" ON user_documents
    FOR DELETE USING (auth.uid()::text = user_id::text);

-- Create RLS policies for user_career_profiles table
CREATE POLICY "Service role can manage all career profiles" ON user_career_profiles
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Users can view their own career profiles" ON user_career_profiles
    FOR SELECT USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can insert their own career profiles" ON user_career_profiles
    FOR INSERT WITH CHECK (auth.uid()::text = user_id::text);

CREATE POLICY "Users can update their own career profiles" ON user_career_profiles
    FOR UPDATE USING (auth.uid()::text = user_id::text);

-- Create RLS policies for resume_analyses table
CREATE POLICY "Service role can manage all resume analyses" ON resume_analyses
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Users can view their own resume analyses" ON resume_analyses
    FOR SELECT USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can insert their own resume analyses" ON resume_analyses
    FOR INSERT WITH CHECK (auth.uid()::text = user_id::text);

CREATE POLICY "Users can update their own resume analyses" ON resume_analyses
    FOR UPDATE USING (auth.uid()::text = user_id::text);

-- Create RLS policies for job_opportunities table (public read, authenticated insert)
CREATE POLICY "Service role can manage all job opportunities" ON job_opportunities
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Anyone can view job opportunities" ON job_opportunities
    FOR SELECT USING (true);

CREATE POLICY "Authenticated users can insert job opportunities" ON job_opportunities
    FOR INSERT WITH CHECK (auth.role() = 'authenticated');

-- Create RLS policies for job_matches table
CREATE POLICY "Service role can manage all job matches" ON job_matches
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Users can view their own job matches" ON job_matches
    FOR SELECT USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can insert their own job matches" ON job_matches
    FOR INSERT WITH CHECK (auth.uid()::text = user_id::text);

CREATE POLICY "Users can update their own job matches" ON job_matches
    FOR UPDATE USING (auth.uid()::text = user_id::text);

-- Create RLS policies for skill_gap_analyses table
CREATE POLICY "Service role can manage all skill gap analyses" ON skill_gap_analyses
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Users can view their own skill gap analyses" ON skill_gap_analyses
    FOR SELECT USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can insert their own skill gap analyses" ON skill_gap_analyses
    FOR INSERT WITH CHECK (auth.uid()::text = user_id::text);

CREATE POLICY "Users can update their own skill gap analyses" ON skill_gap_analyses
    FOR UPDATE USING (auth.uid()::text = user_id::text);

-- Create RLS policies for enhanced_career_profiles table
CREATE POLICY "Service role can manage all enhanced career profiles" ON enhanced_career_profiles
    FOR ALL USING (auth.role() = 'service_role');

CREATE POLICY "Users can view their own enhanced career profiles" ON enhanced_career_profiles
    FOR SELECT USING (auth.uid()::text = user_id::text);

CREATE POLICY "Users can insert their own enhanced career profiles" ON enhanced_career_profiles
    FOR INSERT WITH CHECK (auth.uid()::text = user_id::text);

CREATE POLICY "Users can update their own enhanced career profiles" ON enhanced_career_profiles
    FOR UPDATE USING (auth.uid()::text = user_id::text);

-- Create function to update updated_at timestamp
CREATE OR REPLACE FUNCTION update_updated_at_column()
RETURNS TRIGGER AS $$
BEGIN
    NEW.updated_at = NOW();
    RETURN NEW;
END;
$$ language 'plpgsql';

-- Create triggers for updated_at
CREATE TRIGGER update_users_updated_at BEFORE UPDATE ON users
    FOR EACH ROW EXECUTE FUNCTION update_updated_at_column();

CREATE TRIGGER update_user_career_profiles_updated_at BEFORE UPDATE ON user_career_profiles
    FOR EACH ROW EXECUTE FUNCTION update_updated_at_column();

CREATE TRIGGER update_enhanced_career_profiles_updated_at BEFORE UPDATE ON enhanced_career_profiles
    FOR EACH ROW EXECUTE FUNCTION update_updated_at_column();
````

## File: test-api.js
````javascript
const axios = require('axios');

async function testAPI() {
  const baseURL = 'http://localhost:5500';
  
  try {
    console.log('Testing API endpoints...\n');
    
    // Test health endpoint
    console.log('1. Testing health endpoint...');
    const healthResponse = await axios.get(`${baseURL}/api/health`);
    console.log('✅ Health endpoint working:', healthResponse.data);
    
    // Test versions endpoint
    console.log('\n2. Testing versions endpoint...');
    const versionsResponse = await axios.get(`${baseURL}/api/versions`);
    console.log('✅ Versions endpoint working:', versionsResponse.data);
    
    // Test resume generate endpoint (this should work now)
    console.log('\n3. Testing resume generate endpoint...');
    try {
      const generateResponse = await axios.post(`${baseURL}/api/v1/resume/generate`, {
        // Add minimal test data
        test: true
      });
      console.log('✅ Resume generate endpoint working:', generateResponse.status);
    } catch (error) {
      if (error.response) {
        console.log('⚠️ Resume generate endpoint responded with:', error.response.status, error.response.data);
      } else {
        console.log('❌ Resume generate endpoint error:', error.message);
      }
    }
    
  } catch (error) {
    console.error('❌ API test failed:', error.message);
    if (error.code === 'ECONNREFUSED') {
      console.log('💡 Make sure the server is running on port 5500');
    }
  }
}

testAPI();
````

## File: test-auth.js
````javascript
const { createClient } = require('@supabase/supabase-js');
const SupabaseDatabase = require('./services/supabaseDatabase');

// Test script to verify authentication and database operations
async function testAuthAndDatabase() {
  console.log('🧪 Starting authentication and database test...\n');
  
  // Initialize Supabase client
  const supabase = createClient(
    process.env.SUPABASE_URL,
    process.env.SUPABASE_ANON_KEY
  );
  
  // Initialize database service
  const supabaseDb = new SupabaseDatabase();
  
  try {
    // Test 1: Check if we can connect to Supabase
    console.log('1️⃣ Testing Supabase connection...');
    const { data, error } = await supabase.from('users').select('count').limit(1);
    if (error) {
      console.error('❌ Supabase connection failed:', error);
      return;
    }
    console.log('✅ Supabase connection successful\n');
    
    // Test 2: Check if we can connect to database service
    console.log('2️⃣ Testing database service connection...');
    await supabaseDb.connect();
    console.log('✅ Database service connection successful\n');
    
    // Test 3: Test user lookup by email
    console.log('3️⃣ Testing user lookup...');
    const testUser = await supabaseDb.findOrCreateUser({
      email: 'test@example.com',
      fullName: 'Test User'
    });
    console.log('✅ User lookup successful:', {
      id: testUser.id,
      email: testUser.email,
      fullName: testUser.full_name
    });
    console.log('✅ User ID type:', typeof testUser.id);
    console.log('✅ User ID is numeric:', !isNaN(testUser.id));
    console.log('');
    
    // Test 4: Test resume analysis save (with test data)
    console.log('4️⃣ Testing resume analysis save...');
    const testAnalysisData = {
      originalFileName: 'test-resume.pdf',
      personalInfo: { name: 'Test User', email: 'test@example.com' },
      skills: { technical: ['JavaScript', 'React'], soft: ['Communication'] },
      workExperience: [{ company: 'Test Corp', position: 'Developer' }],
      education: [{ degree: 'BS Computer Science', institution: 'Test University' }],
      canadianMarketAnalysis: { overallRelevance: 'High', strengthsForCanadianMarket: ['Technical skills'] },
      confidenceScores: { overall: 0.85 },
      metadata: { processingMethod: 'test', fileSize: 1024 }
    };
    
    const savedAnalysis = await supabaseDb.saveResumeAnalysis(testUser.id, testAnalysisData);
    console.log('✅ Resume analysis saved successfully:', {
      id: savedAnalysis.id,
      userId: savedAnalysis.user_id,
      fileName: savedAnalysis.original_file_name
    });
    console.log('');
    
    // Test 5: Test resume analysis retrieval
    console.log('5️⃣ Testing resume analysis retrieval...');
    const analyses = await supabaseDb.getUserResumeAnalyses(testUser.id);
    console.log('✅ Retrieved analyses:', analyses.length);
    if (analyses.length > 0) {
      console.log('✅ Sample analysis:', {
        id: analyses[0].id,
        userId: analyses[0].user_id,
        fileName: analyses[0].original_file_name
      });
    }
    console.log('');
    
    console.log('🎉 All tests passed! Authentication and database operations are working correctly.');
    
  } catch (error) {
    console.error('❌ Test failed:', error);
    console.error('❌ Error stack:', error.stack);
  } finally {
    // Clean up
    await supabaseDb.disconnect();
  }
}

// Run the test if this file is executed directly
if (require.main === module) {
  // Load environment variables
  require('dotenv').config();
  
  testAuthAndDatabase().catch(console.error);
}

module.exports = { testAuthAndDatabase };
````
