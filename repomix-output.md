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
.bolt/config.json
.bolt/ignore
.bolt/prompt
.eslintrc.json
.gitignore
.repomixignore
app/dashboard/page.tsx
app/globals.css
app/layout.tsx
app/page.tsx
components/AuthForm.tsx
components/DriverDashboard.tsx
components/Header.tsx
components/PassengerDashboard.tsx
hooks/use-toast.ts
lib/auth.ts
lib/rides.ts
lib/supabase.ts
lib/utils.ts
package.json
repomix.config.json
supabase/migrations/20250630031142_velvet_block.sql
```

# Files

## File: .bolt/config.json
```json
{
  "template": "nextjs-shadcn"
}
```

## File: .bolt/ignore
```
components/ui/*
hooks/use-toast.ts
```

## File: .bolt/prompt
```
For all designs I ask you to make, have them be beautiful, not cookie cutter. Make webpages that are fully featured and worthy for production.

When using client-side hooks (useState and useEffect) in a component that's being treated as a Server Component by Next.js, always add the "use client" directive at the top of the file.

Do not write code that will trigger this error: "Warning: Extra attributes from the server: %s%s""class,style"

By default, this template supports JSX syntax with Tailwind CSS classes, the shadcn/ui library, React hooks, and Lucide React for icons. Do not install other packages for UI themes, icons, etc unless absolutely necessary or I request them.

Use icons from lucide-react for logos.
```

## File: .eslintrc.json
```json
{
  "extends": "next/core-web-vitals"
}
```

## File: .gitignore
```
# See https://help.github.com/articles/ignoring-files/ for more about ignoring files.

# dependencies
/node_modules
/.pnp
.pnp.js

# testing
/coverage

# next.js
/.next/
/out/

# production
/build

# misc
.DS_Store
*.pem

# debug
npm-debug.log*
yarn-debug.log*
yarn-error.log*

# local env files
.env
.env*.local

# vercel
.vercel

# typescript
*.tsbuildinfo
next-env.d.ts
```

## File: .repomixignore
```
# Add patterns to ignore here, one per line
# Example:
# *.log
# tmp/

# Dependency and lock files
package-lock.json
yarn.lock
pnpm-lock.yaml

# Log files
*.log

# System files
.DS_Store
Thumbs.db

# IDE and editor files
.vscode/
.idea/
*.swp
*.swo

# Build and generated directories
.next/
dist/
build/
.turbo/
coverage/
.nyc_output/

# UI component library (shadcn/ui boilerplate)
components/ui/**

# Configuration files
*.config.js
*.config.ts
tailwind.config.*
postcss.config.*
next.config.*
tsconfig.json
components.json

# Environment files (if sensitive)
.env.local
.env.development.local
.env.test.local
.env.production.local
```

## File: app/dashboard/page.tsx
```typescript
'use client';

import { useEffect, useState } from 'react';
import { useRouter } from 'next/navigation';
import { getCurrentUser, getUserProfile } from '@/lib/auth';
import Header from '@/components/Header';
import DriverDashboard from '@/components/DriverDashboard';
import PassengerDashboard from '@/components/PassengerDashboard';
import type { UserProfile } from '@/lib/supabase';

export default function Dashboard() {
  const [user, setUser] = useState<UserProfile | null>(null);
  const [loading, setLoading] = useState(true);
  const router = useRouter();

  useEffect(() => {
    const loadUser = async () => {
      try {
        const currentUser = await getCurrentUser();
        if (!currentUser) {
          router.push('/');
          return;
        }

        const profile = await getUserProfile(currentUser.id);
        if (!profile) {
          router.push('/');
          return;
        }

        setUser(profile);
      } catch (error) {
        console.error('Error loading user:', error);
        router.push('/');
      } finally {
        setLoading(false);
      }
    };

    loadUser();
  }, [router]);

  if (loading) {
    return (
      <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-cyan-50 flex items-center justify-center">
        <div className="text-center">
          <div className="w-16 h-16 bg-gradient-to-r from-blue-600 to-cyan-600 rounded-full flex items-center justify-center mb-4 mx-auto animate-pulse">
            <div className="w-8 h-8 bg-white rounded-full" />
          </div>
          <p className="text-gray-600">Loading dashboard...</p>
        </div>
      </div>
    );
  }

  if (!user) {
    return null;
  }

  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-cyan-50">
      <Header />
      {user.role === 'driver' ? <DriverDashboard /> : <PassengerDashboard />}
    </div>
  );
}
```

## File: app/globals.css
```css
@tailwind base;
@tailwind components;
@tailwind utilities;

:root {
  --foreground-rgb: 0, 0, 0;
  --background-start-rgb: 214, 219, 220;
  --background-end-rgb: 255, 255, 255;
}

@media (prefers-color-scheme: dark) {
  :root {
    --foreground-rgb: 255, 255, 255;
    --background-start-rgb: 0, 0, 0;
    --background-end-rgb: 0, 0, 0;
  }
}

@layer base {
  :root {
    --background: 0 0% 100%;
    --foreground: 0 0% 3.9%;
    --card: 0 0% 100%;
    --card-foreground: 0 0% 3.9%;
    --popover: 0 0% 100%;
    --popover-foreground: 0 0% 3.9%;
    --primary: 0 0% 9%;
    --primary-foreground: 0 0% 98%;
    --secondary: 0 0% 96.1%;
    --secondary-foreground: 0 0% 9%;
    --muted: 0 0% 96.1%;
    --muted-foreground: 0 0% 45.1%;
    --accent: 0 0% 96.1%;
    --accent-foreground: 0 0% 9%;
    --destructive: 0 84.2% 60.2%;
    --destructive-foreground: 0 0% 98%;
    --border: 0 0% 89.8%;
    --input: 0 0% 89.8%;
    --ring: 0 0% 3.9%;
    --chart-1: 12 76% 61%;
    --chart-2: 173 58% 39%;
    --chart-3: 197 37% 24%;
    --chart-4: 43 74% 66%;
    --chart-5: 27 87% 67%;
    --radius: 0.5rem;
  }
  .dark {
    --background: 0 0% 3.9%;
    --foreground: 0 0% 98%;
    --card: 0 0% 3.9%;
    --card-foreground: 0 0% 98%;
    --popover: 0 0% 3.9%;
    --popover-foreground: 0 0% 98%;
    --primary: 0 0% 98%;
    --primary-foreground: 0 0% 9%;
    --secondary: 0 0% 14.9%;
    --secondary-foreground: 0 0% 98%;
    --muted: 0 0% 14.9%;
    --muted-foreground: 0 0% 63.9%;
    --accent: 0 0% 14.9%;
    --accent-foreground: 0 0% 98%;
    --destructive: 0 62.8% 30.6%;
    --destructive-foreground: 0 0% 98%;
    --border: 0 0% 14.9%;
    --input: 0 0% 14.9%;
    --ring: 0 0% 83.1%;
    --chart-1: 220 70% 50%;
    --chart-2: 160 60% 45%;
    --chart-3: 30 80% 55%;
    --chart-4: 280 65% 60%;
    --chart-5: 340 75% 55%;
  }
}

@layer base {
  * {
    @apply border-border;
  }
  body {
    @apply bg-background text-foreground;
  }
}
```

## File: app/layout.tsx
```typescript
import './globals.css';
import type { Metadata } from 'next';
import { Inter } from 'next/font/google';
import { Toaster } from '@/components/ui/sonner';

const inter = Inter({ subsets: ['latin'] });

export const metadata: Metadata = {
  title: 'RideShare - Connect Drivers and Passengers',
  description: 'Find rides or offer rides in your community',
};

export default function RootLayout({
  children,
}: {
  children: React.ReactNode;
}) {
  return (
    <html lang="en">
      <body className={inter.className}>
        {children}
        <Toaster />
      </body>
    </html>
  );
}
```

## File: app/page.tsx
```typescript
'use client';

import { useEffect, useState } from 'react';
import { useRouter } from 'next/navigation';
import { getCurrentUser, getUserProfile } from '@/lib/auth';
import AuthForm from '@/components/AuthForm';

export default function Home() {
  const [loading, setLoading] = useState(true);
  const router = useRouter();

  useEffect(() => {
    const checkAuth = async () => {
      try {
        const user = await getCurrentUser();
        if (user) {
          const profile = await getUserProfile(user.id);
          if (profile) {
            router.push('/dashboard');
            return;
          }
        }
      } catch (error) {
        console.error('Auth check failed:', error);
      } finally {
        setLoading(false);
      }
    };

    checkAuth();
  }, [router]);

  if (loading) {
    return (
      <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-cyan-50 flex items-center justify-center">
        <div className="text-center">
          <div className="w-16 h-16 bg-gradient-to-r from-blue-600 to-cyan-600 rounded-full flex items-center justify-center mb-4 mx-auto animate-pulse">
            <div className="w-8 h-8 bg-white rounded-full" />
          </div>
          <p className="text-gray-600">Loading...</p>
        </div>
      </div>
    );
  }

  return <AuthForm />;
}
```

## File: components/AuthForm.tsx
```typescript
'use client';

import { useState } from 'react';
import { useRouter } from 'next/navigation';
import { Button } from '@/components/ui/button';
import { Input } from '@/components/ui/input';
import { Label } from '@/components/ui/label';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { RadioGroup, RadioGroupItem } from '@/components/ui/radio-group';
import { signUp, signIn } from '@/lib/auth';
import { Car, Users } from 'lucide-react';
import { toast } from 'sonner';

export default function AuthForm() {
  const [isLogin, setIsLogin] = useState(true);
  const [loading, setLoading] = useState(false);
  const router = useRouter();

  const [formData, setFormData] = useState({
    email: '',
    password: '',
    firstName: '',
    lastName: '',
    phone: '',
    role: 'passenger' as 'driver' | 'passenger',
  });

  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();
    setLoading(true);

    try {
      if (isLogin) {
        await signIn(formData.email, formData.password);
        toast.success('Welcome back!');
      } else {
        await signUp(formData.email, formData.password, {
          role: formData.role,
          first_name: formData.firstName,
          last_name: formData.lastName,
          phone: formData.phone,
        });
        toast.success('Account created successfully!');
      }
      
      router.push('/dashboard');
    } catch (error: any) {
      toast.error(error.message || 'An error occurred');
    } finally {
      setLoading(false);
    }
  };

  const handleInputChange = (field: string, value: string) => {
    setFormData(prev => ({ ...prev, [field]: value }));
  };

  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-cyan-50 flex items-center justify-center p-4">
      <div className="w-full max-w-md">
        <Card className="backdrop-blur-sm bg-white/90 shadow-xl border-0">
          <CardHeader className="text-center pb-6">
            <div className="mx-auto w-16 h-16 bg-gradient-to-r from-blue-600 to-cyan-600 rounded-full flex items-center justify-center mb-4">
              <Car className="h-8 w-8 text-white" />
            </div>
            <CardTitle className="text-2xl font-bold bg-gradient-to-r from-blue-600 to-cyan-600 bg-clip-text text-transparent">
              RideShare
            </CardTitle>
            <CardDescription className="text-gray-600">
              {isLogin ? 'Welcome back! Please sign in.' : 'Create your account to get started.'}
            </CardDescription>
          </CardHeader>
          <CardContent>
            <form onSubmit={handleSubmit} className="space-y-4">
              <div className="space-y-2">
                <Label htmlFor="email">Email</Label>
                <Input
                  id="email"
                  type="email"
                  value={formData.email}
                  onChange={(e) => handleInputChange('email', e.target.value)}
                  required
                  className="transition-all duration-200 focus:ring-2 focus:ring-blue-500"
                />
              </div>
              
              <div className="space-y-2">
                <Label htmlFor="password">Password</Label>
                <Input
                  id="password"
                  type="password"
                  value={formData.password}
                  onChange={(e) => handleInputChange('password', e.target.value)}
                  required
                  className="transition-all duration-200 focus:ring-2 focus:ring-blue-500"
                />
              </div>

              {!isLogin && (
                <>
                  <div className="grid grid-cols-2 gap-3">
                    <div className="space-y-2">
                      <Label htmlFor="firstName">First Name</Label>
                      <Input
                        id="firstName"
                        value={formData.firstName}
                        onChange={(e) => handleInputChange('firstName', e.target.value)}
                        required
                        className="transition-all duration-200 focus:ring-2 focus:ring-blue-500"
                      />
                    </div>
                    <div className="space-y-2">
                      <Label htmlFor="lastName">Last Name</Label>
                      <Input
                        id="lastName"
                        value={formData.lastName}
                        onChange={(e) => handleInputChange('lastName', e.target.value)}
                        required
                        className="transition-all duration-200 focus:ring-2 focus:ring-blue-500"
                      />
                    </div>
                  </div>

                  <div className="space-y-2">
                    <Label htmlFor="phone">Phone (Optional)</Label>
                    <Input
                      id="phone"
                      value={formData.phone}
                      onChange={(e) => handleInputChange('phone', e.target.value)}
                      className="transition-all duration-200 focus:ring-2 focus:ring-blue-500"
                    />
                  </div>

                  <div className="space-y-3">
                    <Label>I want to:</Label>
                    <RadioGroup
                      value={formData.role}
                      onValueChange={(value) => handleInputChange('role', value)}
                      className="grid grid-cols-2 gap-4"
                    >
                      <div className="flex items-center space-x-2 p-3 border rounded-lg hover:bg-gray-50 transition-colors">
                        <RadioGroupItem value="passenger" id="passenger" />
                        <Label htmlFor="passenger" className="flex items-center gap-2 cursor-pointer">
                          <Users className="h-4 w-4" />
                          Find Rides
                        </Label>
                      </div>
                      <div className="flex items-center space-x-2 p-3 border rounded-lg hover:bg-gray-50 transition-colors">
                        <RadioGroupItem value="driver" id="driver" />
                        <Label htmlFor="driver" className="flex items-center gap-2 cursor-pointer">
                          <Car className="h-4 w-4" />
                          Offer Rides
                        </Label>
                      </div>
                    </RadioGroup>
                  </div>
                </>
              )}

              <Button 
                type="submit" 
                className="w-full bg-gradient-to-r from-blue-600 to-cyan-600 hover:from-blue-700 hover:to-cyan-700 transition-all duration-200 transform hover:scale-105"
                disabled={loading}
              >
                {loading ? 'Please wait...' : (isLogin ? 'Sign In' : 'Create Account')}
              </Button>
            </form>

            <div className="mt-6 text-center">
              <button
                type="button"
                onClick={() => setIsLogin(!isLogin)}
                className="text-blue-600 hover:text-blue-700 text-sm font-medium transition-colors"
              >
                {isLogin ? "Don't have an account? Sign up" : 'Already have an account? Sign in'}
              </button>
            </div>
          </CardContent>
        </Card>
      </div>
    </div>
  );
}
```

## File: components/DriverDashboard.tsx
```typescript
'use client';

import { useState, useEffect } from 'react';
import { Button } from '@/components/ui/button';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Badge } from '@/components/ui/badge';
import { Input } from '@/components/ui/input';
import { Label } from '@/components/ui/label';
import { Textarea } from '@/components/ui/textarea';
import { Dialog, DialogContent, DialogDescription, DialogHeader, DialogTitle, DialogTrigger } from '@/components/ui/dialog';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { getRidesByDriver, getApplicationsForRide, updateApplicationStatus, findMatchingRequests, createRide } from '@/lib/rides';
import { getCurrentUser } from '@/lib/auth';
import { Car, Plus, Users, Clock, MapPin, DollarSign, CheckCircle, XCircle } from 'lucide-react';
import { toast } from 'sonner';
import type { Ride, RideApplication, RideRequest } from '@/lib/supabase';

export default function DriverDashboard() {
  const [rides, setRides] = useState<Ride[]>([]);
  const [applications, setApplications] = useState<RideApplication[]>([]);
  const [matchingRequests, setMatchingRequests] = useState<RideRequest[]>([]);
  const [loading, setLoading] = useState(true);
  const [selectedRide, setSelectedRide] = useState<Ride | null>(null);
  const [showCreateRide, setShowCreateRide] = useState(false);

  const [newRide, setNewRide] = useState({
    start_point: '',
    end_point: '',
    stops: '',
    departure_time: '',
    available_seats: 1,
    price_per_seat: '',
  });

  const loadData = async () => {
    try {
      const user = await getCurrentUser();
      if (user) {
        const userRides = await getRidesByDriver(user.id);
        setRides(userRides);
        
        // Load applications for all rides
        const allApplications: RideApplication[] = [];
        for (const ride of userRides) {
          const rideApplications = await getApplicationsForRide(ride.id);
          allApplications.push(...rideApplications);
        }
        setApplications(allApplications);
      }
    } catch (error: any) {
      toast.error('Failed to load dashboard data');
    } finally {
      setLoading(false);
    }
  };

  const handleCreateRide = async (e: React.FormEvent) => {
    e.preventDefault();
    try {
      const user = await getCurrentUser();
      if (!user) return;

      const rideData = {
        driver_id: user.id,
        start_point: newRide.start_point,
        end_point: newRide.end_point,
        stops: newRide.stops ? newRide.stops.split(',').map(s => s.trim()) : [],
        departure_time: newRide.departure_time,
        available_seats: newRide.available_seats,
        price_per_seat: newRide.price_per_seat ? parseFloat(newRide.price_per_seat) : undefined,
        status: 'active' as const,
      };

      const createdRide = await createRide(rideData);
      
      // Find matching requests
      const matches = await findMatchingRequests(createdRide);
      setMatchingRequests(matches);
      
      if (matches.length > 0) {
        toast.success(`Ride created! Found ${matches.length} matching passenger requests.`);
      } else {
        toast.success('Ride created successfully!');
      }
      
      setShowCreateRide(false);
      setNewRide({
        start_point: '',
        end_point: '',
        stops: '',
        departure_time: '',
        available_seats: 1,
        price_per_seat: '',
      });
      
      loadData();
    } catch (error: any) {
      toast.error('Failed to create ride');
    }
  };

  const handleApplicationAction = async (applicationId: string, action: 'approved' | 'rejected') => {
    try {
      await updateApplicationStatus(applicationId, action);
      toast.success(`Application ${action}!`);
      loadData();
    } catch (error: any) {
      toast.error(`Failed to ${action} application`);
    }
  };

  const formatDateTime = (dateString: string) => {
    return new Date(dateString).toLocaleString();
  };

  const getStatusColor = (status: string) => {
    switch (status) {
      case 'active': return 'bg-green-100 text-green-800';
      case 'completed': return 'bg-blue-100 text-blue-800';
      case 'cancelled': return 'bg-red-100 text-red-800';
      default: return 'bg-gray-100 text-gray-800';
    }
  };

  const getApplicationStatusColor = (status: string) => {
    switch (status) {
      case 'pending': return 'bg-yellow-100 text-yellow-800';
      case 'approved': return 'bg-green-100 text-green-800';
      case 'rejected': return 'bg-red-100 text-red-800';
      default: return 'bg-gray-100 text-gray-800';
    }
  };

  useEffect(() => {
    loadData();
  }, []);

  if (loading) {
    return (
      <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-cyan-50 flex items-center justify-center">
        <div className="text-center">
          <Car className="h-12 w-12 mx-auto text-blue-600 animate-pulse mb-4" />
          <p className="text-gray-600">Loading your dashboard...</p>
        </div>
      </div>
    );
  }

  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-cyan-50 p-6">
      <div className="max-w-7xl mx-auto">
        <div className="flex justify-between items-center mb-8">
          <div>
            <h1 className="text-3xl font-bold text-gray-900">Driver Dashboard</h1>
            <p className="text-gray-600 mt-2">Manage your rides and passenger applications</p>
          </div>
          
          <Dialog open={showCreateRide} onOpenChange={setShowCreateRide}>
            <DialogTrigger asChild>
              <Button className="bg-gradient-to-r from-blue-600 to-cyan-600 hover:from-blue-700 hover:to-cyan-700">
                <Plus className="h-4 w-4 mr-2" />
                Post New Ride
              </Button>
            </DialogTrigger>
            <DialogContent className="max-w-md">
              <DialogHeader>
                <DialogTitle>Post a New Ride</DialogTitle>
                <DialogDescription>
                  Fill in the details of your ride to find passengers
                </DialogDescription>
              </DialogHeader>
              <form onSubmit={handleCreateRide} className="space-y-4">
                <div className="grid grid-cols-2 gap-3">
                  <div className="space-y-2">
                    <Label htmlFor="start_point">From</Label>
                    <Input
                      id="start_point"
                      value={newRide.start_point}
                      onChange={(e) => setNewRide({ ...newRide, start_point: e.target.value })}
                      placeholder="Starting location"
                      required
                    />
                  </div>
                  <div className="space-y-2">
                    <Label htmlFor="end_point">To</Label>
                    <Input
                      id="end_point"
                      value={newRide.end_point}
                      onChange={(e) => setNewRide({ ...newRide, end_point: e.target.value })}
                      placeholder="Destination"
                      required
                    />
                  </div>
                </div>
                
                <div className="space-y-2">
                  <Label htmlFor="stops">Stops (Optional)</Label>
                  <Input
                    id="stops"
                    value={newRide.stops}
                    onChange={(e) => setNewRide({ ...newRide, stops: e.target.value })}
                    placeholder="Stop 1, Stop 2, Stop 3..."
                  />
                </div>
                
                <div className="grid grid-cols-2 gap-3">
                  <div className="space-y-2">
                    <Label htmlFor="departure_time">Departure</Label>
                    <Input
                      id="departure_time"
                      type="datetime-local"
                      value={newRide.departure_time}
                      onChange={(e) => setNewRide({ ...newRide, departure_time: e.target.value })}
                      required
                    />
                  </div>
                  <div className="space-y-2">
                    <Label htmlFor="available_seats">Seats</Label>
                    <Input
                      id="available_seats"
                      type="number"
                      min="1"
                      max="8"
                      value={newRide.available_seats}
                      onChange={(e) => setNewRide({ ...newRide, available_seats: parseInt(e.target.value) })}
                      required
                    />
                  </div>
                </div>
                
                <div className="space-y-2">
                  <Label htmlFor="price_per_seat">Price per Seat (Optional)</Label>
                  <Input
                    id="price_per_seat"
                    type="number"
                    step="0.01"
                    value={newRide.price_per_seat}
                    onChange={(e) => setNewRide({ ...newRide, price_per_seat: e.target.value })}
                    placeholder="0.00"
                  />
                </div>
                
                <Button type="submit" className="w-full">
                  Post Ride
                </Button>
              </form>
            </DialogContent>
          </Dialog>
        </div>

        <Tabs defaultValue="rides" className="space-y-6">
          <TabsList className="grid w-full grid-cols-3">
            <TabsTrigger value="rides">My Rides</TabsTrigger>
            <TabsTrigger value="applications">Applications</TabsTrigger>
            <TabsTrigger value="matches">Matching Requests</TabsTrigger>
          </TabsList>

          <TabsContent value="rides" className="space-y-4">
            {rides.length === 0 ? (
              <Card>
                <CardContent className="text-center py-12">
                  <Car className="h-12 w-12 mx-auto text-gray-400 mb-4" />
                  <p className="text-gray-600">No rides posted yet</p>
                  <p className="text-sm text-gray-500 mt-2">Click "Post New Ride" to get started</p>
                </CardContent>
              </Card>
            ) : (
              <div className="grid gap-4">
                {rides.map((ride) => (
                  <Card key={ride.id} className="hover:shadow-md transition-shadow">
                    <CardContent className="p-6">
                      <div className="flex justify-between items-start mb-4">
                        <div className="flex-1">
                          <div className="flex items-center gap-2 mb-2">
                            <MapPin className="h-4 w-4 text-blue-600" />
                            <span className="font-medium">{ride.start_point}</span>
                            <span className="text-gray-400">→</span>
                            <span className="font-medium">{ride.end_point}</span>
                          </div>
                          {ride.stops.length > 0 && (
                            <div className="text-sm text-gray-600 mb-2">
                              Stops: {ride.stops.join(', ')}
                            </div>
                          )}
                          <div className="flex items-center gap-4 text-sm text-gray-600">
                            <div className="flex items-center gap-1">
                              <Clock className="h-4 w-4" />
                              {formatDateTime(ride.departure_time)}
                            </div>
                            <div className="flex items-center gap-1">
                              <Users className="h-4 w-4" />
                              {ride.available_seats} seats
                            </div>
                            {ride.price_per_seat && (
                              <div className="flex items-center gap-1">
                                <DollarSign className="h-4 w-4" />
                                ${ride.price_per_seat}/seat
                              </div>
                            )}
                          </div>
                        </div>
                        <Badge className={getStatusColor(ride.status)}>
                          {ride.status}
                        </Badge>
                      </div>
                    </CardContent>
                  </Card>
                ))}
              </div>
            )}
          </TabsContent>

          <TabsContent value="applications" className="space-y-4">
            {applications.length === 0 ? (
              <Card>
                <CardContent className="text-center py-12">
                  <Users className="h-12 w-12 mx-auto text-gray-400 mb-4" />
                  <p className="text-gray-600">No applications yet</p>
                  <p className="text-sm text-gray-500 mt-2">Applications will appear here when passengers apply for your rides</p>
                </CardContent>
              </Card>
            ) : (
              <div className="grid gap-4">
                {applications.map((application) => (
                  <Card key={application.id} className="hover:shadow-md transition-shadow">
                    <CardContent className="p-6">
                      <div className="flex justify-between items-start mb-4">
                        <div className="flex-1">
                          <div className="flex items-center gap-2 mb-2">
                            <h3 className="font-medium">
                              {application.passenger?.first_name} {application.passenger?.last_name}
                            </h3>
                            <Badge className={getApplicationStatusColor(application.status)}>
                              {application.status}
                            </Badge>
                          </div>
                          <div className="flex items-center gap-4 text-sm text-gray-600 mb-2">
                            <div className="flex items-center gap-1">
                              <Users className="h-4 w-4" />
                              {application.seats_requested} seat{application.seats_requested > 1 ? 's' : ''}
                            </div>
                            <div className="flex items-center gap-1">
                              <Clock className="h-4 w-4" />
                              Applied {formatDateTime(application.created_at)}
                            </div>
                          </div>
                          {application.message && (
                            <p className="text-sm text-gray-700 bg-gray-50 p-3 rounded-lg">
                              "{application.message}"
                            </p>
                          )}
                        </div>
                        {application.status === 'pending' && (
                          <div className="flex gap-2">
                            <Button
                              size="sm"
                              onClick={() => handleApplicationAction(application.id, 'approved')}
                              className="bg-green-600 hover:bg-green-700"
                            >
                              <CheckCircle className="h-4 w-4 mr-1" />
                              Approve
                            </Button>
                            <Button
                              size="sm"
                              variant="outline"
                              onClick={() => handleApplicationAction(application.id, 'rejected')}
                              className="text-red-600 border-red-600 hover:bg-red-50"
                            >
                              <XCircle className="h-4 w-4 mr-1" />
                              Reject
                            </Button>
                          </div>
                        )}
                      </div>
                    </CardContent>
                  </Card>
                ))}
              </div>
            )}
          </TabsContent>

          <TabsContent value="matches" className="space-y-4">
            {matchingRequests.length === 0 ? (
              <Card>
                <CardContent className="text-center py-12">
                  <MapPin className="h-12 w-12 mx-auto text-gray-400 mb-4" />
                  <p className="text-gray-600">No matching requests found</p>
                  <p className="text-sm text-gray-500 mt-2">Matching passenger requests will appear here</p>
                </CardContent>
              </Card>
            ) : (
              <div className="grid gap-4">
                {matchingRequests.map((request) => (
                  <Card key={request.id} className="hover:shadow-md transition-shadow border-l-4 border-l-orange-500">
                    <CardContent className="p-6">
                      <div className="flex justify-between items-start mb-4">
                        <div className="flex-1">
                          <div className="flex items-center gap-2 mb-2">
                            <h3 className="font-medium">
                              {request.passenger?.first_name} {request.passenger?.last_name}
                            </h3>
                            <Badge className="bg-orange-100 text-orange-800">
                              Match Found
                            </Badge>
                          </div>
                          <div className="flex items-center gap-2 mb-2">
                            <MapPin className="h-4 w-4 text-orange-600" />
                            <span className="font-medium">{request.start_point}</span>
                            <span className="text-gray-400">→</span>
                            <span className="font-medium">{request.end_point}</span>
                          </div>
                          <div className="flex items-center gap-4 text-sm text-gray-600">
                            <div className="flex items-center gap-1">
                              <Clock className="h-4 w-4" />
                              {formatDateTime(request.departure_time)}
                            </div>
                            {request.max_price && (
                              <div className="flex items-center gap-1">
                                <DollarSign className="h-4 w-4" />
                                Max: ${request.max_price}
                              </div>
                            )}
                          </div>
                        </div>
                      </div>
                    </CardContent>
                  </Card>
                ))}
              </div>
            )}
          </TabsContent>
        </Tabs>
      </div>
    </div>
  );
}
```

## File: components/Header.tsx
```typescript
'use client';

import { useState, useEffect } from 'react';
import { useRouter } from 'next/navigation';
import { Button } from '@/components/ui/button';
import { Avatar, AvatarFallback } from '@/components/ui/avatar';
import { DropdownMenu, DropdownMenuContent, DropdownMenuItem, DropdownMenuTrigger } from '@/components/ui/dropdown-menu';
import { getCurrentUser, getUserProfile, signOut } from '@/lib/auth';
import { Car, LogOut, User } from 'lucide-react';
import type { UserProfile } from '@/lib/supabase';

export default function Header() {
  const [user, setUser] = useState<UserProfile | null>(null);
  const [loading, setLoading] = useState(true);
  const router = useRouter();

  useEffect(() => {
    const loadUser = async () => {
      try {
        const currentUser = await getCurrentUser();
        if (currentUser) {
          const profile = await getUserProfile(currentUser.id);
          setUser(profile);
        }
      } catch (error) {
        console.error('Error loading user:', error);
      } finally {
        setLoading(false);
      }
    };

    loadUser();
  }, []);

  const handleSignOut = async () => {
    try {
      await signOut();
      router.push('/');
    } catch (error) {
      console.error('Error signing out:', error);
    }
  };

  if (loading) {
    return (
      <header className="bg-white/80 backdrop-blur-sm border-b border-gray-200 sticky top-0 z-50">
        <div className="max-w-7xl mx-auto px-6 py-4">
          <div className="flex justify-between items-center">
            <div className="flex items-center gap-2">
              <Car className="h-8 w-8 text-blue-600" />
              <span className="text-xl font-bold bg-gradient-to-r from-blue-600 to-cyan-600 bg-clip-text text-transparent">
                RideShare
              </span>
            </div>
            <div className="w-8 h-8 bg-gray-200 rounded-full animate-pulse" />
          </div>
        </div>
      </header>
    );
  }

  if (!user) {
    return null;
  }

  return (
    <header className="bg-white/80 backdrop-blur-sm border-b border-gray-200 sticky top-0 z-50">
      <div className="max-w-7xl mx-auto px-6 py-4">
        <div className="flex justify-between items-center">
          <div className="flex items-center gap-2">
            <Car className="h-8 w-8 text-blue-600" />
            <span className="text-xl font-bold bg-gradient-to-r from-blue-600 to-cyan-600 bg-clip-text text-transparent">
              RideShare
            </span>
          </div>
          
          <div className="flex items-center gap-4">
            <div className="text-sm text-gray-600 capitalize">
              {user.role} Dashboard
            </div>
            
            <DropdownMenu>
              <DropdownMenuTrigger asChild>
                <Button variant="ghost" className="relative h-10 w-10 rounded-full">
                  <Avatar className="h-10 w-10">
                    <AvatarFallback className="bg-gradient-to-r from-blue-600 to-cyan-600 text-white">
                      {user.first_name[0]}{user.last_name[0]}
                    </AvatarFallback>
                  </Avatar>
                </Button>
              </DropdownMenuTrigger>
              <DropdownMenuContent className="w-56" align="end" forceMount>
                <DropdownMenuItem className="flex items-center gap-2">
                  <User className="h-4 w-4" />
                  <div className="flex flex-col space-y-1">
                    <p className="text-sm font-medium">
                      {user.first_name} {user.last_name}
                    </p>
                    <p className="text-xs text-gray-500 capitalize">
                      {user.role}
                    </p>
                  </div>
                </DropdownMenuItem>
                <DropdownMenuItem onClick={handleSignOut} className="flex items-center gap-2 text-red-600">
                  <LogOut className="h-4 w-4" />
                  Sign Out
                </DropdownMenuItem>
              </DropdownMenuContent>
            </DropdownMenu>
          </div>
        </div>
      </div>
    </header>
  );
}
```

## File: components/PassengerDashboard.tsx
```typescript
'use client';

import { useState, useEffect } from 'react';
import { Button } from '@/components/ui/button';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Badge } from '@/components/ui/badge';
import { Input } from '@/components/ui/input';
import { Label } from '@/components/ui/label';
import { Textarea } from '@/components/ui/textarea';
import { Dialog, DialogContent, DialogDescription, DialogHeader, DialogTitle, DialogTrigger } from '@/components/ui/dialog';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { getActiveRides, getRideRequestsByPassenger, getApplicationsByPassenger, applyForRide, createRideRequest, findMatchingRides } from '@/lib/rides';
import { getCurrentUser } from '@/lib/auth';
import { Users, Plus, Car, Clock, MapPin, DollarSign, Send } from 'lucide-react';
import { toast } from 'sonner';
import type { Ride, RideRequest, RideApplication } from '@/lib/supabase';

export default function PassengerDashboard() {
  const [availableRides, setAvailableRides] = useState<Ride[]>([]);
  const [myRequests, setMyRequests] = useState<RideRequest[]>([]);
  const [myApplications, setMyApplications] = useState<RideApplication[]>([]);
  const [matchingRides, setMatchingRides] = useState<Ride[]>([]);
  const [loading, setLoading] = useState(true);
  const [showCreateRequest, setShowCreateRequest] = useState(false);
  const [showApplicationDialog, setShowApplicationDialog] = useState(false);
  const [selectedRide, setSelectedRide] = useState<Ride | null>(null);

  const [newRequest, setNewRequest] = useState({
    start_point: '',
    end_point: '',
    departure_time: '',
    max_price: '',
  });

  const [applicationData, setApplicationData] = useState({
    seats_requested: 1,
    message: '',
  });

  const loadData = async () => {
    try {
      const user = await getCurrentUser();
      if (user) {
        const [rides, requests, applications] = await Promise.all([
          getActiveRides(),
          getRideRequestsByPassenger(user.id),
          getApplicationsByPassenger(user.id),
        ]);
        
        setAvailableRides(rides);
        setMyRequests(requests);
        setMyApplications(applications);
      }
    } catch (error: any) {
      toast.error('Failed to load dashboard data');
    } finally {
      setLoading(false);
    }
  };

  const handleCreateRequest = async (e: React.FormEvent) => {
    e.preventDefault();
    try {
      const user = await getCurrentUser();
      if (!user) return;

      const requestData = {
        passenger_id: user.id,
        start_point: newRequest.start_point,
        end_point: newRequest.end_point,
        departure_time: newRequest.departure_time,
        max_price: newRequest.max_price ? parseFloat(newRequest.max_price) : undefined,
        status: 'active' as const,
      };

      const createdRequest = await createRideRequest(requestData);
      
      // Find matching rides
      const matches = await findMatchingRides(createdRequest);
      setMatchingRides(matches);
      
      if (matches.length > 0) {
        toast.success(`Request created! Found ${matches.length} matching rides.`);
      } else {
        toast.success('Request created successfully!');
      }
      
      setShowCreateRequest(false);
      setNewRequest({
        start_point: '',
        end_point: '',
        departure_time: '',
        max_price: '',
      });
      
      loadData();
    } catch (error: any) {
      toast.error('Failed to create request');
    }
  };

  const handleApplyForRide = async () => {
    if (!selectedRide) return;
    
    try {
      const user = await getCurrentUser();
      if (!user) return;

      await applyForRide({
        ride_id: selectedRide.id,
        passenger_id: user.id,
        seats_requested: applicationData.seats_requested,
        message: applicationData.message,
        status: 'pending',
      });

      toast.success('Application submitted successfully!');
      setShowApplicationDialog(false);
      setSelectedRide(null);
      setApplicationData({ seats_requested: 1, message: '' });
      loadData();
    } catch (error: any) {
      if (error.message.includes('duplicate')) {
        toast.error('You have already applied for this ride');
      } else {
        toast.error('Failed to submit application');
      }
    }
  };

  const openApplicationDialog = (ride: Ride) => {
    setSelectedRide(ride);
    setShowApplicationDialog(true);
  };

  const formatDateTime = (dateString: string) => {
    return new Date(dateString).toLocaleString();
  };

  const getStatusColor = (status: string) => {
    switch (status) {
      case 'active': return 'bg-green-100 text-green-800';
      case 'matched': return 'bg-blue-100 text-blue-800';
      case 'completed': return 'bg-purple-100 text-purple-800';
      case 'cancelled': return 'bg-red-100 text-red-800';
      default: return 'bg-gray-100 text-gray-800';
    }
  };

  const getApplicationStatusColor = (status: string) => {
    switch (status) {
      case 'pending': return 'bg-yellow-100 text-yellow-800';
      case 'approved': return 'bg-green-100 text-green-800';
      case 'rejected': return 'bg-red-100 text-red-800';
      default: return 'bg-gray-100 text-gray-800';
    }
  };

  useEffect(() => {
    loadData();
  }, []);

  if (loading) {
    return (
      <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-cyan-50 flex items-center justify-center">
        <div className="text-center">
          <Users className="h-12 w-12 mx-auto text-blue-600 animate-pulse mb-4" />
          <p className="text-gray-600">Loading your dashboard...</p>
        </div>
      </div>
    );
  }

  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-cyan-50 p-6">
      <div className="max-w-7xl mx-auto">
        <div className="flex justify-between items-center mb-8">
          <div>
            <h1 className="text-3xl font-bold text-gray-900">Passenger Dashboard</h1>
            <p className="text-gray-600 mt-2">Find rides and manage your travel requests</p>
          </div>
          
          <Dialog open={showCreateRequest} onOpenChange={setShowCreateRequest}>
            <DialogTrigger asChild>
              <Button className="bg-gradient-to-r from-blue-600 to-cyan-600 hover:from-blue-700 hover:to-cyan-700">
                <Plus className="h-4 w-4 mr-2" />
                Create Ride Request
              </Button>
            </DialogTrigger>
            <DialogContent className="max-w-md">
              <DialogHeader>
                <DialogTitle>Create a Ride Request</DialogTitle>
                <DialogDescription>
                  Let drivers know where you want to go
                </DialogDescription>
              </DialogHeader>
              <form onSubmit={handleCreateRequest} className="space-y-4">
                <div className="grid grid-cols-2 gap-3">
                  <div className="space-y-2">
                    <Label htmlFor="start_point">From</Label>
                    <Input
                      id="start_point"
                      value={newRequest.start_point}
                      onChange={(e) => setNewRequest({ ...newRequest, start_point: e.target.value })}
                      placeholder="Starting location"
                      required
                    />
                  </div>
                  <div className="space-y-2">
                    <Label htmlFor="end_point">To</Label>
                    <Input
                      id="end_point"
                      value={newRequest.end_point}
                      onChange={(e) => setNewRequest({ ...newRequest, end_point: e.target.value })}
                      placeholder="Destination"
                      required
                    />
                  </div>
                </div>
                
                <div className="grid grid-cols-2 gap-3">
                  <div className="space-y-2">
                    <Label htmlFor="departure_time">Departure</Label>
                    <Input
                      id="departure_time"
                      type="datetime-local"
                      value={newRequest.departure_time}
                      onChange={(e) => setNewRequest({ ...newRequest, departure_time: e.target.value })}
                      required
                    />
                  </div>
                  <div className="space-y-2">
                    <Label htmlFor="max_price">Max Price</Label>
                    <Input
                      id="max_price"
                      type="number"
                      step="0.01"
                      value={newRequest.max_price}
                      onChange={(e) => setNewRequest({ ...newRequest, max_price: e.target.value })}
                      placeholder="0.00"
                    />
                  </div>
                </div>
                
                <Button type="submit" className="w-full">
                  Create Request
                </Button>
              </form>
            </DialogContent>
          </Dialog>
        </div>

        <Tabs defaultValue="available" className="space-y-6">
          <TabsList className="grid w-full grid-cols-4">
            <TabsTrigger value="available">Available Rides</TabsTrigger>
            <TabsTrigger value="requests">My Requests</TabsTrigger>
            <TabsTrigger value="applications">My Applications</TabsTrigger>
            <TabsTrigger value="matches">Matching Rides</TabsTrigger>
          </TabsList>

          <TabsContent value="available" className="space-y-4">
            {availableRides.length === 0 ? (
              <Card>
                <CardContent className="text-center py-12">
                  <Car className="h-12 w-12 mx-auto text-gray-400 mb-4" />
                  <p className="text-gray-600">No available rides</p>
                  <p className="text-sm text-gray-500 mt-2">Create a ride request to find drivers</p>
                </CardContent>
              </Card>
            ) : (
              <div className="grid gap-4">
                {availableRides.map((ride) => (
                  <Card key={ride.id} className="hover:shadow-md transition-shadow">
                    <CardContent className="p-6">
                      <div className="flex justify-between items-start mb-4">
                        <div className="flex-1">
                          <div className="flex items-center gap-2 mb-2">
                            <h3 className="font-medium">
                              {ride.driver?.first_name} {ride.driver?.last_name}
                            </h3>
                            <Badge className={getStatusColor(ride.status)}>
                              {ride.status}
                            </Badge>
                          </div>
                          <div className="flex items-center gap-2 mb-2">
                            <MapPin className="h-4 w-4 text-blue-600" />
                            <span className="font-medium">{ride.start_point}</span>
                            <span className="text-gray-400">→</span>
                            <span className="font-medium">{ride.end_point}</span>
                          </div>
                          {ride.stops.length > 0 && (
                            <div className="text-sm text-gray-600 mb-2">
                              Stops: {ride.stops.join(', ')}
                            </div>
                          )}
                          <div className="flex items-center gap-4 text-sm text-gray-600">
                            <div className="flex items-center gap-1">
                              <Clock className="h-4 w-4" />
                              {formatDateTime(ride.departure_time)}
                            </div>
                            <div className="flex items-center gap-1">
                              <Users className="h-4 w-4" />
                              {ride.available_seats} seats
                            </div>
                            {ride.price_per_seat && (
                              <div className="flex items-center gap-1">
                                <DollarSign className="h-4 w-4" />
                                ${ride.price_per_seat}/seat
                              </div>
                            )}
                          </div>
                        </div>
                        <Button
                          onClick={() => openApplicationDialog(ride)}
                          className="bg-green-600 hover:bg-green-700"
                        >
                          <Send className="h-4 w-4 mr-2" />
                          Apply
                        </Button>
                      </div>
                    </CardContent>
                  </Card>
                ))}
              </div>
            )}
          </TabsContent>

          <TabsContent value="requests" className="space-y-4">
            {myRequests.length === 0 ? (
              <Card>
                <CardContent className="text-center py-12">
                  <Plus className="h-12 w-12 mx-auto text-gray-400 mb-4" />
                  <p className="text-gray-600">No ride requests yet</p>
                  <p className="text-sm text-gray-500 mt-2">Click "Create Ride Request" to get started</p>
                </CardContent>
              </Card>
            ) : (
              <div className="grid gap-4">
                {myRequests.map((request) => (
                  <Card key={request.id} className="hover:shadow-md transition-shadow">
                    <CardContent className="p-6">
                      <div className="flex justify-between items-start mb-4">
                        <div className="flex-1">
                          <div className="flex items-center gap-2 mb-2">
                            <MapPin className="h-4 w-4 text-blue-600" />
                            <span className="font-medium">{request.start_point}</span>
                            <span className="text-gray-400">→</span>
                            <span className="font-medium">{request.end_point}</span>
                          </div>
                          <div className="flex items-center gap-4 text-sm text-gray-600">
                            <div className="flex items-center gap-1">
                              <Clock className="h-4 w-4" />
                              {formatDateTime(request.departure_time)}
                            </div>
                            {request.max_price && (
                              <div className="flex items-center gap-1">
                                <DollarSign className="h-4 w-4" />
                                Max: ${request.max_price}
                              </div>
                            )}
                          </div>
                        </div>
                        <Badge className={getStatusColor(request.status)}>
                          {request.status}
                        </Badge>
                      </div>
                    </CardContent>
                  </Card>
                ))}
              </div>
            )}
          </TabsContent>

          <TabsContent value="applications" className="space-y-4">
            {myApplications.length === 0 ? (
              <Card>
                <CardContent className="text-center py-12">
                  <Send className="h-12 w-12 mx-auto text-gray-400 mb-4" />
                  <p className="text-gray-600">No applications yet</p>
                  <p className="text-sm text-gray-500 mt-2">Apply for rides to see your applications here</p>
                </CardContent>
              </Card>
            ) : (
              <div className="grid gap-4">
                {myApplications.map((application) => (
                  <Card key={application.id} className="hover:shadow-md transition-shadow">
                    <CardContent className="p-6">
                      <div className="flex justify-between items-start mb-4">
                        <div className="flex-1">
                          <div className="flex items-center gap-2 mb-2">
                            <h3 className="font-medium">
                              Ride by {application.ride?.driver?.first_name} {application.ride?.driver?.last_name}
                            </h3>
                            <Badge className={getApplicationStatusColor(application.status)}>
                              {application.status}
                            </Badge>
                          </div>
                          <div className="flex items-center gap-2 mb-2">
                            <MapPin className="h-4 w-4 text-blue-600" />
                            <span className="font-medium">{application.ride?.start_point}</span>
                            <span className="text-gray-400">→</span>
                            <span className="font-medium">{application.ride?.end_point}</span>
                          </div>
                          <div className="flex items-center gap-4 text-sm text-gray-600">
                            <div className="flex items-center gap-1">
                              <Clock className="h-4 w-4" />
                              {application.ride?.departure_time && formatDateTime(application.ride.departure_time)}
                            </div>
                            <div className="flex items-center gap-1">
                              <Users className="h-4 w-4" />
                              {application.seats_requested} seat{application.seats_requested > 1 ? 's' : ''}
                            </div>
                          </div>
                          {application.message && (
                            <div className="mt-2 text-sm text-gray-700 bg-gray-50 p-3 rounded-lg">
                              "{application.message}"
                            </div>
                          )}
                        </div>
                      </div>
                    </CardContent>
                  </Card>
                ))}
              </div>
            )}
          </TabsContent>

          <TabsContent value="matches" className="space-y-4">
            {matchingRides.length === 0 ? (
              <Card>
                <CardContent className="text-center py-12">
                  <MapPin className="h-12 w-12 mx-auto text-gray-400 mb-4" />
                  <p className="text-gray-600">No matching rides found</p>
                  <p className="text-sm text-gray-500 mt-2">Matching rides will appear here after creating requests</p>
                </CardContent>
              </Card>
            ) : (
              <div className="grid gap-4">
                {matchingRides.map((ride) => (
                  <Card key={ride.id} className="hover:shadow-md transition-shadow border-l-4 border-l-orange-500">
                    <CardContent className="p-6">
                      <div className="flex justify-between items-start mb-4">
                        <div className="flex-1">
                          <div className="flex items-center gap-2 mb-2">
                            <h3 className="font-medium">
                              {ride.driver?.first_name} {ride.driver?.last_name}
                            </h3>
                            <Badge className="bg-orange-100 text-orange-800">
                              Match Found
                            </Badge>
                          </div>
                          <div className="flex items-center gap-2 mb-2">
                            <MapPin className="h-4 w-4 text-orange-600" />
                            <span className="font-medium">{ride.start_point}</span>
                            <span className="text-gray-400">→</span>
                            <span className="font-medium">{ride.end_point}</span>
                          </div>
                          <div className="flex items-center gap-4 text-sm text-gray-600">
                            <div className="flex items-center gap-1">
                              <Clock className="h-4 w-4" />
                              {formatDateTime(ride.departure_time)}
                            </div>
                            <div className="flex items-center gap-1">
                              <Users className="h-4 w-4" />
                              {ride.available_seats} seats
                            </div>
                            {ride.price_per_seat && (
                              <div className="flex items-center gap-1">
                                <DollarSign className="h-4 w-4" />
                                ${ride.price_per_seat}/seat
                              </div>
                            )}
                          </div>
                        </div>
                        <Button
                          onClick={() => openApplicationDialog(ride)}
                          className="bg-orange-600 hover:bg-orange-700"
                        >
                          <Send className="h-4 w-4 mr-2" />
                          Apply
                        </Button>
                      </div>
                    </CardContent>
                  </Card>
                ))}
              </div>
            )}
          </TabsContent>
        </Tabs>

        {/* Application Dialog */}
        <Dialog open={showApplicationDialog} onOpenChange={setShowApplicationDialog}>
          <DialogContent className="max-w-md">
            <DialogHeader>
              <DialogTitle>Apply for Ride</DialogTitle>
              <DialogDescription>
                Send an application to join this ride
              </DialogDescription>
            </DialogHeader>
            {selectedRide && (
              <div className="space-y-4">
                <div className="bg-gray-50 p-4 rounded-lg">
                  <div className="flex items-center gap-2 mb-2">
                    <MapPin className="h-4 w-4 text-blue-600" />
                    <span className="font-medium">{selectedRide.start_point}</span>
                    <span className="text-gray-400">→</span>
                    <span className="font-medium">{selectedRide.end_point}</span>
                  </div>
                  <div className="text-sm text-gray-600">
                    Driver: {selectedRide.driver?.first_name} {selectedRide.driver?.last_name}
                  </div>
                  <div className="text-sm text-gray-600">
                    Departure: {formatDateTime(selectedRide.departure_time)}
                  </div>
                </div>
                
                <div className="space-y-2">
                  <Label htmlFor="seats_requested">Seats Needed</Label>
                  <Input
                    id="seats_requested"
                    type="number"
                    min="1"
                    max={selectedRide.available_seats}
                    value={applicationData.seats_requested}
                    onChange={(e) => setApplicationData({ ...applicationData, seats_requested: parseInt(e.target.value) })}
                  />
                </div>
                
                <div className="space-y-2">
                  <Label htmlFor="message">Message (Optional)</Label>
                  <Textarea
                    id="message"
                    value={applicationData.message}
                    onChange={(e) => setApplicationData({ ...applicationData, message: e.target.value })}
                    placeholder="Tell the driver why you'd like to join this ride..."
                    rows={3}
                  />
                </div>
                
                <Button onClick={handleApplyForRide} className="w-full">
                  Send Application
                </Button>
              </div>
            )}
          </DialogContent>
        </Dialog>
      </div>
    </div>
  );
}
```

## File: hooks/use-toast.ts
```typescript
'use client';

// Inspired by react-hot-toast library
import * as React from 'react';

import type { ToastActionElement, ToastProps } from '@/components/ui/toast';

const TOAST_LIMIT = 1;
const TOAST_REMOVE_DELAY = 1000000;

type ToasterToast = ToastProps & {
  id: string;
  title?: React.ReactNode;
  description?: React.ReactNode;
  action?: ToastActionElement;
};

const actionTypes = {
  ADD_TOAST: 'ADD_TOAST',
  UPDATE_TOAST: 'UPDATE_TOAST',
  DISMISS_TOAST: 'DISMISS_TOAST',
  REMOVE_TOAST: 'REMOVE_TOAST',
} as const;

let count = 0;

function genId() {
  count = (count + 1) % Number.MAX_SAFE_INTEGER;
  return count.toString();
}

type ActionType = typeof actionTypes;

type Action =
  | {
      type: ActionType['ADD_TOAST'];
      toast: ToasterToast;
    }
  | {
      type: ActionType['UPDATE_TOAST'];
      toast: Partial<ToasterToast>;
    }
  | {
      type: ActionType['DISMISS_TOAST'];
      toastId?: ToasterToast['id'];
    }
  | {
      type: ActionType['REMOVE_TOAST'];
      toastId?: ToasterToast['id'];
    };

interface State {
  toasts: ToasterToast[];
}

const toastTimeouts = new Map<string, ReturnType<typeof setTimeout>>();

const addToRemoveQueue = (toastId: string) => {
  if (toastTimeouts.has(toastId)) {
    return;
  }

  const timeout = setTimeout(() => {
    toastTimeouts.delete(toastId);
    dispatch({
      type: 'REMOVE_TOAST',
      toastId: toastId,
    });
  }, TOAST_REMOVE_DELAY);

  toastTimeouts.set(toastId, timeout);
};

export const reducer = (state: State, action: Action): State => {
  switch (action.type) {
    case 'ADD_TOAST':
      return {
        ...state,
        toasts: [action.toast, ...state.toasts].slice(0, TOAST_LIMIT),
      };

    case 'UPDATE_TOAST':
      return {
        ...state,
        toasts: state.toasts.map((t) =>
          t.id === action.toast.id ? { ...t, ...action.toast } : t
        ),
      };

    case 'DISMISS_TOAST': {
      const { toastId } = action;

      // ! Side effects ! - This could be extracted into a dismissToast() action,
      // but I'll keep it here for simplicity
      if (toastId) {
        addToRemoveQueue(toastId);
      } else {
        state.toasts.forEach((toast) => {
          addToRemoveQueue(toast.id);
        });
      }

      return {
        ...state,
        toasts: state.toasts.map((t) =>
          t.id === toastId || toastId === undefined
            ? {
                ...t,
                open: false,
              }
            : t
        ),
      };
    }
    case 'REMOVE_TOAST':
      if (action.toastId === undefined) {
        return {
          ...state,
          toasts: [],
        };
      }
      return {
        ...state,
        toasts: state.toasts.filter((t) => t.id !== action.toastId),
      };
  }
};

const listeners: Array<(state: State) => void> = [];

let memoryState: State = { toasts: [] };

function dispatch(action: Action) {
  memoryState = reducer(memoryState, action);
  listeners.forEach((listener) => {
    listener(memoryState);
  });
}

type Toast = Omit<ToasterToast, 'id'>;

function toast({ ...props }: Toast) {
  const id = genId();

  const update = (props: ToasterToast) =>
    dispatch({
      type: 'UPDATE_TOAST',
      toast: { ...props, id },
    });
  const dismiss = () => dispatch({ type: 'DISMISS_TOAST', toastId: id });

  dispatch({
    type: 'ADD_TOAST',
    toast: {
      ...props,
      id,
      open: true,
      onOpenChange: (open) => {
        if (!open) dismiss();
      },
    },
  });

  return {
    id: id,
    dismiss,
    update,
  };
}

function useToast() {
  const [state, setState] = React.useState<State>(memoryState);

  React.useEffect(() => {
    listeners.push(setState);
    return () => {
      const index = listeners.indexOf(setState);
      if (index > -1) {
        listeners.splice(index, 1);
      }
    };
  }, [state]);

  return {
    ...state,
    toast,
    dismiss: (toastId?: string) => dispatch({ type: 'DISMISS_TOAST', toastId }),
  };
}

export { useToast, toast };
```

## File: lib/auth.ts
```typescript
import { supabase } from './supabase';
import type { UserProfile } from './supabase';

export const signUp = async (email: string, password: string, userData: Omit<UserProfile, 'id' | 'created_at' | 'updated_at'>) => {
  const { data, error } = await supabase.auth.signUp({
    email,
    password,
  });

  if (error) throw error;

  if (data.user) {
    const { error: profileError } = await supabase
      .from('user_profiles')
      .insert([{
        id: data.user.id,
        ...userData,
      }]);

    if (profileError) throw profileError;
  }

  return data;
};

export const signIn = async (email: string, password: string) => {
  const { data, error } = await supabase.auth.signInWithPassword({
    email,
    password,
  });

  if (error) throw error;
  return data;
};

export const signOut = async () => {
  const { error } = await supabase.auth.signOut();
  if (error) throw error;
};

export const getCurrentUser = async () => {
  const { data: { user } } = await supabase.auth.getUser();
  return user;
};

export const getUserProfile = async (userId: string): Promise<UserProfile | null> => {
  const { data, error } = await supabase
    .from('user_profiles')
    .select('*')
    .eq('id', userId)
    .single();

  if (error) return null;
  return data;
};
```

## File: lib/rides.ts
```typescript
import { supabase } from './supabase';
import type { Ride, RideRequest, RideApplication, RideMatch } from './supabase';

// Ride management
export const createRide = async (rideData: Omit<Ride, 'id' | 'created_at' | 'updated_at'>) => {
  const { data, error } = await supabase
    .from('rides')
    .insert([rideData])
    .select()
    .single();

  if (error) throw error;
  return data;
};

export const getRidesByDriver = async (driverId: string) => {
  const { data, error } = await supabase
    .from('rides')
    .select(`
      *,
      driver:user_profiles(*)
    `)
    .eq('driver_id', driverId)
    .order('departure_time', { ascending: true });

  if (error) throw error;
  return data;
};

export const getActiveRides = async () => {
  const { data, error } = await supabase
    .from('rides')
    .select(`
      *,
      driver:user_profiles(*)
    `)
    .eq('status', 'active')
    .gte('departure_time', new Date().toISOString())
    .order('departure_time', { ascending: true });

  if (error) throw error;
  return data;
};

// Ride request management
export const createRideRequest = async (requestData: Omit<RideRequest, 'id' | 'created_at' | 'updated_at'>) => {
  const { data, error } = await supabase
    .from('ride_requests')
    .insert([requestData])
    .select()
    .single();

  if (error) throw error;
  return data;
};

export const getRideRequestsByPassenger = async (passengerId: string) => {
  const { data, error } = await supabase
    .from('ride_requests')
    .select(`
      *,
      passenger:user_profiles(*)
    `)
    .eq('passenger_id', passengerId)
    .order('departure_time', { ascending: true });

  if (error) throw error;
  return data;
};

export const getActiveRideRequests = async () => {
  const { data, error } = await supabase
    .from('ride_requests')
    .select(`
      *,
      passenger:user_profiles(*)
    `)
    .eq('status', 'active')
    .gte('departure_time', new Date().toISOString())
    .order('departure_time', { ascending: true });

  if (error) throw error;
  return data;
};

// Application management
export const applyForRide = async (applicationData: Omit<RideApplication, 'id' | 'created_at' | 'updated_at'>) => {
  const { data, error } = await supabase
    .from('ride_applications')
    .insert([applicationData])
    .select()
    .single();

  if (error) throw error;
  return data;
};

export const getApplicationsForRide = async (rideId: string) => {
  const { data, error } = await supabase
    .from('ride_applications')
    .select(`
      *,
      passenger:user_profiles(*),
      ride:rides(*)
    `)
    .eq('ride_id', rideId)
    .order('created_at', { ascending: false });

  if (error) throw error;
  return data;
};

export const getApplicationsByPassenger = async (passengerId: string) => {
  const { data, error } = await supabase
    .from('ride_applications')
    .select(`
      *,
      passenger:user_profiles(*),
      ride:rides(*, driver:user_profiles(*))
    `)
    .eq('passenger_id', passengerId)
    .order('created_at', { ascending: false });

  if (error) throw error;
  return data;
};

export const updateApplicationStatus = async (applicationId: string, status: 'approved' | 'rejected') => {
  const { data, error } = await supabase
    .from('ride_applications')
    .update({ status })
    .eq('id', applicationId)
    .select()
    .single();

  if (error) throw error;
  return data;
};

// Matching logic
export const findMatchingRides = async (rideRequest: RideRequest): Promise<Ride[]> => {
  const { data, error } = await supabase
    .from('rides')
    .select(`
      *,
      driver:user_profiles(*)
    `)
    .eq('status', 'active')
    .gte('departure_time', new Date().toISOString());

  if (error) throw error;

  // Filter rides that match the request
  return data.filter(ride => {
    const ridePoints = [ride.start_point, ride.end_point, ...ride.stops];
    const requestPoints = [rideRequest.start_point, rideRequest.end_point];
    
    // Check if any ride point matches any request point (case-insensitive)
    return ridePoints.some(ridePoint => 
      requestPoints.some(requestPoint => 
        ridePoint.toLowerCase().includes(requestPoint.toLowerCase()) ||
        requestPoint.toLowerCase().includes(ridePoint.toLowerCase())
      )
    );
  });
};

export const findMatchingRequests = async (ride: Ride): Promise<RideRequest[]> => {
  const { data, error } = await supabase
    .from('ride_requests')
    .select(`
      *,
      passenger:user_profiles(*)
    `)
    .eq('status', 'active')
    .gte('departure_time', new Date().toISOString());

  if (error) throw error;

  // Filter requests that match the ride
  return data.filter(request => {
    const ridePoints = [ride.start_point, ride.end_point, ...ride.stops];
    const requestPoints = [request.start_point, request.end_point];
    
    // Check if any ride point matches any request point (case-insensitive)
    return ridePoints.some(ridePoint => 
      requestPoints.some(requestPoint => 
        ridePoint.toLowerCase().includes(requestPoint.toLowerCase()) ||
        requestPoint.toLowerCase().includes(ridePoint.toLowerCase())
      )
    );
  });
};
```

## File: lib/supabase.ts
```typescript
import { createClient } from '@supabase/supabase-js';

const supabaseUrl = process.env.NEXT_PUBLIC_SUPABASE_URL!;
const supabaseKey = process.env.NEXT_PUBLIC_SUPABASE_ANON_KEY!;

export const supabase = createClient(supabaseUrl, supabaseKey);

export type UserProfile = {
  id: string;
  role: 'driver' | 'passenger';
  first_name: string;
  last_name: string;
  phone?: string;
  created_at: string;
  updated_at: string;
};

export type Ride = {
  id: string;
  driver_id: string;
  start_point: string;
  end_point: string;
  stops: string[];
  departure_time: string;
  available_seats: number;
  price_per_seat?: number;
  status: 'active' | 'completed' | 'cancelled';
  created_at: string;
  updated_at: string;
  driver?: UserProfile;
};

export type RideRequest = {
  id: string;
  passenger_id: string;
  start_point: string;
  end_point: string;
  departure_time: string;
  max_price?: number;
  status: 'active' | 'matched' | 'completed' | 'cancelled';
  created_at: string;
  updated_at: string;
  passenger?: UserProfile;
};

export type RideApplication = {
  id: string;
  ride_id: string;
  passenger_id: string;
  status: 'pending' | 'approved' | 'rejected';
  seats_requested: number;
  message?: string;
  created_at: string;
  updated_at: string;
  passenger?: UserProfile;
  ride?: Ride;
};

export type RideMatch = {
  id: string;
  ride_id: string;
  ride_request_id: string;
  match_type: 'exact' | 'partial';
  created_at: string;
  ride?: Ride;
  ride_request?: RideRequest;
};
```

## File: lib/utils.ts
```typescript
import { clsx, type ClassValue } from 'clsx';
import { twMerge } from 'tailwind-merge';

export function cn(...inputs: ClassValue[]) {
  return twMerge(clsx(inputs));
}
```

## File: package.json
```json
{
  "name": "rideshare-app",
  "version": "0.1.0",
  "private": true,
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "next lint"
  },
  "dependencies": {
    "@hookform/resolvers": "^3.9.0",
    "@next/swc-wasm-nodejs": "13.5.1",
    "@radix-ui/react-accordion": "^1.2.0",
    "@radix-ui/react-alert-dialog": "^1.1.1",
    "@radix-ui/react-aspect-ratio": "^1.1.0",
    "@radix-ui/react-avatar": "^1.1.0",
    "@radix-ui/react-checkbox": "^1.1.1",
    "@radix-ui/react-collapsible": "^1.1.0",
    "@radix-ui/react-context-menu": "^2.2.1",
    "@radix-ui/react-dialog": "^1.1.1",
    "@radix-ui/react-dropdown-menu": "^2.1.1",
    "@radix-ui/react-hover-card": "^1.1.1",
    "@radix-ui/react-label": "^2.1.0",
    "@radix-ui/react-menubar": "^1.1.1",
    "@radix-ui/react-navigation-menu": "^1.2.0",
    "@radix-ui/react-popover": "^1.1.1",
    "@radix-ui/react-progress": "^1.1.0",
    "@radix-ui/react-radio-group": "^1.2.0",
    "@radix-ui/react-scroll-area": "^1.1.0",
    "@radix-ui/react-select": "^2.1.1",
    "@radix-ui/react-separator": "^1.1.0",
    "@radix-ui/react-slider": "^1.2.0",
    "@radix-ui/react-slot": "^1.1.0",
    "@radix-ui/react-switch": "^1.1.0",
    "@radix-ui/react-tabs": "^1.1.0",
    "@radix-ui/react-toast": "^1.2.1",
    "@radix-ui/react-toggle": "^1.1.0",
    "@radix-ui/react-toggle-group": "^1.1.0",
    "@radix-ui/react-tooltip": "^1.1.2",
    "@supabase/supabase-js": "^2.45.4",
    "@types/node": "20.6.2",
    "@types/react": "18.2.22",
    "@types/react-dom": "18.2.7",
    "autoprefixer": "10.4.15",
    "class-variance-authority": "^0.7.0",
    "clsx": "^2.1.1",
    "cmdk": "^1.0.0",
    "date-fns": "^3.6.0",
    "embla-carousel-react": "^8.3.0",
    "eslint": "8.49.0",
    "eslint-config-next": "13.5.1",
    "input-otp": "^1.2.4",
    "lucide-react": "^0.446.0",
    "next": "13.5.1",
    "next-themes": "^0.3.0",
    "postcss": "8.4.30",
    "react": "18.2.0",
    "react-day-picker": "^8.10.1",
    "react-dom": "18.2.0",
    "react-hook-form": "^7.53.0",
    "react-resizable-panels": "^2.1.3",
    "recharts": "^2.12.7",
    "sonner": "^1.5.0",
    "tailwind-merge": "^2.5.2",
    "tailwindcss": "3.3.3",
    "tailwindcss-animate": "^1.0.7",
    "typescript": "5.2.2",
    "vaul": "^0.9.9",
    "zod": "^3.23.8"
  }
}
```

## File: repomix.config.json
```json
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
```

## File: supabase/migrations/20250630031142_velvet_block.sql
```sql
/*
  # Ride Share Application Database Schema

  1. New Tables
    - `user_profiles`
      - `id` (uuid, references auth.users)
      - `role` (text, either 'driver' or 'passenger')
      - `first_name` (text)
      - `last_name` (text)
      - `phone` (text)
      - `created_at` (timestamp)
      - `updated_at` (timestamp)

    - `rides`
      - `id` (uuid, primary key)
      - `driver_id` (uuid, references user_profiles)
      - `start_point` (text)
      - `end_point` (text)
      - `stops` (text array, optional intermediate stops)
      - `departure_time` (timestamp)
      - `available_seats` (integer)
      - `price_per_seat` (decimal)
      - `status` (text, 'active', 'completed', 'cancelled')
      - `created_at` (timestamp)
      - `updated_at` (timestamp)

    - `ride_requests`
      - `id` (uuid, primary key)
      - `passenger_id` (uuid, references user_profiles)
      - `start_point` (text)
      - `end_point` (text)
      - `departure_time` (timestamp)
      - `max_price` (decimal)
      - `status` (text, 'active', 'matched', 'completed', 'cancelled')
      - `created_at` (timestamp)
      - `updated_at` (timestamp)

    - `ride_applications`
      - `id` (uuid, primary key)
      - `ride_id` (uuid, references rides)
      - `passenger_id` (uuid, references user_profiles)
      - `status` (text, 'pending', 'approved', 'rejected')
      - `seats_requested` (integer)
      - `message` (text)
      - `created_at` (timestamp)
      - `updated_at` (timestamp)

    - `ride_matches`
      - `id` (uuid, primary key)
      - `ride_id` (uuid, references rides)
      - `ride_request_id` (uuid, references ride_requests)
      - `match_type` (text, 'exact', 'partial')
      - `created_at` (timestamp)

  2. Security
    - Enable RLS on all tables
    - Add policies for authenticated users to access their own data
    - Drivers can only modify their own rides
    - Passengers can only modify their own requests
    - Public read access for matching logic

  3. Indexes
    - Performance indexes on location and time fields for matching
*/

-- Create user_profiles table
CREATE TABLE IF NOT EXISTS user_profiles (
  id uuid PRIMARY KEY REFERENCES auth.users(id) ON DELETE CASCADE,
  role text NOT NULL CHECK (role IN ('driver', 'passenger')),
  first_name text NOT NULL,
  last_name text NOT NULL,
  phone text,
  created_at timestamptz DEFAULT now(),
  updated_at timestamptz DEFAULT now()
);

-- Create rides table
CREATE TABLE IF NOT EXISTS rides (
  id uuid PRIMARY KEY DEFAULT gen_random_uuid(),
  driver_id uuid NOT NULL REFERENCES user_profiles(id) ON DELETE CASCADE,
  start_point text NOT NULL,
  end_point text NOT NULL,
  stops text[] DEFAULT '{}',
  departure_time timestamptz NOT NULL,
  available_seats integer NOT NULL DEFAULT 1,
  price_per_seat decimal(10,2),
  status text NOT NULL DEFAULT 'active' CHECK (status IN ('active', 'completed', 'cancelled')),
  created_at timestamptz DEFAULT now(),
  updated_at timestamptz DEFAULT now()
);

-- Create ride_requests table
CREATE TABLE IF NOT EXISTS ride_requests (
  id uuid PRIMARY KEY DEFAULT gen_random_uuid(),
  passenger_id uuid NOT NULL REFERENCES user_profiles(id) ON DELETE CASCADE,
  start_point text NOT NULL,
  end_point text NOT NULL,
  departure_time timestamptz NOT NULL,
  max_price decimal(10,2),
  status text NOT NULL DEFAULT 'active' CHECK (status IN ('active', 'matched', 'completed', 'cancelled')),
  created_at timestamptz DEFAULT now(),
  updated_at timestamptz DEFAULT now()
);

-- Create ride_applications table
CREATE TABLE IF NOT EXISTS ride_applications (
  id uuid PRIMARY KEY DEFAULT gen_random_uuid(),
  ride_id uuid NOT NULL REFERENCES rides(id) ON DELETE CASCADE,
  passenger_id uuid NOT NULL REFERENCES user_profiles(id) ON DELETE CASCADE,
  status text NOT NULL DEFAULT 'pending' CHECK (status IN ('pending', 'approved', 'rejected')),
  seats_requested integer NOT NULL DEFAULT 1,
  message text,
  created_at timestamptz DEFAULT now(),
  updated_at timestamptz DEFAULT now(),
  UNIQUE(ride_id, passenger_id)
);

-- Create ride_matches table
CREATE TABLE IF NOT EXISTS ride_matches (
  id uuid PRIMARY KEY DEFAULT gen_random_uuid(),
  ride_id uuid NOT NULL REFERENCES rides(id) ON DELETE CASCADE,
  ride_request_id uuid NOT NULL REFERENCES ride_requests(id) ON DELETE CASCADE,
  match_type text NOT NULL CHECK (match_type IN ('exact', 'partial')),
  created_at timestamptz DEFAULT now(),
  UNIQUE(ride_id, ride_request_id)
);

-- Enable Row Level Security
ALTER TABLE user_profiles ENABLE ROW LEVEL SECURITY;
ALTER TABLE rides ENABLE ROW LEVEL SECURITY;
ALTER TABLE ride_requests ENABLE ROW LEVEL SECURITY;
ALTER TABLE ride_applications ENABLE ROW LEVEL SECURITY;
ALTER TABLE ride_matches ENABLE ROW LEVEL SECURITY;

-- User profiles policies
CREATE POLICY "Users can read all profiles" ON user_profiles FOR SELECT TO authenticated USING (true);
CREATE POLICY "Users can update own profile" ON user_profiles FOR UPDATE TO authenticated USING (auth.uid() = id);
CREATE POLICY "Users can insert own profile" ON user_profiles FOR INSERT TO authenticated WITH CHECK (auth.uid() = id);

-- Rides policies
CREATE POLICY "Anyone can view active rides" ON rides FOR SELECT TO authenticated USING (status = 'active');
CREATE POLICY "Drivers can manage own rides" ON rides FOR ALL TO authenticated USING (driver_id = auth.uid());

-- Ride requests policies
CREATE POLICY "Anyone can view active ride requests" ON ride_requests FOR SELECT TO authenticated USING (status = 'active');
CREATE POLICY "Passengers can manage own requests" ON ride_requests FOR ALL TO authenticated USING (passenger_id = auth.uid());

-- Ride applications policies
CREATE POLICY "Drivers can view applications for their rides" ON ride_applications FOR SELECT TO authenticated 
  USING (EXISTS (SELECT 1 FROM rides WHERE rides.id = ride_applications.ride_id AND rides.driver_id = auth.uid()));
CREATE POLICY "Passengers can view own applications" ON ride_applications FOR SELECT TO authenticated 
  USING (passenger_id = auth.uid());
CREATE POLICY "Passengers can create applications" ON ride_applications FOR INSERT TO authenticated 
  WITH CHECK (passenger_id = auth.uid());
CREATE POLICY "Drivers can update applications for their rides" ON ride_applications FOR UPDATE TO authenticated 
  USING (EXISTS (SELECT 1 FROM rides WHERE rides.id = ride_applications.ride_id AND rides.driver_id = auth.uid()));

-- Ride matches policies
CREATE POLICY "Users can view relevant matches" ON ride_matches FOR SELECT TO authenticated USING (
  EXISTS (SELECT 1 FROM rides WHERE rides.id = ride_matches.ride_id AND rides.driver_id = auth.uid()) OR
  EXISTS (SELECT 1 FROM ride_requests WHERE ride_requests.id = ride_matches.ride_request_id AND ride_requests.passenger_id = auth.uid())
);

-- Create indexes for performance
CREATE INDEX IF NOT EXISTS idx_rides_departure_time ON rides(departure_time);
CREATE INDEX IF NOT EXISTS idx_rides_start_point ON rides(start_point);
CREATE INDEX IF NOT EXISTS idx_rides_end_point ON rides(end_point);
CREATE INDEX IF NOT EXISTS idx_rides_status ON rides(status);
CREATE INDEX IF NOT EXISTS idx_ride_requests_departure_time ON ride_requests(departure_time);
CREATE INDEX IF NOT EXISTS idx_ride_requests_start_point ON ride_requests(start_point);
CREATE INDEX IF NOT EXISTS idx_ride_requests_end_point ON ride_requests(end_point);
CREATE INDEX IF NOT EXISTS idx_ride_requests_status ON ride_requests(status);

-- Create function to update updated_at timestamp
CREATE OR REPLACE FUNCTION update_updated_at_column()
RETURNS TRIGGER AS $$
BEGIN
  NEW.updated_at = now();
  RETURN NEW;
END;
$$ language 'plpgsql';

-- Create triggers for updated_at
CREATE TRIGGER update_user_profiles_updated_at BEFORE UPDATE ON user_profiles FOR EACH ROW EXECUTE FUNCTION update_updated_at_column();
CREATE TRIGGER update_rides_updated_at BEFORE UPDATE ON rides FOR EACH ROW EXECUTE FUNCTION update_updated_at_column();
CREATE TRIGGER update_ride_requests_updated_at BEFORE UPDATE ON ride_requests FOR EACH ROW EXECUTE FUNCTION update_updated_at_column();
CREATE TRIGGER update_ride_applications_updated_at BEFORE UPDATE ON ride_applications FOR EACH ROW EXECUTE FUNCTION update_updated_at_column();
```
