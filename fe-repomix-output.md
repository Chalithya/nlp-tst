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
components.json
eslint.config.mjs
next.config.ts
package.json
postcss.config.mjs
repomix.config.json
src/app/api/career/search/route.ts
src/app/api/resume/analyses/route.ts
src/app/api/resume/pdf-download/route.ts
src/app/auth/page.tsx
src/app/dashboard/career/page.tsx
src/app/dashboard/history/page.tsx
src/app/dashboard/layout.tsx
src/app/dashboard/page.tsx
src/app/dashboard/profile/page.tsx
src/app/dashboard/profile/settings/page.tsx
src/app/dashboard/resume/generator/edit/[resumeId]/page.tsx
src/app/dashboard/resume/generator/page.tsx
src/app/dashboard/resume/generator/processing/page.tsx
src/app/dashboard/resume/page.tsx
src/app/error.tsx
src/app/layout.tsx
src/app/loading.tsx
src/app/page.tsx
src/components/common/__tests__/LoadingSpinner.test.tsx
src/components/common/Breadcrumbs.tsx
src/components/common/ErrorBoundary.tsx
src/components/common/Footer.tsx
src/components/common/Header.tsx
src/components/common/index.ts
src/components/common/LoadingSpinner.tsx
src/components/common/Logo.tsx
src/components/common/Navigation.tsx
src/components/common/Sidebar.tsx
src/components/common/ThemeSwitcher.tsx
src/components/common/UserProfile.tsx
src/components/features/auth/AuthDebug.tsx
src/components/features/auth/index.ts
src/components/features/auth/LoginForm.tsx
src/components/features/auth/RegisterForm.tsx
src/components/features/career/index.ts
src/components/features/career/JobSearchModal.tsx
src/components/features/resume/FeaturesPanel.tsx
src/components/features/resume/generator/EditableField.tsx
src/components/features/resume/generator/EditableSection.tsx
src/components/features/resume/generator/GenerationProgress.tsx
src/components/features/resume/generator/InteractiveResumeEditor.tsx
src/components/features/resume/generator/JobTargeting.tsx
src/components/features/resume/generator/ResumePDFView.tsx
src/components/features/resume/generator/ResumeSelector.tsx
src/components/features/resume/generator/SuggestionPanel.tsx
src/components/features/resume/index.ts
src/components/features/resume/ResumeAnalysisDetail.tsx
src/components/features/resume/ResumeAnalysisList.tsx
src/components/features/resume/ResumeUpload.tsx
src/components/features/resume/templates/CanadianPDFTemplate.tsx
src/components/forms/BaseForm.tsx
src/components/forms/FormError.tsx
src/components/forms/FormField.tsx
src/components/forms/FormSubmitButton.tsx
src/components/forms/index.ts
src/components/forms/validation/auth.ts
src/components/forms/validation/career.ts
src/components/forms/validation/resume.ts
src/components/forms/validation/user.ts
src/components/index.ts
src/components/providers/api-provider.tsx
src/components/providers/auth-provider.tsx
src/components/providers/index.ts
src/components/providers/theme-provider.tsx
src/components/providers/toast-provider.tsx
src/components/ui/alert.tsx
src/components/ui/avatar.tsx
src/components/ui/badge.tsx
src/components/ui/button.tsx
src/components/ui/calendar.tsx
src/components/ui/card.tsx
src/components/ui/chart.tsx
src/components/ui/checkbox.tsx
src/components/ui/dialog.tsx
src/components/ui/dropdown-menu.tsx
src/components/ui/form.tsx
src/components/ui/index.ts
src/components/ui/input.tsx
src/components/ui/label.tsx
src/components/ui/popover.tsx
src/components/ui/progress.tsx
src/components/ui/radio-group.tsx
src/components/ui/scroll-area.tsx
src/components/ui/select.tsx
src/components/ui/skeleton.tsx
src/components/ui/table.tsx
src/components/ui/tabs.tsx
src/components/ui/textarea.tsx
src/components/ui/toast.tsx
src/components/ui/toaster.tsx
src/hooks/index.ts
src/hooks/use-toast.ts
src/hooks/useApi.ts
src/hooks/useAuth.ts
src/hooks/useForm.ts
src/hooks/useLocalStorage.ts
src/hooks/useResumeAnalysis.ts
src/hooks/useToast.ts
src/lib/api.ts
src/lib/api/resumeGenerator.ts
src/lib/auth.ts
src/lib/config.ts
src/lib/config/constants.ts
src/lib/config/environment.ts
src/lib/config/features.ts
src/lib/config/index.ts
src/lib/index.ts
src/lib/pdfGenerator.ts
src/lib/utils.ts
src/middleware.ts
src/stores/authStore.ts
src/stores/index.ts
src/stores/resumeGeneratorStore.ts
src/stores/types.ts
src/stores/userStore.ts
src/styles/globals.css
src/types/api.ts
src/types/auth.ts
src/types/components.ts
src/types/index.ts
src/types/resume-generator.ts
tailwind.config.ts
tsconfig.json
```

# Files

## File: .gitignore
```
# See https://help.github.com/articles/ignoring-files/ for more about ignoring files.

# dependencies
/node_modules
/.pnp
.pnp.*
.yarn/*
!.yarn/patches
!.yarn/plugins
!.yarn/releases
!.yarn/versions

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
.pnpm-debug.log*

# env files (can opt-in for committing if needed)
.env*

# vercel
.vercel

# typescript
*.tsbuildinfo
next-env.d.ts
```

## File: .repomixignore
```
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
```

## File: components.json
```json
{
  "$schema": "https://ui.shadcn.com/schema.json",
  "style": "new-york",
  "rsc": true,
  "tsx": true,
  "tailwind": {
    "config": "tailwind.config.ts",
    "css": "src/app/globals.css",
    "baseColor": "zinc",
    "cssVariables": true,
    "prefix": ""
  },
  "aliases": {
    "components": "@/components",
    "utils": "@/lib/utils",
    "ui": "@/components/ui",
    "lib": "@/lib",
    "hooks": "@/hooks"
  },
  "iconLibrary": "lucide"
}
```

## File: eslint.config.mjs
```
import { dirname } from "path";
import { fileURLToPath } from "url";
import { FlatCompat } from "@eslint/eslintrc";

const __filename = fileURLToPath(import.meta.url);
const __dirname = dirname(__filename);

const compat = new FlatCompat({
  baseDirectory: __dirname,
});

const eslintConfig = [
  ...compat.extends("next/core-web-vitals", "next/typescript"),
];

export default eslintConfig;
```

## File: next.config.ts
```typescript
import type { NextConfig } from "next";

const nextConfig: NextConfig = {
  reactStrictMode: true,
  env: {
    BASE_URL: process.env.BASE_URL, 
  },
};

export default nextConfig;
```

## File: package.json
```json
{
  "name": "ImmiGrow-frontend",
  "version": "0.1.0",
  "private": true,
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "next lint"
  },
  "dependencies": {
    "@hookform/resolvers": "^3.10.0",
    "@next/env": "^15.2.0",
    "@radix-ui/react-avatar": "^1.1.10",
    "@radix-ui/react-checkbox": "^1.1.3",
    "@radix-ui/react-dialog": "^1.1.6",
    "@radix-ui/react-dropdown-menu": "^2.1.6",
    "@radix-ui/react-label": "^2.1.2",
    "@radix-ui/react-popover": "^1.1.6",
    "@radix-ui/react-progress": "^1.1.7",
    "@radix-ui/react-radio-group": "^1.2.3",
    "@radix-ui/react-scroll-area": "^1.2.3",
    "@radix-ui/react-select": "^2.1.6",
    "@radix-ui/react-slot": "^1.1.2",
    "@radix-ui/react-tabs": "^1.1.2",
    "@radix-ui/react-toast": "^1.2.5",
    "@shadcn/ui": "^0.0.4",
    "@supabase/supabase-js": "^2.55.0",
    "@tanstack/react-query": "^5.68.0",
    "@tanstack/react-table": "^8.21.2",
    "@types/puppeteer": "^5.4.7",
    "@wojtekmaj/react-hooks": "^1.22.0",
    "axios": "^1.11.0",
    "class-variance-authority": "^0.7.1",
    "clsx": "^2.1.1",
    "date-fns": "^3.6.0",
    "html-pdf-node": "^1.0.7",
    "js-cookie": "^3.0.5",
    "jsdom": "^26.1.0",
    "lucide-react": "^0.474.0",
    "next": "^15.3.4",
    "next-themes": "^0.4.4",
    "puppeteer": "^24.17.1",
    "react": "^19.0.0",
    "react-day-picker": "^9.5.1",
    "react-dom": "^19.0.0",
    "react-dropzone": "^14.3.8",
    "react-hook-form": "^7.54.2",
    "react-icons": "^5.4.0",
    "recharts": "^2.15.1",
    "slick-carousel": "^1.8.1",
    "tailwind-merge": "^2.6.0",
    "tailwindcss-animate": "^1.0.7",
    "zod": "^3.25.76",
    "zustand": "^5.0.8"
  },
  "devDependencies": {
    "@eslint/eslintrc": "^3",
    "@types/js-cookie": "^3.0.6",
    "@types/node": "^20",
    "@types/react": "^19",
    "@types/react-dom": "^19",
    "eslint": "^9",
    "eslint-config-next": "15.1.6",
    "postcss": "^8",
    "tailwindcss": "^3.4.1",
    "typescript": "^5"
  },
  "overrides": {
    "react-is": "^19.0.0-rc-69d4b800-20241021"
  }
}
```

## File: postcss.config.mjs
```
/** @type {import('postcss-load-config').Config} */
const config = {
  plugins: {
    tailwindcss: {},
  },
};

export default config;
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

## File: src/app/api/career/search/route.ts
```typescript
import { NextRequest, NextResponse } from 'next/server';

const BACKEND_URL = (process.env.NEXT_PUBLIC_API_URL || 'http://localhost:5500').replace(/\/$/, '');

export async function POST(request: NextRequest) {
  try {
    // Get the authorization header from the incoming request
    const authHeader = request.headers.get('authorization');
    
    console.log('🔐 Job Search API Proxy - Authorization header:', authHeader ? 'Present' : 'Missing');
    console.log('🔗 Job Search API Proxy - Backend URL:', `${BACKEND_URL}/api/protected/career/search-jobs`);
    
    if (!authHeader) {
      console.log('❌ Job Search API Proxy - No authorization header');
      return NextResponse.json(
        { success: false, message: 'Authorization header required' },
        { status: 401 }
      );
    }

    // Get the request body
    const body = await request.json();
    console.log('📤 Job Search API Proxy - Request body:', body);

    // Forward the request to the backend
    console.log('📤 Job Search API Proxy - Forwarding request to backend...');
    const response = await fetch(`${BACKEND_URL}/api/protected/career/search-jobs`, {
      method: 'POST',
      headers: {
        'Authorization': authHeader,
        'Content-Type': 'application/json',
      },
      body: JSON.stringify(body),
    });

    console.log('📥 Job Search API Proxy - Backend response status:', response.status);
    
    const data = await response.json();
    console.log('📥 Job Search API Proxy - Backend response data preview:', {
      success: data.success,
      jobCount: data.data?.jobs?.length || 0,
      totalCount: data.data?.totalCount || 0,
      error: data.error
    });

    return NextResponse.json(data, { status: response.status });
  } catch (error) {
    console.error('❌ Job Search API Proxy - Error:', error);
    return NextResponse.json(
      { 
        success: false, 
        message: 'Failed to search for jobs', 
        error: error.message,
        fallbackMessage: 'Job search temporarily unavailable. Please try searching directly on job sites like Indeed.ca, LinkedIn, or Workopolis.'
      },
      { status: 500 }
    );
  }
}
```

## File: src/app/api/resume/analyses/route.ts
```typescript
import { NextRequest, NextResponse } from 'next/server';

const BACKEND_URL = (process.env.NEXT_PUBLIC_API_URL || 'http://localhost:5500').replace(/\/$/, '');

export async function GET(request: NextRequest) {
  try {
    // Get the authorization header from the incoming request
    const authHeader = request.headers.get('authorization');
    
    console.log('🔐 API Proxy - Authorization header:', authHeader ? 'Present' : 'Missing');
    console.log('🔗 API Proxy - Backend URL:', `${BACKEND_URL}/api/protected/ai-local/resume/analyses`);
    
    if (!authHeader) {
      console.log('❌ API Proxy - No authorization header');
      return NextResponse.json(
        { success: false, message: 'Authorization header required' },
        { status: 401 }
      );
    }

    // Forward the request to the backend with the correct route
    console.log('📤 API Proxy - Forwarding request to backend...');
    const response = await fetch(`${BACKEND_URL}/api/protected/ai-local/resume/analyses`, {
      method: 'GET',
      headers: {
        'Authorization': authHeader,
        'Content-Type': 'application/json',
      },
    });

    console.log('📥 API Proxy - Backend response status:', response.status);
    console.log('📥 API Proxy - Backend response headers:', Object.fromEntries(response.headers.entries()));

    const data = await response.json();
    console.log('📥 API Proxy - Backend response data:', data);

    return NextResponse.json(data, { status: response.status });
  } catch (error) {
    console.error('❌ API Proxy - Error:', error);
    return NextResponse.json(
      { success: false, message: 'Failed to fetch resume analyses', error: error instanceof Error ? error.message : 'Unknown error' },
      { status: 500 }
    );
  }
}
```

## File: src/app/api/resume/pdf-download/route.ts
```typescript
import { NextRequest, NextResponse } from 'next/server';
import { pdfGenerator, PDFOptions, ResumePDFData } from '@/lib/pdfGenerator';

export async function POST(request: NextRequest) {
  try {
    const body = await request.json();
    const { resumeData, options = {} }: { resumeData: ResumePDFData; options?: PDFOptions } = body;

    // Validate input
    if (!resumeData) {
      return NextResponse.json(
        { success: false, message: 'Resume data is required' },
        { status: 400 }
      );
    }

    // Validate required fields
    if (!resumeData.personalInfo?.name) {
      return NextResponse.json(
        { success: false, message: 'Personal information with name is required' },
        { status: 400 }
      );
    }

    // Generate PDF
    const pdfBuffer = await pdfGenerator.generateResumePDF(resumeData, options);

    // Create filename
    const timestamp = new Date().toISOString().split('T')[0];
    const filename = `${resumeData.personalInfo.name.replace(/[^a-zA-Z0-9]/g, '_')}_resume_${timestamp}.pdf`;

    // Return PDF as response
    return new NextResponse(pdfBuffer, {
      status: 200,
      headers: {
        'Content-Type': 'application/pdf',
        'Content-Disposition': `attachment; filename="${filename}"`,
        'Content-Length': pdfBuffer.length.toString(),
        'Cache-Control': 'no-cache, no-store, must-revalidate',
        'Pragma': 'no-cache',
        'Expires': '0'
      }
    });

  } catch (error) {
    console.error('PDF generation error:', error);
    
    return NextResponse.json(
      { 
        success: false, 
        message: 'Failed to generate PDF',
        error: error instanceof Error ? error.message : 'Unknown error'
      },
      { status: 500 }
    );
  }
}

export async function GET(request: NextRequest) {
  try {
    const { searchParams } = new URL(request.url);
    const resumeId = searchParams.get('resumeId');
    const format = searchParams.get('format') || 'A4';
    const landscape = searchParams.get('landscape') === 'true';

    if (!resumeId) {
      return NextResponse.json(
        { success: false, message: 'Resume ID is required' },
        { status: 400 }
      );
    }

    // TODO: Fetch resume data from database using resumeId
    // For now, return error as this would require database integration
    return NextResponse.json(
      { success: false, message: 'Resume data fetching not implemented yet' },
      { status: 501 }
    );

  } catch (error) {
    console.error('PDF download error:', error);
    
    return NextResponse.json(
      { 
        success: false, 
        message: 'Failed to download PDF',
        error: error instanceof Error ? error.message : 'Unknown error'
      },
      { status: 500 }
    );
  }
}

// Handle OPTIONS request for CORS
export async function OPTIONS() {
  return new NextResponse(null, {
    status: 200,
    headers: {
      'Access-Control-Allow-Origin': '*',
      'Access-Control-Allow-Methods': 'GET, POST, OPTIONS',
      'Access-Control-Allow-Headers': 'Content-Type, Authorization',
      'Access-Control-Max-Age': '86400'
    }
  });
}
```

## File: src/app/auth/page.tsx
```typescript
'use client';

import { useState, useEffect } from 'react';
import { useRouter } from 'next/navigation';
import LoginForm from '@/components/features/auth/LoginForm';
import RegisterForm from '@/components/features/auth/RegisterForm';
import { auth } from '@/lib/auth';

export default function AuthPage() {
  const [isLogin, setIsLogin] = useState(true);
  const router = useRouter();

  useEffect(() => {
    // Redirect if already authenticated
    if (auth.isAuthenticated()) {
      router.push('/dashboard');
    }
  }, [router]);

  const handleAuthSuccess = () => {
    // Refresh the page to update authentication state
    window.location.reload();
  };

  return (
    <div className="min-h-screen flex items-center justify-center bg-gradient-to-br from-blue-50 to-indigo-100 p-4">
      <div className="w-full max-w-md">
        {isLogin ? (
          <LoginForm 
            onSuccess={handleAuthSuccess}
            onSwitchToRegister={() => setIsLogin(false)}
          />
        ) : (
          <RegisterForm 
            onSuccess={handleAuthSuccess}
            onSwitchToLogin={() => setIsLogin(true)}
          />
        )}
      </div>
    </div>
  );
}
```

## File: src/app/dashboard/career/page.tsx
```typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { Progress } from '@/components/ui/progress';

import { 
  Upload, 
  FileText, 
  Target, 
  TrendingUp, 
  Star, 
  ChevronRight, 
  Briefcase,
  DollarSign,
  CheckCircle,
  BookOpen,
  Search
} from 'lucide-react';
import { useToast } from '@/hooks/use-toast';

import JobSearchModal from '@/components/features/career/JobSearchModal';

interface PositionRecommendation {
  title: string;
  industry: string;
  level: string;
  successProbability: number;
  matchScore: number;
  salaryRange: {
    min: number;
    max: number;
    currency: string;
  };
  requiredSkills: string[];
  skillsMatch: {
    matching: string[];
    missing: string[];
    transferable: string[];
  };
  canadianRelevance: {
    workExperienceValue: string;
    educationRecognition: string;
    certificationNeeds: string[];
  };
}

interface EnhancedProfile {
  optimizedSkills: {
    technical: string[];
    soft: string[];
    leadership: string[];
  };
  repositionedExperience: Array<{
    company: string;
    title: string;
    optimizedDescription: string;
    keyAchievements: string[];
  }>;
  applicationStrategy: {
    targetCompanies: string[];
    networkingStrategy: string[];
    timelineRecommendations: string[];
  };
  skillDevelopmentPlan: {
    immediateActions: string[];
    shortTermGoals: string[];
    longTermObjectives: string[];
  };
}

export default function CareerProfilePage() {
  const [currentStep, setCurrentStep] = useState<'upload' | 'recommendations' | 'enhanced'>('upload');
  const [resumeFile, setResumeFile] = useState<File | null>(null);
  const [uploading, setUploading] = useState(false);
  const [loading, setLoading] = useState(false);
  const [analysisData, setAnalysisData] = useState<any>(null);
  const [recommendations, setRecommendations] = useState<PositionRecommendation[]>([]);
  const [selectedPosition, setSelectedPosition] = useState<PositionRecommendation | null>(null);
  const [enhancedProfile, setEnhancedProfile] = useState<EnhancedProfile | null>(null);
  const [skillGapAnalysis, setSkillGapAnalysis] = useState<any>(null);
  const [generatingResume, setGeneratingResume] = useState(false);

  const [jobSearchModalOpen, setJobSearchModalOpen] = useState(false);
  const [jobSearchCareerPath, setJobSearchCareerPath] = useState<{ title: string; industry?: string } | null>(null);
  
  const { toast } = useToast();

  const handleFileUpload = (event: React.ChangeEvent<HTMLInputElement>) => {
    const file = event.target.files?.[0];
    if (file) {
      setResumeFile(file);
    }
  };

  const handleResumeAnalysis = async () => {
    if (!resumeFile) return;

    setUploading(true);
    try {
      const formData = new FormData();
      formData.append('resume', resumeFile);

      const token = 'guest-token';
      
      const response = await fetch('/api/protected/career/analyze-resume', {
        method: 'POST',
        headers: {
          'Authorization': `Bearer ${token}`,
        },
        body: formData
      });

      if (!response.ok) {
        throw new Error('Resume analysis failed');
      }

      const result = await response.json();
      
      if (result.success) {
        setAnalysisData(result.data);
        setRecommendations(result.data.positionRecommendations.positions || []);
        setCurrentStep('recommendations');
        
        toast({
          title: "Resume Analyzed Successfully",
          description: `Found ${result.data.positionRecommendations.positions?.length || 0} position recommendations`,
        });
      }
    } catch (error) {
      console.error('Resume analysis error:', error);
      toast({
        title: "Analysis Failed",
        description: "Unable to analyze your resume. Please try again.",
        variant: "destructive",
      });
    } finally {
      setUploading(false);
    }
  };

  const handlePositionSelect = async (position: PositionRecommendation) => {
    setSelectedPosition(position);
    setLoading(true);

    try {
      const token = 'guest-token';
      
      const response = await fetch('/api/protected/career/enhanced-profile', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
          'Authorization': `Bearer ${token}`,
        },
        body: JSON.stringify({
          targetPosition: position,
          resumeAnalysisId: analysisData?.analysisId,
          userPreferences: {}
        })
      });

      if (!response.ok) {
        throw new Error('Enhanced profile generation failed');
      }

      const result = await response.json();
      
      if (result.success) {
        setEnhancedProfile(result.data.enhancedProfile);
        setSkillGapAnalysis(result.data.skillGapAnalysis);
        setCurrentStep('enhanced');
        
        toast({
          title: "Enhanced Profile Generated",
          description: "Your personalized career profile is ready!",
        });
      }
    } catch (error) {
      console.error('Enhanced profile generation error:', error);
      toast({
        title: "Profile Generation Failed",
        description: "Unable to generate enhanced profile. Please try again.",
        variant: "destructive",
      });
    } finally {
      setLoading(false);
    }
  };

  const handleResumeGeneration = async (position: PositionRecommendation) => {
    setGeneratingResume(true);
    
    try {
      const token = 'guest-token';
      
      const response = await fetch('/api/protected/career/generate-resume', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
          'Authorization': `Bearer ${token}`,
        },
        body: JSON.stringify({
          targetPosition: position,
          existingAnalysisId: analysisData?.analysisId,
          userProfile: null // Will fetch from database if available
        })
      });

      if (!response.ok) {
        throw new Error('Resume generation failed');
      }

      const result = await response.json();
      
      if (result.success) {
        setGeneratedResume(result.data.generatedResume);
        
        toast({
          title: "Resume Generated Successfully",
          description: `Created an optimized resume for ${position.title}`,
        });

        // Optional: Download as JSON
        const resumeBlob = new Blob([JSON.stringify(result.data.generatedResume, null, 2)], 
          { type: 'application/json' });
        const url = URL.createObjectURL(resumeBlob);
        const a = document.createElement('a');
        a.href = url;
        a.download = `AI_Generated_Resume_${position.title.replace(/\s+/g, '_')}.json`;
        document.body.appendChild(a);
        a.click();
        document.body.removeChild(a);
        URL.revokeObjectURL(url);
        
      }
    } catch (error) {
      console.error('Resume generation error:', error);
      toast({
        title: "Resume Generation Failed",
        description: "Unable to generate resume. Please try again.",
        variant: "destructive",
      });
    } finally {
      setGeneratingResume(false);
    }
  };

  const handleJobSearch = (position: PositionRecommendation) => {
    setJobSearchCareerPath({
      title: position.title,
      industry: position.industry
    });
    setJobSearchModalOpen(true);
  };

  const renderUploadStep = () => (
    <Card className="w-full max-w-2xl mx-auto">
      <CardHeader>
        <CardTitle className="flex items-center space-x-2">
          <Upload className="w-6 h-6" />
          <span>Upload Your Resume</span>
        </CardTitle>
        <CardDescription>
          Upload your resume to get personalized career recommendations tailored for the Canadian job market
        </CardDescription>
      </CardHeader>
      <CardContent className="space-y-6">
        <div className="border-2 border-dashed border-gray-300 rounded-lg p-8 text-center">
          <FileText className="w-12 h-12 mx-auto text-gray-400 mb-4" />
          <div className="space-y-2">
            <p className="text-lg font-medium">Choose your resume file</p>
            <p className="text-gray-600">PDF, DOC, or DOCX (max 5MB)</p>
          </div>
          <input
            type="file"
            accept=".pdf,.doc,.docx"
            onChange={handleFileUpload}
            className="hidden"
            id="resume-upload"
          />
          <label htmlFor="resume-upload">
            <Button variant="outline" className="mt-4" asChild>
              <span>Select File</span>
            </Button>
          </label>
        </div>
        
        {resumeFile && (
          <div className="flex items-center justify-between p-4 bg-green-50 rounded-lg">
            <div className="flex items-center space-x-3">
              <FileText className="w-5 h-5 text-green-600" />
              <span className="font-medium">{resumeFile.name}</span>
            </div>
            <Badge variant="secondary">
              {(resumeFile.size / 1024 / 1024).toFixed(2)} MB
            </Badge>
          </div>
        )}
        
        <Button 
          onClick={handleResumeAnalysis}
          disabled={!resumeFile || uploading}
          className="w-full"
          size="lg"
        >
          {uploading ? (
            <>
              <div className="animate-spin rounded-full h-4 w-4 border-b-2 border-white mr-2"></div>
              Analyzing Resume...
            </>
          ) : (
            <>
              <Target className="w-4 h-4 mr-2" />
              Analyze & Get Recommendations
            </>
          )}
        </Button>
      </CardContent>
    </Card>
  );

  const renderRecommendationsStep = () => (
    <div className="space-y-6">
      <div className="text-center">
        <h2 className="text-3xl font-bold mb-2">Career Opportunities</h2>
        <p className="text-gray-600">
          Based on your resume, here are the positions with the highest success probability
        </p>
      </div>
      
      <div className="grid gap-6">
        {recommendations.map((position, index) => (
          <Card key={index} className="hover:shadow-lg transition-shadow cursor-pointer">
            <CardHeader>
              <div className="flex items-start justify-between">
                <div className="space-y-2">
                  <CardTitle className="text-xl">{position.title}</CardTitle>
                  <div className="flex items-center space-x-4 text-sm text-gray-600">
                    <span className="flex items-center">
                      <Briefcase className="w-4 h-4 mr-1" />
                      {position.industry}
                    </span>
                    <span className="flex items-center">
                      <DollarSign className="w-4 h-4 mr-1" />
                      ${position.salaryRange.min.toLocaleString()} - ${position.salaryRange.max.toLocaleString()} {position.salaryRange.currency}
                    </span>
                  </div>
                </div>
                <div className="text-right">
                  <div className="text-2xl font-bold text-green-600">
                    {Math.round(position.successProbability * 100)}%
                  </div>
                  <div className="text-sm text-gray-600">Success Rate</div>
                </div>
              </div>
            </CardHeader>
            <CardContent>
              <div className="space-y-4">
                <div>
                  <div className="flex items-center justify-between mb-2">
                    <span className="text-sm font-medium">Match Score</span>
                    <span className="text-sm">{Math.round(position.matchScore * 100)}%</span>
                  </div>
                  <Progress value={position.matchScore * 100} className="h-2" />
                </div>
                
                <div className="grid md:grid-cols-2 gap-4">
                  <div>
                    <h4 className="font-medium text-green-600 mb-2">✓ Matching Skills</h4>
                    <div className="flex flex-wrap gap-1">
                      {position.skillsMatch.matching.slice(0, 3).map((skill, idx) => (
                        <Badge key={idx} variant="secondary" className="text-xs">
                          {skill}
                        </Badge>
                      ))}
                      {position.skillsMatch.matching.length > 3 && (
                        <Badge variant="outline" className="text-xs">
                          +{position.skillsMatch.matching.length - 3} more
                        </Badge>
                      )}
                    </div>
                  </div>
                  
                  <div>
                    <h4 className="font-medium text-orange-600 mb-2">⚡ Skills to Develop</h4>
                    <div className="flex flex-wrap gap-1">
                      {position.skillsMatch.missing.slice(0, 3).map((skill, idx) => (
                        <Badge key={idx} variant="outline" className="text-xs">
                          {skill}
                        </Badge>
                      ))}
                      {position.skillsMatch.missing.length > 3 && (
                        <Badge variant="outline" className="text-xs">
                          +{position.skillsMatch.missing.length - 3} more
                        </Badge>
                      )}
                    </div>
                  </div>
                </div>
                
                <div className="space-y-2">
                  <Button 
                    onClick={() => handlePositionSelect(position)}
                    disabled={loading}
                    className="w-full"
                  >
                    {loading && selectedPosition === position ? (
                      <>
                        <div className="animate-spin rounded-full h-4 w-4 border-b-2 border-white mr-2"></div>
                        Generating Profile...
                      </>
                    ) : (
                      <>
                        Generate Enhanced Profile
                        <ChevronRight className="w-4 h-4 ml-2" />
                      </>
                    )}
                  </Button>
                  
                  <Button 
                    onClick={() => handleResumeGeneration(position)}
                    disabled={generatingResume}
                    variant="outline"
                    className="w-full"
                  >
                    {generatingResume ? (
                      <>
                        <div className="animate-spin rounded-full h-4 w-4 border-b-2 border-current mr-2"></div>
                        Generating Resume...
                      </>
                    ) : (
                      <>
                        <FileText className="w-4 h-4 mr-2" />
                        Generate New Resume
                      </>
                    )}
                  </Button>
                  
                  <Button 
                    onClick={() => handleJobSearch(position)}
                    variant="default"
                    className="w-full bg-blue-600 hover:bg-blue-700 text-white"
                  >
                    <Search className="w-4 h-4 mr-2" />
                    Jobs Related to {position.title}
                  </Button>
                </div>
              </div>
            </CardContent>
          </Card>
        ))}
      </div>
    </div>
  );

  const renderEnhancedProfileStep = () => (
    <div className="space-y-6">
      <div className="text-center">
        <h2 className="text-3xl font-bold mb-2">Your Enhanced Career Profile</h2>
        <p className="text-gray-600">
          Tailored for: <strong>{selectedPosition?.title}</strong>
        </p>
      </div>
      
      <Tabs defaultValue="profile" className="w-full">
        <TabsList className="grid w-full grid-cols-3">
          <TabsTrigger value="profile">Enhanced Profile</TabsTrigger>
          <TabsTrigger value="skills">Skill Analysis</TabsTrigger>
          <TabsTrigger value="strategy">Action Plan</TabsTrigger>
        </TabsList>
        
        <TabsContent value="profile" className="space-y-6">
          {enhancedProfile && (
            <>
              <Card>
                <CardHeader>
                  <CardTitle className="flex items-center space-x-2">
                    <Star className="w-5 h-5" />
                    <span>Optimized Skills Presentation</span>
                  </CardTitle>
                </CardHeader>
                <CardContent className="space-y-4">
                  <div>
                    <h4 className="font-medium mb-2">Technical Skills</h4>
                    <div className="flex flex-wrap gap-2">
                      {enhancedProfile.optimizedSkills.technical.map((skill, idx) => (
                        <Badge key={idx} className="bg-blue-100 text-blue-800">
                          {skill}
                        </Badge>
                      ))}
                    </div>
                  </div>
                  
                  <div>
                    <h4 className="font-medium mb-2">Soft Skills</h4>
                    <div className="flex flex-wrap gap-2">
                      {enhancedProfile.optimizedSkills.soft.map((skill, idx) => (
                        <Badge key={idx} className="bg-green-100 text-green-800">
                          {skill}
                        </Badge>
                      ))}
                    </div>
                  </div>
                  
                  <div>
                    <h4 className="font-medium mb-2">Leadership Skills</h4>
                    <div className="flex flex-wrap gap-2">
                      {enhancedProfile.optimizedSkills.leadership.map((skill, idx) => (
                        <Badge key={idx} className="bg-purple-100 text-purple-800">
                          {skill}
                        </Badge>
                      ))}
                    </div>
                  </div>
                </CardContent>
              </Card>
              
              <Card>
                <CardHeader>
                  <CardTitle className="flex items-center space-x-2">
                    <Briefcase className="w-5 h-5" />
                    <span>Repositioned Experience</span>
                  </CardTitle>
                </CardHeader>
                <CardContent>
                  <div className="space-y-6">
                    {enhancedProfile.repositionedExperience.map((exp, idx) => (
                      <div key={idx} className="border-l-4 border-blue-500 pl-4">
                        <h4 className="font-semibold">{exp.title} at {exp.company}</h4>
                        <p className="text-gray-600 mt-1">{exp.optimizedDescription}</p>
                        <div className="mt-2">
                          <h5 className="font-medium text-sm">Key Achievements:</h5>
                          <ul className="list-disc list-inside text-sm text-gray-600 mt-1">
                            {exp.keyAchievements.map((achievement, aidx) => (
                              <li key={aidx}>{achievement}</li>
                            ))}
                          </ul>
                        </div>
                      </div>
                    ))}
                  </div>
                </CardContent>
              </Card>
            </>
          )}
        </TabsContent>
        
        <TabsContent value="skills" className="space-y-6">
          {skillGapAnalysis && (
            <Card>
              <CardHeader>
                <CardTitle className="flex items-center space-x-2">
                  <TrendingUp className="w-5 h-5" />
                  <span>Skill Gap Analysis</span>
                </CardTitle>
              </CardHeader>
              <CardContent className="space-y-4">
                {skillGapAnalysis.skillGapAnalysis?.gaps?.map((gap: any, idx: number) => (
                  <div key={idx} className="border rounded-lg p-4">
                    <div className="flex items-center justify-between mb-2">
                      <h4 className="font-medium">{gap.skill}</h4>
                      <Badge variant={gap.priority === 'High' ? 'destructive' : gap.priority === 'Medium' ? 'default' : 'secondary'}>
                        {gap.priority} Priority
                      </Badge>
                    </div>
                    <p className="text-sm text-gray-600 mb-2">{gap.description}</p>
                    <div className="text-sm">
                      <strong>Learning Path:</strong> {gap.learningPath}
                    </div>
                    <div className="text-sm">
                      <strong>Timeline:</strong> {gap.timeline}
                    </div>
                  </div>
                ))}
              </CardContent>
            </Card>
          )}
        </TabsContent>
        
        <TabsContent value="strategy" className="space-y-6">
          {enhancedProfile && (
            <>
              <Card>
                <CardHeader>
                  <CardTitle className="flex items-center space-x-2">
                    <Target className="w-5 h-5" />
                    <span>Application Strategy</span>
                  </CardTitle>
                </CardHeader>
                <CardContent className="space-y-4">
                  <div>
                    <h4 className="font-medium mb-2">Target Companies</h4>
                    <ul className="list-disc list-inside text-sm text-gray-600">
                      {enhancedProfile.applicationStrategy.targetCompanies.map((company, idx) => (
                        <li key={idx}>{company}</li>
                      ))}
                    </ul>
                  </div>
                  
                  <div>
                    <h4 className="font-medium mb-2">Networking Strategy</h4>
                    <ul className="list-disc list-inside text-sm text-gray-600">
                      {enhancedProfile.applicationStrategy.networkingStrategy.map((strategy, idx) => (
                        <li key={idx}>{strategy}</li>
                      ))}
                    </ul>
                  </div>
                </CardContent>
              </Card>
              
              <Card>
                <CardHeader>
                  <CardTitle className="flex items-center space-x-2">
                    <BookOpen className="w-5 h-5" />
                    <span>Development Roadmap</span>
                  </CardTitle>
                </CardHeader>
                <CardContent className="space-y-4">
                  <div>
                    <h4 className="font-medium text-red-600 mb-2">Immediate Actions (1-2 weeks)</h4>
                    <ul className="list-disc list-inside text-sm">
                      {enhancedProfile.skillDevelopmentPlan.immediateActions.map((action, idx) => (
                        <li key={idx}>{action}</li>
                      ))}
                    </ul>
                  </div>
                  
                  <div>
                    <h4 className="font-medium text-orange-600 mb-2">Short-term Goals (1-3 months)</h4>
                    <ul className="list-disc list-inside text-sm">
                      {enhancedProfile.skillDevelopmentPlan.shortTermGoals.map((goal, idx) => (
                        <li key={idx}>{goal}</li>
                      ))}
                    </ul>
                  </div>
                  
                  <div>
                    <h4 className="font-medium text-green-600 mb-2">Long-term Objectives (6+ months)</h4>
                    <ul className="list-disc list-inside text-sm">
                      {enhancedProfile.skillDevelopmentPlan.longTermObjectives.map((objective, idx) => (
                        <li key={idx}>{objective}</li>
                      ))}
                    </ul>
                  </div>
                </CardContent>
              </Card>
            </>
          )}
        </TabsContent>
      </Tabs>
      
      <div className="flex justify-center space-x-4">
        <Button 
          onClick={() => setCurrentStep('recommendations')}
          variant="outline"
        >
          Back to Recommendations
        </Button>
        <Button onClick={() => setCurrentStep('upload')}>
          Analyze New Resume
        </Button>
      </div>
    </div>
  );

  return (
    <div className="min-h-screen bg-gray-50">
      <div className="container mx-auto px-4 py-8">
        {/* Progress indicator */}
        <div className="mb-8">
          <div className="flex items-center justify-center space-x-4 mb-4">
            <div className={`flex items-center space-x-2 ${currentStep === 'upload' ? 'text-blue-600' : 'text-gray-400'}`}>
              <div className={`w-8 h-8 rounded-full border-2 flex items-center justify-center ${currentStep === 'upload' ? 'border-blue-600 bg-blue-600 text-white' : currentStep !== 'upload' ? 'border-green-600 bg-green-600 text-white' : 'border-gray-300'}`}>
                {currentStep !== 'upload' ? <CheckCircle className="w-4 h-4" /> : '1'}
              </div>
              <span className="font-medium">Upload Resume</span>
            </div>
            <div className="flex-1 h-0.5 bg-gray-300"></div>
            <div className={`flex items-center space-x-2 ${currentStep === 'recommendations' ? 'text-blue-600' : currentStep === 'enhanced' ? 'text-green-600' : 'text-gray-400'}`}>
              <div className={`w-8 h-8 rounded-full border-2 flex items-center justify-center ${currentStep === 'recommendations' ? 'border-blue-600 bg-blue-600 text-white' : currentStep === 'enhanced' ? 'border-green-600 bg-green-600 text-white' : 'border-gray-300'}`}>
                {currentStep === 'enhanced' ? <CheckCircle className="w-4 h-4" /> : '2'}
              </div>
              <span className="font-medium">Position Recommendations</span>
            </div>
            <div className="flex-1 h-0.5 bg-gray-300"></div>
            <div className={`flex items-center space-x-2 ${currentStep === 'enhanced' ? 'text-blue-600' : 'text-gray-400'}`}>
              <div className={`w-8 h-8 rounded-full border-2 flex items-center justify-center ${currentStep === 'enhanced' ? 'border-blue-600 bg-blue-600 text-white' : 'border-gray-300'}`}>
                3
              </div>
              <span className="font-medium">Enhanced Profile</span>
            </div>
          </div>
        </div>

        {/* Main content */}
        {currentStep === 'upload' && renderUploadStep()}
        {currentStep === 'recommendations' && renderRecommendationsStep()}
        {currentStep === 'enhanced' && renderEnhancedProfileStep()}
        
        {/* Job Search Modal */}
        <JobSearchModal
          isOpen={jobSearchModalOpen}
          onClose={() => setJobSearchModalOpen(false)}
          careerPath={jobSearchCareerPath || { title: '' }}
        />
      </div>
    </div>
  );
}
```

## File: src/app/dashboard/history/page.tsx
```typescript
"use client";

import React, { useState } from 'react';
import ResumeAnalysisList from '@/components/features/resume/ResumeAnalysisList';
import ResumeAnalysisDetail from '@/components/features/resume/ResumeAnalysisDetail';
import { Button } from '@/components/ui/button';
import { ArrowLeft, History } from 'lucide-react';

interface ResumeAnalysis {
  id: string;
  originalFileName: string;
  createdAt: string;
  personalInfo: {
    name: string;
    email: string;
    phone?: string;
    location?: string;
  };
  skills: string[];
  workExperience: Array<{
    company: string;
    position: string;
    duration: string;
    description: string;
  }>;
  education: Array<{
    institution: string;
    degree: string;
    year: string;
  }>;
  canadianMarketAnalysis: {
    overallScore: number;
    strengths: string[];
    improvementAreas: string[];
    recommendations: string[];
  };
  confidenceScores: {
    overall: number;
    personalInfo: number;
    skills: number;
    workExperience: number;
    education: number;
  };
  metadata: {
    processingMethod: string;
    fileSize: number;
  };
}

export default function HistoryPage() {
  const [currentView, setCurrentView] = useState<'list' | 'detail'>('list');
  const [selectedAnalysis, setSelectedAnalysis] = useState<ResumeAnalysis | null>(null);

  const handleAnalysisSelect = (analysis: ResumeAnalysis) => {
    setSelectedAnalysis(analysis);
    setCurrentView('detail');
  };

  const handleBackToList = () => {
    setSelectedAnalysis(null);
    setCurrentView('list');
  };

  const handleBackToDashboard = () => {
    window.location.href = '/dashboard';
  };

  return (
    <div className="min-h-screen bg-gray-50">
      <div className="container mx-auto px-4 py-8">
        <div className="mb-8">
          <div className="flex items-center justify-between">
            <div className="flex items-center space-x-4">
              <Button
                variant="outline"
                onClick={currentView === 'detail' ? handleBackToList : handleBackToDashboard}
                className="flex items-center space-x-2"
              >
                <ArrowLeft className="w-4 h-4" />
                <span>{currentView === 'detail' ? 'Back to List' : 'Back to Dashboard'}</span>
              </Button>
              
              <div className="flex items-center space-x-2">
                <History className="w-6 h-6 text-blue-600" />
                <h1 className="text-3xl font-bold text-gray-900">
                  {currentView === 'list' ? 'Analysis History' : 'Analysis Details'}
                </h1>
              </div>
            </div>
            
            {currentView === 'list' && (
              <Button
                onClick={() => window.location.href = '/dashboard/resume'}
                className="bg-blue-600 hover:bg-blue-700"
              >
                Upload New Resume
              </Button>
            )}
          </div>
          
          <p className="text-xl text-gray-600 mt-2">
            {currentView === 'list' 
              ? 'View and manage your previous resume analyses'
              : `Detailed analysis for ${selectedAnalysis?.originalFileName}`
            }
          </p>
        </div>
        
        {/* Content based on current view */}
        {currentView === 'list' && (
          <ResumeAnalysisList onAnalysisSelect={handleAnalysisSelect} />
        )}
        
        {currentView === 'detail' && selectedAnalysis && (
          <ResumeAnalysisDetail 
            analysis={selectedAnalysis} 
            onBack={handleBackToList}
          />
        )}
      </div>
    </div>
  );
}
```

## File: src/app/dashboard/layout.tsx
```typescript
import Header from "@/components/common/Header";
import React, { ReactNode } from "react";

async function Layout({ children }: { children: ReactNode }) {
  // No authentication required - direct access to dashboard
  return (
    <div className="flex flex-col h-screen min-w-full bg-background">
      <Header />
      <main className="w-full h-full">{children}</main>
    </div>
  );
}

export default Layout;
```

## File: src/app/dashboard/page.tsx
```typescript
import { redirect } from "next/navigation";

const Dashboard = () => {
  redirect("/dashboard/profile");
};

export default Dashboard;
```

## File: src/app/dashboard/profile/page.tsx
```typescript
"use client";

import { useState, useEffect } from "react";
import FeaturesPanel from "@/components/features/resume/FeaturesPanel";
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import Link from "next/link";
import { Brain, FileText, History, Search } from "lucide-react";
import { auth } from "@/lib/auth";

export default function DashboardLayout() {
  const [user, setUser] = useState<any>(null);
  const [isLoading, setIsLoading] = useState(true);

  useEffect(() => {
    const checkAuth = () => {
      const currentUser = auth.getCurrentUser();
      setUser(currentUser);
      setIsLoading(false);
    };

    checkAuth();
  }, []);

  const getFirstName = (fullName: string) => {
    return fullName.split(' ')[0] || fullName;
  };

  const aiFeatures = [
    {
      title: "Resume Analysis",
      description: "Upload and analyze your resume with AI-powered insights",
      icon: FileText,
      href: "/dashboard/resume",
      color: "text-blue-600"
    },
    {
      title: "Resume Generator",
      description: "Generate Canadian resumes optimized for ATS systems",
      icon: FileText,
      href: "/dashboard/resume/generator",
      color: "text-indigo-600"
    },
    {
      title: "Career Profile",
      description: "Create and manage your AI-powered career profile",
      icon: Brain,
      href: "/dashboard/career",
      color: "text-green-600"
    },
    {
      title: "Job Search",
      description: "Find relevant job opportunities using AI recommendations",
      icon: Search,
      href: "/dashboard",
      color: "text-purple-600"
    },
    {
      title: "Analysis History",
      description: "View your previous AI analyses and insights",
      icon: History,
      href: "/dashboard/history",
      color: "text-orange-600"
    }
  ];

  return (
    <div className="container mx-auto p-6">
      <div className="mb-8">
        <h1 className="text-3xl font-bold text-gray-900 mb-2">
          {!isLoading && user ? (
            <>Welcome back, {getFirstName(user.fullName)}! 👋</>
          ) : (
            <>AI Career Assistant</>
          )}
        </h1>
        <p className="text-gray-600">
          {!isLoading && user ? (
            <>Ready to enhance your career journey with AI-powered insights?</>
          ) : (
            <>Leverage AI to enhance your career journey</>
          )}
        </p>
      </div>

      {/* AI Features Panel */}
      <div className="mb-8">
        <FeaturesPanel />
      </div>

      {/* AI Tools Grid */}
      <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
        {aiFeatures.map((feature, index) => (
          <Card key={index} className="hover:shadow-lg transition-shadow">
            <CardHeader>
              <div className="flex items-center space-x-2">
                <feature.icon className={`h-6 w-6 ${feature.color}`} />
                <CardTitle className="text-lg">{feature.title}</CardTitle>
              </div>
              <CardDescription>{feature.description}</CardDescription>
            </CardHeader>
            <CardContent>
              <Link href={feature.href}>
                <Button className="w-full" variant="outline">
                  Get Started
                </Button>
              </Link>
            </CardContent>
          </Card>
        ))}
      </div>

      {/* Quick Stats */}
      <div className="mt-8 grid grid-cols-1 md:grid-cols-3 gap-6">
        <Card>
          <CardHeader>
            <CardTitle className="text-sm font-medium text-gray-600">Total Analyses</CardTitle>
          </CardHeader>
          <CardContent>
            <div className="text-2xl font-bold">0</div>
            <p className="text-xs text-gray-500">Resume analyses completed</p>
          </CardContent>
        </Card>
        <Card>
          <CardHeader>
            <CardTitle className="text-sm font-medium text-gray-600">Career Insights</CardTitle>
          </CardHeader>
          <CardContent>
            <div className="text-2xl font-bold">0</div>
            <p className="text-xs text-gray-500">AI-generated insights</p>
          </CardContent>
        </Card>
        <Card>
          <CardHeader>
            <CardTitle className="text-sm font-medium text-gray-600">Job Matches</CardTitle>
          </CardHeader>
          <CardContent>
            <div className="text-2xl font-bold">0</div>
            <p className="text-xs text-gray-500">Recommended positions</p>
          </CardContent>
        </Card>
      </div>
    </div>
  );
}
```

## File: src/app/dashboard/profile/settings/page.tsx
```typescript
"use client";

import { Button } from "@/components/ui/button";
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card";
import Link from "next/link";
import { ArrowLeft, Settings } from "lucide-react";

export default function SettingsPage() {
  return (
    <div className="container mx-auto p-6">
      {/* Header */}
      <div className="mb-8">
        <div className="flex items-center gap-4 mb-4">
          <Button variant="outline" size="sm" asChild>
            <Link href="/dashboard/profile">
              <ArrowLeft className="h-4 w-4 mr-2" />
              Back to Profile
            </Link>
          </Button>
        </div>
        <h1 className="text-3xl font-bold text-gray-900 mb-2">
          Account Settings
        </h1>
        <p className="text-gray-600">
          Manage your account preferences and settings
        </p>
      </div>

      <div className="max-w-2xl">
        <Card>
          <CardHeader>
            <CardTitle className="flex items-center gap-2">
              <Settings className="h-5 w-5" />
              Settings
            </CardTitle>
            <CardDescription>
              This page is under development. More settings will be available soon.
            </CardDescription>
          </CardHeader>
          <CardContent>
            <div className="space-y-4">
              <div className="p-4 border rounded-lg">
                <h3 className="font-medium mb-2">Profile Information</h3>
                <p className="text-sm text-gray-600 mb-3">
                  Update your personal information and preferences.
                </p>
                <Button variant="outline" disabled>
                  Coming Soon
                </Button>
              </div>
              
              <div className="p-4 border rounded-lg">
                <h3 className="font-medium mb-2">Notification Preferences</h3>
                <p className="text-sm text-gray-600 mb-3">
                  Control how and when you receive notifications.
                </p>
                <Button variant="outline" disabled>
                  Coming Soon
                </Button>
              </div>
              
              <div className="p-4 border rounded-lg">
                <h3 className="font-medium mb-2">Language & Region</h3>
                <p className="text-sm text-gray-600 mb-3">
                  Set your preferred language and region settings.
                </p>
                <Button variant="outline" disabled>
                  Coming Soon
                </Button>
              </div>
            </div>
          </CardContent>
        </Card>
      </div>
    </div>
  );
}
```

## File: src/app/dashboard/resume/generator/edit/[resumeId]/page.tsx
```typescript
"use client";

import React, { useState, useEffect } from 'react';
import { useRouter, useParams } from 'next/navigation';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Alert, AlertDescription } from '@/components/ui/alert';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { 
  Save, 
  Download, 
  Eye, 
  Edit3, 
  Settings, 
  Share2, 
  History, 
  Loader2, 
  CheckCircle, 
  XCircle, 
  ArrowLeft,
  FileText,
  Sparkles,
  Target,
  Brain,
  Clock,
  AlertTriangle
} from 'lucide-react';
import { useResumeGeneratorStore } from '@/stores/resumeGeneratorStore';
import { auth } from '@/lib/auth';
import { getGeneratedResumeById, updateGeneratedResume, exportResume } from '@/lib/api/resumeGenerator';
import InteractiveResumeEditor from '@/components/features/resume/generator/InteractiveResumeEditor';
import SuggestionPanel from '@/components/features/resume/generator/SuggestionPanel';
import ResumePDFView from '@/components/features/resume/generator/ResumePDFView';

export default function InteractiveResumeEditorPage() {
  const router = useRouter();
  const params = useParams();
  const resumeId = params.resumeId as string;
  
  const [user, setUser] = useState<any>(null);
  const [isLoading, setIsLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);
  const [resume, setResume] = useState<any>(null);
  const [activeTab, setActiveTab] = useState('editor');
  const [isSaving, setIsSaving] = useState(false);
  const [lastSaved, setLastSaved] = useState<Date | null>(null);
  const [hasUnsavedChanges, setHasUnsavedChanges] = useState(false);
  const [isExporting, setIsExporting] = useState(false);

  const { 
    setCurrentResume,
    setIsEditing,
    setLastAutoSave
  } = useResumeGeneratorStore();

  useEffect(() => {
    const checkAuth = async () => {
      try {
        const currentUser = auth.getCurrentUser();
        setUser(currentUser);
        
        if (!currentUser) {
          setError('Authentication failed. Please log in again.');
        }
      } catch (error) {
        console.error('Auth check failed:', error);
        setError('Authentication failed. Please log in again.');
      } finally {
        setIsLoading(false);
      }
    };

    checkAuth();
  }, []);

  useEffect(() => {
    if (user && resumeId) {
      loadResume();
    }
  }, [user, resumeId]);

  const loadResume = async () => {
    try {
      setIsLoading(true);
      const response = await getGeneratedResumeById(resumeId);
      
      if (response.success) {
        setResume(response.data);
        setCurrentResume(response.data);
        setIsEditing(true);
        setLastSaved(new Date(response.data.updatedAt));
      } else {
        throw new Error(response.message || 'Failed to load resume');
      }
    } catch (error) {
      console.error('Failed to load resume:', error);
      setError(error instanceof Error ? error.message : 'Failed to load resume');
    } finally {
      setIsLoading(false);
    }
  };

  const handleSave = async () => {
    if (!resume) return;
    
    try {
      setIsSaving(true);
      const response = await updateGeneratedResume(resumeId, {
        resumeData: resume.resumeData,
        userEdits: resume.userEdits || {},
        lastEdited: new Date().toISOString()
      });
      
      if (response.success) {
        setLastSaved(new Date());
        setHasUnsavedChanges(false);
        setLastAutoSave(new Date());
      } else {
        throw new Error(response.message || 'Failed to save resume');
      }
    } catch (error) {
      console.error('Save failed:', error);
      setError(error instanceof Error ? error.message : 'Failed to save resume');
    } finally {
      setIsSaving(false);
    }
  };

  const handleExport = async (format: 'pdf' | 'docx') => {
    try {
      setIsExporting(true);
      const response = await exportResume(resumeId, { format });
      
      if (response.success) {
        // Handle file download
        const link = document.createElement('a');
        link.href = response.data.downloadUrl;
        link.download = `resume-${resumeId}.${format}`;
        document.body.appendChild(link);
        link.click();
        document.body.removeChild(link);
      } else {
        throw new Error(response.message || 'Failed to export resume');
      }
    } catch (error) {
      console.error('Export failed:', error);
      setError(error instanceof Error ? error.message : 'Failed to export resume');
    } finally {
      setIsExporting(false);
    }
  };

  const handleResumeUpdate = (updatedResume: any) => {
    setResume(updatedResume);
    setHasUnsavedChanges(true);
  };

  const handleBack = () => {
    if (hasUnsavedChanges) {
      if (confirm('You have unsaved changes. Are you sure you want to leave?')) {
        router.push('/dashboard/resume/generator');
      }
    } else {
      router.push('/dashboard/resume/generator');
    }
  };

  if (isLoading) {
    return (
      <div className="container mx-auto p-6">
        <div className="flex items-center justify-center min-h-[400px]">
          <Loader2 className="h-8 w-8 animate-spin" />
          <span className="ml-2">Loading resume...</span>
        </div>
      </div>
    );
  }

  if (!user) {
    return (
      <div className="container mx-auto p-6">
        <Alert>
          <XCircle className="h-4 w-4" />
          <AlertDescription>
            Please log in to access the resume editor.
          </AlertDescription>
        </Alert>
      </div>
    );
  }

  if (error) {
    return (
      <div className="container mx-auto p-6">
        <Alert>
          <AlertTriangle className="h-4 w-4" />
          <AlertDescription>{error}</AlertDescription>
        </Alert>
        <Button onClick={handleBack} className="mt-4">
          <ArrowLeft className="h-4 w-4 mr-2" />
          Back to Resume Generator
        </Button>
      </div>
    );
  }

  if (!resume) {
    return (
      <div className="container mx-auto p-6">
        <Alert>
          <AlertTriangle className="h-4 w-4" />
          <AlertDescription>
            Resume not found or you don't have permission to edit it.
          </AlertDescription>
        </Alert>
        <Button onClick={handleBack} className="mt-4">
          <ArrowLeft className="h-4 w-4 mr-2" />
          Back to Resume Generator
        </Button>
      </div>
    );
  }

  return (
    <div className="h-screen flex flex-col">
      {/* Header */}
      <div className="border-b bg-white">
        <div className="container mx-auto px-6 py-4">
          <div className="flex items-center justify-between">
            <div className="flex items-center gap-4">
              <Button onClick={handleBack} variant="outline" size="sm">
                <ArrowLeft className="h-4 w-4 mr-2" />
                Back
              </Button>
              
              <div>
                <h1 className="text-xl font-semibold text-gray-900">
                  Resume Editor
                </h1>
                <p className="text-sm text-gray-600">
                  {resume.jobTargeting?.jobTitle} at {resume.jobTargeting?.companyName}
                </p>
              </div>
            </div>

            <div className="flex items-center gap-3">
              {/* Save Status */}
              <div className="flex items-center gap-2 text-sm">
                {isSaving ? (
                  <>
                    <Loader2 className="h-4 w-4 animate-spin text-blue-600" />
                    <span className="text-blue-600">Saving...</span>
                  </>
                ) : lastSaved ? (
                  <>
                    <CheckCircle className="h-4 w-4 text-green-600" />
                    <span className="text-green-600">
                      Saved {lastSaved.toLocaleTimeString()}
                    </span>
                  </>
                ) : (
                  <>
                    <Clock className="h-4 w-4 text-gray-400" />
                    <span className="text-gray-500">Not saved</span>
                  </>
                )}
              </div>

              {/* Action Buttons */}
              <div className="flex items-center gap-2">
                <Button
                  onClick={handleSave}
                  disabled={isSaving || !hasUnsavedChanges}
                  size="sm"
                >
                  <Save className="h-4 w-4 mr-2" />
                  Save
                </Button>

                <Button
                  onClick={() => handleExport('pdf')}
                  disabled={isExporting}
                  variant="outline"
                  size="sm"
                >
                  <Download className="h-4 w-4 mr-2" />
                  Export PDF
                </Button>

                <Button
                  onClick={() => handleExport('docx')}
                  disabled={isExporting}
                  variant="outline"
                  size="sm"
                >
                  <FileText className="h-4 w-4 mr-2" />
                  Export DOCX
                </Button>
              </div>
            </div>
          </div>
        </div>
      </div>

      {/* Main Content */}
      <div className="flex-1 flex overflow-hidden">
        {/* Left Panel - Editor */}
        <div className="flex-1 flex flex-col">
          <Tabs value={activeTab} onValueChange={setActiveTab} className="flex-1 flex flex-col">
            <div className="border-b bg-gray-50">
              <div className="container mx-auto px-6">
                <TabsList className="grid w-full grid-cols-3">
                  <TabsTrigger value="editor" className="flex items-center gap-2">
                    <Edit3 className="h-4 w-4" />
                    Editor
                  </TabsTrigger>
                  <TabsTrigger value="preview" className="flex items-center gap-2">
                    <Eye className="h-4 w-4" />
                    Preview
                  </TabsTrigger>
                  <TabsTrigger value="settings" className="flex items-center gap-2">
                    <Settings className="h-4 w-4" />
                    Settings
                  </TabsTrigger>
                </TabsList>
              </div>
            </div>

            <TabsContent value="editor" className="flex-1 overflow-hidden">
              <InteractiveResumeEditor
                resume={resume}
                onResumeUpdate={handleResumeUpdate}
                onSave={handleSave}
              />
            </TabsContent>

            <TabsContent value="preview" className="flex-1 overflow-hidden">
              <ResumePDFView resume={resume} />
            </TabsContent>

            <TabsContent value="settings" className="flex-1 overflow-auto p-6">
              <div className="max-w-2xl mx-auto space-y-6">
                <Card>
                  <CardHeader>
                    <CardTitle>Resume Settings</CardTitle>
                    <CardDescription>
                      Configure your resume preferences and export options
                    </CardDescription>
                  </CardHeader>
                  <CardContent className="space-y-4">
                    <div>
                      <h4 className="font-medium mb-2">Template</h4>
                      <p className="text-sm text-gray-600">
                        Current: Canadian Professional Template
                      </p>
                    </div>
                    
                    <div>
                      <h4 className="font-medium mb-2">ATS Score</h4>
                      <div className="flex items-center gap-2">
                        <Badge variant="secondary" className="text-sm">
                          {resume.atsScore || 85}/100
                        </Badge>
                        <span className="text-sm text-gray-600">
                          Optimized for Applicant Tracking Systems
                        </span>
                      </div>
                    </div>

                    <div>
                      <h4 className="font-medium mb-2">Generation Info</h4>
                      <div className="text-sm text-gray-600 space-y-1">
                        <p>Generated: {new Date(resume.createdAt).toLocaleDateString()}</p>
                        <p>Last Modified: {new Date(resume.updatedAt).toLocaleDateString()}</p>
                        <p>Version: {resume.version || '1.0'}</p>
                      </div>
                    </div>
                  </CardContent>
                </Card>
              </div>
            </TabsContent>
          </Tabs>
        </div>

        {/* Right Panel - Suggestions */}
        <div className="w-80 border-l bg-gray-50 overflow-y-auto">
          <SuggestionPanel
            resume={resume}
            onSuggestionApply={(suggestion) => {
              // Handle suggestion application
              console.log('Applying suggestion:', suggestion);
            }}
          />
        </div>
      </div>
    </div>
  );
}
```

## File: src/app/dashboard/resume/generator/page.tsx
```typescript
"use client";

import React, { useState, useEffect } from 'react';
import { useRouter } from 'next/navigation';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Alert, AlertDescription } from '@/components/ui/alert';
import { Input } from '@/components/ui/input';
import { Label } from '@/components/ui/label';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { 
  FileText, 
  Upload, 
  CheckCircle, 
  XCircle, 
  Loader2, 
  ArrowRight, 
  Plus,
  Search,
  Calendar,
  User,
  Briefcase,
  GraduationCap,
  Award,
  Star,
  Clock,
  TrendingUp
} from 'lucide-react';
import { useResumeGeneratorStore } from '@/stores/resumeGeneratorStore';
import { auth } from '@/lib/auth';

interface ResumeAnalysis {
  id: string;
  originalFileName: string;
  createdAt: string;
  personalInfo?: {
    name?: string;
    email?: string;
  };
  canadianMarketAnalysis?: {
    overallRelevance?: string;
    strengthsForCanadianMarket?: string[];
    potentialChallenges?: string[];
    recommendedImprovements?: string[];
    targetIndustries?: string[];
    confidence?: number;
  };
  confidenceScores?: {
    overall?: number;
  };
  metadata?: {
    processingMethod?: string;
    fileSize?: number;
  };
}

export default function ResumeGeneratorPage() {
  const router = useRouter();
  const [user, setUser] = useState<any>(null);
  const [isLoading, setIsLoading] = useState(true);
  const [resumeAnalyses, setResumeAnalyses] = useState<ResumeAnalysis[]>([]);
  const [selectedResumeId, setSelectedResumeId] = useState<string | null>(null);
  const [searchQuery, setSearchQuery] = useState('');
  const [uploadFile, setUploadFile] = useState<File | null>(null);
  const [isUploading, setIsUploading] = useState(false);
  const [error, setError] = useState<string | null>(null);

  const { setSelectedResumeId: setStoreSelectedResumeId } = useResumeGeneratorStore();

  useEffect(() => {
    const checkAuth = async () => {
      try {
        const currentUser = auth.getCurrentUser();
        setUser(currentUser);
        
        if (currentUser) {
          await loadResumeAnalyses();
        }
      } catch (error) {
        console.error('Auth check failed:', error);
        setError('Authentication failed. Please log in again.');
      } finally {
        setIsLoading(false);
      }
    };

    checkAuth();
  }, []);

  const loadResumeAnalyses = async () => {
    try {
      // Use auth token for fetching analyses (same approach as history page)
      const token = auth.getAuthToken() || 'guest-token';
      const currentUser = auth.getCurrentUser();
      
      console.log('🔐 Resume Generator - Using token:', token ? 'authenticated' : 'guest');
      console.log('👤 Resume Generator - Current user:', currentUser);
      
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/protected/ai-local/resume/analyses`, {
        headers: {
          'Authorization': `Bearer ${token}`
        }
      });

      console.log('📥 Resume Generator - Response status:', response.status);

      const result = await response.json();
      console.log('📥 Resume Generator - Response data:', result);
      
      if (result.success && result.data) {
        setResumeAnalyses(result.data);
      } else {
        console.error('❌ Resume Generator - API Error:', result.message);
        setError(result.message || 'Failed to load your resume analyses. Please try again.');
      }
    } catch (error) {
      console.error('Failed to load resume analyses:', error);
      setError('Failed to load your resume analyses. Please try again.');
    }
  };

  const handleResumeSelect = (analysisId: string) => {
    setSelectedResumeId(analysisId);
    setStoreSelectedResumeId(analysisId);
  };

  const handleFileUpload = (event: React.ChangeEvent<HTMLInputElement>) => {
    const file = event.target.files?.[0];
    if (file) {
      if (file.type !== 'application/pdf' && file.type !== 'application/msword' && file.type !== 'application/vnd.openxmlformats-officedocument.wordprocessingml.document') {
        setError('Please upload a PDF, DOC, or DOCX file.');
        return;
      }
      if (file.size > 10 * 1024 * 1024) { // 10MB limit
        setError('File size must be less than 10MB.');
        return;
      }
      setUploadFile(file);
      setError(null);
    }
  };

  const handleUploadAndAnalyze = async () => {
    if (!uploadFile) return;

    setIsUploading(true);
    setError(null);

    try {
      // TODO: Implement file upload and analysis
      // For now, we'll simulate the process
      await new Promise(resolve => setTimeout(resolve, 2000));
      
      // Navigate to job targeting page with the new analysis
      router.push('/dashboard/resume/generator/target');
    } catch (error) {
      console.error('Upload failed:', error);
      setError('Failed to upload and analyze resume. Please try again.');
    } finally {
      setIsUploading(false);
    }
  };

  const handleContinue = () => {
    if (selectedResumeId) {
      router.push('/dashboard/resume/generator/target');
    }
  };

  const filteredResumes = resumeAnalyses.filter(resume => 
    (resume.personalInfo?.name || '').toLowerCase().includes(searchQuery.toLowerCase()) ||
    (resume.originalFileName || '').toLowerCase().includes(searchQuery.toLowerCase()) ||
    (resume.canadianMarketAnalysis?.overallRelevance || '').toLowerCase().includes(searchQuery.toLowerCase())
  );

  const getConfidenceColor = (confidence: number) => {
    if (confidence >= 80) return 'bg-green-100 text-green-800';
    if (confidence >= 60) return 'bg-yellow-100 text-yellow-800';
    return 'bg-red-100 text-red-800';
  };

  const getConfidenceIcon = (confidence: number) => {
    if (confidence >= 80) return <CheckCircle className="h-4 w-4" />;
    if (confidence >= 60) return <Clock className="h-4 w-4" />;
    return <XCircle className="h-4 w-4" />;
  };

  const toPercentage = (value: number) => {
    if (value <= 1) {
      return Math.round(value * 100);
    }
    return Math.round(value);
  };

  if (isLoading) {
    return (
      <div className="container mx-auto p-6">
        <div className="flex items-center justify-center min-h-[400px]">
          <Loader2 className="h-8 w-8 animate-spin" />
          <span className="ml-2">Loading...</span>
        </div>
      </div>
    );
  }

  if (!user) {
    return (
      <div className="container mx-auto p-6">
        <Alert>
          <XCircle className="h-4 w-4" />
          <AlertDescription>
            Please log in to access the resume generator.
          </AlertDescription>
        </Alert>
      </div>
    );
  }

  return (
    <div className="container mx-auto p-6">
      <div className="mb-8">
        <h1 className="text-3xl font-bold text-gray-900 mb-2">
          Resume Generator
        </h1>
        <p className="text-gray-600">
          Select an existing resume analysis or upload a new resume to generate a Canadian-optimized version.
        </p>
      </div>

      {error && (
        <Alert className="mb-6">
          <XCircle className="h-4 w-4" />
          <AlertDescription>{error}</AlertDescription>
        </Alert>
      )}

      <Tabs defaultValue="existing" className="space-y-6">
        <TabsList className="grid w-full grid-cols-2">
          <TabsTrigger value="existing" className="flex items-center gap-2">
            <FileText className="h-4 w-4" />
            Existing Resumes
          </TabsTrigger>
          <TabsTrigger value="upload" className="flex items-center gap-2">
            <Upload className="h-4 w-4" />
            Upload New Resume
          </TabsTrigger>
        </TabsList>

        <TabsContent value="existing" className="space-y-6">
          <div className="flex items-center gap-4">
            <div className="relative flex-1">
              <Search className="absolute left-3 top-1/2 transform -translate-y-1/2 text-gray-400 h-4 w-4" />
              <Input
                placeholder="Search resumes by name, title, or company..."
                value={searchQuery}
                onChange={(e) => setSearchQuery(e.target.value)}
                className="pl-10"
              />
            </div>
          </div>

          {filteredResumes.length === 0 ? (
            <Card>
              <CardContent className="flex flex-col items-center justify-center py-12">
                <FileText className="h-12 w-12 text-gray-400 mb-4" />
                <h3 className="text-lg font-semibold text-gray-900 mb-2">
                  No resume analyses found
                </h3>
                <p className="text-gray-600 text-center mb-4">
                  {searchQuery ? 'No resumes match your search criteria.' : 'You haven\'t analyzed any resumes yet.'}
                </p>
                <Button 
                  onClick={() => router.push('/dashboard/resume')}
                  variant="outline"
                >
                  <Plus className="h-4 w-4 mr-2" />
                  Analyze a Resume
                </Button>
              </CardContent>
            </Card>
          ) : (
                         <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
               {filteredResumes.map((resume) => (
                 <Card 
                   key={resume.id}
                   className={`cursor-pointer transition-all hover:shadow-lg ${
                     selectedResumeId === resume.id 
                       ? 'ring-2 ring-blue-500 bg-blue-50' 
                       : ''
                   }`}
                   onClick={() => handleResumeSelect(resume.id)}
                 >
                   <CardHeader>
                     <div className="flex items-start justify-between">
                       <div className="flex-1">
                         <CardTitle className="text-lg mb-2">
                           {resume.personalInfo?.name || 'Unknown Name'}
                         </CardTitle>
                         <CardDescription className="line-clamp-2">
                           {resume.canadianMarketAnalysis?.overallRelevance || 'No summary available'}
                         </CardDescription>
                       </div>
                       {selectedResumeId === resume.id && (
                         <CheckCircle className="h-5 w-5 text-blue-500" />
                       )}
                     </div>
                   </CardHeader>
                   <CardContent className="space-y-3">
                     <div className="flex items-center gap-2 text-sm text-gray-600">
                       <FileText className="h-4 w-4" />
                       <span className="truncate">
                         {resume.originalFileName}
                       </span>
                     </div>
                     
                     <div className="flex items-center gap-2 text-sm text-gray-600">
                       <TrendingUp className="h-4 w-4" />
                       <span>
                         {resume.canadianMarketAnalysis?.targetIndustries?.length || 0} target industries
                       </span>
                     </div>

                     <div className="flex items-center gap-2 text-sm text-gray-600">
                       <Award className="h-4 w-4" />
                       <span>
                         {resume.canadianMarketAnalysis?.strengthsForCanadianMarket?.length || 0} strengths
                       </span>
                     </div>

                     <div className="flex items-center justify-between">
                       <Badge className={getConfidenceColor(resume.confidenceScores?.overall || 0)}>
                         <div className="flex items-center gap-1">
                           {getConfidenceIcon(resume.confidenceScores?.overall || 0)}
                           {toPercentage(resume.confidenceScores?.overall || 0)}% confidence
                         </div>
                       </Badge>
                       
                       <div className="flex items-center gap-1 text-xs text-gray-500">
                         <Calendar className="h-3 w-3" />
                         {new Date(resume.createdAt).toLocaleDateString()}
                       </div>
                     </div>
                   </CardContent>
                 </Card>
               ))}
             </div>
          )}
        </TabsContent>

        <TabsContent value="upload" className="space-y-6">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <Upload className="h-5 w-5" />
                Upload New Resume
              </CardTitle>
              <CardDescription>
                Upload a PDF, DOC, or DOCX file to analyze and generate a Canadian resume.
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              <div className="space-y-2">
                <Label htmlFor="resume-upload">Resume File</Label>
                <Input
                  id="resume-upload"
                  type="file"
                  accept=".pdf,.doc,.docx"
                  onChange={handleFileUpload}
                  className="cursor-pointer"
                />
                <p className="text-sm text-gray-500">
                  Maximum file size: 10MB. Supported formats: PDF, DOC, DOCX
                </p>
              </div>

              {uploadFile && (
                <div className="flex items-center gap-2 p-3 bg-green-50 border border-green-200 rounded-md">
                  <CheckCircle className="h-4 w-4 text-green-600" />
                  <span className="text-sm text-green-800">
                    Selected: {uploadFile.name}
                  </span>
                </div>
              )}

              <Button 
                onClick={handleUploadAndAnalyze}
                disabled={!uploadFile || isUploading}
                className="w-full"
              >
                {isUploading ? (
                  <>
                    <Loader2 className="h-4 w-4 mr-2 animate-spin" />
                    Uploading and Analyzing...
                  </>
                ) : (
                  <>
                    <Upload className="h-4 w-4 mr-2" />
                    Upload and Analyze
                  </>
                )}
              </Button>
            </CardContent>
          </Card>
        </TabsContent>
      </Tabs>

      {selectedResumeId && (
        <div className="fixed bottom-6 right-6">
          <Button 
            onClick={handleContinue}
            size="lg"
            className="shadow-lg"
          >
            Continue to Job Targeting
            <ArrowRight className="h-4 w-4 ml-2" />
          </Button>
        </div>
      )}
    </div>
  );
}
```

## File: src/app/dashboard/resume/generator/processing/page.tsx
```typescript
"use client";

import React, { useState, useEffect } from 'react';
import { useRouter } from 'next/navigation';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Alert, AlertDescription } from '@/components/ui/alert';
import { Progress } from '@/components/ui/progress';
import { 
  Loader2, 
  CheckCircle, 
  XCircle, 
  ArrowLeft,
  Sparkles,
  Brain,
  Target,
  FileText,
  Clock,
  AlertTriangle
} from 'lucide-react';
import { useResumeGeneratorStore } from '@/stores/resumeGeneratorStore';
import { auth } from '@/lib/auth';
import { generateCanadianResume } from '@/lib/api/resumeGenerator';
import GenerationProgress from '@/components/features/resume/generator/GenerationProgress';

interface GenerationStep {
  id: string;
  name: string;
  description: string;
  status: 'pending' | 'processing' | 'completed' | 'error';
  progress: number;
  estimatedTime: number;
}

const GENERATION_STEPS: GenerationStep[] = [
  {
    id: 'analysis',
    name: 'Resume Analysis',
    description: 'Analyzing your existing resume and extracting key information',
    status: 'pending',
    progress: 0,
    estimatedTime: 15
  },
  {
    id: 'targeting',
    name: 'Job Targeting Analysis',
    description: 'Analyzing job requirements and optimizing for the target position',
    status: 'pending',
    progress: 0,
    estimatedTime: 20
  },
  {
    id: 'translation',
    name: 'Skills Translation',
    description: 'Translating skills and experience for Canadian market',
    status: 'pending',
    progress: 0,
    estimatedTime: 25
  },
  {
    id: 'optimization',
    name: 'ATS Optimization',
    description: 'Optimizing resume for Applicant Tracking Systems',
    status: 'pending',
    progress: 0,
    estimatedTime: 30
  },
  {
    id: 'generation',
    name: 'Resume Generation',
    description: 'Generating your optimized Canadian resume',
    status: 'pending',
    progress: 0,
    estimatedTime: 35
  }
];

export default function GenerationProcessingPage() {
  const router = useRouter();
  const [user, setUser] = useState<any>(null);
  const [isLoading, setIsLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);
  const [steps, setSteps] = useState<GenerationStep[]>(GENERATION_STEPS);
  const [currentStep, setCurrentStep] = useState(0);
  const [overallProgress, setOverallProgress] = useState(0);
  const [estimatedTimeRemaining, setEstimatedTimeRemaining] = useState(0);
  const [generationId, setGenerationId] = useState<string | null>(null);
  const [isCompleted, setIsCompleted] = useState(false);

  const { 
    selectedResumeId, 
    jobTargeting, 
    validateJobTargeting,
    startGeneration: startStoreGeneration,
    updateGenerationProgress,
    failGeneration,
    resetGeneration
  } = useResumeGeneratorStore();

  useEffect(() => {
    const checkAuth = async () => {
      try {
        const currentUser = auth.getCurrentUser();
        setUser(currentUser);
        
        if (!currentUser) {
          setError('Authentication failed. Please log in again.');
        }
      } catch (error) {
        console.error('Auth check failed:', error);
        setError('Authentication failed. Please log in again.');
      } finally {
        setIsLoading(false);
      }
    };

    checkAuth();
  }, []);

  useEffect(() => {
    if (user && selectedResumeId) {
      startGeneration();
    }
  }, [user, selectedResumeId]);

  const startGeneration = async () => {
    try {
      // Validate job targeting
      const validation = validateJobTargeting();
      if (!validation.isValid) {
        setError('Please complete all required job targeting information.');
        return;
      }

      // Start the generation process using store functions
      startStoreGeneration();
      updateGenerationProgress(0, 'Starting generation...');

      // Start the generation process
      const response = await generateCanadianResume({
        originalAnalysisId: selectedResumeId,
        jobTargeting: jobTargeting
      });

      if (response.success) {
        setGenerationId(response.data.generationId);
        simulateGenerationProgress();
      } else {
        throw new Error(response.message || 'Failed to start generation');
      }
    } catch (error) {
      console.error('Generation failed:', error);
      const errorMessage = error instanceof Error ? error.message : 'Generation failed. Please try again.';
      setError(errorMessage);
      failGeneration(errorMessage);
    }
  };

  const simulateGenerationProgress = () => {
    let stepIndex = 0;
    let stepProgress = 0;
    let totalProgress = 0;

    const updateStep = () => {
      if (stepIndex >= steps.length) {
        completeGeneration();
        return;
      }

      const step = steps[stepIndex];
      setCurrentStep(stepIndex);
      updateGenerationProgress(totalProgress, `${step.name}...`);

      const stepInterval = setInterval(() => {
        stepProgress += Math.random() * 15 + 5; // 5-20% progress per interval

        if (stepProgress >= 100) {
          stepProgress = 100;
          clearInterval(stepInterval);
          
          // Mark step as completed
          setSteps(prev => prev.map((s, i) => 
            i === stepIndex 
              ? { ...s, status: 'completed', progress: 100 }
              : s
          ));

          // Move to next step
          stepIndex++;
          stepProgress = 0;
          setTimeout(updateStep, 500);
        } else {
          // Update current step progress
          setSteps(prev => prev.map((s, i) => 
            i === stepIndex 
              ? { ...s, status: 'processing', progress: stepProgress }
              : s
          ));

          // Update overall progress
          totalProgress = ((stepIndex * 100) + stepProgress) / steps.length;
          setOverallProgress(totalProgress);
          updateGenerationProgress(totalProgress, `${step.name}...`);

          // Update estimated time
          const remainingSteps = steps.length - stepIndex - 1;
          const estimatedTime = remainingSteps * 30 + (100 - stepProgress) / 20;
          setEstimatedTimeRemaining(estimatedTime);
        }
      }, 800); // Update every 800ms
    };

    updateStep();
  };

  const completeGeneration = () => {
    setOverallProgress(100);
    updateGenerationProgress(100, 'Generation completed!');
    setIsCompleted(true);

    // Redirect to editor after a short delay
    setTimeout(() => {
      if (generationId) {
        router.push(`/dashboard/resume/generator/edit/${generationId}`);
      }
    }, 2000);
  };

  const handleCancel = () => {
    // In a real implementation, this would cancel the generation on the backend
    resetGeneration();
    router.push('/dashboard/resume/generator');
  };

  const handleBack = () => {
    router.push('/dashboard/resume/generator/target');
  };

  if (isLoading) {
    return (
      <div className="container mx-auto p-6">
        <div className="flex items-center justify-center min-h-[400px]">
          <Loader2 className="h-8 w-8 animate-spin" />
          <span className="ml-2">Loading...</span>
        </div>
      </div>
    );
  }

  if (!user) {
    return (
      <div className="container mx-auto p-6">
        <Alert>
          <XCircle className="h-4 w-4" />
          <AlertDescription>
            Please log in to access the resume generator.
          </AlertDescription>
        </Alert>
      </div>
    );
  }

  if (!selectedResumeId) {
    return (
      <div className="container mx-auto p-6">
        <Alert>
          <AlertTriangle className="h-4 w-4" />
          <AlertDescription>
            Please select a resume first.
          </AlertDescription>
        </Alert>
        <Button onClick={handleBack} className="mt-4">
          <ArrowLeft className="h-4 w-4 mr-2" />
          Back to Resume Selection
        </Button>
      </div>
    );
  }

  return (
    <div className="container mx-auto p-6">
      <div className="mb-8">
        <div className="flex items-center gap-2 mb-2">
          <div className="flex items-center gap-2">
            <div className="w-8 h-8 bg-green-100 rounded-full flex items-center justify-center">
              <CheckCircle className="h-4 w-4 text-green-600" />
            </div>
            <span className="text-green-600 text-sm">Resume Selection</span>
          </div>
          <div className="flex-1 h-px bg-gray-300"></div>
          <div className="flex items-center gap-2">
            <div className="w-8 h-8 bg-green-100 rounded-full flex items-center justify-center">
              <CheckCircle className="h-4 w-4 text-green-600" />
            </div>
            <span className="text-green-600 text-sm">Job Targeting</span>
          </div>
          <div className="flex-1 h-px bg-gray-300"></div>
          <div className="flex items-center gap-2">
            <div className="w-8 h-8 bg-blue-600 rounded-full flex items-center justify-center">
              <span className="text-white font-semibold text-sm">3</span>
            </div>
            <span className="text-blue-600 font-medium text-sm">Generation</span>
          </div>
        </div>

        <h1 className="text-3xl font-bold text-gray-900 mb-2">
          Generating Your Resume
        </h1>
        <p className="text-gray-600">
          Our AI is analyzing your resume and creating an optimized version for Canadian employers.
        </p>
      </div>

      {error && (
        <Alert className="mb-6">
          <XCircle className="h-4 w-4" />
          <AlertDescription>{error}</AlertDescription>
        </Alert>
      )}

      <div className="grid grid-cols-1 lg:grid-cols-3 gap-6">
        {/* Main Progress */}
        <div className="lg:col-span-2">
          <GenerationProgress 
            steps={steps}
            currentStep={currentStep}
            overallProgress={overallProgress}
            estimatedTimeRemaining={estimatedTimeRemaining}
            isCompleted={isCompleted}
            onCancel={handleCancel}
          />
        </div>

        {/* Sidebar */}
        <div className="space-y-6">
          {/* Job Targeting Summary */}
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2 text-lg">
                <Target className="h-5 w-5 text-blue-600" />
                Job Targeting
              </CardTitle>
            </CardHeader>
            <CardContent className="space-y-3">
              <div>
                <h4 className="font-medium text-sm text-gray-700">Position</h4>
                <p className="text-sm text-gray-600">{jobTargeting.jobTitle}</p>
              </div>
              <div>
                <h4 className="font-medium text-sm text-gray-700">Company</h4>
                <p className="text-sm text-gray-600">{jobTargeting.companyName}</p>
              </div>
              {jobTargeting.location && (
                <div>
                  <h4 className="font-medium text-sm text-gray-700">Location</h4>
                  <p className="text-sm text-gray-600">{jobTargeting.location}</p>
                </div>
              )}
              {jobTargeting.industry && (
                <div>
                  <h4 className="font-medium text-sm text-gray-700">Industry</h4>
                  <p className="text-sm text-gray-600">{jobTargeting.industry}</p>
                </div>
              )}
            </CardContent>
          </Card>

          {/* AI Features */}
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2 text-lg">
                <Sparkles className="h-5 w-5 text-purple-600" />
                AI Features
              </CardTitle>
            </CardHeader>
            <CardContent className="space-y-3">
              <div className="flex items-center gap-2 text-sm">
                <Brain className="h-4 w-4 text-green-600" />
                <span>Canadian Market Optimization</span>
              </div>
              <div className="flex items-center gap-2 text-sm">
                <Target className="h-4 w-4 text-blue-600" />
                <span>ATS Score Optimization</span>
              </div>
              <div className="flex items-center gap-2 text-sm">
                <FileText className="h-4 w-4 text-orange-600" />
                <span>Skills Translation</span>
              </div>
              <div className="flex items-center gap-2 text-sm">
                <CheckCircle className="h-4 w-4 text-green-600" />
                <span>Keyword Matching</span>
              </div>
            </CardContent>
          </Card>

          {/* Estimated Time */}
          {!isCompleted && (
            <Card>
              <CardHeader>
                <CardTitle className="flex items-center gap-2 text-lg">
                  <Clock className="h-5 w-5 text-orange-600" />
                  Estimated Time
                </CardTitle>
              </CardHeader>
              <CardContent>
                <p className="text-2xl font-bold text-orange-600">
                  {Math.ceil(estimatedTimeRemaining)}s
                </p>
                <p className="text-sm text-gray-600">
                  Remaining time
                </p>
              </CardContent>
            </Card>
          )}
        </div>
      </div>

      {/* Navigation */}
      {!isCompleted && (
        <div className="flex justify-between items-center mt-8 pt-6 border-t">
          <Button onClick={handleBack} variant="outline">
            <ArrowLeft className="h-4 w-4 mr-2" />
            Back to Job Targeting
          </Button>

          <Button 
            onClick={handleCancel}
            variant="destructive"
            disabled={isCompleted}
          >
            Cancel Generation
          </Button>
        </div>
      )}
    </div>
  );
}
```

## File: src/app/dashboard/resume/page.tsx
```typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Alert } from '@/components/ui/alert';
import { Upload, FileText, CheckCircle, XCircle, Loader2, User, Briefcase, GraduationCap, Award, Globe, Zap, Target, TrendingUp, ArrowRight } from 'lucide-react';
import { auth } from '@/lib/auth';

interface ResumeAnalysis {
  analysisId?: string;
  personalInfo: {
    name: string;
    email: string;
    phone: string;
    location: string;
    confidence: number;
  };
  education: Array<{
    degree: string;
    institution: string;
    year: string;
    location: string;
    confidence: number;
  }>;
  workExperience: Array<{
    title: string;
    company: string;
    startDate: string;
    endDate: string;
    location: string;
    responsibilities: string[];
    confidence: number;
  }>;
  skills: {
    technical: string[];
    soft: string[];
    languages: Array<string | { language: string; proficiency: string }>;
    confidence: number;
  };
  certifications: Array<{
    name: string;
    issuer: string;
    year: string;
    confidence: number;
  }>;
  summary: {
    professionalSummary: string;
    careerLevel: string;
    industries: string[];
    confidence: number;
  };
  canadianMarketAnalysis?: {
    overallRelevance: 'High' | 'Medium' | 'Low';
    strengthsForCanadianMarket: string[];
    potentialChallenges: string[];
    recommendedImprovements: string[];
    targetIndustries: string[];
    salaryRangeEstimate: string;
    confidence: number;
  };
  positionRecommendations?: {
    position: string;
    successProbability: number;
    reasons: string[];
    skillMatch: number;
    salaryRange: string;
    marketDemand: string;
    immigrantFriendly: boolean;
    requiredSkills: string[];
    skillGaps: string[];
    confidence: number;
  }[];
  metadata?: {
    processedAt: string;
    originalFileName: string;
    processingMethod: 'direct_pdf' | 'text_extraction';
    apiVersion: string;
  };
}

interface PositionRecommendation {
  title: string;
  matchScore: number;
  successProbability: number;
  salaryRange: string;
  description: string;
  requiredSkills: string[];
  matchingSkills: string[];
  skillGaps: string[];
  marketDemand: string;
  growthPotential: string;
  immigrantFriendly: boolean;
  detailedAnalysis: {
    strengthsMatch: string[];
    potentialConcerns: string[];
    recommendedPreparation: string[];
  };
}

export default function ResumeUploadPage() {
  const [file, setFile] = useState(null);
  const [uploading, setUploading] = useState(false);
  const [analysis, setAnalysis] = useState(null);
  const [error, setError] = useState('');
  const [dragActive, setDragActive] = useState(false);
  const [generatingProfile, setGeneratingProfile] = useState(false);
  const [positionRecommendations, setPositionRecommendations] = useState([]);
  const [showPositionSelection, setShowPositionSelection] = useState(false);
  const [selectedPosition, setSelectedPosition] = useState(null);

  const handleDrag = (e) => {
    e.preventDefault();
    e.stopPropagation();
    if (e.type === "dragenter" || e.type === "dragover") {
      setDragActive(true);
    } else if (e.type === "dragleave") {
      setDragActive(false);
    }
  };

  const handleDrop = (e) => {
    e.preventDefault();
    e.stopPropagation();
    setDragActive(false);
    
    if (e.dataTransfer.files && e.dataTransfer.files[0]) {
      handleFileSelect(e.dataTransfer.files[0]);
    }
  };

  const handleFileSelect = (selectedFile) => {
    setError('');
    
    // Validate file type
    const allowedTypes = ['application/pdf', 'application/vnd.openxmlformats-officedocument.wordprocessingml.document', 'image/jpeg', 'image/png'];
    if (!allowedTypes.includes(selectedFile.type)) {
      setError('Please upload a PDF, DOCX, JPG, or PNG file');
      return;
    }
    
    // Validate file size (10MB - Enhanced with Gemini API)
    if (selectedFile.size > 10 * 1024 * 1024) {
      setError('File size must be less than 10MB');
      return;
    }
    
    setFile(selectedFile);
  };

  const uploadResume = async () => {
    if (!file) return;
    
    setUploading(true);
    setError('');
    
    try {
      const formData = new FormData();
      formData.append('resume', file);
      
      const token = auth.getAuthToken() || 'guest-token';
      const currentUser = auth.getCurrentUser();
      
      console.log('🔐 Frontend - Upload authentication status:');
      console.log('👤 Current user:', currentUser);
      console.log('🔐 Token type:', typeof token);
      console.log('🔐 Token length:', token ? token.length : 0);
      console.log('🔐 Is authenticated:', auth.isAuthenticated());
      
      console.log('Uploading to:', `${process.env.NEXT_PUBLIC_API_URL}/api/protected/ai-local/resume/upload`);
      
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/protected/ai-local/resume/upload`, {
        method: 'POST',
        headers: {
          'Authorization': `Bearer ${token}`
        },
        body: formData
      });
      
      console.log('Response status:', response.status);
      console.log('Response headers:', response.headers);
      
      // Check if response is JSON
      const contentType = response.headers.get('content-type');
      if (!contentType || !contentType.includes('application/json')) {
        const textResponse = await response.text();
        console.error('Non-JSON response:', textResponse);
        setError(`Server returned non-JSON response. Status: ${response.status}`);
        return;
      }
      
      const result = await response.json();
      console.log('Response result:', result);
      
      if (result.success) {
        console.log('✅ Analysis saved with ID:', result.data.analysisId);
        console.log('✅ Is guest user:', result.data.isGuest);
        setAnalysis(result.data.analysis);
      } else {
        setError(result.message || 'Failed to analyze resume');
      }
    } catch (err) {
      console.error('Upload error:', err);
      setError(`Upload failed: ${err.message}`);
    } finally {
      setUploading(false);
    }
  };

  const generateCareerProfile = async () => {
    setGeneratingProfile(true);
    setError('');
    
    try {
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/protected/ai-local/career-profile/position-recommendations`, {
        method: 'POST',
        headers: {
          'Authorization': `Bearer ${auth.getAuthToken() || 'guest-token'}`,
          'Content-Type': 'application/json'
        },
        body: JSON.stringify({
          resumeAnalysis: analysis
        })
      });
      
      const result = await response.json();
      if (result.success) {
        setPositionRecommendations(result.data.positions || []);
        setShowPositionSelection(true);
      } else {
        setError(result.message || 'Failed to generate position recommendations');
      }
    } catch (err) {
      console.error('Career profile generation error:', err);
      setError('Failed to generate career recommendations');
    } finally {
      setGeneratingProfile(false);
    }
  };

  const selectCareerPath = async (position) => {
    setSelectedPosition(position);
    
    try {
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/protected/ai-local/career-profile/enhanced-profile`, {
        method: 'POST',
        headers: {
          'Authorization': `Bearer ${auth.getAuthToken() || 'guest-token'}`,
          'Content-Type': 'application/json'
        },
        body: JSON.stringify({
          targetPosition: position,
          resumeAnalysis: analysis
        })
      });
      
      const result = await response.json();
      if (result.success) {
        // Redirect to career profile page with the generated data
        window.location.href = '/dashboard/career';
      } else {
        setError('Failed to generate enhanced profile');
      }
    } catch (err) {
      console.error('Enhanced profile generation error:', err);
      setError('Failed to generate enhanced profile');
    }
  };

  return (
    <div className="min-h-screen bg-gray-50">
      <div className="container mx-auto px-4 py-8 max-w-4xl">
        <div className="mb-8">
          <h1 className="text-3xl font-bold text-gray-900 mb-2">
            Resume Analysis
          </h1>
          <p className="text-gray-600">
            Upload your resume for AI-powered analysis and insights tailored for the Canadian job market
          </p>
        </div>

        {!analysis ? (
          <Card className="mb-6">
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <Upload className="h-5 w-5" />
                Upload Your Resume
              </CardTitle>
              <CardDescription>
                Supported formats: PDF, DOCX, JPG, PNG (Max 10MB) • Enhanced with Gemini Developer API
              </CardDescription>
            </CardHeader>
            <CardContent>
              {error && (
                <Alert className="mb-4 border-red-200 bg-red-50">
                  <XCircle className="h-4 w-4 text-red-500" />
                  <div className="text-red-700">{error}</div>
                </Alert>
              )}
              
              <div
                className={`border-2 border-dashed rounded-lg p-8 text-center transition-colors ${
                  dragActive ? 'border-blue-400 bg-blue-50' : 'border-gray-300'
                }`}
                onDragEnter={handleDrag}
                onDragLeave={handleDrag}
                onDragOver={handleDrag}
                onDrop={handleDrop}
              >
                {file ? (
                  <div className="space-y-4">
                    <FileText className="h-12 w-12 mx-auto text-green-500" />
                    <div>
                      <p className="font-medium text-gray-900">{file.name}</p>
                      <p className="text-sm text-gray-500">
                        {(file.size / 1024 / 1024).toFixed(2)} MB
                      </p>
                    </div>
                    <div className="flex gap-2 justify-center">
                      <Button 
                        onClick={uploadResume} 
                        disabled={uploading}
                        className="bg-blue-600 hover:bg-blue-700"
                      >
                        {uploading ? (
                          <>
                            <Loader2 className="h-4 w-4 mr-2 animate-spin" />
                            Analyzing...
                          </>
                        ) : (
                          'Analyze Resume'
                        )}
                      </Button>
                      <Button 
                        variant="outline" 
                        onClick={() => setFile(null)}
                        disabled={uploading}
                      >
                        Choose Different File
                      </Button>
                    </div>
                  </div>
                ) : (
                  <div className="space-y-4">
                    <Upload className="h-12 w-12 mx-auto text-gray-400" />
                    <div>
                      <p className="text-lg font-medium text-gray-900">
                        Drag and drop your resume here
                      </p>
                      <p className="text-gray-500">or</p>
                    </div>
                    <label>
                      <Button variant="outline" asChild>
                        <span className="cursor-pointer">
                          Browse Files
                        </span>
                      </Button>
                      <input
                        type="file"
                        className="hidden"
                        accept=".pdf,.docx,.jpg,.jpeg,.png"
                        onChange={(e) => e.target.files && handleFileSelect(e.target.files[0])}
                      />
                    </label>
                  </div>
                )}
              </div>
            </CardContent>
          </Card>
        ) : (
          <div className="space-y-6">
            <Alert className="border-green-200 bg-green-50">
              <CheckCircle className="h-4 w-4 text-green-500" />
              <div className="text-green-700">
                Resume analyzed successfully! Here are your results:
              </div>
            </Alert>

            {/* Personal Information */}
            <Card>
              <CardHeader>
                <CardTitle className="flex items-center gap-2">
                  <User className="h-5 w-5" />
                  Personal Information
                  <Badge variant="secondary">
                    {Math.round((analysis.personalInfo?.confidence || 0) * 100)}% confidence
                  </Badge>
                </CardTitle>
              </CardHeader>
              <CardContent>
                <div className="grid grid-cols-2 gap-4">
                  <div>
                    <p className="text-sm text-gray-500">Name</p>
                    <p className="font-medium">{analysis.personalInfo?.name || 'Not detected'}</p>
                  </div>
                  <div>
                    <p className="text-sm text-gray-500">Email</p>
                    <p className="font-medium">{analysis.personalInfo?.email || 'Not detected'}</p>
                  </div>
                  <div>
                    <p className="text-sm text-gray-500">Phone</p>
                    <p className="font-medium">{analysis.personalInfo?.phone || 'Not detected'}</p>
                  </div>
                  <div>
                    <p className="text-sm text-gray-500">Location</p>
                    <p className="font-medium">{analysis.personalInfo?.location || 'Not detected'}</p>
                  </div>
                </div>
              </CardContent>
            </Card>

            {/* Canadian Market Analysis - ALWAYS SHOW */}
            <Card className="border-2 border-red-200 bg-red-50">
              <CardHeader>
                <CardTitle className="flex items-center gap-2">
                  <Globe className="h-5 w-5 text-red-600" />
                  Canadian Market Analysis
                  <Badge variant="secondary" className="bg-red-100 text-red-700">
                    🇨🇦 Powered by Gemini AI
                  </Badge>
                </CardTitle>
                <CardDescription>
                  AI-powered analysis of your resume's compatibility with the Canadian job market
                </CardDescription>
              </CardHeader>
              <CardContent>
                {analysis.canadianMarketAnalysis ? (
                  <div className="space-y-4">
                    <div>
                      <p className="text-sm font-medium text-gray-700 mb-2">Market Relevance</p>
                      <Badge 
                        variant={
                          analysis.canadianMarketAnalysis.overallRelevance === 'High' ? 'default' :
                          analysis.canadianMarketAnalysis.overallRelevance === 'Medium' ? 'secondary' : 'outline'
                        }
                        className={`${
                          analysis.canadianMarketAnalysis.overallRelevance === 'High' ? 'bg-green-100 text-green-800' :
                          analysis.canadianMarketAnalysis.overallRelevance === 'Medium' ? 'bg-yellow-100 text-yellow-800' :
                          'bg-red-100 text-red-800'
                        }`}
                      >
                        {analysis.canadianMarketAnalysis.overallRelevance} Relevance
                      </Badge>
                    </div>
                    
                    {analysis.canadianMarketAnalysis.strengthsForCanadianMarket?.length > 0 && (
                      <div>
                        <p className="text-sm font-medium text-gray-700 mb-2">Canadian Market Strengths</p>
                        <ul className="list-disc list-inside space-y-1 text-sm text-gray-600">
                          {analysis.canadianMarketAnalysis.strengthsForCanadianMarket.map((strength, index) => (
                            <li key={index}>{strength}</li>
                          ))}
                        </ul>
                      </div>
                    )}
                    
                    {analysis.canadianMarketAnalysis.potentialChallenges?.length > 0 && (
                      <div>
                        <p className="text-sm font-medium text-gray-700 mb-2">Potential Challenges</p>
                        <ul className="list-disc list-inside space-y-1 text-sm text-red-600">
                          {analysis.canadianMarketAnalysis.potentialChallenges.map((challenge, index) => (
                            <li key={index}>{challenge}</li>
                          ))}
                        </ul>
                      </div>
                    )}
                    
                    {analysis.canadianMarketAnalysis.recommendedImprovements?.length > 0 && (
                      <div>
                        <p className="text-sm font-medium text-gray-700 mb-2">Recommended Improvements</p>
                        <ul className="list-disc list-inside space-y-1 text-sm text-blue-600">
                          {analysis.canadianMarketAnalysis.recommendedImprovements.map((improvement, index) => (
                            <li key={index}>{improvement}</li>
                          ))}
                        </ul>
                      </div>
                    )}
                    
                    {analysis.canadianMarketAnalysis.targetIndustries?.length > 0 && (
                      <div>
                        <p className="text-sm font-medium text-gray-700 mb-2">Target Industries in Canada</p>
                        <div className="flex flex-wrap gap-2">
                          {analysis.canadianMarketAnalysis.targetIndustries.map((industry, index) => (
                            <Badge key={index} variant="outline" className="bg-blue-50">
                              {industry}
                            </Badge>
                          ))}
                        </div>
                      </div>
                    )}
                    
                    {analysis.canadianMarketAnalysis.salaryRangeEstimate && (
                      <div>
                        <p className="text-sm font-medium text-gray-700 mb-2">Estimated Salary Range (CAD)</p>
                        <Badge variant="secondary" className="bg-green-100 text-green-700">
                          {analysis.canadianMarketAnalysis.salaryRangeEstimate}
                        </Badge>
                      </div>
                    )}
                  </div>
                ) : (
                  <div className="text-center py-8">
                    <Globe className="h-12 w-12 mx-auto text-gray-400 mb-4" />
                    <p className="text-gray-500 mb-2">Canadian Market Analysis will be generated with your resume analysis</p>
                    <p className="text-sm text-gray-400">Upload a resume to see tailored insights for the Canadian job market</p>
                  </div>
                )}
              </CardContent>
            </Card>

            {/* Skills */}
            <Card>
              <CardHeader>
                <CardTitle className="flex items-center gap-2">
                  <Award className="h-5 w-5" />
                  Skills
                  <Badge variant="secondary">
                    {Math.round((analysis.skills?.confidence || 0) * 100)}% confidence
                  </Badge>
                </CardTitle>
              </CardHeader>
              <CardContent>
                <div className="space-y-4">
                  <div>
                    <p className="text-sm font-medium text-gray-700 mb-2">Technical Skills</p>
                    <div className="flex flex-wrap gap-2">
                      {analysis.skills?.technical?.map((skill, index) => (
                        <Badge key={index} variant="outline">{skill}</Badge>
                      )) || <p className="text-gray-500">No technical skills detected</p>}
                    </div>
                  </div>
                  <div>
                    <p className="text-sm font-medium text-gray-700 mb-2">Soft Skills</p>
                    <div className="flex flex-wrap gap-2">
                      {analysis.skills?.soft?.map((skill, index) => (
                        <Badge key={index} variant="outline" className="bg-blue-50">{skill}</Badge>
                      )) || <p className="text-gray-500">No soft skills detected</p>}
                    </div>
                  </div>
                  <div>
                    <p className="text-sm font-medium text-gray-700 mb-2">Languages</p>
                    <div className="flex flex-wrap gap-2">
                      {analysis.skills?.languages?.map((lang, index) => (
                        <Badge key={index} variant="outline" className="bg-green-50">
                          {typeof lang === 'string' ? lang : `${lang.language} (${lang.proficiency})`}
                        </Badge>
                      )) || <p className="text-gray-500">No languages detected</p>}
                    </div>
                  </div>
                </div>
              </CardContent>
            </Card>

            {/* Work Experience */}
            <Card>
              <CardHeader>
                <CardTitle className="flex items-center gap-2">
                  <Briefcase className="h-5 w-5" />
                  Work Experience
                </CardTitle>
              </CardHeader>
              <CardContent>
                <div className="space-y-4">
                  {analysis.workExperience?.length > 0 ? (
                    analysis.workExperience.map((exp, index) => (
                      <div key={index} className="border-l-4 border-blue-500 pl-4">
                        <div className="flex justify-between items-start">
                          <div>
                            <h4 className="font-medium">{exp.title}</h4>
                            <p className="text-gray-600">{exp.company}</p>
                          </div>
                          <Badge variant="secondary">
                            {Math.round((exp.confidence || 0) * 100)}% confidence
                          </Badge>
                        </div>
                        <p className="text-sm text-gray-500">{exp.startDate} - {exp.endDate}</p>
                        <p className="text-sm text-gray-600 mt-1">{exp.location}</p>
                      </div>
                    ))
                  ) : (
                    <p className="text-gray-500">No work experience detected</p>
                  )}
                </div>
              </CardContent>
            </Card>

            {/* Education */}
            <Card>
              <CardHeader>
                <CardTitle className="flex items-center gap-2">
                  <GraduationCap className="h-5 w-5" />
                  Education
                </CardTitle>
              </CardHeader>
              <CardContent>
                <div className="space-y-3">
                  {analysis.education?.length > 0 ? (
                    analysis.education.map((edu, index) => (
                      <div key={index} className="flex justify-between items-start">
                        <div>
                          <h4 className="font-medium">{edu.degree}</h4>
                          <p className="text-gray-600">{edu.institution}</p>
                          <p className="text-sm text-gray-500">{edu.year} • {edu.location}</p>
                        </div>
                        <Badge variant="secondary">
                          {Math.round((edu.confidence || 0) * 100)}% confidence
                        </Badge>
                      </div>
                    ))
                  ) : (
                    <p className="text-gray-500">No education detected</p>
                  )}
                </div>
              </CardContent>
            </Card>

            {/* Position Recommendations Modal */}
            {showPositionSelection && (
              <Card className="border-2 border-green-200 bg-green-50">
                <CardHeader>
                  <CardTitle className="flex items-center gap-2">
                    <Target className="h-5 w-5 text-green-600" />
                    Recommended Career Paths
                    <Badge variant="secondary" className="bg-green-100 text-green-700">
                      Choose Your Path
                    </Badge>
                  </CardTitle>
                  <CardDescription>
                    Select a career path to generate your personalized career profile and development plan
                  </CardDescription>
                </CardHeader>
                <CardContent>
                  <div className="space-y-4">
                    {positionRecommendations.map((position, index) => (
                      <div key={index} className="border rounded-lg p-4 bg-white hover:bg-gray-50 transition-colors">
                        <div className="flex justify-between items-start mb-3">
                          <div>
                            <h4 className="font-semibold text-lg">{position.title}</h4>
                            <p className="text-gray-600 text-sm">{position.description}</p>
                          </div>
                          <div className="text-right">
                            <Badge variant="secondary" className="mb-1">
                              {Math.round(position.successProbability)}% Success Rate
                            </Badge>
                            <p className="text-sm text-gray-500">{position.salaryRange}</p>
                          </div>
                        </div>
                        
                        <div className="grid grid-cols-2 gap-4 mb-4">
                          <div>
                            <p className="text-sm font-medium text-gray-700 mb-1">Matching Skills</p>
                            <div className="flex flex-wrap gap-1">
                              {position.matchingSkills?.slice(0, 3).map((skill, idx) => (
                                <Badge key={idx} variant="outline" className="text-xs bg-green-50">
                                  {skill}
                                </Badge>
                              ))}
                              {position.matchingSkills?.length > 3 && (
                                <Badge variant="outline" className="text-xs">
                                  +{position.matchingSkills.length - 3} more
                                </Badge>
                              )}
                            </div>
                          </div>
                          <div>
                            <p className="text-sm font-medium text-gray-700 mb-1">Skill Gaps</p>
                            <div className="flex flex-wrap gap-1">
                              {position.skillGaps?.slice(0, 2).map((gap, idx) => (
                                <Badge key={idx} variant="outline" className="text-xs bg-red-50">
                                  {gap}
                                </Badge>
                              ))}
                              {position.skillGaps?.length > 2 && (
                                <Badge variant="outline" className="text-xs">
                                  +{position.skillGaps.length - 2} more
                                </Badge>
                              )}
                            </div>
                          </div>
                        </div>
                        
                        <div className="flex justify-between items-center">
                          <div className="flex items-center gap-4">
                            <Badge variant={position.immigrantFriendly ? 'default' : 'secondary'} className="text-xs">
                              {position.immigrantFriendly ? '🇨🇦 Immigrant Friendly' : 'Standard Requirements'}
                            </Badge>
                            <span className="text-sm text-gray-600">
                              <TrendingUp className="h-4 w-4 inline mr-1" />
                              {position.growthPotential}
                            </span>
                          </div>
                          <Button 
                            onClick={() => selectCareerPath(position)}
                            className="bg-green-600 hover:bg-green-700"
                          >
                            Select This Path
                            <ArrowRight className="h-4 w-4 ml-2" />
                          </Button>
                        </div>
                      </div>
                    ))}
                  </div>
                  
                  <div className="mt-4 pt-4 border-t">
                    <Button 
                      variant="outline" 
                      onClick={() => setShowPositionSelection(false)}
                      className="w-full"
                    >
                      Back to Resume Analysis
                    </Button>
                  </div>
                </CardContent>
              </Card>
            )}

            {/* Processing Method & Improvements */}
            <Card className="bg-gradient-to-r from-blue-50 to-purple-50 border-blue-200">
              <CardHeader>
                <CardTitle className="flex items-center gap-2">
                  <Zap className="h-5 w-5 text-blue-600" />
                  Enhanced Processing with Gemini API
                </CardTitle>
              </CardHeader>
              <CardContent>
                <div className="grid grid-cols-2 gap-4">
                  <div>
                    <p className="text-sm font-medium text-gray-700">Processing Method</p>
                    <Badge variant="secondary" className="bg-blue-100 text-blue-800">
                      {analysis.metadata?.processingMethod === 'direct_pdf' ? '📄 Direct PDF Reading' : '📝 Text Extraction'}
                    </Badge>
                  </div>
                  <div>
                    <p className="text-sm font-medium text-gray-700">API Version</p>
                    <Badge variant="secondary" className="bg-purple-100 text-purple-800">
                      {analysis.metadata?.apiVersion || 'gemini-1.5-flash'}
                    </Badge>
                  </div>
                  <div>
                    <p className="text-sm font-medium text-gray-700">Processing Speed</p>
                    <Badge variant="secondary" className="bg-green-100 text-green-800">
                      ⚡ 67x Faster
                    </Badge>
                  </div>
                  <div>
                    <p className="text-sm font-medium text-gray-700">File Size Limit</p>
                    <Badge variant="secondary" className="bg-yellow-100 text-yellow-800">
                      📁 Up to 10MB
                    </Badge>
                  </div>
                </div>
                <div className="mt-4 p-3 bg-white rounded-lg border">
                  <p className="text-xs text-gray-600">
                    <strong>🎯 Key Improvements:</strong> Direct PDF processing, 1000 requests/minute (vs 15 previously), 
                    enhanced Canadian job market analysis, better confidence scoring, and no intermediate file conversion needed.
                  </p>
                </div>
              </CardContent>
            </Card>

            {/* Action Buttons */}
            {!showPositionSelection && (
              <div className="flex gap-4">
                <Button 
                  onClick={generateCareerProfile}
                  disabled={generatingProfile}
                  className="bg-green-600 hover:bg-green-700"
                >
                  {generatingProfile ? (
                    <>
                      <Loader2 className="h-4 w-4 mr-2 animate-spin" />
                      Generating Career Paths...
                    </>
                  ) : (
                    <>
                      <Target className="h-4 w-4 mr-2" />
                      Generate Career Profile
                    </>
                  )}
                </Button>
                <Button 
                  variant="outline" 
                  onClick={() => {
                    setFile(null);
                    setAnalysis(null);
                    setError('');
                    setShowPositionSelection(false);
                    setPositionRecommendations([]);
                  }}
                >
                  Upload Another Resume
                </Button>
              </div>
            )}
          </div>
        )}
      </div>
    </div>
  );
}
```

## File: src/app/error.tsx
```typescript
'use client'

import { ErrorBoundary } from "@/components/common/ErrorBoundary"

export default function Error({
  error,
  reset,
}: {
  error: Error & { digest?: string }
  reset: () => void
}) {
  return (
    <html>
      <body>
        <ErrorBoundary error={error} reset={reset} />
      </body>
    </html>
  )
}
```

## File: src/app/layout.tsx
```typescript
import type { Metadata } from "next";
import { Poppins } from "next/font/google";
import "@/styles/globals.css";
//import { ThemeProvider } from "@/components/providers/theme-provider";
import "slick-carousel/slick/slick.css";
import "slick-carousel/slick/slick-theme.css";
// import Header from "@/components/Header";

const poppins = Poppins({
  variable: "--font-poppins",
  subsets: [],
  weight: "400",
});

export const metadata: Metadata = {
  title: "ImmiGrowAI",
  description: "ImmiGrowAI",
  icons: {
    icon: "/images/logos/logo.png",
  },
};

export default function RootLayout({
  children,
}: Readonly<{
  children: React.ReactNode;
}>) {
  return (
    <html lang="en" suppressHydrationWarning>
      <body
        className={`${poppins.variable} antialiased overscroll-y-none overscroll-none`}
      >
        {/* <ThemeProvider
          attribute="class"
          defaultTheme="system"
          enableSystem
          disableTransitionOnChange
        > */}
        {children}
        {/* </ThemeProvider> */}
      </body>
    </html>
  );
}
```

## File: src/app/loading.tsx
```typescript
import { LoadingSpinner } from "@/components/common/LoadingSpinner"

export default function Loading() {
  return (
    <div className="flex items-center justify-center min-h-screen">
      <div className="text-center">
        <LoadingSpinner size="lg" className="mx-auto mb-4" />
        <p className="text-muted-foreground">Loading...</p>
      </div>
    </div>
  )
}
```

## File: src/app/page.tsx
```typescript
import Header from "@/components/common/Header";
import Footer from "@/components/common/Footer";
import FeaturesPanel from "@/components/features/resume/FeaturesPanel";

export default function HomePage() {
  return (
    <div className="flex flex-col min-h-screen min-w-full bg-background">
      {/* Header */}
      <Header />
      <main className="flex-1">
        {/* AI Features Section */}
        <section className="py-20 bg-gray-50">
          <div className="container mx-auto px-4">
            <FeaturesPanel />
          </div>
        </section>
      </main>
      {/* Footer */}
      <Footer />
    </div>
  );
}
```

## File: src/components/common/__tests__/LoadingSpinner.test.tsx
```typescript
import React from 'react';
import { render, screen } from '@testing-library/react';
import { LoadingSpinner } from '../LoadingSpinner';

describe('LoadingSpinner', () => {
  it('renders with default props', () => {
    render(<LoadingSpinner />);
    
    const spinner = screen.getByRole('status');
    expect(spinner).toBeInTheDocument();
    expect(spinner).toHaveAttribute('aria-label', 'Loading');
  });

  it('renders with custom text', () => {
    render(<LoadingSpinner text="Loading data..." />);
    
    expect(screen.getByText('Loading data...')).toBeInTheDocument();
  });

  it('renders with showText prop', () => {
    render(<LoadingSpinner showText={true} />);
    
    expect(screen.getByText('Loading...')).toBeInTheDocument();
  });

  it('applies different size classes', () => {
    const { rerender } = render(<LoadingSpinner size="xs" />);
    expect(screen.getByRole('status')).toHaveClass('h-3', 'w-3');

    rerender(<LoadingSpinner size="sm" />);
    expect(screen.getByRole('status')).toHaveClass('h-4', 'w-4');

    rerender(<LoadingSpinner size="default" />);
    expect(screen.getByRole('status')).toHaveClass('h-6', 'w-6');

    rerender(<LoadingSpinner size="lg" />);
    expect(screen.getByRole('status')).toHaveClass('h-8', 'w-8');

    rerender(<LoadingSpinner size="xl" />);
    expect(screen.getByRole('status')).toHaveClass('h-12', 'w-12');
  });

  it('applies different color classes', () => {
    const { rerender } = render(<LoadingSpinner color="default" />);
    expect(screen.getByRole('status')).toHaveClass('text-foreground');

    rerender(<LoadingSpinner color="primary" />);
    expect(screen.getByRole('status')).toHaveClass('text-primary');

    rerender(<LoadingSpinner color="secondary" />);
    expect(screen.getByRole('status')).toHaveClass('text-secondary-foreground');

    rerender(<LoadingSpinner color="muted" />);
    expect(screen.getByRole('status')).toHaveClass('text-muted-foreground');
  });

  it('renders different variants', () => {
    const { rerender } = render(<LoadingSpinner variant="default" />);
    expect(screen.getByRole('status')).toHaveClass('animate-spin');

    rerender(<LoadingSpinner variant="dots" />);
    const dotsContainer = screen.getByRole('status');
    expect(dotsContainer.children.length).toBe(3);

    rerender(<LoadingSpinner variant="bars" />);
    const barsContainer = screen.getByRole('status');
    expect(barsContainer.children.length).toBe(3);

    rerender(<LoadingSpinner variant="pulse" />);
    expect(screen.getByRole('status')).toHaveClass('animate-pulse');
  });

  it('applies custom className', () => {
    render(<LoadingSpinner className="custom-spinner" />);
    
    expect(screen.getByRole('status')).toHaveClass('custom-spinner');
  });

  it('does not show text when showText is false and no text is provided', () => {
    render(<LoadingSpinner showText={false} />);
    
    expect(screen.queryByText('Loading...')).not.toBeInTheDocument();
  });
});
```

## File: src/components/common/Breadcrumbs.tsx
```typescript
import React from 'react';
import Link from 'next/link';
import { usePathname } from 'next/navigation';
import { cn } from '@/lib/utils';
import { ChevronRight, Home } from 'lucide-react';

export interface BreadcrumbItem {
  title: string;
  href: string;
  icon?: React.ComponentType<{ className?: string }>;
}

export interface BreadcrumbsProps {
  items?: BreadcrumbItem[];
  showHome?: boolean;
  homeTitle?: string;
  homeHref?: string;
  separator?: React.ReactNode;
  className?: string;
  maxItems?: number;
}

export const Breadcrumbs: React.FC<BreadcrumbsProps> = ({
  items,
  showHome = true,
  homeTitle = 'Home',
  homeHref = '/',
  separator = <ChevronRight className="h-4 w-4" />,
  className,
  maxItems = 5,
}) => {
  const pathname = usePathname();

  const generateBreadcrumbs = (): BreadcrumbItem[] => {
    if (items) {
      return items;
    }

    const pathSegments = pathname.split('/').filter(Boolean);
    const breadcrumbs: BreadcrumbItem[] = [];

    if (showHome) {
      breadcrumbs.push({
        title: homeTitle,
        href: homeHref,
        icon: Home,
      });
    }

    let currentPath = '';
    pathSegments.forEach((segment, index) => {
      currentPath += `/${segment}`;
      
      // Convert segment to title (capitalize and replace dashes/underscores)
      const title = segment
        .split(/[-_]/)
        .map(word => word.charAt(0).toUpperCase() + word.slice(1))
        .join(' ');

      breadcrumbs.push({
        title,
        href: currentPath,
      });
    });

    return breadcrumbs;
  };

  const breadcrumbItems = generateBreadcrumbs();

  // Limit the number of items if maxItems is set
  const limitedItems = maxItems && breadcrumbItems.length > maxItems
    ? [
        ...breadcrumbItems.slice(0, 1),
        { title: '...', href: '#' },
        ...breadcrumbItems.slice(-(maxItems - 2))
      ]
    : breadcrumbItems;

  if (breadcrumbItems.length <= 1) {
    return null;
  }

  return (
    <nav
      aria-label="Breadcrumb"
      className={cn('flex items-center space-x-1 text-sm text-muted-foreground', className)}
    >
      {limitedItems.map((item, index) => {
        const isLast = index === limitedItems.length - 1;
        const Icon = item.icon;

        if (isLast) {
          return (
            <span
              key={item.href}
              className="flex items-center gap-1 font-medium text-foreground"
              aria-current="page"
            >
              {Icon && <Icon className="h-4 w-4" />}
              {item.title}
            </span>
          );
        }

        if (item.title === '...') {
          return (
            <span key={`ellipsis-${index}`} className="flex items-center gap-1">
              {separator}
              <span className="px-1">...</span>
            </span>
          );
        }

        return (
          <React.Fragment key={item.href}>
            <Link
              href={item.href}
              className="flex items-center gap-1 hover:text-foreground transition-colors"
            >
              {Icon && <Icon className="h-4 w-4" />}
              {item.title}
            </Link>
            {!isLast && (
              <span className="flex items-center gap-1">
                {separator}
              </span>
            )}
          </React.Fragment>
        );
      })}
    </nav>
  );
};
```

## File: src/components/common/ErrorBoundary.tsx
```typescript
'use client';

import React, { Component, ErrorInfo, ReactNode } from 'react';
import { Button } from '@/components/ui/button';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { AlertTriangle, RefreshCw } from 'lucide-react';

interface Props {
  children: ReactNode;
  fallback?: ReactNode;
  onError?: (error: Error, errorInfo: ErrorInfo) => void;
}

interface State {
  hasError: boolean;
  error?: Error;
}

export class ErrorBoundary extends Component<Props, State> {
  constructor(props: Props) {
    super(props);
    this.state = { hasError: false };
  }

  static getDerivedStateFromError(error: Error): State {
    return { hasError: true, error };
  }

  componentDidCatch(error: Error, errorInfo: ErrorInfo) {
    console.error('ErrorBoundary caught an error:', error, errorInfo);
    
    // Call the onError callback if provided
    if (this.props.onError) {
      this.props.onError(error, errorInfo);
    }
  }

  handleReset = () => {
    this.setState({ hasError: false, error: undefined });
  };

  render() {
    if (this.state.hasError) {
      // Use custom fallback if provided
      if (this.props.fallback) {
        return this.props.fallback;
      }

      // Default error UI
      return (
        <div className="min-h-screen flex items-center justify-center p-4">
          <Card className="w-full max-w-md">
            <CardHeader className="text-center">
              <div className="mx-auto mb-4 flex h-12 w-12 items-center justify-center rounded-full bg-red-100">
                <AlertTriangle className="h-6 w-6 text-red-600" />
              </div>
              <CardTitle className="text-xl">Something went wrong</CardTitle>
              <CardDescription>
                An unexpected error occurred. Please try refreshing the page.
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              {process.env.NODE_ENV === 'development' && this.state.error && (
                <details className="rounded-md bg-gray-50 p-3 text-sm">
                  <summary className="cursor-pointer font-medium">Error Details</summary>
                  <pre className="mt-2 whitespace-pre-wrap text-xs">
                    {this.state.error.message}
                  </pre>
                </details>
              )}
              <div className="flex gap-2">
                <Button 
                  onClick={this.handleReset} 
                  variant="outline" 
                  className="flex-1"
                >
                  <RefreshCw className="mr-2 h-4 w-4" />
                  Try Again
                </Button>
                <Button 
                  onClick={() => window.location.reload()} 
                  className="flex-1"
                >
                  Refresh Page
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>
      );
    }

    return this.props.children;
  }
}

// Functional component wrapper for easier use
interface ErrorBoundaryWrapperProps {
  children: ReactNode;
  fallback?: ReactNode;
  onError?: (error: Error, errorInfo: ErrorInfo) => void;
}

export const ErrorBoundaryWrapper: React.FC<ErrorBoundaryWrapperProps> = ({
  children,
  fallback,
  onError,
}) => {
  return (
    <ErrorBoundary fallback={fallback} onError={onError}>
      {children}
    </ErrorBoundary>
  );
};

export default ErrorBoundary;
```

## File: src/components/common/Footer.tsx
```typescript
import React from "react";
import Logo from "@/components/common/Logo";
import { IoLogoLinkedin } from "react-icons/io5";
import { FaXTwitter } from "react-icons/fa6";
import { FaInstagram } from "react-icons/fa";
import Link from "next/link";

export default function Footer() {
  return (
    <footer className="container mx-auto text-center py-10">
      <div className="flex justify-evenly flex-wrap">
        <div className="flex flex-col">
          <Logo path="/" />
          <p className="text-sm mt-2">&copy; 2025 ImmiGrowAI</p>
          <p className="text-sm">Toronto, Ontario, Canada</p>
        </div>
        <div>
          <div className="flex justify-center mt-4 space-x-4">
            <Link
              href="#"
              aria-label="Linkedin"
            >
              <IoLogoLinkedin size={30} />
            </Link>
            <Link href="#" aria-label="X">
              <FaXTwitter size={30} />
            </Link>
            <Link href="#" aria-label="Instagram">
              <FaInstagram size={30} />
            </Link>
          </div>
        </div>
      </div>
      <div className="mt-6 px-4 text-sm">
        <p className="font-semibold">Land Acknowledgment</p>
        <p className="mt-2 md:px-40">
          At ImmiGrowAI, we acknowledge that we operate on the traditional
          territories of Indigenous Peoples across Canada. We honor the rich
          history, culture, and contributions of First Nations, Métis, and Inuit
          communities. We are committed to fostering respectful relationships
          with Indigenous Peoples and recognizing their enduring presence and
          rights within their ancestral lands. As we work to support newcomers
          in their journey to Canada, we strive to promote equity, inclusion,
          and understanding for all.
        </p>
      </div>
    </footer>
  );
}
```

## File: src/components/common/Header.tsx
```typescript
"use client";
import { useState, useEffect } from "react";
import { FiMenu, FiX, FiUser, FiLogOut } from "react-icons/fi";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import { usePathname, useRouter } from "next/navigation";
import Logo from "./Logo";
import ThemeSwitcher from "./ThemeSwitcher";
import { auth } from "@/lib/auth";

export default function Header() {
  const [isMenuOpen, setIsMenuOpen] = useState(false);
  const [user, setUser] = useState<any>(null);
  const [isLoading, setIsLoading] = useState(true);
  const pathname = usePathname();
  const router = useRouter();

  useEffect(() => {
    // Check authentication status on component mount
    const checkAuth = () => {
      const currentUser = auth.getCurrentUser();
      setUser(currentUser);
      setIsLoading(false);
    };

    checkAuth();
  }, []);

  const handleLogout = async () => {
    try {
      await auth.logout();
      setUser(null);
      router.push('/');
      // Refresh the page to update all components
      window.location.reload();
    } catch (error) {
      console.error('Logout error:', error);
    }
  };

  const getFirstName = (fullName: string) => {
    return fullName.split(' ')[0] || fullName;
  };

  return (
    <header className="border-b border-border px-4 md:px-8 py-4 sticky top-0 z-50 w-full bg-background/95 backdrop-blur supports-[backdrop-filter]:bg-background/60">
      <nav className="flex justify-between items-center">
        <Logo path={pathname} />
        {/* Mobile Menu Toggle Button */}
        <button
          className="md:hidden p-2"
          onClick={() => setIsMenuOpen(!isMenuOpen)}
        >
          {isMenuOpen ? <FiX size={24} /> : <FiMenu size={24} />}
        </button>

        {/* Right Actions */}
        <div className="hidden md:flex items-center gap-4">
          <ThemeSwitcher />
          
          {!isLoading && (
            <>
              {user ? (
                // Logged in user
                <div className="flex items-center gap-3">
                  <div className="flex items-center gap-2 text-sm">
                    <FiUser className="h-4 w-4 text-gray-600" />
                    <span className="text-gray-700">
                      Welcome, {getFirstName(user.fullName)}
                    </span>
                  </div>
                  <Button 
                    variant="outline" 
                    size="sm"
                    onClick={handleLogout}
                    className="flex items-center gap-2 text-red-600 border-red-200 hover:bg-red-50"
                  >
                    <FiLogOut className="h-4 w-4" />
                    Logout
                  </Button>
                </div>
              ) : (
                // Guest user
                <Button variant="outline" className="border-blue-600 text-blue-600 hover:bg-blue-50">
                  <Link href="/auth">
                    Login / Register
                  </Link>
                </Button>
              )}
            </>
          )}
          
          <Button variant="outline" className="border-gray-600 text-gray-600 hover:bg-gray-50">
            <Link href="/dashboard/profile">
              Dashboard
            </Link>
          </Button>
          
          <Button className="bg-blue-600 hover:bg-blue-500">
            <Link href="/dashboard/profile">
              <FiUser className="h-4 w-4 mr-2" />
              Profile
            </Link>
          </Button>
        </div>
      </nav>

      {/* Mobile Navigation Menu */}
      {isMenuOpen && (
        <div className="md:hidden flex flex-col items-center gap-4 px-4 py-4">
          <div className="flex flex-col items-center gap-4 mt-4">
            <ThemeSwitcher />
            
            {!isLoading && (
              <>
                {user ? (
                  // Logged in user (mobile)
                  <div className="flex flex-col items-center gap-3 w-full">
                    <div className="flex items-center gap-2 text-sm">
                      <FiUser className="h-4 w-4 text-gray-600" />
                      <span className="text-gray-700">
                        Welcome, {getFirstName(user.fullName)}
                      </span>
                    </div>
                    <Button 
                      variant="outline" 
                      size="sm"
                      onClick={handleLogout}
                      className="flex items-center gap-2 text-red-600 border-red-200 hover:bg-red-50 w-full"
                    >
                      <FiLogOut className="h-4 w-4" />
                      Logout
                    </Button>
                  </div>
                ) : (
                  // Guest user (mobile)
                  <Button variant="outline" className="border-blue-600 text-blue-600 hover:bg-blue-50 w-full">
                    <Link href="/auth">
                      Login / Register
                    </Link>
                  </Button>
                )}
              </>
            )}
            
            <Button variant="outline" className="border-gray-600 text-gray-600 hover:bg-gray-50 w-full">
              <Link href="/dashboard/profile">
                Dashboard
              </Link>
            </Button>
            
            <Button className="bg-blue-600 hover:bg-blue-500 w-full">
              <Link href="/dashboard/profile">
                <FiUser className="h-4 w-4 mr-2" />
                Profile
              </Link>
            </Button>
          </div>
        </div>
      )}
    </header>
  );
}
```

## File: src/components/common/index.ts
```typescript
export { default as Header } from './Header';
export { default as Footer } from './Footer';
export { default as Logo } from './Logo';
export { default as ThemeSwitcher } from './ThemeSwitcher';
export { default as UserProfile } from './UserProfile';
export { default as Navigation } from './Navigation';
export { default as Sidebar } from './Sidebar';
export { default as Breadcrumbs } from './Breadcrumbs';
export { default as LoadingSpinner } from './LoadingSpinner';
export { default as ErrorBoundary } from './ErrorBoundary';
```

## File: src/components/common/LoadingSpinner.tsx
```typescript
'use client';

import React from 'react';
import { cn } from '@/lib/utils';
import { Loader2 } from 'lucide-react';

export interface LoadingSpinnerProps {
  size?: 'sm' | 'md' | 'lg' | 'xl';
  className?: string;
  text?: string;
  variant?: 'default' | 'overlay' | 'inline';
}

const sizeClasses = {
  sm: 'h-4 w-4',
  md: 'h-6 w-6',
  lg: 'h-8 w-8',
  xl: 'h-12 w-12',
};

export const LoadingSpinner: React.FC<LoadingSpinnerProps> = ({
  size = 'md',
  className,
  text,
  variant = 'default',
}) => {
  const spinner = (
    <Loader2 
      className={cn(
        'animate-spin text-primary',
        sizeClasses[size],
        className
      )} 
    />
  );

  if (variant === 'overlay') {
    return (
      <div className="fixed inset-0 z-50 flex items-center justify-center bg-background/80 backdrop-blur-sm">
        <div className="flex flex-col items-center gap-2">
          {spinner}
          {text && (
            <p className="text-sm text-muted-foreground">{text}</p>
          )}
        </div>
      </div>
    );
  }

  if (variant === 'inline') {
    return (
      <div className="flex items-center gap-2">
        {spinner}
        {text && (
          <span className="text-sm text-muted-foreground">{text}</span>
        )}
      </div>
    );
  }

  return (
    <div className="flex flex-col items-center justify-center gap-2">
      {spinner}
      {text && (
        <p className="text-sm text-muted-foreground">{text}</p>
      )}
    </div>
  );
};

// Convenience components for common use cases
export const LoadingOverlay: React.FC<Omit<LoadingSpinnerProps, 'variant'>> = (props) => (
  <LoadingSpinner {...props} variant="overlay" />
);

export const InlineLoading: React.FC<Omit<LoadingSpinnerProps, 'variant'>> = (props) => (
  <LoadingSpinner {...props} variant="inline" />
);

export default LoadingSpinner;
```

## File: src/components/common/Logo.tsx
```typescript
import Image from "next/image";
import Link from "next/link";
// import { usePathname } from "next/navigation";
import React from "react";
// import logo from "./public/logo.png";

const Logo = ({ path }: { path: string }) => {
  // const pathname = usePathname();
  const isProtectedPath =
    path?.startsWith("/dashboard") || path?.startsWith("/onboarding");
  return (
    <Link
      className="flex gap-1 justify-center items-center"
      href={isProtectedPath ? path : "/"}
    >
              <Image src={"/images/logos/logo.png"} width={40} height={40} alt="ImmiGrowAI" />
      <p className="text-3xl font-bold tracking-tighter">ImmiGrowAI</p>
    </Link>
  );
};

export default Logo;
```

## File: src/components/common/Navigation.tsx
```typescript
import React from 'react';
import Link from 'next/link';
import { usePathname } from 'next/navigation';
import { cn } from '@/lib/utils';
import { Button } from '@/components/ui/button';
import { 
  DropdownMenu,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuTrigger,
} from '@/components/ui/dropdown-menu';
import { ChevronDown, Menu } from 'lucide-react';

export interface NavigationItem {
  title: string;
  href: string;
  children?: Omit<NavigationItem, 'children'>[];
  disabled?: boolean;
  external?: boolean;
}

export interface NavigationProps {
  items?: NavigationItem[];
  className?: string;
  variant?: 'horizontal' | 'vertical' | 'mobile';
  showMobileMenu?: boolean;
  onMobileMenuToggle?: () => void;
}

const defaultItems: NavigationItem[] = [
  {
    title: 'Home',
    href: '/',
  },
  {
    title: 'Features',
    href: '/features',
    children: [
      {
        title: 'Resume Analysis',
        href: '/features/resume-analysis',
      },
      {
        title: 'Career Guidance',
        href: '/features/career-guidance',
      },
      {
        title: 'Job Search',
        href: '/features/job-search',
      },
    ],
  },
  {
    title: 'Pricing',
    href: '/pricing',
  },
  {
    title: 'About',
    href: '/about',
  },
  {
    title: 'Contact',
    href: '/contact',
  },
];

export const Navigation: React.FC<NavigationProps> = ({
  items = defaultItems,
  className,
  variant = 'horizontal',
  showMobileMenu = false,
  onMobileMenuToggle,
}) => {
  const pathname = usePathname();

  const isActive = (href: string) => {
    if (href === '/') {
      return pathname === '/';
    }
    return pathname.startsWith(href);
  };

  const renderItem = (item: NavigationItem) => {
    const active = isActive(item.href);
    const hasChildren = item.children && item.children.length > 0;

    if (hasChildren) {
      return (
        <DropdownMenu key={item.href}>
          <DropdownMenuTrigger asChild>
            <Button
              variant="ghost"
              className={cn(
                'flex items-center gap-1',
                active && 'bg-accent text-accent-foreground',
                item.disabled && 'opacity-50 cursor-not-allowed'
              )}
              disabled={item.disabled}
            >
              {item.title}
              <ChevronDown className="h-4 w-4" />
            </Button>
          </DropdownMenuTrigger>
          <DropdownMenuContent align="start" className="w-48">
            {item.children?.map((child) => (
              <DropdownMenuItem key={child.href} asChild>
                <Link
                  href={child.href}
                  className={cn(
                    'w-full',
                    isActive(child.href) && 'bg-accent'
                  )}
                >
                  {child.title}
                </Link>
              </DropdownMenuItem>
            ))}
          </DropdownMenuContent>
        </DropdownMenu>
      );
    }

    if (item.external) {
      return (
        <a
          key={item.href}
          href={item.href}
          target="_blank"
          rel="noopener noreferrer"
          className={cn(
            'flex items-center px-3 py-2 text-sm font-medium transition-colors',
            'hover:bg-accent hover:text-accent-foreground',
            active && 'bg-accent text-accent-foreground',
            item.disabled && 'opacity-50 cursor-not-allowed'
          )}
        >
          {item.title}
        </a>
      );
    }

    return (
      <Link
        key={item.href}
        href={item.href}
        className={cn(
          'flex items-center px-3 py-2 text-sm font-medium transition-colors',
          'hover:bg-accent hover:text-accent-foreground',
          active && 'bg-accent text-accent-foreground',
          item.disabled && 'opacity-50 cursor-not-allowed'
        )}
        onClick={item.disabled ? (e) => e.preventDefault() : undefined}
      >
        {item.title}
      </Link>
    );
  };

  if (variant === 'mobile') {
    return (
      <div className={cn('flex flex-col space-y-2', className)}>
        {items.map(renderItem)}
      </div>
    );
  }

  if (variant === 'vertical') {
    return (
      <nav className={cn('flex flex-col space-y-1', className)}>
        {items.map(renderItem)}
      </nav>
    );
  }

  return (
    <nav className={cn('flex items-center space-x-4', className)}>
      {/* Desktop Navigation */}
      <div className="hidden md:flex items-center space-x-4">
        {items.map(renderItem)}
      </div>

      {/* Mobile Menu Button */}
      <Button
        variant="ghost"
        size="sm"
        className="md:hidden"
        onClick={onMobileMenuToggle}
      >
        <Menu className="h-5 w-5" />
      </Button>

      {/* Mobile Menu */}
      {showMobileMenu && (
        <div className="absolute top-full left-0 right-0 bg-background border-b md:hidden">
          <div className="px-4 py-2">
            <Navigation
              items={items}
              variant="mobile"
            />
          </div>
        </div>
      )}
    </nav>
  );
};
```

## File: src/components/common/Sidebar.tsx
```typescript
import React from 'react';
import Link from 'next/link';
import { usePathname } from 'next/navigation';
import { cn } from '@/lib/utils';
import { Button } from '@/components/ui/button';
import { ScrollArea } from '@/components/ui/scroll-area';
import { 
  Home, 
  User, 
  FileText, 
  Briefcase, 
  Settings, 

  Search,
  History,
  BookOpen,
  ChevronLeft,
  ChevronRight
} from 'lucide-react';

export interface SidebarItem {
  title: string;
  href: string;
  icon: React.ComponentType<{ className?: string }>;
  badge?: string | number;
  disabled?: boolean;
  children?: Omit<SidebarItem, 'children'>[];
}

export interface SidebarProps {
  items?: SidebarItem[];
  collapsed?: boolean;
  onToggle?: () => void;
  className?: string;
  showToggle?: boolean;
}

const defaultItems: SidebarItem[] = [
  {
    title: 'Dashboard',
    href: '/dashboard',
    icon: Home,
  },
  {
    title: 'Resume Analysis',
    href: '/dashboard/resume',
    icon: FileText,
  },
  {
    title: 'Career Profile',
    href: '/dashboard/career',
    icon: User,
  },
  {
    title: 'Analysis History',
    href: '/dashboard/history',
    icon: History,
  },
  {
    title: 'Career',
    href: '/dashboard/career',
    icon: Briefcase,
    children: [
      {
        title: 'Job Search',
        href: '/dashboard/career/search',
        icon: Search,
      },
      {
        title: 'Learning',
        href: '/dashboard/career/learning',
        icon: BookOpen,
      },
    ],
  },
  {
    title: 'Profile',
    href: '/dashboard/profile',
    icon: User,
  },
  {
    title: 'Settings',
    href: '/dashboard/profile/settings',
    icon: Settings,
  },
];

export const Sidebar: React.FC<SidebarProps> = ({
  items = defaultItems,
  collapsed = false,
  onToggle,
  className,
  showToggle = true,
}) => {
  const pathname = usePathname();

  const isActive = (href: string) => {
    if (href === '/dashboard') {
      return pathname === '/dashboard';
    }
    return pathname.startsWith(href);
  };

  const renderItem = (item: SidebarItem, isChild = false) => {
    const Icon = item.icon;
    const active = isActive(item.href);

    return (
      <Link
        key={item.href}
        href={item.disabled ? '#' : item.href}
        className={cn(
          'flex items-center gap-3 rounded-lg px-3 py-2 text-sm font-medium transition-colors',
          'hover:bg-accent hover:text-accent-foreground',
          active && 'bg-accent text-accent-foreground',
          item.disabled && 'opacity-50 cursor-not-allowed',
          isChild && 'ml-4',
          collapsed && 'justify-center'
        )}
        onClick={item.disabled ? (e) => e.preventDefault() : undefined}
      >
        <Icon className={cn('h-4 w-4', collapsed && 'h-5 w-5')} />
        {!collapsed && (
          <>
            <span className="truncate">{item.title}</span>
            {item.badge && (
              <span className="ml-auto rounded-full bg-primary px-2 py-0.5 text-xs text-primary-foreground">
                {item.badge}
              </span>
            )}
          </>
        )}
      </Link>
    );
  };

  return (
    <div
      className={cn(
        'flex h-full flex-col border-r bg-background',
        collapsed ? 'w-16' : 'w-64',
        className
      )}
    >
      {/* Header */}
      <div className="flex h-14 items-center border-b px-4">
        {!collapsed && (
          <h2 className="text-lg font-semibold">ImmiGrow AI</h2>
        )}
        {showToggle && (
          <Button
            variant="ghost"
            size="sm"
            onClick={onToggle}
            className={cn(
              'ml-auto h-8 w-8 p-0',
              collapsed && 'mx-auto'
            )}
          >
            {collapsed ? (
              <ChevronRight className="h-4 w-4" />
            ) : (
              <ChevronLeft className="h-4 w-4" />
            )}
          </Button>
        )}
      </div>

      {/* Navigation */}
      <ScrollArea className="flex-1 px-3 py-4">
        <nav className="space-y-2">
          {items.map((item) => (
            <div key={item.href}>
              {renderItem(item)}
              {!collapsed && item.children && (
                <div className="mt-2 space-y-1">
                  {item.children.map((child) => renderItem(child, true))}
                </div>
              )}
            </div>
          ))}
        </nav>
      </ScrollArea>
    </div>
  );
};
```

## File: src/components/common/ThemeSwitcher.tsx
```typescript
"use client";

import { useTheme } from "next-themes";
import React, { useEffect } from "react";
import { Tabs, TabsList, TabsTrigger } from "@/components/ui/tabs";
import { FaSun, FaMoon, FaLaptop } from "react-icons/fa";

function ThemeSwitcher() {
  const { theme, setTheme } = useTheme();
  const [mounted, setMounted] = React.useState(false);

  useEffect(() => {
    setMounted(true);
  }, []);

  if (!mounted) return null;

  return (
    <Tabs defaultValue={theme}>
      <TabsList className="border">
        <TabsTrigger value="light" onClick={() => setTheme("light")}>
          <FaSun size={16} />
        </TabsTrigger>
        <TabsTrigger value="dark" onClick={() => setTheme("dark")}>
          <FaMoon size={16} />
        </TabsTrigger>
        <TabsTrigger value="system" onClick={() => setTheme("system")}>
          <FaLaptop size={16} />
        </TabsTrigger>
      </TabsList>
    </Tabs>
  );
}

export default ThemeSwitcher;
```

## File: src/components/common/UserProfile.tsx
```typescript
"use client";

import { useState, useEffect } from "react";
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Badge } from "@/components/ui/badge";
import { FiUser, FiMail, FiPhone, FiMapPin, FiFlag, FiCalendar } from "react-icons/fi";
import { auth } from "@/lib/auth";

interface UserProfileProps {
  className?: string;
}

export default function UserProfile({ className = "" }: UserProfileProps) {
  const [user, setUser] = useState<any>(null);
  const [isLoading, setIsLoading] = useState(true);

  useEffect(() => {
    const checkAuth = () => {
      const currentUser = auth.getCurrentUser();
      setUser(currentUser);
      setIsLoading(false);
    };

    checkAuth();
  }, []);

  const getStatusBadgeColor = (status: string) => {
    switch (status) {
      case 'permanent_resident':
        return 'bg-green-100 text-green-800';
      case 'work_permit':
        return 'bg-blue-100 text-blue-800';
      case 'student_visa':
        return 'bg-purple-100 text-purple-800';
      case 'citizen':
        return 'bg-emerald-100 text-emerald-800';
      default:
        return 'bg-gray-100 text-gray-800';
    }
  };

  const getStatusDisplayName = (status: string) => {
    switch (status) {
      case 'permanent_resident':
        return 'Permanent Resident';
      case 'work_permit':
        return 'Work Permit';
      case 'student_visa':
        return 'Student Visa';
      case 'visitor_visa':
        return 'Visitor Visa';
      case 'citizen':
        return 'Canadian Citizen';
      case 'not_in_canada':
        return 'Not in Canada';
      default:
        return status || 'Not specified';
    }
  };

  if (isLoading) {
    return (
      <Card className={className}>
        <CardHeader>
          <CardTitle>Profile</CardTitle>
          <CardDescription>Loading user information...</CardDescription>
        </CardHeader>
      </Card>
    );
  }

  if (!user) {
    return (
      <Card className={className}>
        <CardHeader>
          <CardTitle>Profile</CardTitle>
          <CardDescription>Please log in to view your profile</CardDescription>
        </CardHeader>
        <CardContent>
          <Button asChild>
            <a href="/auth">Login / Register</a>
          </Button>
        </CardContent>
      </Card>
    );
  }

  return (
    <Card className={className}>
      <CardHeader>
        <CardTitle className="flex items-center gap-2">
          <FiUser className="h-5 w-5" />
          Profile Information
        </CardTitle>
        <CardDescription>Your account details and preferences</CardDescription>
      </CardHeader>
      <CardContent className="space-y-4">
        {/* Basic Info */}
        <div className="space-y-3">
          <div className="flex items-center gap-3">
            <FiUser className="h-4 w-4 text-gray-500" />
            <div>
              <p className="font-medium">{user.fullName}</p>
              <p className="text-sm text-gray-500">Full Name</p>
            </div>
          </div>
          
          <div className="flex items-center gap-3">
            <FiMail className="h-4 w-4 text-gray-500" />
            <div>
              <p className="font-medium">{user.email}</p>
              <p className="text-sm text-gray-500">Email Address</p>
            </div>
          </div>
        </div>

        {/* Additional Info (if available) */}
        {user.phoneNo && (
          <div className="flex items-center gap-3">
            <FiPhone className="h-4 w-4 text-gray-500" />
            <div>
              <p className="font-medium">{user.phoneNo}</p>
              <p className="text-sm text-gray-500">Phone Number</p>
            </div>
          </div>
        )}

        {user.statusInCanada && (
          <div className="flex items-center gap-3">
            <FiFlag className="h-4 w-4 text-gray-500" />
            <div>
              <Badge className={getStatusBadgeColor(user.statusInCanada)}>
                {getStatusDisplayName(user.statusInCanada)}
              </Badge>
              <p className="text-sm text-gray-500 mt-1">Status in Canada</p>
            </div>
          </div>
        )}

        {user.countryOfOrigin && (
          <div className="flex items-center gap-3">
            <FiMapPin className="h-4 w-4 text-gray-500" />
            <div>
              <p className="font-medium">{user.countryOfOrigin}</p>
              <p className="text-sm text-gray-500">Country of Origin</p>
            </div>
          </div>
        )}

        {user.currentLocation && (
          <div className="flex items-center gap-3">
            <FiMapPin className="h-4 w-4 text-gray-500" />
            <div>
              <p className="font-medium">{user.currentLocation}</p>
              <p className="text-sm text-gray-500">Current Location</p>
            </div>
          </div>
        )}

        {/* Account Info */}
        <div className="pt-4 border-t">
          <div className="flex items-center gap-3">
            <FiCalendar className="h-4 w-4 text-gray-500" />
            <div>
              <p className="font-medium">Member since {new Date().toLocaleDateString()}</p>
              <p className="text-sm text-gray-500">Account created</p>
            </div>
          </div>
        </div>

        {/* Actions */}
        <div className="pt-4 border-t space-y-2">
          <Button variant="outline" className="w-full">
            Edit Profile
          </Button>
          <Button 
            variant="outline" 
            className="w-full text-red-600 border-red-200 hover:bg-red-50"
            onClick={async () => {
              try {
                await auth.logout();
                window.location.reload();
              } catch (error) {
                console.error('Logout error:', error);
              }
            }}
          >
            Logout
          </Button>
        </div>
      </CardContent>
    </Card>
  );
}
```

## File: src/components/features/auth/AuthDebug.tsx
```typescript
'use client';

import React, { useState, useEffect } from 'react';
import { Button } from '@/components/ui/button';
import { Card, CardContent, CardHeader, CardTitle } from '@/components/ui/card';
import { auth } from '@/lib/auth';

export default function AuthDebug() {
  const [authStatus, setAuthStatus] = useState<any>(null);
  const [loading, setLoading] = useState(false);
  const [error, setError] = useState<string | null>(null);

  const checkAuthStatus = async () => {
    setLoading(true);
    setError(null);
    
    try {
      const token = auth.getAuthToken();
      const currentUser = auth.getCurrentUser();
      
      console.log('🔐 Frontend Auth Debug:');
      console.log('Token:', token ? 'Present' : 'Missing');
      console.log('Current User:', currentUser);
      console.log('Is Authenticated:', auth.isAuthenticated());
      
      if (!token) {
        setAuthStatus({
          frontend: {
            token: 'Missing',
            currentUser,
            isAuthenticated: auth.isAuthenticated()
          },
          backend: null
        });
        return;
      }
      
      // Call backend debug endpoint
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/protected/ai-local/debug-auth`, {
        headers: {
          'Authorization': `Bearer ${token}`
        }
      });
      
      const result = await response.json();
      
      setAuthStatus({
        frontend: {
          token: token ? 'Present' : 'Missing',
          currentUser,
          isAuthenticated: auth.isAuthenticated()
        },
        backend: result.success ? result.data : null
      });
      
    } catch (err: any) {
      console.error('Auth debug error:', err);
      setError(err.message);
    } finally {
      setLoading(false);
    }
  };

  useEffect(() => {
    checkAuthStatus();
  }, []);

  return (
    <Card className="w-full max-w-4xl mx-auto">
      <CardHeader>
        <CardTitle className="flex items-center justify-between">
          Authentication Debug
          <Button onClick={checkAuthStatus} disabled={loading}>
            {loading ? 'Checking...' : 'Refresh'}
          </Button>
        </CardTitle>
      </CardHeader>
      <CardContent>
        {error && (
          <div className="mb-4 p-3 bg-red-50 border border-red-200 rounded text-red-700">
            Error: {error}
          </div>
        )}
        
        {authStatus && (
          <div className="space-y-4">
            <div>
              <h3 className="font-semibold mb-2">Frontend Status</h3>
              <pre className="bg-gray-50 p-3 rounded text-sm overflow-auto">
                {JSON.stringify(authStatus.frontend, null, 2)}
              </pre>
            </div>
            
            {authStatus.backend && (
              <div>
                <h3 className="font-semibold mb-2">Backend Status</h3>
                <pre className="bg-gray-50 p-3 rounded text-sm overflow-auto">
                  {JSON.stringify(authStatus.backend, null, 2)}
                </pre>
              </div>
            )}
            
            {!authStatus.backend && authStatus.frontend.token === 'Present' && (
              <div className="p-3 bg-yellow-50 border border-yellow-200 rounded text-yellow-700">
                ⚠️ Token present but backend authentication failed. Check console for details.
              </div>
            )}
          </div>
        )}
      </CardContent>
    </Card>
  );
}
```

## File: src/components/features/auth/index.ts
```typescript
export * from './LoginForm'
export * from './RegisterForm'
export * from './AuthDebug'
```

## File: src/components/features/auth/LoginForm.tsx
```typescript
'use client';

import { useState } from 'react';
import { Button } from '@/components/ui/button';
import { Input } from '@/components/ui/input';
import { Label } from '@/components/ui/label';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Alert, AlertDescription } from '@/components/ui/alert';
import { auth } from '@/lib/auth';
import { useRouter } from 'next/navigation';

interface LoginFormProps {
  onSuccess?: () => void;
  onSwitchToRegister?: () => void;
}

export default function LoginForm({ onSuccess, onSwitchToRegister }: LoginFormProps) {
  const [email, setEmail] = useState('');
  const [password, setPassword] = useState('');
  const [isLoading, setIsLoading] = useState(false);
  const [error, setError] = useState('');
  const router = useRouter();

  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();
    setIsLoading(true);
    setError('');

    try {
      const response = await auth.login(email, password);
      
      if (response.success) {
        onSuccess?.();
        router.push('/dashboard');
      } else {
        setError(response.message);
      }
    } catch (err) {
      setError('Login failed. Please try again.');
    } finally {
      setIsLoading(false);
    }
  };

  return (
    <Card className="w-full max-w-md mx-auto">
      <CardHeader>
        <CardTitle>Welcome Back</CardTitle>
        <CardDescription>
          Sign in to your account to continue
        </CardDescription>
      </CardHeader>
      <CardContent>
        <form onSubmit={handleSubmit} className="space-y-4">
          {error && (
            <Alert variant="destructive">
              <AlertDescription>{error}</AlertDescription>
            </Alert>
          )}
          
          <div className="space-y-2">
            <Label htmlFor="email">Email</Label>
            <Input
              id="email"
              type="email"
              placeholder="Enter your email"
              value={email}
              onChange={(e) => setEmail(e.target.value)}
              required
              disabled={isLoading}
            />
          </div>
          
          <div className="space-y-2">
            <Label htmlFor="password">Password</Label>
            <Input
              id="password"
              type="password"
              placeholder="Enter your password"
              value={password}
              onChange={(e) => setPassword(e.target.value)}
              required
              disabled={isLoading}
            />
          </div>
          
          <Button 
            type="submit" 
            className="w-full" 
            disabled={isLoading}
          >
            {isLoading ? 'Signing in...' : 'Sign In'}
          </Button>
        </form>
        
        <div className="mt-4 text-center">
          <p className="text-sm text-muted-foreground">
            Don't have an account?{' '}
            <button
              type="button"
              onClick={onSwitchToRegister}
              className="text-primary hover:underline"
            >
              Sign up
            </button>
          </p>
        </div>
      </CardContent>
    </Card>
  );
}
```

## File: src/components/features/auth/RegisterForm.tsx
```typescript
'use client';

import { useState } from 'react';
import { Button } from '@/components/ui/button';
import { Input } from '@/components/ui/input';
import { Label } from '@/components/ui/label';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Alert, AlertDescription } from '@/components/ui/alert';
import { Select, SelectContent, SelectItem, SelectTrigger, SelectValue } from '@/components/ui/select';
import { auth } from '@/lib/auth';
import { useRouter } from 'next/navigation';

interface RegisterFormProps {
  onSuccess?: () => void;
  onSwitchToLogin?: () => void;
}

export default function RegisterForm({ onSuccess, onSwitchToLogin }: RegisterFormProps) {
  const [formData, setFormData] = useState({
    email: '',
    password: '',
    confirmPassword: '',
    fullName: '',
    phoneNo: '',
    statusInCanada: '',
    countryOfOrigin: '',
    currentLocation: ''
  });
  const [isLoading, setIsLoading] = useState(false);
  const [error, setError] = useState('');
  const router = useRouter();

  const handleInputChange = (field: string, value: string) => {
    setFormData(prev => ({ ...prev, [field]: value }));
  };

  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();
    setIsLoading(true);
    setError('');

    // Validate passwords match
    if (formData.password !== formData.confirmPassword) {
      setError('Passwords do not match');
      setIsLoading(false);
      return;
    }

    // Validate password strength
    if (formData.password.length < 6) {
      setError('Password must be at least 6 characters long');
      setIsLoading(false);
      return;
    }

    try {
      const response = await auth.register(
        formData.email,
        formData.password,
        formData.fullName,
        {
          phoneNo: formData.phoneNo,
          statusInCanada: formData.statusInCanada,
          countryOfOrigin: formData.countryOfOrigin,
          currentLocation: formData.currentLocation
        }
      );
      
      if (response.success) {
        onSuccess?.();
        router.push('/dashboard');
      } else {
        setError(response.message);
      }
    } catch (err) {
      setError('Registration failed. Please try again.');
    } finally {
      setIsLoading(false);
    }
  };

  return (
    <Card className="w-full max-w-md mx-auto">
      <CardHeader>
        <CardTitle>Create Account</CardTitle>
        <CardDescription>
          Join ImmiGrowAI to start your career journey
        </CardDescription>
      </CardHeader>
      <CardContent>
        <form onSubmit={handleSubmit} className="space-y-4">
          {error && (
            <Alert variant="destructive">
              <AlertDescription>{error}</AlertDescription>
            </Alert>
          )}
          
          <div className="space-y-2">
            <Label htmlFor="fullName">Full Name *</Label>
            <Input
              id="fullName"
              type="text"
              placeholder="Enter your full name"
              value={formData.fullName}
              onChange={(e) => handleInputChange('fullName', e.target.value)}
              required
              disabled={isLoading}
            />
          </div>
          
          <div className="space-y-2">
            <Label htmlFor="email">Email *</Label>
            <Input
              id="email"
              type="email"
              placeholder="Enter your email"
              value={formData.email}
              onChange={(e) => handleInputChange('email', e.target.value)}
              required
              disabled={isLoading}
            />
          </div>
          
          <div className="space-y-2">
            <Label htmlFor="password">Password *</Label>
            <Input
              id="password"
              type="password"
              placeholder="Create a password"
              value={formData.password}
              onChange={(e) => handleInputChange('password', e.target.value)}
              required
              disabled={isLoading}
            />
          </div>
          
          <div className="space-y-2">
            <Label htmlFor="confirmPassword">Confirm Password *</Label>
            <Input
              id="confirmPassword"
              type="password"
              placeholder="Confirm your password"
              value={formData.confirmPassword}
              onChange={(e) => handleInputChange('confirmPassword', e.target.value)}
              required
              disabled={isLoading}
            />
          </div>
          
          <div className="space-y-2">
            <Label htmlFor="phoneNo">Phone Number</Label>
            <Input
              id="phoneNo"
              type="tel"
              placeholder="Enter your phone number"
              value={formData.phoneNo}
              onChange={(e) => handleInputChange('phoneNo', e.target.value)}
              disabled={isLoading}
            />
          </div>
          
          <div className="space-y-2">
            <Label htmlFor="statusInCanada">Status in Canada</Label>
            <Select 
              value={formData.statusInCanada} 
              onValueChange={(value) => handleInputChange('statusInCanada', value)}
              disabled={isLoading}
            >
              <SelectTrigger>
                <SelectValue placeholder="Select your status" />
              </SelectTrigger>
              <SelectContent>
                <SelectItem value="permanent_resident">Permanent Resident</SelectItem>
                <SelectItem value="work_permit">Work Permit</SelectItem>
                <SelectItem value="student_visa">Student Visa</SelectItem>
                <SelectItem value="visitor_visa">Visitor Visa</SelectItem>
                <SelectItem value="citizen">Canadian Citizen</SelectItem>
                <SelectItem value="not_in_canada">Not in Canada</SelectItem>
              </SelectContent>
            </Select>
          </div>
          
          <div className="space-y-2">
            <Label htmlFor="countryOfOrigin">Country of Origin</Label>
            <Input
              id="countryOfOrigin"
              type="text"
              placeholder="Enter your country of origin"
              value={formData.countryOfOrigin}
              onChange={(e) => handleInputChange('countryOfOrigin', e.target.value)}
              disabled={isLoading}
            />
          </div>
          
          <div className="space-y-2">
            <Label htmlFor="currentLocation">Current Location</Label>
            <Input
              id="currentLocation"
              type="text"
              placeholder="Enter your current location"
              value={formData.currentLocation}
              onChange={(e) => handleInputChange('currentLocation', e.target.value)}
              disabled={isLoading}
            />
          </div>
          
          <Button 
            type="submit" 
            className="w-full" 
            disabled={isLoading}
          >
            {isLoading ? 'Creating account...' : 'Create Account'}
          </Button>
        </form>
        
        <div className="mt-4 text-center">
          <p className="text-sm text-muted-foreground">
            Already have an account?{' '}
            <button
              type="button"
              onClick={onSwitchToLogin}
              className="text-primary hover:underline"
            >
              Sign in
            </button>
          </p>
        </div>
      </CardContent>
    </Card>
  );
}
```

## File: src/components/features/career/index.ts
```typescript
export { default as JobSearchModal } from './JobSearchModal';
```

## File: src/components/features/career/JobSearchModal.tsx
```typescript
'use client';

import React, { useState } from 'react';
import { Dialog, DialogContent, DialogHeader, DialogTitle, DialogDescription } from '@/components/ui/dialog';
import { Button } from '@/components/ui/button';
import { Input } from '@/components/ui/input';
import { Badge } from '@/components/ui/badge';
import { Card, CardContent, CardHeader, CardTitle } from '@/components/ui/card';
import { ScrollArea } from '@/components/ui/scroll-area';
import { ExternalLink, MapPin, Building2, DollarSign, Clock, Search, Loader2, AlertCircle } from 'lucide-react';

interface JobResult {
  id: string;
  title: string;
  company: string;
  location: string;
  description: string;
  salaryInfo?: {
    formatted: string;
    currency: string;
  };
  jobLevel?: string;
  employmentTypes?: string[];
  applicationInfo?: {
    applicationUrls?: string[];
    applicationEmails?: string[];
    instruction?: string;
  };
  postingPublishTime?: string;
  jobBenefits?: string[];
}

interface JobSearchModalProps {
  isOpen: boolean;
  onClose: () => void;
  careerPath: {
    title: string;
    industry?: string;
  };
}

export default function JobSearchModal({ isOpen, onClose, careerPath }: JobSearchModalProps) {
  const [isLoading, setIsLoading] = useState(false);
  const [jobs, setJobs] = useState<JobResult[]>([]);
  const [searchLocation, setSearchLocation] = useState('Canada');
  const [error, setError] = useState<string | null>(null);
  const [totalCount, setTotalCount] = useState(0);
  const [hasSearched, setHasSearched] = useState(false);

  // Reset state when modal closes
  React.useEffect(() => {
    if (!isOpen) {
      setJobs([]);
      setError(null);
      setHasSearched(false);
      setTotalCount(0);
      setIsLoading(false);
    }
  }, [isOpen]);

  // Auto-search when modal opens with a career path
  React.useEffect(() => {
    if (isOpen && careerPath.title && !hasSearched && !isLoading) {
      searchJobs();
    }
  }, [isOpen, careerPath.title]);

  const searchJobs = async () => {
    if (!careerPath?.title) return;

    setIsLoading(true);
    setError(null);
    setHasSearched(false);

    try {
      // Use guest token for job search
      const token = 'guest-token';
      console.log('🔐 Job Search - Using guest token for public access');

      const response = await fetch('/api/career/search', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
          'Authorization': `Bearer ${token}`
        },
        body: JSON.stringify({
          careerPath: {
            title: careerPath.title,
            industry: careerPath.industry
          },
          location: searchLocation,
          filters: {}
        })
      });

      const data = await response.json();

      if (data.success) {
        setJobs(data.data.jobs || []);
        setTotalCount(data.data.totalCount || 0);
        setHasSearched(true);
      } else {
        setError(data.error || data.fallbackMessage || 'Failed to search for jobs');
      }
    } catch (err) {
      console.error('Job search error:', err);
      setError('Network error. Please check your connection and try again.');
    } finally {
      setIsLoading(false);
    }
  };

  const formatEmploymentTypes = (types?: string[]) => {
    if (!types || !Array.isArray(types)) return '';
    return types.map(type => 
      type.replace(/_/g, ' ').toLowerCase().replace(/\b\w/g, l => l.toUpperCase())
    ).join(', ');
  };

  const formatDate = (dateString?: string) => {
    if (!dateString) return 'Recently posted';
    try {
      return new Date(dateString).toLocaleDateString('en-CA', {
        year: 'numeric',
        month: 'short',
        day: 'numeric'
      });
    } catch {
      return 'Recently posted';
    }
  };

  const openJobApplication = (job: JobResult) => {
    if (job.applicationInfo?.applicationUrls?.length > 0) {
      window.open(job.applicationInfo.applicationUrls[0], '_blank');
    } else if (job.applicationInfo?.applicationEmails?.length > 0) {
      window.open(`mailto:${job.applicationInfo.applicationEmails[0]}?subject=Application for ${job.title}`, '_blank');
    }
  };

  const getJobSearchUrls = () => {
    const query = encodeURIComponent(`${careerPath.title} ${searchLocation}`);
    return [
      {
        name: 'Indeed Canada',
        url: `https://ca.indeed.com/jobs?q=${query}&l=${encodeURIComponent(searchLocation)}`
      },
      {
        name: 'LinkedIn',
        url: `https://www.linkedin.com/jobs/search/?keywords=${query}&location=${encodeURIComponent(searchLocation)}`
      },
      {
        name: 'Glassdoor',
        url: `https://www.glassdoor.ca/Job/jobs.htm?sc.keyword=${query}&locT=C&locId=2`
      },
      {
        name: 'Job Bank Canada',
        url: `https://www.jobbank.gc.ca/jobsearch/jobsearch?searchstring=${query}`
      }
    ];
  };

  return (
    <Dialog open={isOpen} onOpenChange={onClose}>
      <DialogContent className="max-w-4xl max-h-[90vh]">
        <DialogHeader>
          <DialogTitle className="flex items-center gap-2">
            <Search className="h-5 w-5" />
            {careerPath.title} Jobs in Canada
          </DialogTitle>
          <DialogDescription>
            Search and browse job opportunities for {careerPath.title} positions across Canada
          </DialogDescription>
        </DialogHeader>

        <div className="space-y-4">
          {/* Loading indicator */}
          {isLoading && (
            <div className="flex items-center justify-center py-8">
              <Loader2 className="h-8 w-8 animate-spin text-blue-600" />
              <span className="ml-2 text-lg">Searching for {careerPath.title} jobs in Canada...</span>
            </div>
          )}

          {/* Error State */}
          {error && (
            <div className="bg-red-50 border border-red-200 rounded-lg p-4">
              <div className="flex items-center gap-2 mb-2">
                <AlertCircle className="h-5 w-5 text-red-600" />
                <span className="font-medium text-red-800">Search Error</span>
              </div>
              <p className="text-red-700 mb-3">{error}</p>
              
              <div className="space-y-2">
                <p className="text-sm text-red-600 font-medium">Try searching on these job sites directly:</p>
                <div className="flex flex-wrap gap-2">
                  {getJobSearchUrls().map((site, index) => (
                    <Button
                      key={index}
                      variant="outline"
                      size="sm"
                      onClick={() => window.open(site.url, '_blank')}
                      className="border-red-200 text-red-700 hover:bg-red-50"
                    >
                      <ExternalLink className="mr-1 h-3 w-3" />
                      {site.name}
                    </Button>
                  ))}
                </div>
              </div>
            </div>
          )}

          {/* Results */}
          {hasSearched && (
            <div className="space-y-3">
              <div className="flex items-center justify-between">
                <p className="text-sm text-gray-600">
                  Found {totalCount} jobs for "{careerPath.title}" in {searchLocation}
                </p>
                {(!jobs || jobs.length === 0) && totalCount === 0 && (
                  <div className="text-sm text-gray-500">
                    No jobs found. Try searching on external job sites below.
                  </div>
                )}
              </div>

              {/* External Job Site Links */}
              <div className="bg-blue-50 border border-blue-200 rounded-lg p-4">
                <p className="text-sm font-medium text-blue-800 mb-2">
                  Search on popular job sites:
                </p>
                <div className="flex flex-wrap gap-2">
                  {getJobSearchUrls().map((site, index) => (
                    <Button
                      key={index}
                      variant="outline"
                      size="sm"
                      onClick={() => window.open(site.url, '_blank')}
                      className="border-blue-200 text-blue-700 hover:bg-blue-100"
                    >
                      <ExternalLink className="mr-1 h-3 w-3" />
                      {site.name}
                    </Button>
                  ))}
                </div>
              </div>

              {/* Job Results */}
              <ScrollArea className="h-96">
                <div className="space-y-3">
                  {(jobs || []).map((job) => (
                    <Card key={job.id} className="hover:shadow-md transition-shadow">
                      <CardHeader className="pb-3">
                        <div className="flex items-start justify-between">
                          <div className="space-y-1">
                            <CardTitle className="text-lg font-semibold">{job.title}</CardTitle>
                            <div className="flex items-center gap-4 text-sm text-gray-600">
                              <div className="flex items-center gap-1">
                                <Building2 className="h-4 w-4" />
                                {job.company}
                              </div>
                              <div className="flex items-center gap-1">
                                <MapPin className="h-4 w-4" />
                                {job.location}
                              </div>
                              {job.salaryInfo?.formatted && (
                                <div className="flex items-center gap-1">
                                  <DollarSign className="h-4 w-4" />
                                  {job.salaryInfo.formatted}
                                </div>
                              )}
                            </div>
                          </div>
                          <Button
                            onClick={() => openJobApplication(job)}
                            disabled={!job.applicationInfo?.applicationUrls?.length && !job.applicationInfo?.applicationEmails?.length}
                            className="shrink-0"
                          >
                            <ExternalLink className="mr-2 h-4 w-4" />
                            Apply
                          </Button>
                        </div>
                      </CardHeader>
                      
                      <CardContent className="space-y-3">
                        <p className="text-sm text-gray-700 leading-relaxed">
                          {job.description}
                        </p>
                        
                        <div className="flex items-center justify-between">
                          <div className="flex flex-wrap gap-2">
                            {job.employmentTypes?.length > 0 && (
                              <Badge variant="secondary">
                                {formatEmploymentTypes(job.employmentTypes)}
                              </Badge>
                            )}
                            {job.jobLevel && (
                              <Badge variant="outline">{job.jobLevel}</Badge>
                            )}
                          </div>
                          
                          <div className="flex items-center gap-1 text-xs text-gray-500">
                            <Clock className="h-3 w-3" />
                            {formatDate(job.postingPublishTime)}
                          </div>
                        </div>
                        
                        {job.jobBenefits?.length > 0 && (
                          <div className="space-y-1">
                            <p className="text-xs font-medium text-gray-600">Benefits:</p>
                            <div className="flex flex-wrap gap-1">
                              {job.jobBenefits.slice(0, 3).map((benefit, index) => (
                                <Badge key={index} variant="outline" className="text-xs">
                                  {benefit}
                                </Badge>
                              ))}
                              {job.jobBenefits.length > 3 && (
                                <Badge variant="outline" className="text-xs">
                                  +{job.jobBenefits.length - 3} more
                                </Badge>
                              )}
                            </div>
                          </div>
                        )}
                      </CardContent>
                    </Card>
                  ))}
                </div>
              </ScrollArea>
            </div>
          )}

          {/* Initial state message */}
          {!hasSearched && !isLoading && !error && (
            <div className="text-center py-8 text-gray-500">
              <Search className="h-12 w-12 mx-auto mb-3 text-gray-300" />
              <p>Click "Search Jobs" to find opportunities for {careerPath.title}</p>
            </div>
          )}
        </div>

        <div className="flex justify-end pt-4 border-t">
          <Button variant="outline" onClick={onClose}>
            Close
          </Button>
        </div>
      </DialogContent>
    </Dialog>
  );
}
```

## File: src/components/features/resume/FeaturesPanel.tsx
```typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';

const AIFeaturesPanel = () => {
  const [expandedCard, setExpandedCard] = useState(null);

  const features = [
    {
      id: 'resume',
      title: 'Resume Analysis',
      description: 'AI-powered resume analysis and auto-fill',
      icon: '📄',
      color: 'border-blue-200 bg-blue-50',
      benefits: ['Extract work experience', 'Identify skills', 'Canadian market analysis'],
              route: '/dashboard/resume'
    },
    {
      id: 'profile',
      title: 'Career Profile Generator',
      description: 'Generate tailored career profiles with position recommendations',
      icon: '🎯',
      color: 'border-green-200 bg-green-50',
      benefits: ['Position recommendations', 'Success probability analysis', 'Enhanced profile generation'],
              route: '/dashboard/career'
    },

    {
      id: 'resume-generation',
      title: 'Resume Generation',
      description: 'Generate Canadian resumes optimized for ATS systems',
      icon: '📝',
      color: 'border-indigo-200 bg-indigo-50',
      benefits: ['ATS optimization', 'Canadian market focus', 'Multiple templates', 'Interactive editing'],
              route: '/dashboard/resume/generator'
    },
    {
      id: 'jobs',
      title: 'Job Discovery',
      description: 'Find matching job opportunities',
      icon: '🔍',
      color: 'border-cyan-200 bg-cyan-50',
      benefits: ['Smart matching', 'Compatibility scores', 'Job alerts'],
              route: '/dashboard/ai/jobs'
    },
    {
      id: 'skills',
      title: 'Skill Gap Analysis',
      description: 'Identify and bridge skill gaps',
      icon: '📈',
      color: 'border-yellow-200 bg-yellow-50',
      benefits: ['Gap identification', 'Learning path', 'Progress tracking'],
              route: '/dashboard/ai/skills'
    },
    {
      id: 'history',
      title: 'View History',
      description: 'Access your previous resume analyses and profiles',
      icon: '📋',
      color: 'border-gray-200 bg-gray-50',
      benefits: ['Previous analyses', 'Comparison view', 'Progress tracking'],
              route: '/dashboard/history'
    }
  ];

  const toggleCard = (id) => {
    setExpandedCard(expandedCard === id ? null : id);
  };

  return (
    <div className="space-y-6">
      <div className="text-center space-y-3">
        <h2 className="text-3xl font-bold text-gray-900 flex items-center justify-center gap-2 mt-6">
          ✨ AI Career Assistant
        </h2>
        <p className="text-gray-600 max-w-2xl mx-auto">
          Leverage AI-powered tools to accelerate your career growth in Canada. 
          Get personalized insights, find mentors, and navigate your professional journey with confidence.
        </p>
      </div>

      <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        {features.map((feature) => (
          <Card 
            key={feature.id} 
            className={`cursor-pointer transition-all hover:shadow-lg ${feature.color} ${
              expandedCard === feature.id ? 'ring-2 ring-blue-500' : ''
            }`}
            onClick={() => toggleCard(feature.id)}
          >
            <CardHeader className="pb-3">
              <div className="flex items-center justify-between">
                <div className="flex items-center gap-3">
                  <span className="text-2xl">{feature.icon}</span>
                  <div>
                    <CardTitle className="text-lg">{feature.title}</CardTitle>
                    <Badge variant="secondary" className="text-xs">
                      {feature.id === 'profile' || feature.id === 'resume' || feature.id === 'history' || feature.id === 'resume-generation' ? 'Available' : 'Coming Soon'}
                    </Badge>
                  </div>
                </div>
              </div>
              <CardDescription className="text-sm">
                {feature.description}
              </CardDescription>
            </CardHeader>
            
            {expandedCard === feature.id && (
              <CardContent className="pt-0">
                <div className="space-y-3">
                  <h4 className="font-semibold text-sm">Features:</h4>
                  <ul className="space-y-1">
                    {feature.benefits.map((benefit, index) => (
                      <li key={index} className="text-sm flex items-center gap-2">
                        <span className="text-green-500">✓</span>
                        {benefit}
                      </li>
                    ))}
                  </ul>
                  <Button 
                    size="sm" 
                    className="w-full mt-3"
                    disabled={feature.id !== 'profile' && feature.id !== 'resume' && feature.id !== 'history' && feature.id !== 'resume-generation'}
                    onClick={(e) => {
                      e.stopPropagation();
                      if (feature.id === 'profile' || feature.id === 'resume' || feature.id === 'history' || feature.id === 'resume-generation') {
                        window.location.href = feature.route;
                      }
                    }}
                  >
                    {feature.id === 'profile' || feature.id === 'resume' || feature.id === 'history' || feature.id === 'resume-generation' ? 'Get Started' : 'Coming Soon'}
                  </Button>
                </div>
              </CardContent>
            )}
          </Card>
        ))}
      </div>

      <div className="bg-blue-50 border border-blue-200 rounded-lg p-6">
        <h3 className="font-semibold text-blue-900 mb-2">🚀 Get Started</h3>
        <p className="text-blue-800 text-sm mb-4">
          Begin your AI-powered career journey by uploading your resume for analysis, 
          or generate a tailored career profile with position recommendations.
        </p>
        <div className="flex flex-wrap gap-3">
          <Button 
            onClick={() => window.location.href = '/dashboard/resume'}
            className="bg-blue-600 hover:bg-blue-700"
          >
            Upload Resume
          </Button>
          <Button 
            onClick={() => window.location.href = '/dashboard/resume/generator'}
            className="bg-indigo-600 hover:bg-indigo-700"
          >
            Generate Resume
          </Button>
          <Button 
            onClick={() => window.location.href = '/dashboard/career'}
            className="bg-green-600 hover:bg-green-700"
          >
            Career Profile
          </Button>
          <Button 
            onClick={() => window.location.href = '/dashboard/history'}
            variant="outline" 
            className="border-gray-600 text-gray-600"
          >
            View History
          </Button>
        </div>
      </div>
    </div>
  );
};

export default AIFeaturesPanel;
```

## File: src/components/features/resume/generator/EditableField.tsx
```typescript
"use client";

import React, { useState, useRef, useEffect } from 'react';
import { Input } from '@/components/ui/input';
import { Textarea } from '@/components/ui/textarea';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { 
  Edit3, 
  Check, 
  X, 
  Plus, 
  Trash2,
  AlertCircle
} from 'lucide-react';

export type FieldType = 'text' | 'textarea' | 'email' | 'phone' | 'url' | 'list' | 'date' | 'number';

export interface EditableFieldProps {
  value: string | string[];
  type: FieldType;
  placeholder?: string;
  label?: string;
  required?: boolean;
  maxLength?: number;
  minLength?: number;
  pattern?: string;
  validation?: (value: string | string[]) => string | null;
  onSave: (value: string | string[]) => void;
  onCancel?: () => void;
  className?: string;
  disabled?: boolean;
  autoFocus?: boolean;
}

export default function EditableField({
  value,
  type,
  placeholder,
  label,
  required = false,
  maxLength,
  minLength,
  pattern,
  validation,
  onSave,
  onCancel,
  className = '',
  disabled = false,
  autoFocus = false
}: EditableFieldProps) {
  const [isEditing, setIsEditing] = useState(false);
  const [editValue, setEditValue] = useState<string | string[]>(value);
  const [error, setError] = useState<string | null>(null);
  const [isValidating, setIsValidating] = useState(false);
  
  const inputRef = useRef<HTMLInputElement>(null);
  const textareaRef = useRef<HTMLTextAreaElement>(null);

  useEffect(() => {
    setEditValue(value);
  }, [value]);

  useEffect(() => {
    if (isEditing && autoFocus) {
      if (type === 'textarea' && textareaRef.current) {
        textareaRef.current.focus();
        textareaRef.current.select();
      } else if (inputRef.current) {
        inputRef.current.focus();
        inputRef.current.select();
      }
    }
  }, [isEditing, autoFocus, type]);

  const validateField = (value: string | string[]): string | null => {
    // Required validation
    if (required) {
      if (typeof value === 'string' && !value.trim()) {
        return 'This field is required';
      }
      if (Array.isArray(value) && value.length === 0) {
        return 'At least one item is required';
      }
    }

    // Length validation
    if (typeof value === 'string') {
      if (minLength && value.length < minLength) {
        return `Minimum ${minLength} characters required`;
      }
      if (maxLength && value.length > maxLength) {
        return `Maximum ${maxLength} characters allowed`;
      }
    }

    // Pattern validation
    if (pattern && typeof value === 'string') {
      const regex = new RegExp(pattern);
      if (!regex.test(value)) {
        return 'Invalid format';
      }
    }

    // Type-specific validation
    switch (type) {
      case 'email':
        if (typeof value === 'string' && value && !/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(value)) {
          return 'Invalid email format';
        }
        break;
      case 'phone':
        if (typeof value === 'string' && value && !/^[\+]?[1-9][\d]{0,15}$/.test(value.replace(/\s/g, ''))) {
          return 'Invalid phone number format';
        }
        break;
      case 'url':
        if (typeof value === 'string' && value && !/^https?:\/\/.+/.test(value)) {
          return 'Invalid URL format (must start with http:// or https://)';
        }
        break;
      case 'number':
        if (typeof value === 'string' && value && isNaN(Number(value))) {
          return 'Must be a valid number';
        }
        break;
    }

    // Custom validation
    if (validation) {
      return validation(value);
    }

    return null;
  };

  const handleEdit = () => {
    if (disabled) return;
    setIsEditing(true);
    setError(null);
  };

  const handleSave = async () => {
    setIsValidating(true);
    const validationError = validateField(editValue);
    
    if (validationError) {
      setError(validationError);
      setIsValidating(false);
      return;
    }

    try {
      await onSave(editValue);
      setIsEditing(false);
      setError(null);
    } catch (error) {
      setError(error instanceof Error ? error.message : 'Failed to save');
    } finally {
      setIsValidating(false);
    }
  };

  const handleCancel = () => {
    setEditValue(value);
    setIsEditing(false);
    setError(null);
    onCancel?.();
  };

  const handleKeyDown = (e: React.KeyboardEvent) => {
    if (e.key === 'Enter' && !e.shiftKey) {
      e.preventDefault();
      handleSave();
    } else if (e.key === 'Escape') {
      handleCancel();
    }
  };

  const handleListAdd = () => {
    if (Array.isArray(editValue)) {
      setEditValue([...editValue, '']);
    }
  };

  const handleListRemove = (index: number) => {
    if (Array.isArray(editValue)) {
      setEditValue(editValue.filter((_, i) => i !== index));
    }
  };

  const handleListChange = (index: number, newValue: string) => {
    if (Array.isArray(editValue)) {
      const newList = [...editValue];
      newList[index] = newValue;
      setEditValue(newList);
    }
  };

  const renderDisplayValue = () => {
    if (Array.isArray(value)) {
      return (
        <div className="flex flex-wrap gap-1">
          {value.map((item, index) => (
            <Badge key={index} variant="secondary" className="text-sm">
              {item}
            </Badge>
          ))}
        </div>
      );
    }

    if (!value || value.trim() === '') {
      return (
        <span className="text-gray-400 italic">
          {placeholder || 'Click to edit'}
        </span>
      );
    }

    return <span>{value}</span>;
  };

  const renderEditInput = () => {
    switch (type) {
      case 'textarea':
        return (
          <Textarea
            ref={textareaRef}
            value={typeof editValue === 'string' ? editValue : ''}
            onChange={(e) => setEditValue(e.target.value)}
            onKeyDown={handleKeyDown}
            placeholder={placeholder}
            maxLength={maxLength}
            className="min-h-[100px] resize-none"
          />
        );

      case 'list':
        if (Array.isArray(editValue)) {
          return (
            <div className="space-y-2">
              {editValue.map((item, index) => (
                <div key={index} className="flex gap-2">
                  <Input
                    value={item}
                    onChange={(e) => handleListChange(index, e.target.value)}
                    placeholder={`Item ${index + 1}`}
                    maxLength={maxLength}
                  />
                  <Button
                    type="button"
                    variant="outline"
                    size="sm"
                    onClick={() => handleListRemove(index)}
                    className="flex-shrink-0"
                  >
                    <Trash2 className="h-4 w-4" />
                  </Button>
                </div>
              ))}
              <Button
                type="button"
                variant="outline"
                size="sm"
                onClick={handleListAdd}
                className="w-full"
              >
                <Plus className="h-4 w-4 mr-2" />
                Add Item
              </Button>
            </div>
          );
        }
        return null;

      default:
        return (
          <Input
            ref={inputRef}
            type={type === 'number' ? 'number' : 'text'}
            value={typeof editValue === 'string' ? editValue : ''}
            onChange={(e) => setEditValue(e.target.value)}
            onKeyDown={handleKeyDown}
            placeholder={placeholder}
            maxLength={maxLength}
            minLength={minLength}
            pattern={pattern}
          />
        );
    }
  };

  return (
    <div className={`group ${className}`}>
      {label && (
        <label className="block text-sm font-medium text-gray-700 mb-1">
          {label}
          {required && <span className="text-red-500 ml-1">*</span>}
        </label>
      )}

      {isEditing ? (
        <div className="space-y-2">
          {renderEditInput()}
          
          {error && (
            <div className="flex items-center gap-2 text-sm text-red-600">
              <AlertCircle className="h-4 w-4" />
              <span>{error}</span>
            </div>
          )}

          <div className="flex gap-2">
            <Button
              onClick={handleSave}
              disabled={isValidating}
              size="sm"
              className="flex-1"
            >
              <Check className="h-4 w-4 mr-2" />
              Save
            </Button>
            <Button
              onClick={handleCancel}
              variant="outline"
              size="sm"
              className="flex-1"
            >
              <X className="h-4 w-4 mr-2" />
              Cancel
            </Button>
          </div>
        </div>
      ) : (
        <div
          onClick={handleEdit}
          className={`
            p-3 border border-gray-200 rounded-md cursor-pointer
            hover:border-gray-300 hover:bg-gray-50 transition-colors
            ${disabled ? 'cursor-not-allowed opacity-50' : ''}
            ${error ? 'border-red-300 bg-red-50' : ''}
          `}
        >
          <div className="flex items-start justify-between">
            <div className="flex-1 min-w-0">
              {renderDisplayValue()}
            </div>
            {!disabled && (
              <Edit3 className="h-4 w-4 text-gray-400 ml-2 flex-shrink-0 opacity-0 group-hover:opacity-100 transition-opacity" />
            )}
          </div>
        </div>
      )}
    </div>
  );
}
```

## File: src/components/features/resume/generator/EditableSection.tsx
```typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { 
  Plus, 
  GripVertical, 
  Trash2, 
  Edit3, 
  Eye,
  ChevronDown,
  ChevronRight
} from 'lucide-react';
import EditableField, { FieldType } from './EditableField';

export interface SectionItem {
  id: string;
  [key: string]: any;
}

export interface SectionTemplate {
  id: string;
  name: string;
  fields: {
    key: string;
    label: string;
    type: FieldType;
    required?: boolean;
    placeholder?: string;
    maxLength?: number;
  }[];
}

export interface EditableSectionProps {
  title: string;
  description?: string;
  items: SectionItem[];
  template: SectionTemplate;
  onItemsChange: (items: SectionItem[]) => void;
  onAddItem?: () => void;
  onRemoveItem?: (itemId: string) => void;
  onReorderItems?: (fromIndex: number, toIndex: number) => void;
  className?: string;
  collapsible?: boolean;
  defaultCollapsed?: boolean;
  maxItems?: number;
  minItems?: number;
}

export default function EditableSection({
  title,
  description,
  items,
  template,
  onItemsChange,
  onAddItem,
  onRemoveItem,
  onReorderItems,
  className = '',
  collapsible = false,
  defaultCollapsed = false,
  maxItems,
  minItems = 0
}: EditableSectionProps) {
  const [isCollapsed, setIsCollapsed] = useState(defaultCollapsed);
  const [expandedItems, setExpandedItems] = useState<Set<string>>(new Set());

  const handleAddItem = () => {
    if (maxItems && items.length >= maxItems) return;
    
    const newItem: SectionItem = {
      id: `item-${Date.now()}-${Math.random().toString(36).substr(2, 9)}`,
      ...template.fields.reduce((acc, field) => {
        acc[field.key] = field.type === 'list' ? [] : '';
        return acc;
      }, {} as any)
    };

    const newItems = [...items, newItem];
    onItemsChange(newItems);
    onAddItem?.();
    
    // Auto-expand the new item
    setExpandedItems(prev => new Set([...prev, newItem.id]));
  };

  const handleRemoveItem = (itemId: string) => {
    if (items.length <= minItems) return;
    
    const newItems = items.filter(item => item.id !== itemId);
    onItemsChange(newItems);
    onRemoveItem?.(itemId);
    
    // Remove from expanded items
    setExpandedItems(prev => {
      const newSet = new Set(prev);
      newSet.delete(itemId);
      return newSet;
    });
  };

  const handleItemChange = (itemId: string, fieldKey: string, value: any) => {
    const newItems = items.map(item => 
      item.id === itemId 
        ? { ...item, [fieldKey]: value }
        : item
    );
    onItemsChange(newItems);
  };

  const handleToggleItem = (itemId: string) => {
    setExpandedItems(prev => {
      const newSet = new Set(prev);
      if (newSet.has(itemId)) {
        newSet.delete(itemId);
      } else {
        newSet.add(itemId);
      }
      return newSet;
    });
  };

  const handleDragStart = (e: React.DragEvent, index: number) => {
    e.dataTransfer.setData('text/plain', index.toString());
  };

  const handleDragOver = (e: React.DragEvent) => {
    e.preventDefault();
  };

  const handleDrop = (e: React.DragEvent, dropIndex: number) => {
    e.preventDefault();
    const dragIndex = parseInt(e.dataTransfer.getData('text/plain'));
    
    if (dragIndex !== dropIndex && onReorderItems) {
      onReorderItems(dragIndex, dropIndex);
    }
  };

  const renderItem = (item: SectionItem, index: number) => {
    const isExpanded = expandedItems.has(item.id);
    const primaryField = template.fields.find(f => f.key === 'title' || f.key === 'name' || f.key === 'company');
    const primaryValue = primaryField ? item[primaryField.key] : `Item ${index + 1}`;

    return (
      <div
        key={item.id}
        draggable={!!onReorderItems}
        onDragStart={(e) => handleDragStart(e, index)}
        onDragOver={handleDragOver}
        onDrop={(e) => handleDrop(e, index)}
        className="border border-gray-200 rounded-lg mb-3 bg-white"
      >
        {/* Item Header */}
        <div className="flex items-center justify-between p-3 border-b border-gray-100">
          <div className="flex items-center gap-2 flex-1 min-w-0">
            {onReorderItems && (
              <GripVertical className="h-4 w-4 text-gray-400 cursor-move" />
            )}
            
            <button
              onClick={() => handleToggleItem(item.id)}
              className="flex items-center gap-2 flex-1 min-w-0 text-left hover:bg-gray-50 p-1 rounded"
            >
              {isExpanded ? (
                <ChevronDown className="h-4 w-4 text-gray-500" />
              ) : (
                <ChevronRight className="h-4 w-4 text-gray-500" />
              )}
              <span className="font-medium text-gray-900 truncate">
                {primaryValue || `Item ${index + 1}`}
              </span>
            </button>
          </div>

          <div className="flex items-center gap-1">
            <Button
              variant="ghost"
              size="sm"
              onClick={() => handleToggleItem(item.id)}
            >
              {isExpanded ? <Eye className="h-4 w-4" /> : <Edit3 className="h-4 w-4" />}
            </Button>
            
            <Button
              variant="ghost"
              size="sm"
              onClick={() => handleRemoveItem(item.id)}
              disabled={items.length <= minItems}
              className="text-red-600 hover:text-red-700 hover:bg-red-50"
            >
              <Trash2 className="h-4 w-4" />
            </Button>
          </div>
        </div>

        {/* Item Content */}
        {isExpanded && (
          <div className="p-4 space-y-4">
            {template.fields.map((field) => (
              <EditableField
                key={field.key}
                value={item[field.key] || ''}
                type={field.type}
                label={field.label}
                placeholder={field.placeholder}
                required={field.required}
                maxLength={field.maxLength}
                onSave={(value) => handleItemChange(item.id, field.key, value)}
                className="w-full"
              />
            ))}
          </div>
        )}
      </div>
    );
  };

  return (
    <Card className={className}>
      <CardHeader>
        <div className="flex items-center justify-between">
          <div className="flex items-center gap-2">
            {collapsible && (
              <button
                onClick={() => setIsCollapsed(!isCollapsed)}
                className="p-1 hover:bg-gray-100 rounded"
              >
                {isCollapsed ? (
                  <ChevronRight className="h-4 w-4" />
                ) : (
                  <ChevronDown className="h-4 w-4" />
                )}
              </button>
            )}
            
            <div>
              <CardTitle className="text-lg">{title}</CardTitle>
              {description && (
                <CardDescription>{description}</CardDescription>
              )}
            </div>
          </div>

          <div className="flex items-center gap-2">
            <Badge variant="secondary" className="text-sm">
              {items.length} {items.length === 1 ? 'item' : 'items'}
            </Badge>
            
            <Button
              onClick={handleAddItem}
              disabled={maxItems ? items.length >= maxItems : false}
              size="sm"
            >
              <Plus className="h-4 w-4 mr-2" />
              Add {template.name}
            </Button>
          </div>
        </div>
      </CardHeader>

      {!isCollapsed && (
        <CardContent>
          {items.length === 0 ? (
            <div className="text-center py-8 text-gray-500">
              <p>No {template.name.toLowerCase()} added yet.</p>
              <p className="text-sm">Click "Add {template.name}" to get started.</p>
            </div>
          ) : (
            <div className="space-y-2">
              {items.map((item, index) => renderItem(item, index))}
            </div>
          )}

          {maxItems && items.length >= maxItems && (
            <div className="mt-4 p-3 bg-yellow-50 border border-yellow-200 rounded-md">
              <p className="text-sm text-yellow-800">
                Maximum of {maxItems} {template.name.toLowerCase()} reached.
              </p>
            </div>
          )}

          {minItems && items.length <= minItems && (
            <div className="mt-4 p-3 bg-blue-50 border border-blue-200 rounded-md">
              <p className="text-sm text-blue-800">
                At least {minItems} {template.name.toLowerCase()} required.
              </p>
            </div>
          )}
        </CardContent>
      )}
    </Card>
  );
}
```

## File: src/components/features/resume/generator/GenerationProgress.tsx
```typescript
"use client";

import React from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Progress } from '@/components/ui/progress';
import { 
  Loader2, 
  CheckCircle, 
  XCircle, 
  Clock,
  AlertTriangle,
  Sparkles
} from 'lucide-react';

interface GenerationStep {
  id: string;
  name: string;
  description: string;
  status: 'pending' | 'processing' | 'completed' | 'error';
  progress: number;
  estimatedTime: number;
}

interface GenerationProgressProps {
  steps: GenerationStep[];
  currentStep: number;
  overallProgress: number;
  estimatedTimeRemaining: number;
  isCompleted: boolean;
  onCancel: () => void;
}

export default function GenerationProgress({
  steps,
  currentStep,
  overallProgress,
  estimatedTimeRemaining,
  isCompleted,
  onCancel
}: GenerationProgressProps) {
  const getStepIcon = (step: GenerationStep, index: number) => {
    if (step.status === 'completed') {
      return <CheckCircle className="h-5 w-5 text-green-600" />;
    }
    
    if (step.status === 'error') {
      return <XCircle className="h-5 w-5 text-red-600" />;
    }
    
    if (index === currentStep && step.status === 'processing') {
      return <Loader2 className="h-5 w-5 text-blue-600 animate-spin" />;
    }
    
    if (index < currentStep) {
      return <CheckCircle className="h-5 w-5 text-green-600" />;
    }
    
    return <Clock className="h-5 w-5 text-gray-400" />;
  };

  const getStepStatusColor = (step: GenerationStep, index: number) => {
    if (step.status === 'completed') {
      return 'text-green-600';
    }
    
    if (step.status === 'error') {
      return 'text-red-600';
    }
    
    if (index === currentStep && step.status === 'processing') {
      return 'text-blue-600';
    }
    
    if (index < currentStep) {
      return 'text-green-600';
    }
    
    return 'text-gray-500';
  };

  const getStepBorderColor = (step: GenerationStep, index: number) => {
    if (step.status === 'completed') {
      return 'border-green-200 bg-green-50';
    }
    
    if (step.status === 'error') {
      return 'border-red-200 bg-red-50';
    }
    
    if (index === currentStep && step.status === 'processing') {
      return 'border-blue-200 bg-blue-50';
    }
    
    if (index < currentStep) {
      return 'border-green-200 bg-green-50';
    }
    
    return 'border-gray-200 bg-white';
  };

  const formatTime = (seconds: number): string => {
    if (seconds < 60) {
      return `${Math.ceil(seconds)}s`;
    }
    
    const minutes = Math.floor(seconds / 60);
    const remainingSeconds = Math.ceil(seconds % 60);
    
    if (remainingSeconds === 0) {
      return `${minutes}m`;
    }
    
    return `${minutes}m ${remainingSeconds}s`;
  };

  return (
    <div className="space-y-6">
      {/* Overall Progress */}
      <Card>
        <CardHeader>
          <CardTitle className="flex items-center gap-2">
            {isCompleted ? (
              <CheckCircle className="h-6 w-6 text-green-600" />
            ) : (
              <Loader2 className="h-6 w-6 text-blue-600 animate-spin" />
            )}
            {isCompleted ? 'Generation Complete!' : 'Generation Progress'}
          </CardTitle>
          <CardDescription>
            {isCompleted 
              ? 'Your resume has been successfully generated and is ready for editing.'
              : `Processing step ${currentStep + 1} of ${steps.length}`
            }
          </CardDescription>
        </CardHeader>
        <CardContent className="space-y-4">
          {/* Progress Bar */}
          <div className="space-y-2">
            <div className="flex justify-between items-center">
              <span className="text-sm font-medium text-gray-700">
                Overall Progress
              </span>
              <span className="text-sm text-gray-500">
                {Math.round(overallProgress)}%
              </span>
            </div>
            <Progress value={overallProgress} className="h-3" />
          </div>

          {/* Current Status */}
          {!isCompleted && (
            <div className="flex items-center gap-3 p-3 bg-blue-50 rounded-lg border border-blue-200">
              <Sparkles className="h-5 w-5 text-blue-600" />
              <div>
                <p className="text-sm font-medium text-blue-900">
                  {steps[currentStep]?.name || 'Processing...'}
                </p>
                <p className="text-xs text-blue-700">
                  {steps[currentStep]?.description || 'Please wait while we process your request.'}
                </p>
              </div>
            </div>
          )}

          {/* Estimated Time */}
          {!isCompleted && estimatedTimeRemaining > 0 && (
            <div className="flex items-center gap-2 text-sm text-gray-600">
              <Clock className="h-4 w-4" />
              <span>Estimated time remaining: {formatTime(estimatedTimeRemaining)}</span>
            </div>
          )}

          {/* Cancel Button */}
          {!isCompleted && (
            <Button 
              onClick={onCancel}
              variant="outline"
              size="sm"
              className="w-full"
            >
              Cancel Generation
            </Button>
          )}
        </CardContent>
      </Card>

      {/* Step-by-Step Progress */}
      <Card>
        <CardHeader>
          <CardTitle>Generation Steps</CardTitle>
          <CardDescription>
            Detailed progress of each generation step
          </CardDescription>
        </CardHeader>
        <CardContent>
          <div className="space-y-4">
            {steps.map((step, index) => (
              <div
                key={step.id}
                className={`p-4 rounded-lg border transition-all duration-300 ${getStepBorderColor(step, index)}`}
              >
                <div className="flex items-start gap-3">
                  {/* Step Icon */}
                  <div className="flex-shrink-0 mt-1">
                    {getStepIcon(step, index)}
                  </div>

                  {/* Step Content */}
                  <div className="flex-1 min-w-0">
                    <div className="flex items-center justify-between mb-2">
                      <h4 className={`font-medium ${getStepStatusColor(step, index)}`}>
                        {step.name}
                      </h4>
                      {step.status === 'processing' && (
                        <span className="text-xs text-blue-600 font-medium">
                          {Math.round(step.progress)}%
                        </span>
                      )}
                    </div>
                    
                    <p className="text-sm text-gray-600 mb-3">
                      {step.description}
                    </p>

                    {/* Step Progress Bar */}
                    {step.status === 'processing' && (
                      <div className="space-y-1">
                        <div className="flex justify-between items-center">
                          <span className="text-xs text-gray-500">Progress</span>
                          <span className="text-xs text-gray-500">
                            {Math.round(step.progress)}%
                          </span>
                        </div>
                        <Progress value={step.progress} className="h-2" />
                      </div>
                    )}

                    {/* Step Status */}
                    {step.status === 'completed' && (
                      <div className="flex items-center gap-2 text-xs text-green-600">
                        <CheckCircle className="h-3 w-3" />
                        <span>Completed</span>
                      </div>
                    )}

                    {step.status === 'error' && (
                      <div className="flex items-center gap-2 text-xs text-red-600">
                        <AlertTriangle className="h-3 w-3" />
                        <span>Error occurred</span>
                      </div>
                    )}

                    {step.status === 'pending' && index > currentStep && (
                      <div className="flex items-center gap-2 text-xs text-gray-500">
                        <Clock className="h-3 w-3" />
                        <span>Estimated: {step.estimatedTime}s</span>
                      </div>
                    )}
                  </div>
                </div>
              </div>
            ))}
          </div>
        </CardContent>
      </Card>

      {/* Completion Message */}
      {isCompleted && (
        <Card className="border-green-200 bg-green-50">
          <CardContent className="pt-6">
            <div className="flex items-center gap-3">
              <CheckCircle className="h-6 w-6 text-green-600" />
              <div>
                <h3 className="font-medium text-green-900">
                  Resume Generated Successfully!
                </h3>
                <p className="text-sm text-green-700 mt-1">
                  Your optimized Canadian resume is ready. You'll be redirected to the editor shortly.
                </p>
              </div>
            </div>
          </CardContent>
        </Card>
      )}
    </div>
  );
}
```

## File: src/components/features/resume/generator/InteractiveResumeEditor.tsx
```typescript
"use client";

import React, { useState, useEffect } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { ScrollArea } from '@/components/ui/scroll-area';
import {
  Save,
  Eye,
  Edit3,
  Plus,
  Trash2,
  Copy,
  Undo,
  Redo,
  Settings,
  Download,
  Share2,
  History,
  CheckCircle,
  AlertTriangle,
  Info,
  Sparkles,
  User
} from 'lucide-react';
import EditableField, { FieldType } from './EditableField';
import EditableSection, { SectionItem, SectionTemplate } from './EditableSection';

export interface InteractiveResumeEditorProps {
  resume: any;
  onResumeUpdate: (resume: any) => void;
  onSave: () => void;
  className?: string;
}

// Section templates for different resume sections
const SECTION_TEMPLATES: Record<string, SectionTemplate> = {
  personalInfo: {
    id: 'personalInfo',
    name: 'Personal Information',
    fields: [
      { key: 'name', label: 'Full Name', type: 'text', required: true, maxLength: 100 },
      { key: 'email', label: 'Email', type: 'email', required: true, maxLength: 100 },
      { key: 'phone', label: 'Phone', type: 'phone', required: true, maxLength: 20 },
      { key: 'location', label: 'Location', type: 'text', required: true, maxLength: 100 },
      { key: 'linkedin', label: 'LinkedIn', type: 'url', maxLength: 200 },
      { key: 'website', label: 'Website', type: 'url', maxLength: 200 }
    ]
  },
  professionalSummary: {
    id: 'professionalSummary',
    name: 'Professional Summary',
    fields: [
      { key: 'summary', label: 'Summary', type: 'textarea', required: true, maxLength: 500 }
    ]
  },
  workExperience: {
    id: 'workExperience',
    name: 'Work Experience',
    fields: [
      { key: 'title', label: 'Job Title', type: 'text', required: true, maxLength: 100 },
      { key: 'company', label: 'Company', type: 'text', required: true, maxLength: 100 },
      { key: 'location', label: 'Location', type: 'text', maxLength: 100 },
      { key: 'startDate', label: 'Start Date', type: 'date', required: true },
      { key: 'endDate', label: 'End Date', type: 'date' },
      { key: 'current', label: 'Current Position', type: 'text', maxLength: 10 },
      { key: 'description', label: 'Job Description', type: 'textarea', maxLength: 300 },
      { key: 'achievements', label: 'Key Achievements', type: 'list', maxLength: 200 }
    ]
  },
  education: {
    id: 'education',
    name: 'Education',
    fields: [
      { key: 'degree', label: 'Degree', type: 'text', required: true, maxLength: 100 },
      { key: 'institution', label: 'Institution', type: 'text', required: true, maxLength: 100 },
      { key: 'location', label: 'Location', type: 'text', maxLength: 100 },
      { key: 'startDate', label: 'Start Date', type: 'date', required: true },
      { key: 'endDate', label: 'End Date', type: 'date' },
      { key: 'current', label: 'Currently Studying', type: 'text', maxLength: 10 },
      { key: 'gpa', label: 'GPA', type: 'text', maxLength: 10 },
      { key: 'relevantCourses', label: 'Relevant Courses', type: 'list', maxLength: 100 }
    ]
  },
  skills: {
    id: 'skills',
    name: 'Skills',
    fields: [
      { key: 'name', label: 'Skill Name', type: 'text', required: true, maxLength: 50 },
      { key: 'level', label: 'Proficiency Level', type: 'text', required: true, maxLength: 20 },
      { key: 'canadianEquivalent', label: 'Canadian Equivalent', type: 'text', maxLength: 50 }
    ]
  },
  certifications: {
    id: 'certifications',
    name: 'Certifications',
    fields: [
      { key: 'name', label: 'Certification Name', type: 'text', required: true, maxLength: 100 },
      { key: 'issuer', label: 'Issuing Organization', type: 'text', required: true, maxLength: 100 },
      { key: 'date', label: 'Date Obtained', type: 'date', required: true },
      { key: 'expiryDate', label: 'Expiry Date', type: 'date' },
      { key: 'credentialId', label: 'Credential ID', type: 'text', maxLength: 50 }
    ]
  },
  languages: {
    id: 'languages',
    name: 'Languages',
    fields: [
      { key: 'language', label: 'Language', type: 'text', required: true, maxLength: 50 },
      { key: 'proficiency', label: 'Proficiency Level', type: 'text', required: true, maxLength: 20 }
    ]
  }
};

export default function InteractiveResumeEditor({
  resume,
  onResumeUpdate,
  onSave,
  className = ''
}: InteractiveResumeEditorProps) {
  const [activeTab, setActiveTab] = useState('editor');
  const [resumeData, setResumeData] = useState(resume?.resumeData || {});
  const [history, setHistory] = useState<any[]>([]);
  const [historyIndex, setHistoryIndex] = useState(-1);
  const [hasUnsavedChanges, setHasUnsavedChanges] = useState(false);
  const [autoSaveEnabled, setAutoSaveEnabled] = useState(true);
  const [lastAutoSave, setLastAutoSave] = useState<Date | null>(null);

  // Initialize resume data if empty
  useEffect(() => {
    if (!resumeData.personalInfo) {
      setResumeData(prev => ({
        ...prev,
        personalInfo: {},
        professionalSummary: {},
        workExperience: [],
        education: [],
        skills: [],
        certifications: [],
        languages: []
      }));
    }
  }, [resumeData.personalInfo]);

  // Auto-save functionality
  useEffect(() => {
    if (autoSaveEnabled && hasUnsavedChanges) {
      const timer = setTimeout(() => {
        handleAutoSave();
      }, 3000); // Auto-save after 3 seconds of inactivity

      return () => clearTimeout(timer);
    }
  }, [resumeData, autoSaveEnabled, hasUnsavedChanges]);

  const handleAutoSave = async () => {
    try {
      await onSave();
      setLastAutoSave(new Date());
      setHasUnsavedChanges(false);
    } catch (error) {
      console.error('Auto-save failed:', error);
    }
  };

  const updateResumeData = (section: string, data: any) => {
    const newResumeData = {
      ...resumeData,
      [section]: data
    };

    setResumeData(newResumeData);
    setHasUnsavedChanges(true);

    // Add to history
    const newHistory = history.slice(0, historyIndex + 1);
    newHistory.push({ section, data: resumeData[section], timestamp: new Date() });
    setHistory(newHistory);
    setHistoryIndex(newHistory.length - 1);

    // Update parent component
    onResumeUpdate({
      ...resume,
      resumeData: newResumeData
    });
  };

  const handleUndo = () => {
    if (historyIndex > 0) {
      const previousState = history[historyIndex - 1];
      const newResumeData = {
        ...resumeData,
        [previousState.section]: previousState.data
      };

      setResumeData(newResumeData);
      setHistoryIndex(historyIndex - 1);
      onResumeUpdate({
        ...resume,
        resumeData: newResumeData
      });
    }
  };

  const handleRedo = () => {
    if (historyIndex < history.length - 1) {
      const nextState = history[historyIndex + 1];
      const newResumeData = {
        ...resumeData,
        [nextState.section]: nextState.data
      };

      setResumeData(newResumeData);
      setHistoryIndex(historyIndex + 1);
      onResumeUpdate({
        ...resume,
        resumeData: newResumeData
      });
    }
  };

  const handleSectionItemsChange = (section: string, items: SectionItem[]) => {
    updateResumeData(section, items);
  };

  const handlePersonalInfoChange = (field: string, value: any) => {
    const newPersonalInfo = {
      ...resumeData.personalInfo,
      [field]: value
    };
    updateResumeData('personalInfo', newPersonalInfo);
  };

  const handleProfessionalSummaryChange = (field: string, value: any) => {
    const newSummary = {
      ...resumeData.professionalSummary,
      [field]: value
    };
    updateResumeData('professionalSummary', newSummary);
  };

  const canUndo = historyIndex > 0;
  const canRedo = historyIndex < history.length - 1;

  return (
    <div className={`h-full flex flex-col ${className}`}>
      {/* Toolbar */}
      <div className="border-b bg-white p-4">
        <div className="flex items-center justify-between">
          <div className="flex items-center gap-2">
            <Button
              onClick={handleUndo}
              disabled={!canUndo}
              variant="outline"
              size="sm"
            >
              <Undo className="h-4 w-4" />
            </Button>
            <Button
              onClick={handleRedo}
              disabled={!canRedo}
              variant="outline"
              size="sm"
            >
              <Redo className="h-4 w-4" />
            </Button>
          </div>

          <div className="flex items-center gap-2">
            {lastAutoSave && (
              <div className="flex items-center gap-1 text-xs text-gray-500">
                <CheckCircle className="h-3 w-3" />
                <span>Auto-saved {lastAutoSave.toLocaleTimeString()}</span>
              </div>
            )}

            <Button
              onClick={onSave}
              disabled={!hasUnsavedChanges}
              size="sm"
            >
              <Save className="h-4 w-4 mr-2" />
              Save
            </Button>
          </div>
        </div>
      </div>

      {/* Main Content */}
      <div className="flex-1 overflow-hidden">
        <Tabs value={activeTab} onValueChange={setActiveTab} className="h-full flex flex-col">
          <div className="border-b bg-gray-50">
            <TabsList className="grid w-full grid-cols-2">
              <TabsTrigger value="editor" className="flex items-center gap-2">
                <Edit3 className="h-4 w-4" />
                Editor
              </TabsTrigger>
              <TabsTrigger value="preview" className="flex items-center gap-2">
                <Eye className="h-4 w-4" />
                Preview
              </TabsTrigger>
            </TabsList>
          </div>

          <TabsContent value="editor" className="flex-1 overflow-hidden">
            <ScrollArea className="h-full">
              <div className="p-6 space-y-6">
                {/* Personal Information */}
                <Card>
                  <CardHeader>
                    <CardTitle className="flex items-center gap-2">
                      <User className="h-5 w-5" />
                      Personal Information
                    </CardTitle>
                    <CardDescription>
                      Your basic contact and personal details
                    </CardDescription>
                  </CardHeader>
                  <CardContent className="space-y-4">
                    <div className="grid grid-cols-2 gap-4">
                      <EditableField
                        value={resumeData.personalInfo?.name || ''}
                        type="text"
                        label="Full Name"
                        placeholder="Enter your full name"
                        required
                        maxLength={100}
                        onSave={(value) => handlePersonalInfoChange('name', value)}
                      />
                      <EditableField
                        value={resumeData.personalInfo?.email || ''}
                        type="email"
                        label="Email"
                        placeholder="your.email@example.com"
                        required
                        maxLength={100}
                        onSave={(value) => handlePersonalInfoChange('email', value)}
                      />
                    </div>
                    <div className="grid grid-cols-2 gap-4">
                      <EditableField
                        value={resumeData.personalInfo?.phone || ''}
                        type="phone"
                        label="Phone"
                        placeholder="+1 (555) 123-4567"
                        required
                        maxLength={20}
                        onSave={(value) => handlePersonalInfoChange('phone', value)}
                      />
                      <EditableField
                        value={resumeData.personalInfo?.location || ''}
                        type="text"
                        label="Location"
                        placeholder="City, Province"
                        required
                        maxLength={100}
                        onSave={(value) => handlePersonalInfoChange('location', value)}
                      />
                    </div>
                    <div className="grid grid-cols-2 gap-4">
                      <EditableField
                        value={resumeData.personalInfo?.linkedin || ''}
                        type="url"
                        label="LinkedIn"
                        placeholder="https://linkedin.com/in/yourprofile"
                        maxLength={200}
                        onSave={(value) => handlePersonalInfoChange('linkedin', value)}
                      />
                      <EditableField
                        value={resumeData.personalInfo?.website || ''}
                        type="url"
                        label="Website"
                        placeholder="https://yourwebsite.com"
                        maxLength={200}
                        onSave={(value) => handlePersonalInfoChange('website', value)}
                      />
                    </div>
                  </CardContent>
                </Card>

                {/* Professional Summary */}
                <Card>
                  <CardHeader>
                    <CardTitle className="flex items-center gap-2">
                      <Sparkles className="h-5 w-5" />
                      Professional Summary
                    </CardTitle>
                    <CardDescription>
                      A compelling overview of your professional background
                    </CardDescription>
                  </CardHeader>
                  <CardContent>
                    <EditableField
                      value={resumeData.professionalSummary?.summary || ''}
                      type="textarea"
                      label="Summary"
                      placeholder="Write a compelling professional summary that highlights your key strengths, experience, and career objectives..."
                      required
                      maxLength={500}
                      onSave={(value) => handleProfessionalSummaryChange('summary', value)}
                    />
                  </CardContent>
                </Card>

                {/* Work Experience */}
                <EditableSection
                  title="Work Experience"
                  description="Your professional work history"
                  items={resumeData.workExperience || []}
                  template={SECTION_TEMPLATES.workExperience}
                  onItemsChange={(items) => handleSectionItemsChange('workExperience', items)}
                  minItems={1}
                  maxItems={10}
                />

                {/* Skills */}
                <EditableSection
                  title="Skills & Competencies"
                  description="Your technical and soft skills"
                  items={resumeData.skills || []}
                  template={SECTION_TEMPLATES.skills}
                  onItemsChange={(items) => handleSectionItemsChange('skills', items)}
                  minItems={3}
                  maxItems={20}
                />

                {/* Education */}
                <EditableSection
                  title="Education"
                  description="Your academic background"
                  items={resumeData.education || []}
                  template={SECTION_TEMPLATES.education}
                  onItemsChange={(items) => handleSectionItemsChange('education', items)}
                  minItems={1}
                  maxItems={5}
                />

                {/* Certifications */}
                <EditableSection
                  title="Certifications"
                  description="Professional certifications and licenses"
                  items={resumeData.certifications || []}
                  template={SECTION_TEMPLATES.certifications}
                  onItemsChange={(items) => handleSectionItemsChange('certifications', items)}
                  minItems={0}
                  maxItems={10}
                />

                {/* Languages */}
                <EditableSection
                  title="Languages"
                  description="Languages you speak and proficiency levels"
                  items={resumeData.languages || []}
                  template={SECTION_TEMPLATES.languages}
                  onItemsChange={(items) => handleSectionItemsChange('languages', items)}
                  minItems={1}
                  maxItems={5}
                />

                {/* Additional Information */}
                <Card>
                  <CardHeader>
                    <CardTitle className="flex items-center gap-2">
                      <Info className="h-5 w-5" />
                      Additional Information
                    </CardTitle>
                    <CardDescription>
                      Any additional relevant information (volunteer work, awards, etc.)
                    </CardDescription>
                  </CardHeader>
                  <CardContent>
                    <EditableField
                      value={resumeData.additionalInfo || ''}
                      type="textarea"
                      label="Additional Information"
                      placeholder="Include any additional relevant information such as volunteer work, awards, publications, or other achievements..."
                      maxLength={300}
                      onSave={(value) => updateResumeData('additionalInfo', value)}
                    />
                  </CardContent>
                </Card>
              </div>
            </ScrollArea>
          </TabsContent>

          <TabsContent value="preview" className="flex-1 overflow-hidden">
            <ScrollArea className="h-full">
              <div className="p-6">
                <div className="bg-white shadow-lg rounded-lg p-8">
                  {/* Preview Header */}
                  <div className="text-center mb-6">
                    <h1 className="text-3xl font-bold text-gray-900 mb-2">
                      {resumeData.personalInfo?.name || 'Your Name'}
                    </h1>
                    
                    <div className="flex items-center justify-center gap-4 text-sm text-gray-600">
                      {resumeData.personalInfo?.email && (
                        <span>{resumeData.personalInfo.email}</span>
                      )}
                      {resumeData.personalInfo?.phone && (
                        <span>{resumeData.personalInfo.phone}</span>
                      )}
                      {resumeData.personalInfo?.location && (
                        <span>{resumeData.personalInfo.location}</span>
                      )}
                    </div>
                  </div>

                  {/* Preview Content */}
                  {resumeData.professionalSummary?.summary && (
                    <div className="mb-6">
                      <h2 className="text-lg font-semibold text-gray-900 mb-2">
                        Professional Summary
                      </h2>
                      <p className="text-gray-700">
                        {resumeData.professionalSummary.summary}
                      </p>
                    </div>
                  )}

                  {/* Work Experience Preview */}
                  {resumeData.workExperience && resumeData.workExperience.length > 0 && (
                    <div className="mb-6">
                      <h2 className="text-lg font-semibold text-gray-900 mb-3">
                        Professional Experience
                      </h2>
                      <div className="space-y-4">
                        {resumeData.workExperience.map((job: any, index: number) => (
                          <div key={index} className="border-l-4 border-blue-500 pl-4">
                            <div className="flex justify-between items-start mb-1">
                              <h3 className="font-semibold text-gray-900">
                                {job.title}
                              </h3>
                              <span className="text-sm text-gray-600">
                                {job.startDate} - {job.current ? 'Present' : job.endDate}
                              </span>
                            </div>
                            <div className="text-gray-700 mb-2">
                              <span className="font-medium">{job.company}</span>
                              {job.location && (
                                <span className="text-gray-600"> • {job.location}</span>
                              )}
                            </div>
                            {job.description && (
                              <p className="text-gray-700 text-sm mb-2">
                                {job.description}
                              </p>
                            )}
                            {job.achievements && job.achievements.length > 0 && (
                              <ul className="list-disc list-inside text-sm text-gray-700 space-y-1">
                                {job.achievements.map((achievement: string, idx: number) => (
                                  <li key={idx}>{achievement}</li>
                                ))}
                              </ul>
                            )}
                          </div>
                        ))}
                      </div>
                    </div>
                  )}

                  {/* Skills Preview */}
                  {resumeData.skills && resumeData.skills.length > 0 && (
                    <div className="mb-6">
                      <h2 className="text-lg font-semibold text-gray-900 mb-3">
                        Skills & Competencies
                      </h2>
                      <div className="grid grid-cols-2 gap-4">
                        {resumeData.skills.map((skill: any, index: number) => (
                          <div key={index} className="flex justify-between items-center">
                            <span className="font-medium text-gray-900">
                              {skill.name}
                              {skill.canadianEquivalent && (
                                <span className="text-xs text-gray-500 ml-1">
                                  ({skill.canadianEquivalent})
                                </span>
                              )}
                            </span>
                            <Badge variant="outline" className="text-xs">
                              {skill.level}
                            </Badge>
                          </div>
                        ))}
                      </div>
                    </div>
                  )}

                  {/* Footer */}
                  <div className="mt-8 pt-4 border-t border-gray-200 text-center text-xs text-gray-500">
                    <p>Generated by ImmiGrowAI - Optimized for Canadian Job Market</p>
                    <p>ATS Score: {resume.atsScore || 85}/100</p>
                  </div>
                </div>
              </div>
            </ScrollArea>
          </TabsContent>
        </Tabs>
      </div>
    </div>
  );
}
```

## File: src/components/features/resume/generator/JobTargeting.tsx
```typescript
"use client";

import React, { useState, useEffect } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Input } from '@/components/ui/input';
import { Label } from '@/components/ui/label';
import { Textarea } from '@/components/ui/textarea';
import { Select, SelectContent, SelectItem, SelectTrigger, SelectValue } from '@/components/ui/select';
import { 
  Target, 
  Building2, 
  MapPin, 
  DollarSign, 
  Briefcase, 
  Loader2, 
  CheckCircle,
  XCircle,
  Info,
  Sparkles,
  AlertCircle
} from 'lucide-react';
import { useResumeGeneratorStore } from '@/stores/resumeGeneratorStore';

// Canadian job market data
const CANADIAN_CITIES = [
  'Toronto, ON', 'Vancouver, BC', 'Montreal, QC', 'Calgary, AB', 'Edmonton, AB',
  'Ottawa, ON', 'Winnipeg, MB', 'Quebec City, QC', 'Hamilton, ON', 'Kitchener, ON',
  'London, ON', 'Victoria, BC', 'Halifax, NS', 'Oshawa, ON', 'Windsor, ON',
  'Saskatoon, SK', 'Regina, SK', 'St. John\'s, NL', 'Kelowna, BC', 'Abbotsford, BC'
];

const CANADIAN_INDUSTRIES = [
  'Technology', 'Healthcare', 'Finance', 'Education', 'Manufacturing',
  'Retail', 'Construction', 'Transportation', 'Energy', 'Government',
  'Non-profit', 'Consulting', 'Real Estate', 'Media', 'Hospitality',
  'Agriculture', 'Mining', 'Telecommunications', 'Biotechnology', 'Aerospace'
];

const EXPERIENCE_LEVELS = [
  { value: 'entry', label: 'Entry Level (0-2 years)' },
  { value: 'mid', label: 'Mid Level (3-7 years)' },
  { value: 'senior', label: 'Senior Level (8-15 years)' },
  { value: 'executive', label: 'Executive Level (15+ years)' }
];

export default function JobTargeting() {
  const { jobTargeting, setJobTargeting } = useResumeGeneratorStore();
  const [errors, setErrors] = useState<Record<string, string>>({});

  // Character limits
  const CHAR_LIMITS = {
    jobTitle: 255,
    companyName: 255,
    industry: 100,
    location: 255,
    jobDescription: 10000
  };

  const handleInputChange = (field: string, value: string) => {
    setJobTargeting({ ...jobTargeting, [field]: value });
    
    // Clear error when user starts typing
    if (errors[field]) {
      setErrors(prev => ({ ...prev, [field]: '' }));
    }
  };

  const handleSalaryChange = (type: 'min' | 'max', value: string) => {
    const numValue = value ? parseInt(value) : null;
    setJobTargeting({
      ...jobTargeting,
      salaryRange: {
        ...jobTargeting.salaryRange,
        [type]: numValue
      }
    });
  };

  const handleSkillsChange = (type: 'required' | 'preferred', skills: string[]) => {
    setJobTargeting({
      ...jobTargeting,
      [type === 'required' ? 'requiredSkills' : 'preferredSkills']: skills
    });
  };

  const addSkill = (type: 'required' | 'preferred', skill: string) => {
    if (skill.trim()) {
      const currentSkills = type === 'required' ? jobTargeting.requiredSkills : jobTargeting.preferredSkills;
      if (!currentSkills.includes(skill.trim())) {
        handleSkillsChange(type, [...currentSkills, skill.trim()]);
      }
    }
  };

  const removeSkill = (type: 'required' | 'preferred', skillToRemove: string) => {
    const currentSkills = type === 'required' ? jobTargeting.requiredSkills : jobTargeting.preferredSkills;
    handleSkillsChange(type, currentSkills.filter(skill => skill !== skillToRemove));
  };



  const validateField = (field: string, value: any): string => {
    switch (field) {
      case 'jobTitle':
        if (!value || value.trim().length === 0) {
          return 'Job title is required';
        }
        if (value.length > CHAR_LIMITS.jobTitle) {
          return `Job title cannot exceed ${CHAR_LIMITS.jobTitle} characters`;
        }
        break;
      case 'companyName':
        if (!value || value.trim().length === 0) {
          return 'Company name is required';
        }
        if (value.length > CHAR_LIMITS.companyName) {
          return `Company name cannot exceed ${CHAR_LIMITS.companyName} characters`;
        }
        break;
      case 'jobDescription':
        if (value && value.length > CHAR_LIMITS.jobDescription) {
          return `Job description cannot exceed ${CHAR_LIMITS.jobDescription} characters`;
        }
        break;
      case 'salaryRange':
        if (jobTargeting.salaryRange?.min && jobTargeting.salaryRange?.max) {
          if (jobTargeting.salaryRange.min > jobTargeting.salaryRange.max) {
            return 'Minimum salary cannot be greater than maximum salary';
          }
        }
        break;
    }
    return '';
  };

  const getCharacterCount = (field: string): number => {
    return jobTargeting[field as keyof typeof jobTargeting]?.toString().length || 0;
  };

  const getCharacterCountColor = (field: string): string => {
    const count = getCharacterCount(field);
    const limit = CHAR_LIMITS[field as keyof typeof CHAR_LIMITS];
    const percentage = (count / limit) * 100;
    
    if (percentage >= 90) return 'text-red-600';
    if (percentage >= 75) return 'text-yellow-600';
    return 'text-gray-500';
  };

  return (
    <div className="space-y-6">
      {/* Basic Information */}
      <Card>
        <CardHeader>
          <CardTitle className="flex items-center gap-2">
            <Target className="h-5 w-5 text-blue-600" />
            Basic Information
          </CardTitle>
          <CardDescription>
            Essential details about the position you're targeting.
          </CardDescription>
        </CardHeader>
        <CardContent className="space-y-4">
          {/* Job Title */}
          <div className="space-y-2">
            <Label htmlFor="jobTitle" className="flex items-center gap-2">
              Job Title *
              {errors.jobTitle && <AlertCircle className="h-4 w-4 text-red-500" />}
            </Label>
                                      <Input
               id="jobTitle"
               placeholder="e.g., Senior Software Engineer"
               value={jobTargeting.jobTitle}
               onChange={(e) => handleInputChange('jobTitle', e.target.value)}
               className={errors.jobTitle ? 'border-red-500' : ''}
             />
            <div className="flex justify-between items-center">
              {errors.jobTitle && (
                <span className="text-sm text-red-600">{errors.jobTitle}</span>
              )}
              <span className={`text-xs ${getCharacterCountColor('jobTitle')}`}>
                {getCharacterCount('jobTitle')}/{CHAR_LIMITS.jobTitle}
              </span>
            </div>
          </div>

          {/* Company Name */}
          <div className="space-y-2">
            <Label htmlFor="companyName" className="flex items-center gap-2">
              Company Name *
              {errors.companyName && <AlertCircle className="h-4 w-4 text-red-500" />}
            </Label>
                                      <Input
               id="companyName"
               placeholder="e.g., Shopify"
               value={jobTargeting.companyName}
               onChange={(e) => handleInputChange('companyName', e.target.value)}
               className={errors.companyName ? 'border-red-500' : ''}
             />
            <div className="flex justify-between items-center">
              {errors.companyName && (
                <span className="text-sm text-red-600">{errors.companyName}</span>
              )}
              <span className={`text-xs ${getCharacterCountColor('companyName')}`}>
                {getCharacterCount('companyName')}/{CHAR_LIMITS.companyName}
              </span>
            </div>
          </div>

          {/* Industry and Location */}
          <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
            <div className="space-y-2">
              <Label htmlFor="industry">Industry</Label>
              <Select value={jobTargeting.industry} onValueChange={(value) => handleInputChange('industry', value)}>
                <SelectTrigger>
                  <SelectValue placeholder="Select industry" />
                </SelectTrigger>
                <SelectContent>
                  {CANADIAN_INDUSTRIES.map((industry) => (
                    <SelectItem key={industry} value={industry}>
                      {industry}
                    </SelectItem>
                  ))}
                </SelectContent>
              </Select>
            </div>

            <div className="space-y-2">
              <Label htmlFor="location">Location</Label>
              <Select value={jobTargeting.location} onValueChange={(value) => handleInputChange('location', value)}>
                <SelectTrigger>
                  <SelectValue placeholder="Select location" />
                </SelectTrigger>
                <SelectContent>
                  {CANADIAN_CITIES.map((city) => (
                    <SelectItem key={city} value={city}>
                      {city}
                    </SelectItem>
                  ))}
                </SelectContent>
              </Select>
            </div>
          </div>

          {/* Experience Level */}
          <div className="space-y-2">
            <Label htmlFor="experienceLevel">Experience Level</Label>
            <Select value={jobTargeting.experienceLevel || ''} onValueChange={(value) => handleInputChange('experienceLevel', value)}>
              <SelectTrigger>
                <SelectValue placeholder="Select experience level" />
              </SelectTrigger>
              <SelectContent>
                {EXPERIENCE_LEVELS.map((level) => (
                  <SelectItem key={level.value} value={level.value}>
                    {level.label}
                  </SelectItem>
                ))}
              </SelectContent>
            </Select>
          </div>
        </CardContent>
      </Card>

      {/* Job Description */}
      <Card>
        <CardHeader>
          <CardTitle className="flex items-center gap-2">
            <Info className="h-5 w-5 text-orange-600" />
            Job Description
          </CardTitle>
          <CardDescription>
            Paste the full job description for optimal AI analysis and keyword matching.
          </CardDescription>
        </CardHeader>
        <CardContent>
          <div className="space-y-2">
            <Label htmlFor="jobDescription">Job Description</Label>
            <Textarea
              id="jobDescription"
              placeholder="Paste the complete job description here..."
              value={jobTargeting.jobDescription}
              onChange={(e) => handleInputChange('jobDescription', e.target.value)}
              rows={8}
              className="resize-none"
            />
            <div className="flex justify-between items-center">
              <span className="text-sm text-gray-500">
                Including the full job description helps with keyword optimization and ATS scoring.
              </span>
              <span className={`text-xs ${getCharacterCountColor('jobDescription')}`}>
                {getCharacterCount('jobDescription')}/{CHAR_LIMITS.jobDescription}
              </span>
            </div>
          </div>
        </CardContent>
      </Card>

      {/* Salary Range */}
      <Card>
        <CardHeader>
          <CardTitle className="flex items-center gap-2">
            <DollarSign className="h-5 w-5 text-green-600" />
            Salary Range (Optional)
          </CardTitle>
          <CardDescription>
            Help us optimize your resume for the expected salary range.
          </CardDescription>
        </CardHeader>
        <CardContent>
          <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
            <div className="space-y-2">
              <Label htmlFor="salaryMin">Minimum Salary (CAD)</Label>
              <Input
                id="salaryMin"
                type="number"
                placeholder="e.g., 60000"
                value={jobTargeting.salaryRange?.min || ''}
                onChange={(e) => handleSalaryChange('min', e.target.value)}
              />
            </div>
            <div className="space-y-2">
              <Label htmlFor="salaryMax">Maximum Salary (CAD)</Label>
              <Input
                id="salaryMax"
                type="number"
                placeholder="e.g., 80000"
                value={jobTargeting.salaryRange?.max || ''}
                onChange={(e) => handleSalaryChange('max', e.target.value)}
              />
            </div>
          </div>
          {errors.salaryRange && (
            <span className="text-sm text-red-600 mt-2">{errors.salaryRange}</span>
          )}
        </CardContent>
      </Card>

      {/* Skills */}
      <Card>
        <CardHeader>
          <CardTitle className="flex items-center gap-2">
            <Briefcase className="h-5 w-5 text-purple-600" />
            Required & Preferred Skills (Optional)
          </CardTitle>
          <CardDescription>
            Add skills mentioned in the job description for better ATS optimization.
          </CardDescription>
        </CardHeader>
        <CardContent className="space-y-6">
          {/* Required Skills */}
          <div className="space-y-3">
            <Label>Required Skills</Label>
            <div className="flex flex-wrap gap-2">
              {jobTargeting.requiredSkills.map((skill, index) => (
                <Badge key={index} variant="secondary" className="flex items-center gap-1">
                  {skill}
                  <button
                    onClick={() => removeSkill('required', skill)}
                    className="ml-1 hover:text-red-600"
                  >
                    <XCircle className="h-3 w-3" />
                  </button>
                </Badge>
              ))}
            </div>
            <div className="flex gap-2">
              <Input
                placeholder="Add required skill"
                onKeyPress={(e) => {
                  if (e.key === 'Enter') {
                    addSkill('required', e.currentTarget.value);
                    e.currentTarget.value = '';
                  }
                }}
              />
              <Button
                variant="outline"
                onClick={(e) => {
                  const input = e.currentTarget.previousElementSibling as HTMLInputElement;
                  addSkill('required', input.value);
                  input.value = '';
                }}
              >
                Add
              </Button>
            </div>
          </div>

          {/* Preferred Skills */}
          <div className="space-y-3">
            <Label>Preferred Skills</Label>
            <div className="flex flex-wrap gap-2">
              {jobTargeting.preferredSkills.map((skill, index) => (
                <Badge key={index} variant="outline" className="flex items-center gap-1">
                  {skill}
                  <button
                    onClick={() => removeSkill('preferred', skill)}
                    className="ml-1 hover:text-red-600"
                  >
                    <XCircle className="h-3 w-3" />
                  </button>
                </Badge>
              ))}
            </div>
            <div className="flex gap-2">
              <Input
                placeholder="Add preferred skill"
                onKeyPress={(e) => {
                  if (e.key === 'Enter') {
                    addSkill('preferred', e.currentTarget.value);
                    e.currentTarget.value = '';
                  }
                }}
              />
              <Button
                variant="outline"
                onClick={(e) => {
                  const input = e.currentTarget.previousElementSibling as HTMLInputElement;
                  addSkill('preferred', input.value);
                  input.value = '';
                }}
              >
                Add
              </Button>
            </div>
          </div>
        </CardContent>
      </Card>
    </div>
  );
}
```

## File: src/components/features/resume/generator/ResumePDFView.tsx
```typescript
"use client";

import React from 'react';
import { Badge } from '@/components/ui/badge';
import { 
  Mail, 
  Phone, 
  MapPin, 
  Globe, 
  Linkedin,
  Calendar,
  Star,
  Award,
  GraduationCap,
  Briefcase,
  User,
  Target
} from 'lucide-react';

export interface ResumePDFViewProps {
  resume: any;
  className?: string;
}

export default function ResumePDFView({ resume, className = '' }: ResumePDFViewProps) {
  const resumeData = resume?.resumeData || {};
  const personalInfo = resumeData.personalInfo || {};
  const professionalSummary = resumeData.professionalSummary || {};
  const workExperience = resumeData.workExperience || [];
  const education = resumeData.education || [];
  const skills = resumeData.skills || [];
  const certifications = resumeData.certifications || [];
  const languages = resumeData.languages || [];

  const formatDate = (date: string) => {
    if (!date) return '';
    return new Date(date).toLocaleDateString('en-CA', {
      year: 'numeric',
      month: 'short'
    });
  };

  const getSkillLevel = (level: string) => {
    switch (level) {
      case 'expert': return 'Expert';
      case 'advanced': return 'Advanced';
      case 'intermediate': return 'Intermediate';
      case 'beginner': return 'Beginner';
      default: return level;
    }
  };

  return (
    <div className={`bg-white ${className}`}>
      {/* A4 Container */}
      <div className="mx-auto bg-white shadow-lg" style={{ 
        width: '210mm', 
        minHeight: '297mm',
        padding: '20mm',
        boxSizing: 'border-box'
      }}>
        {/* Header */}
        <div className="text-center mb-6">
          <h1 className="text-3xl font-bold text-gray-900 mb-2">
            {personalInfo.name || 'Your Name'}
          </h1>
          
          <div className="flex items-center justify-center gap-4 text-sm text-gray-600 mb-2">
            {personalInfo.email && (
              <div className="flex items-center gap-1">
                <Mail className="h-4 w-4" />
                <span>{personalInfo.email}</span>
              </div>
            )}
            
            {personalInfo.phone && (
              <div className="flex items-center gap-1">
                <Phone className="h-4 w-4" />
                <span>{personalInfo.phone}</span>
              </div>
            )}
            
            {personalInfo.location && (
              <div className="flex items-center gap-1">
                <MapPin className="h-4 w-4" />
                <span>{personalInfo.location}</span>
              </div>
            )}
          </div>
          
          <div className="flex items-center justify-center gap-4 text-sm text-gray-600">
            {personalInfo.linkedin && (
              <div className="flex items-center gap-1">
                <Linkedin className="h-4 w-4" />
                <span>{personalInfo.linkedin}</span>
              </div>
            )}
            
            {personalInfo.website && (
              <div className="flex items-center gap-1">
                <Globe className="h-4 w-4" />
                <span>{personalInfo.website}</span>
              </div>
            )}
          </div>
        </div>

        {/* Professional Summary */}
        {professionalSummary.summary && (
          <div className="mb-6">
            <h2 className="text-lg font-semibold text-gray-900 mb-2 flex items-center gap-2">
              <User className="h-5 w-5" />
              Professional Summary
            </h2>
            <p className="text-gray-700 leading-relaxed">
              {professionalSummary.summary}
            </p>
          </div>
        )}

        {/* Work Experience */}
        {workExperience.length > 0 && (
          <div className="mb-6">
            <h2 className="text-lg font-semibold text-gray-900 mb-3 flex items-center gap-2">
              <Briefcase className="h-5 w-5" />
              Professional Experience
            </h2>
            
            <div className="space-y-4">
              {workExperience.map((job: any, index: number) => (
                <div key={index} className="border-l-4 border-blue-500 pl-4">
                  <div className="flex justify-between items-start mb-1">
                    <h3 className="font-semibold text-gray-900">
                      {job.title}
                    </h3>
                    <span className="text-sm text-gray-600">
                      {formatDate(job.startDate)} - {job.current ? 'Present' : formatDate(job.endDate)}
                    </span>
                  </div>
                  
                  <div className="text-gray-700 mb-2">
                    <span className="font-medium">{job.company}</span>
                    {job.location && (
                      <span className="text-gray-600"> • {job.location}</span>
                    )}
                  </div>
                  
                  {job.description && (
                    <p className="text-gray-700 text-sm mb-2">
                      {job.description}
                    </p>
                  )}
                  
                  {job.achievements && job.achievements.length > 0 && (
                    <ul className="list-disc list-inside text-sm text-gray-700 space-y-1">
                      {job.achievements.map((achievement: string, idx: number) => (
                        <li key={idx}>{achievement}</li>
                      ))}
                    </ul>
                  )}
                </div>
              ))}
            </div>
          </div>
        )}

        {/* Skills */}
        {skills.length > 0 && (
          <div className="mb-6">
            <h2 className="text-lg font-semibold text-gray-900 mb-3 flex items-center gap-2">
              <Target className="h-5 w-5" />
              Skills & Competencies
            </h2>
            
            <div className="grid grid-cols-2 gap-4">
              {skills.map((skill: any, index: number) => (
                <div key={index} className="flex justify-between items-center">
                  <span className="font-medium text-gray-900">
                    {skill.name}
                    {skill.canadianEquivalent && (
                      <span className="text-xs text-gray-500 ml-1">
                        ({skill.canadianEquivalent})
                      </span>
                    )}
                  </span>
                  <Badge variant="outline" className="text-xs">
                    {getSkillLevel(skill.level)}
                  </Badge>
                </div>
              ))}
            </div>
          </div>
        )}

        {/* Education */}
        {education.length > 0 && (
          <div className="mb-6">
            <h2 className="text-lg font-semibold text-gray-900 mb-3 flex items-center gap-2">
              <GraduationCap className="h-5 w-5" />
              Education
            </h2>
            
            <div className="space-y-3">
              {education.map((edu: any, index: number) => (
                <div key={index} className="border-l-4 border-green-500 pl-4">
                  <div className="flex justify-between items-start mb-1">
                    <h3 className="font-semibold text-gray-900">
                      {edu.degree}
                    </h3>
                    <span className="text-sm text-gray-600">
                      {formatDate(edu.startDate)} - {edu.current ? 'Present' : formatDate(edu.endDate)}
                    </span>
                  </div>
                  
                  <div className="text-gray-700 mb-1">
                    <span className="font-medium">{edu.institution}</span>
                    {edu.location && (
                      <span className="text-gray-600"> • {edu.location}</span>
                    )}
                  </div>
                  
                  {edu.gpa && (
                    <div className="text-sm text-gray-600">
                      GPA: {edu.gpa}
                    </div>
                  )}
                  
                  {edu.relevantCourses && edu.relevantCourses.length > 0 && (
                    <div className="text-sm text-gray-700 mt-1">
                      <span className="font-medium">Relevant Courses:</span> {edu.relevantCourses.join(', ')}
                    </div>
                  )}
                </div>
              ))}
            </div>
          </div>
        )}

        {/* Certifications */}
        {certifications.length > 0 && (
          <div className="mb-6">
            <h2 className="text-lg font-semibold text-gray-900 mb-3 flex items-center gap-2">
              <Award className="h-5 w-5" />
              Certifications
            </h2>
            
            <div className="space-y-2">
              {certifications.map((cert: any, index: number) => (
                <div key={index} className="flex justify-between items-center">
                  <div>
                    <span className="font-medium text-gray-900">{cert.name}</span>
                    {cert.issuer && (
                      <span className="text-gray-600 text-sm ml-2">• {cert.issuer}</span>
                    )}
                  </div>
                  <span className="text-sm text-gray-600">
                    {formatDate(cert.date)}
                  </span>
                </div>
              ))}
            </div>
          </div>
        )}

        {/* Languages */}
        {languages.length > 0 && (
          <div className="mb-6">
            <h2 className="text-lg font-semibold text-gray-900 mb-3 flex items-center gap-2">
              <Globe className="h-5 w-5" />
              Languages
            </h2>
            
            <div className="grid grid-cols-2 gap-4">
              {languages.map((lang: any, index: number) => (
                <div key={index} className="flex justify-between items-center">
                  <span className="font-medium text-gray-900">{lang.language}</span>
                  <Badge variant="outline" className="text-xs">
                    {lang.proficiency}
                  </Badge>
                </div>
              ))}
            </div>
          </div>
        )}

        {/* Additional Information */}
        {resumeData.additionalInfo && (
          <div className="mb-6">
            <h2 className="text-lg font-semibold text-gray-900 mb-3 flex items-center gap-2">
              <Star className="h-5 w-5" />
              Additional Information
            </h2>
            <p className="text-gray-700 leading-relaxed">
              {resumeData.additionalInfo}
            </p>
          </div>
        )}

        {/* Footer */}
        <div className="mt-8 pt-4 border-t border-gray-200 text-center text-xs text-gray-500">
          <p>Generated by ImmiGrowAI - Optimized for Canadian Job Market</p>
          <p>ATS Score: {resume.atsScore || 85}/100</p>
        </div>
      </div>
    </div>
  );
}
```

## File: src/components/features/resume/generator/ResumeSelector.tsx
```typescript
"use client";

import React, { useState, useEffect } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Input } from '@/components/ui/input';
import { 
  FileText, 
  CheckCircle, 
  XCircle, 
  Search,
  Calendar,
  Briefcase,
  GraduationCap,
  Award,
  Clock,
  Plus,
  Upload
} from 'lucide-react';
import { useResumeGeneratorStore } from '@/stores/resumeGeneratorStore';
import { getUserResumeAnalyses } from '@/lib/api';

interface ResumeAnalysis {
  analysisId: string;
  personalInfo: {
    name: string;
    email: string;
    phone: string;
    location: string;
    confidence: number;
  };
  summary: {
    professionalSummary: string;
    careerLevel: string;
    industries: string[];
    confidence: number;
  };
  workExperience: Array<{
    title: string;
    company: string;
    startDate: string;
    endDate: string;
    location: string;
    responsibilities: string[];
    confidence: number;
  }>;
  education: Array<{
    degree: string;
    institution: string;
    year: string;
    location: string;
    confidence: number;
  }>;
  skills: {
    technical: string[];
    soft: string[];
    languages: Array<string | { language: string; proficiency: string }>;
    confidence: number;
  };
  metadata?: {
    processedAt: string;
    originalFileName: string;
    processingMethod: string;
    apiVersion: string;
  };
}

interface ResumeSelectorProps {
  onResumeSelect?: (analysisId: string) => void;
  onUploadNew?: () => void;
  selectedResumeId?: string | null;
  showUploadOption?: boolean;
  className?: string;
  maxHeight?: string;
}

export default function ResumeSelector({
  onResumeSelect,
  onUploadNew,
  selectedResumeId,
  showUploadOption = true,
  className = "",
  maxHeight = "600px"
}: ResumeSelectorProps) {
  const [resumeAnalyses, setResumeAnalyses] = useState<ResumeAnalysis[]>([]);
  const [isLoading, setIsLoading] = useState(true);
  const [searchQuery, setSearchQuery] = useState('');
  const [error, setError] = useState<string | null>(null);

  const { setSelectedResumeId } = useResumeGeneratorStore();

  useEffect(() => {
    loadResumeAnalyses();
  }, []);

  const loadResumeAnalyses = async () => {
    try {
      setIsLoading(true);
      const response = await getUserResumeAnalyses();
      if (response.success && response.data) {
        setResumeAnalyses(response.data);
      }
    } catch (error) {
      console.error('Failed to load resume analyses:', error);
      setError('Failed to load your resume analyses. Please try again.');
    } finally {
      setIsLoading(false);
    }
  };

  const handleResumeSelect = (analysisId: string) => {
    setSelectedResumeId(analysisId);
    onResumeSelect?.(analysisId);
  };

  const filteredResumes = resumeAnalyses.filter(resume => 
    resume.personalInfo.name.toLowerCase().includes(searchQuery.toLowerCase()) ||
    resume.summary.professionalSummary.toLowerCase().includes(searchQuery.toLowerCase()) ||
    resume.workExperience.some(exp => 
      exp.title.toLowerCase().includes(searchQuery.toLowerCase()) ||
      exp.company.toLowerCase().includes(searchQuery.toLowerCase())
    )
  );

  const getConfidenceColor = (confidence: number) => {
    if (confidence >= 80) return 'bg-green-100 text-green-800';
    if (confidence >= 60) return 'bg-yellow-100 text-yellow-800';
    return 'bg-red-100 text-red-800';
  };

  const getConfidenceIcon = (confidence: number) => {
    if (confidence >= 80) return <CheckCircle className="h-4 w-4" />;
    if (confidence >= 60) return <Clock className="h-4 w-4" />;
    return <XCircle className="h-4 w-4" />;
  };

  if (isLoading) {
    return (
      <div className={`flex items-center justify-center p-8 ${className}`}>
        <div className="flex items-center gap-2">
          <div className="animate-spin rounded-full h-6 w-6 border-b-2 border-blue-600"></div>
          <span className="text-gray-600">Loading resumes...</span>
        </div>
      </div>
    );
  }

  if (error) {
    return (
      <div className={`p-4 ${className}`}>
        <div className="flex items-center gap-2 p-3 bg-red-50 border border-red-200 rounded-md">
          <XCircle className="h-4 w-4 text-red-600" />
          <span className="text-sm text-red-800">{error}</span>
        </div>
      </div>
    );
  }

  return (
    <div className={`space-y-4 ${className}`}>
      {/* Search Bar */}
      <div className="relative">
        <Search className="absolute left-3 top-1/2 transform -translate-y-1/2 text-gray-400 h-4 w-4" />
        <Input
          placeholder="Search resumes by name, title, or company..."
          value={searchQuery}
          onChange={(e) => setSearchQuery(e.target.value)}
          className="pl-10"
        />
      </div>

      {/* Upload New Option */}
      {showUploadOption && (
        <Card 
          className="cursor-pointer transition-all hover:shadow-md border-dashed border-2 border-gray-300 hover:border-blue-400"
          onClick={onUploadNew}
        >
          <CardContent className="flex items-center justify-center py-8">
            <div className="flex items-center gap-3 text-gray-600">
              <Upload className="h-6 w-6" />
              <span className="font-medium">Upload New Resume</span>
            </div>
          </CardContent>
        </Card>
      )}

      {/* Resume List */}
      <div 
        className="space-y-3 overflow-y-auto"
        style={{ maxHeight }}
      >
        {filteredResumes.length === 0 ? (
          <Card>
            <CardContent className="flex flex-col items-center justify-center py-8">
              <FileText className="h-12 w-12 text-gray-400 mb-4" />
              <h3 className="text-lg font-semibold text-gray-900 mb-2">
                No resume analyses found
              </h3>
              <p className="text-gray-600 text-center mb-4">
                {searchQuery ? 'No resumes match your search criteria.' : 'You haven\'t analyzed any resumes yet.'}
              </p>
              {showUploadOption && onUploadNew && (
                <Button 
                  onClick={onUploadNew}
                  variant="outline"
                  size="sm"
                >
                  <Plus className="h-4 w-4 mr-2" />
                  Analyze a Resume
                </Button>
              )}
            </CardContent>
          </Card>
        ) : (
          filteredResumes.map((resume) => (
            <Card 
              key={resume.analysisId}
              className={`cursor-pointer transition-all hover:shadow-md ${
                selectedResumeId === resume.analysisId 
                  ? 'ring-2 ring-blue-500 bg-blue-50' 
                  : 'hover:bg-gray-50'
              }`}
              onClick={() => handleResumeSelect(resume.analysisId)}
            >
              <CardHeader className="pb-3">
                <div className="flex items-start justify-between">
                  <div className="flex-1 min-w-0">
                    <CardTitle className="text-lg mb-1 truncate">
                      {resume.personalInfo.name}
                    </CardTitle>
                    <CardDescription className="line-clamp-2 text-sm">
                      {resume.summary.professionalSummary}
                    </CardDescription>
                  </div>
                  {selectedResumeId === resume.analysisId && (
                    <CheckCircle className="h-5 w-5 text-blue-500 flex-shrink-0 ml-2" />
                  )}
                </div>
              </CardHeader>
              <CardContent className="pt-0">
                <div className="space-y-2">
                  {/* Quick Stats */}
                  <div className="flex items-center gap-4 text-xs text-gray-600">
                    <div className="flex items-center gap-1">
                      <Briefcase className="h-3 w-3" />
                      <span>{resume.workExperience.length} position{resume.workExperience.length !== 1 ? 's' : ''}</span>
                    </div>
                    <div className="flex items-center gap-1">
                      <GraduationCap className="h-3 w-3" />
                      <span>{resume.education.length} education{resume.education.length !== 1 ? 's' : ''}</span>
                    </div>
                    <div className="flex items-center gap-1">
                      <Award className="h-3 w-3" />
                      <span>{resume.skills.technical.length + resume.skills.soft.length} skills</span>
                    </div>
                  </div>

                  {/* Confidence and Date */}
                  <div className="flex items-center justify-between">
                    <Badge className={getConfidenceColor(resume.personalInfo.confidence)}>
                      <div className="flex items-center gap-1">
                        {getConfidenceIcon(resume.personalInfo.confidence)}
                        {resume.personalInfo.confidence}% confidence
                      </div>
                    </Badge>
                    
                    {resume.metadata && (
                      <div className="flex items-center gap-1 text-xs text-gray-500">
                        <Calendar className="h-3 w-3" />
                        {new Date(resume.metadata.processedAt).toLocaleDateString()}
                      </div>
                    )}
                  </div>

                  {/* Top Skills Preview */}
                  {resume.skills.technical.length > 0 && (
                    <div className="flex flex-wrap gap-1">
                      {resume.skills.technical.slice(0, 3).map((skill, index) => (
                        <Badge key={index} variant="secondary" className="text-xs">
                          {skill}
                        </Badge>
                      ))}
                      {resume.skills.technical.length > 3 && (
                        <Badge variant="outline" className="text-xs">
                          +{resume.skills.technical.length - 3} more
                        </Badge>
                      )}
                    </div>
                  )}
                </div>
              </CardContent>
            </Card>
          ))
        )}
      </div>

      {/* Results Count */}
      {filteredResumes.length > 0 && (
        <div className="text-sm text-gray-500 text-center pt-2">
          Showing {filteredResumes.length} of {resumeAnalyses.length} resume{resumeAnalyses.length !== 1 ? 's' : ''}
        </div>
      )}
    </div>
  );
}
```

## File: src/components/features/resume/generator/SuggestionPanel.tsx
```typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { 
  Sparkles, 
  Target, 
  Brain, 
  FileText, 
  CheckCircle, 
  XCircle, 
  Plus,
  Star,
  TrendingUp,
  Lightbulb,
  MessageSquare,
  Zap
} from 'lucide-react';

export interface Suggestion {
  id: string;
  type: 'content' | 'format' | 'keyword' | 'achievement' | 'skill' | 'optimization';
  category: string;
  title: string;
  description: string;
  content: string;
  confidence: number;
  impact: 'high' | 'medium' | 'low';
  applied: boolean;
  rejected: boolean;
}

export interface SuggestionPanelProps {
  resume: any;
  onSuggestionApply: (suggestion: Suggestion) => void;
  onSuggestionReject?: (suggestionId: string) => void;
  className?: string;
}

const SUGGESTION_CATEGORIES = [
  {
    id: 'content',
    name: 'Content',
    icon: FileText,
    description: 'Improve your resume content'
  },
  {
    id: 'format',
    name: 'Format',
    icon: Target,
    description: 'Optimize formatting and structure'
  },
  {
    id: 'keyword',
    name: 'Keywords',
    icon: Brain,
    description: 'Add relevant keywords for ATS'
  },
  {
    id: 'achievement',
    name: 'Achievements',
    icon: Star,
    description: 'Enhance your achievements'
  },
  {
    id: 'skill',
    name: 'Skills',
    icon: TrendingUp,
    description: 'Improve skills section'
  },
  {
    id: 'optimization',
    name: 'Optimization',
    icon: Zap,
    description: 'General optimization tips'
  }
];

// Mock suggestions - in real app, these would come from AI analysis
const generateMockSuggestions = (resume: any): Suggestion[] => {
  const suggestions: Suggestion[] = [];

  // Content suggestions
  suggestions.push({
    id: 'content-1',
    type: 'content',
    category: 'Professional Summary',
    title: 'Strengthen Professional Summary',
    description: 'Make your summary more impactful with quantifiable achievements',
    content: 'Results-driven professional with 5+ years of experience in software development, specializing in full-stack applications and team leadership. Proven track record of delivering 15+ successful projects on time and within budget.',
    confidence: 0.92,
    impact: 'high',
    applied: false,
    rejected: false
  });

  // Keyword suggestions
  suggestions.push({
    id: 'keyword-1',
    type: 'keyword',
    category: 'Skills',
    title: 'Add Industry Keywords',
    description: 'Include keywords commonly used in Canadian job postings',
    content: 'React, Node.js, TypeScript, AWS, Docker, Kubernetes, CI/CD, Agile, Scrum',
    confidence: 0.88,
    impact: 'high',
    applied: false,
    rejected: false
  });

  // Achievement suggestions
  suggestions.push({
    id: 'achievement-1',
    type: 'achievement',
    category: 'Work Experience',
    title: 'Quantify Achievements',
    description: 'Add specific metrics to demonstrate impact',
    content: 'Led development team of 8 engineers to deliver 3 major features, resulting in 40% increase in user engagement and 25% reduction in system downtime.',
    confidence: 0.85,
    impact: 'medium',
    applied: false,
    rejected: false
  });

  // Format suggestions
  suggestions.push({
    id: 'format-1',
    type: 'format',
    category: 'Layout',
    title: 'Optimize for ATS',
    description: 'Improve formatting for better ATS parsing',
    content: 'Use standard section headers, bullet points for achievements, and consistent formatting throughout.',
    confidence: 0.78,
    impact: 'medium',
    applied: false,
    rejected: false
  });

  // Skill suggestions
  suggestions.push({
    id: 'skill-1',
    type: 'skill',
    category: 'Technical Skills',
    title: 'Add Canadian Market Skills',
    description: 'Include skills valued in the Canadian tech market',
    content: 'Canadian work experience, bilingual (English/French), knowledge of Canadian regulations, experience with Canadian companies',
    confidence: 0.82,
    impact: 'high',
    applied: false,
    rejected: false
  });

  // Optimization suggestions
  suggestions.push({
    id: 'optimization-1',
    type: 'optimization',
    category: 'General',
    title: 'Canadian Resume Best Practices',
    description: 'Follow Canadian resume conventions',
    content: 'Include Canadian phone number format, use Canadian date format (DD/MM/YYYY), mention Canadian work authorization status.',
    confidence: 0.90,
    impact: 'high',
    applied: false,
    rejected: false
  });

  return suggestions;
};

export default function SuggestionPanel({
  resume,
  onSuggestionApply,
  onSuggestionReject,
  className = ''
}: SuggestionPanelProps) {
  const [suggestions, setSuggestions] = useState<Suggestion[]>(() => generateMockSuggestions(resume));
  const [activeCategory, setActiveCategory] = useState('content');

  const handleApplySuggestion = (suggestion: Suggestion) => {
    setSuggestions(prev => 
      prev.map(s => 
        s.id === suggestion.id 
          ? { ...s, applied: true, rejected: false }
          : s
      )
    );
    onSuggestionApply(suggestion);
  };

  const handleRejectSuggestion = (suggestionId: string) => {
    setSuggestions(prev => 
      prev.map(s => 
        s.id === suggestionId 
          ? { ...s, rejected: true, applied: false }
          : s
      )
    );
    onSuggestionReject?.(suggestionId);
  };

  const getImpactColor = (impact: string) => {
    switch (impact) {
      case 'high': return 'text-red-600 bg-red-50';
      case 'medium': return 'text-yellow-600 bg-yellow-50';
      case 'low': return 'text-green-600 bg-green-50';
      default: return 'text-gray-600 bg-gray-50';
    }
  };

  const getConfidenceColor = (confidence: number) => {
    if (confidence >= 0.9) return 'text-green-600';
    if (confidence >= 0.8) return 'text-blue-600';
    if (confidence >= 0.7) return 'text-yellow-600';
    return 'text-gray-600';
  };

  const filteredSuggestions = suggestions.filter(s => 
    s.type === activeCategory && !s.rejected
  );

  const appliedCount = suggestions.filter(s => s.applied).length;
  const totalCount = suggestions.length;

  return (
    <div className={`h-full flex flex-col ${className}`}>
      {/* Header */}
      <div className="p-4 border-b bg-white">
        <div className="flex items-center gap-2 mb-2">
          <Sparkles className="h-5 w-5 text-purple-600" />
          <h2 className="text-lg font-semibold text-gray-900">AI Suggestions</h2>
        </div>
        <p className="text-sm text-gray-600 mb-3">
          AI-powered recommendations to improve your resume
        </p>
        
        <div className="flex items-center justify-between">
          <Badge variant="secondary" className="text-sm">
            {appliedCount}/{totalCount} applied
          </Badge>
          <div className="text-xs text-gray-500">
            Confidence: {Math.round((suggestions.reduce((acc, s) => acc + s.confidence, 0) / suggestions.length) * 100)}%
          </div>
        </div>
      </div>

      {/* Categories */}
      <div className="flex-1 overflow-hidden">
        <Tabs value={activeCategory} onValueChange={setActiveCategory} className="h-full flex flex-col">
          <div className="border-b bg-gray-50">
            <TabsList className="grid w-full grid-cols-2 h-auto p-1">
              {SUGGESTION_CATEGORIES.slice(0, 4).map((category) => (
                <TabsTrigger 
                  key={category.id} 
                  value={category.id}
                  className="flex flex-col items-center gap-1 p-2 text-xs"
                >
                  <category.icon className="h-4 w-4" />
                  <span className="hidden sm:inline">{category.name}</span>
                </TabsTrigger>
              ))}
            </TabsList>
          </div>

          {SUGGESTION_CATEGORIES.map((category) => (
            <TabsContent 
              key={category.id} 
              value={category.id} 
              className="flex-1 overflow-y-auto p-4 space-y-4"
            >
              <div className="mb-4">
                <h3 className="font-medium text-gray-900 mb-1">{category.name}</h3>
                <p className="text-sm text-gray-600">{category.description}</p>
              </div>

              {filteredSuggestions.length === 0 ? (
                <div className="text-center py-8 text-gray-500">
                  <Lightbulb className="h-8 w-8 mx-auto mb-2 text-gray-400" />
                  <p className="text-sm">No suggestions for this category</p>
                </div>
              ) : (
                <div className="space-y-3">
                  {filteredSuggestions.map((suggestion) => (
                    <Card 
                      key={suggestion.id} 
                      className={`transition-all ${
                        suggestion.applied 
                          ? 'border-green-200 bg-green-50' 
                          : 'hover:border-gray-300'
                      }`}
                    >
                      <CardContent className="p-4">
                        <div className="flex items-start justify-between mb-2">
                          <div className="flex-1 min-w-0">
                            <h4 className="font-medium text-sm text-gray-900 mb-1">
                              {suggestion.title}
                            </h4>
                            <p className="text-xs text-gray-600 mb-2">
                              {suggestion.description}
                            </p>
                          </div>
                          
                          <div className="flex items-center gap-1 ml-2">
                            <Badge 
                              variant="outline" 
                              className={`text-xs ${getImpactColor(suggestion.impact)}`}
                            >
                              {suggestion.impact}
                            </Badge>
                          </div>
                        </div>

                        <div className="bg-white border border-gray-200 rounded p-3 mb-3">
                          <p className="text-sm text-gray-700">
                            {suggestion.content}
                          </p>
                        </div>

                        <div className="flex items-center justify-between">
                          <div className="flex items-center gap-2">
                            <span className={`text-xs font-medium ${getConfidenceColor(suggestion.confidence)}`}>
                              {Math.round(suggestion.confidence * 100)}% confidence
                            </span>
                          </div>

                          <div className="flex items-center gap-1">
                            {suggestion.applied ? (
                              <div className="flex items-center gap-1 text-green-600 text-xs">
                                <CheckCircle className="h-3 w-3" />
                                <span>Applied</span>
                              </div>
                            ) : (
                              <>
                                <Button
                                  onClick={() => handleApplySuggestion(suggestion)}
                                  size="sm"
                                  className="h-7 px-2 text-xs"
                                >
                                  <Plus className="h-3 w-3 mr-1" />
                                  Apply
                                </Button>
                                
                                <Button
                                  onClick={() => handleRejectSuggestion(suggestion.id)}
                                  variant="ghost"
                                  size="sm"
                                  className="h-7 px-2 text-xs text-gray-500 hover:text-red-600"
                                >
                                  <XCircle className="h-3 w-3" />
                                </Button>
                              </>
                            )}
                          </div>
                        </div>
                      </CardContent>
                    </Card>
                  ))}
                </div>
              )}
            </TabsContent>
          ))}
        </Tabs>
      </div>

      {/* Footer */}
      <div className="p-4 border-t bg-gray-50">
        <div className="text-center">
          <p className="text-xs text-gray-600 mb-2">
            Suggestions are based on Canadian job market analysis
          </p>
          <Button variant="outline" size="sm" className="w-full text-xs">
            <MessageSquare className="h-3 w-3 mr-1" />
            Request Custom Suggestions
          </Button>
        </div>
      </div>
    </div>
  );
}
```

## File: src/components/features/resume/index.ts
```typescript
export { default as ResumeAnalysisList } from './ResumeAnalysisList';
export { default as ResumeAnalysisDetail } from './ResumeAnalysisDetail';
export { default as ResumeUpload } from './ResumeUpload';
export { default as FeaturesPanel } from './FeaturesPanel';
```

## File: src/components/features/resume/ResumeAnalysisDetail.tsx
```typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Progress } from '@/components/ui/progress';
import { ArrowLeft, FileText, User, Mail, Phone, MapPin, Calendar, TrendingUp, Star, AlertCircle, CheckCircle, Briefcase, GraduationCap, Code, Languages, Target, ArrowRight, X, Loader2, Globe, Award, DollarSign, Search } from 'lucide-react';
import { auth } from '@/lib/auth';
import JobSearchModal from '@/components/features/career/JobSearchModal';

interface ResumeAnalysis {
  id: string;
  originalFileName: string;
  createdAt: string;
  personalInfo?: {
    name?: string;
    email?: string;
    phone?: string;
    location?: string;
    linkedin?: string;
    website?: string;
    confidence?: number;
  };
  skills?: {
    technical?: string[];
    soft?: string[];
    languages?: Array<{
      language: string;
      proficiency: string;
    }>;
    canadianWorkplaceRelevance?: string;
    confidence?: number;
  };
  workExperience?: Array<{
    title: string;
    company: string;
    startDate: string;
    endDate: string;
    location?: string;
    responsibilities?: string[];
    achievements?: string[];
    canadianRelevance?: string;
    confidence?: number;
  }>;
  education?: Array<{
    degree: string;
    institution: string;
    year: string;
    location?: string;
    gpa?: string;
    relevantCoursework?: string[];
    canadianEquivalency?: string;
    confidence?: number;
  }>;
  certifications?: Array<{
    name: string;
    issuer: string;
    year: string;
    expiryDate?: string;
    canadianRecognition?: string;
    confidence?: number;
  }>;
  projects?: Array<{
    name: string;
    description: string;
    technologies: string[];
    role: string;
    year: string;
    confidence?: number;
  }>;
  canadianMarketAnalysis?: {
    overallRelevance?: string;
    strengthsForCanadianMarket?: string[];
    potentialChallenges?: string[];
    recommendedImprovements?: string[];
    targetIndustries?: string[];
    salaryRangeEstimate?: string;
    confidence?: number;
  };
  positionRecommendations?: {
    position: string;
    successProbability: number;
    reasons: string[];
    skillMatch: number;
    salaryRange: string;
    marketDemand: string;
    immigrantFriendly: boolean;
    requiredSkills: string[];
    skillGaps: string[];
    confidence: number;
  }[];
  confidenceScores?: {
    overall?: number;
    dataExtraction?: number;
    marketAnalysis?: number;
  };
  metadata?: {
    processingMethod?: string;
    fileSize?: number;
    processedAt?: string;
    apiVersion?: string;
  };
}

interface PositionRecommendation {
  position: string;
  successProbability: number;
  reasons: string[];
  skillMatch: number;
  marketDemand: string;
  salaryRange: string;
  immigrantFriendly: boolean;
  requiredSkills: string[];
  recommendedActions: string[];
}

interface EnhancedProfile {
  optimized_profile?: {
    professional_title?: string;
    elevator_pitch?: string;
    value_proposition?: string;
    key_achievements?: string[];
  };
  skills_positioning?: {
    primary_skills?: Array<{
      skill: string;
      relevance_to_role: string;
      evidence: string;
      positioning_statement: string;
    }>;
    skill_development_plan?: Array<{
      skill: string;
      importance: string;
      learning_path: string;
      timeline: string;
      resources: string[];
    }>;
  };
  experience_repositioning?: {
    relevant_experience?: Array<{
      original_role: string;
      repositioned_as: string;
      key_transferable_elements: string[];
      success_metrics: string[];
      canadian_context: string;
    }>;
    project_highlights?: Array<{
      project: string;
      relevance: string;
      technologies_used: string[];
      impact: string;
      presentation_tip: string;
    }>;
  };
  application_strategy?: {
    resume_optimization?: {
      key_changes: string[];
      keywords_to_include: string[];
      sections_to_emphasize: string[];
      formatting_tips: string[];
    };
    cover_letter_strategy?: {
      opening_approach: string;
      key_points_to_address: string[];
      company_research_areas: string[];
      closing_strategy: string;
    };
    networking_approach?: {
      target_professionals: string[];
      conversation_starters: string[];
      value_you_bring: string[];
      follow_up_strategies: string[];
    };
  };
  interview_preparation?: {
    common_questions?: Array<{
      question: string;
      strategy: string;
      key_points: string[];
      example_answer_structure: string;
    }>;
    behavioral_examples?: Array<{
      situation: string;
      task: string;
      action: string;
      result: string;
      relevance: string;
    }>;
    technical_preparation?: {
      skills_to_demonstrate: string[];
      portfolio_items: string[];
      coding_challenges: string[];
      system_design_topics: string[];
    };
    cultural_fit_preparation?: {
      company_culture_research: string[];
      canadian_workplace_norms: string[];
      questions_to_ask: string[];
    };
  };
  "90_day_action_plan"?: {
    week_1_2?: string[];
    month_1?: string[];
    month_2?: string[];
    month_3?: string[];
    success_metrics?: string[];
  };
}

interface ResumeAnalysisDetailProps {
  analysis: ResumeAnalysis;
  onBack: () => void;
}

const ResumeAnalysisDetail: React.FC<ResumeAnalysisDetailProps> = ({ analysis, onBack }) => {
  // State for career profile generation
  const [showPositionModal, setShowPositionModal] = useState(false);
  const [positions, setPositions] = useState<PositionRecommendation[]>([]);
  const [loadingPositions, setLoadingPositions] = useState(false);
  const [selectedPosition, setSelectedPosition] = useState<PositionRecommendation | null>(null);
  const [enhancedProfile, setEnhancedProfile] = useState<EnhancedProfile | null>(null);
  const [loadingProfile, setLoadingProfile] = useState(false);
  
  // Job search modal state
  const [jobSearchModalOpen, setJobSearchModalOpen] = useState(false);
  const [jobSearchCareerPath, setJobSearchCareerPath] = useState<{ title: string; industry?: string } | null>(null);

  const formatDate = (dateString: string) => {
    return new Date(dateString).toLocaleDateString('en-US', {
      year: 'numeric',
      month: 'long',
      day: 'numeric',
      hour: '2-digit',
      minute: '2-digit'
    });
  };

  const formatFileSize = (bytes: number) => {
    return (bytes / (1024 * 1024)).toFixed(2) + ' MB';
  };

  // Convert decimal confidence scores to percentages
  const toPercentage = (decimal: number | undefined): number => {
    if (decimal === undefined || decimal === null) return 0;
    // If already a percentage (>1), return as is, otherwise multiply by 100
    return decimal > 1 ? Math.round(decimal) : Math.round(decimal * 100);
  };

  const getScoreColor = (score: number) => {
    if (score >= 80) return 'text-green-600 bg-green-50 border-green-200';
    if (score >= 60) return 'text-yellow-600 bg-yellow-50 border-yellow-200';
    return 'text-red-600 bg-red-50 border-red-200';
  };

  const getScoreIcon = (score: number) => {
    if (score >= 80) return <CheckCircle className="w-5 h-5 text-green-600" />;
    if (score >= 60) return <AlertCircle className="w-5 h-5 text-yellow-600" />;
    return <AlertCircle className="w-5 h-5 text-red-600" />;
  };

  const getRelevanceColor = (relevance: string) => {
    switch (relevance?.toLowerCase()) {
      case 'high': return 'bg-green-100 text-green-800 border-green-200';
      case 'medium': return 'bg-yellow-100 text-yellow-800 border-yellow-200';
      case 'low': return 'bg-red-100 text-red-800 border-red-200';
      default: return 'bg-gray-100 text-gray-800 border-gray-200';
    }
  };

  // Safe accessors with defaults
  const personalInfo = analysis.personalInfo || {};
  const canadianMarketAnalysis = analysis.canadianMarketAnalysis || {};
  const confidenceScores = analysis.confidenceScores || {};
  const metadata = analysis.metadata || {};
  const skills = analysis.skills || {};
  const workExperience = Array.isArray(analysis.workExperience) ? analysis.workExperience : [];
  const education = Array.isArray(analysis.education) ? analysis.education : [];
  const certifications = Array.isArray(analysis.certifications) ? analysis.certifications : [];
  const projects = Array.isArray(analysis.projects) ? analysis.projects : [];

  // Default values for nested properties
  const strengthsForCanadianMarket = Array.isArray(canadianMarketAnalysis.strengthsForCanadianMarket) ? canadianMarketAnalysis.strengthsForCanadianMarket : [];
  const potentialChallenges = Array.isArray(canadianMarketAnalysis.potentialChallenges) ? canadianMarketAnalysis.potentialChallenges : [];
  const recommendedImprovements = Array.isArray(canadianMarketAnalysis.recommendedImprovements) ? canadianMarketAnalysis.recommendedImprovements : [];
  const targetIndustries = Array.isArray(canadianMarketAnalysis.targetIndustries) ? canadianMarketAnalysis.targetIndustries : [];

  // Get overall market relevance score
  const getMarketRelevanceScore = () => {
    const relevance = canadianMarketAnalysis.overallRelevance?.toLowerCase();
    switch (relevance) {
      case 'high': return 85;
      case 'medium': return 65;
      case 'low': return 35;
      default: return 0;
    }
  };

  // Helper functions for career profile generation
  const getScoreColorClass = (score: number) => {
    if (score >= 80) return 'border-green-500 bg-green-50';
    if (score >= 60) return 'border-yellow-500 bg-yellow-50';
    return 'border-red-500 bg-red-50';
  };

  const getDemandColor = (demand: string) => {
    switch (demand?.toLowerCase()) {
      case 'high': return 'bg-green-100 text-green-800';
      case 'medium': return 'bg-yellow-100 text-yellow-800';
      case 'low': return 'bg-red-100 text-red-800';
      default: return 'bg-gray-100 text-gray-800';
    }
  };

  // Generate position recommendations
  const handleGenerateCareerProfile = async () => {
    // Use stored position recommendations if available
    if (analysis.positionRecommendations && analysis.positionRecommendations.length > 0) {
      const formattedPositions = analysis.positionRecommendations.map(pos => ({
        position: pos.position,
        successProbability: pos.successProbability,
        reasons: pos.reasons,
        skillMatch: pos.skillMatch,
        salaryRange: pos.salaryRange,
        marketDemand: pos.marketDemand,
        immigrantFriendly: pos.immigrantFriendly,
        requiredSkills: pos.requiredSkills,
        recommendedActions: pos.skillGaps?.map(gap => `Improve ${gap}`) || []
      }));
      setPositions(formattedPositions);
      setShowPositionModal(true);
      return;
    }

    // Use existing target industries from Canadian Market Analysis
    if (targetIndustries.length > 0) {
      const industryBasedPositions = targetIndustries.map((industry, index) => ({
        position: `${industry} Professional`,
        successProbability: 75 + (index * 5), // Slightly different scores for each
        reasons: [
          `Strong alignment with ${industry} sector`,
          'Canadian market demand for this industry',
          'Your skills match industry requirements'
        ],
        skillMatch: 80 - (index * 5), // Slightly decreasing skill match
        salaryRange: canadianMarketAnalysis.salaryRangeEstimate || '$60,000 - $85,000 CAD',
        marketDemand: index === 0 ? 'High' : index === 1 ? 'Medium-High' : 'Medium',
        immigrantFriendly: true,
        requiredSkills: skills.technical?.slice(0, 5) || ['Professional skills', 'Communication', 'Technical expertise'],
        recommendedActions: recommendedImprovements.slice(0, 3) || ['Gain Canadian work experience', 'Network within the industry', 'Obtain relevant certifications']
      }));
      
      setPositions(industryBasedPositions);
      setShowPositionModal(true);
      return;
    }

    // If no target industries or position recommendations available, show message
    alert('No career recommendations available. Please ensure your resume has been properly analyzed.');
  };

  // Generate enhanced profile for selected position
  const handleSelectPosition = async (position: PositionRecommendation) => {
    try {
      setSelectedPosition(position);
      setLoadingProfile(true);

      const token = auth.getAuthToken() || 'guest-token';
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/protected/ai-local/career-profile/enhanced-profile`, {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
          'Authorization': `Bearer ${token}`
        },
        body: JSON.stringify({
          targetPosition: position,
          resumeAnalysis: analysis
        })
      });

      if (response.ok) {
        const data = await response.json();
        console.log('Enhanced profile response:', data);
        // The backend returns enhancedProfile in data.data.enhancedProfile
        setEnhancedProfile(data.data?.enhancedProfile || data.enhancedProfile);
      } else {
        const errorText = await response.text();
        console.error('Failed to generate enhanced profile. Status:', response.status, 'Response:', errorText);
        alert('Failed to generate enhanced profile. Please try again.');
      }
    } catch (error) {
      console.error('Error generating enhanced profile:', error);
      alert('Error generating enhanced profile. Please try again.');
    } finally {
      setLoadingProfile(false);
    }
  };

  const closeModal = () => {
    setShowPositionModal(false);
    setPositions([]);
    setSelectedPosition(null);
    setEnhancedProfile(null);
    setLoadingPositions(false);
    setLoadingProfile(false);
  };

  // Job search handler
  const handleJobSearch = (position: PositionRecommendation) => {
    setJobSearchCareerPath({
      title: position.position,
      industry: undefined // You can extract industry from position if available
    });
    setJobSearchModalOpen(true);
  };

  return (
    <div className="space-y-6">
      {/* Header */}
      <div className="flex items-center justify-between">
        <div className="flex items-center space-x-4">
          <Button onClick={onBack} variant="outline" size="sm">
            <ArrowLeft className="w-4 h-4 mr-2" />
            Back to List
          </Button>
          <div>
            <h2 className="text-2xl font-bold text-gray-900 flex items-center space-x-2">
              <FileText className="w-6 h-6" />
              <span>{analysis.originalFileName}</span>
            </h2>
            <p className="text-gray-600">Analysis completed on {formatDate(analysis.createdAt)}</p>
          </div>
        </div>
        <div className="flex items-center space-x-2">
          <Badge variant="outline">
            {formatFileSize(metadata.fileSize || 0)}
          </Badge>
          <Badge variant="secondary">
            {metadata.processingMethod === 'direct_pdf' ? 'Direct PDF' : 'Text Extract'}
          </Badge>
        </div>
      </div>

      {/* Personal Information */}
      <Card>
        <CardHeader>
          <CardTitle className="flex items-center space-x-2">
            <User className="w-5 h-5" />
            <span>Personal Information</span>
            <Badge variant="outline" className={getScoreColor(toPercentage(personalInfo.confidence))}>
              {toPercentage(personalInfo.confidence)}% confidence
            </Badge>
          </CardTitle>
        </CardHeader>
        <CardContent>
          <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
            <div className="space-y-3">
              <div className="flex items-center space-x-2">
                <User className="w-4 h-4 text-gray-500" />
                <span className="font-medium">Name:</span>
                <span>{personalInfo.name || 'Not extracted'}</span>
              </div>
              <div className="flex items-center space-x-2">
                <Mail className="w-4 h-4 text-gray-500" />
                <span className="font-medium">Email:</span>
                <span>{personalInfo.email || 'Not found'}</span>
              </div>
              {personalInfo.linkedin && (
                <div className="flex items-center space-x-2">
                  <span className="font-medium">LinkedIn:</span>
                  <a href={personalInfo.linkedin} target="_blank" rel="noopener noreferrer" className="text-blue-600 hover:underline">
                    {personalInfo.linkedin}
                  </a>
                </div>
              )}
            </div>
            <div className="space-y-3">
              {personalInfo.phone && (
                <div className="flex items-center space-x-2">
                  <Phone className="w-4 h-4 text-gray-500" />
                  <span className="font-medium">Phone:</span>
                  <span>{personalInfo.phone}</span>
                </div>
              )}
              {personalInfo.location && (
                <div className="flex items-center space-x-2">
                  <MapPin className="w-4 h-4 text-gray-500" />
                  <span className="font-medium">Location:</span>
                  <span>{personalInfo.location}</span>
                </div>
              )}
              {personalInfo.website && (
                <div className="flex items-center space-x-2">
                  <span className="font-medium">Website:</span>
                  <a href={personalInfo.website} target="_blank" rel="noopener noreferrer" className="text-blue-600 hover:underline">
                    {personalInfo.website}
                  </a>
                </div>
              )}
            </div>
          </div>
        </CardContent>
      </Card>

      {/* Confidence Scores */}
      <Card>
        <CardHeader>
          <CardTitle className="flex items-center space-x-2">
            <TrendingUp className="w-5 h-5" />
            <span>Extraction Confidence Scores</span>
          </CardTitle>
          <CardDescription>
            How confident our AI is about the extracted information
          </CardDescription>
        </CardHeader>
        <CardContent>
          <div className="grid grid-cols-1 md:grid-cols-3 gap-4">
            <div className={`p-4 rounded-lg border ${getScoreColor(toPercentage(confidenceScores.overall))}`}>
              <div className="flex items-center justify-between mb-2">
                <span className="text-sm font-medium">Overall</span>
                {getScoreIcon(toPercentage(confidenceScores.overall))}
              </div>
              <div className="text-2xl font-bold">{toPercentage(confidenceScores.overall)}%</div>
            </div>
            <div className={`p-4 rounded-lg border ${getScoreColor(toPercentage(confidenceScores.dataExtraction))}`}>
              <div className="flex items-center justify-between mb-2">
                <span className="text-sm font-medium">Data Extraction</span>
                {getScoreIcon(toPercentage(confidenceScores.dataExtraction))}
              </div>
              <div className="text-2xl font-bold">{toPercentage(confidenceScores.dataExtraction)}%</div>
            </div>
            <div className={`p-4 rounded-lg border ${getScoreColor(toPercentage(confidenceScores.marketAnalysis))}`}>
              <div className="flex items-center justify-between mb-2">
                <span className="text-sm font-medium">Market Analysis</span>
                {getScoreIcon(toPercentage(confidenceScores.marketAnalysis))}
              </div>
              <div className="text-2xl font-bold">{toPercentage(confidenceScores.marketAnalysis)}%</div>
            </div>
          </div>
        </CardContent>
      </Card>

      {/* Canadian Market Analysis Card */}
      <Card className="bg-gradient-to-br from-green-50 to-blue-50 border-green-200">
        <CardHeader>
          <CardTitle className="flex items-center space-x-2 text-green-800">
            <Globe className="w-6 h-6" />
            <span>Canadian Market Analysis</span>
          </CardTitle>
          <CardDescription className="text-green-700">
            How well your resume aligns with the Canadian job market
          </CardDescription>
        </CardHeader>
        <CardContent>
          <div className="space-y-6">
            <div className={`p-6 rounded-lg border ${getScoreColor(getMarketRelevanceScore())}`}>
              <div className="flex items-center justify-between mb-4">
                <span className="text-lg font-semibold">Overall Market Relevance</span>
                <div className="flex items-center space-x-2">
                  <Badge className={getRelevanceColor(canadianMarketAnalysis.overallRelevance)}>
                    {canadianMarketAnalysis.overallRelevance || 'Not assessed'}
                  </Badge>
                  <div className="text-3xl font-bold">{getMarketRelevanceScore()}%</div>
                </div>
              </div>
              <div className="w-full bg-gray-200 rounded-full h-2">
                <div 
                  className="bg-current h-2 rounded-full" 
                  style={{ width: `${getMarketRelevanceScore()}%` }}
                ></div>
              </div>
            </div>

            {canadianMarketAnalysis.salaryRangeEstimate && (
              <div className="p-4 bg-blue-50 border border-blue-200 rounded-lg">
                <h4 className="font-semibold text-blue-800 mb-2">Estimated Salary Range</h4>
                <p className="text-blue-700">{canadianMarketAnalysis.salaryRangeEstimate}</p>
              </div>
            )}

            {targetIndustries.length > 0 && (
              <div>
                <h4 className="font-semibold text-gray-800 mb-3">Target Industries</h4>
                <div className="flex flex-wrap gap-2">
                  {targetIndustries.map((industry, index) => (
                    <Badge key={index} variant="outline" className="bg-purple-50 text-purple-700 border-purple-200">
                      {industry}
                    </Badge>
                  ))}
                </div>
              </div>
            )}

            <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
              <div>
                <h4 className="font-semibold text-green-700 mb-3 flex items-center space-x-2">
                  <CheckCircle className="w-4 h-4" />
                  <span>Strengths for Canadian Market</span>
                </h4>
                {strengthsForCanadianMarket.length > 0 ? (
                  <ul className="space-y-2">
                    {strengthsForCanadianMarket.map((strength, index) => (
                      <li key={index} className="flex items-start space-x-2">
                        <div className="w-2 h-2 bg-green-500 rounded-full mt-2 flex-shrink-0"></div>
                        <span className="text-sm text-gray-700">{strength}</span>
                      </li>
                    ))}
                  </ul>
                ) : (
                  <p className="text-sm text-gray-500 italic">No strengths identified yet. Try uploading a more detailed resume.</p>
                )}
              </div>

              <div>
                <h4 className="font-semibold text-orange-700 mb-3 flex items-center space-x-2">
                  <AlertCircle className="w-4 h-4" />
                  <span>Potential Challenges</span>
                </h4>
                {potentialChallenges.length > 0 ? (
                  <ul className="space-y-2">
                    {potentialChallenges.map((challenge, index) => (
                      <li key={index} className="flex items-start space-x-2">
                        <div className="w-2 h-2 bg-orange-500 rounded-full mt-2 flex-shrink-0"></div>
                        <span className="text-sm text-gray-700">{challenge}</span>
                      </li>
                    ))}
                  </ul>
                ) : (
                  <p className="text-sm text-gray-500 italic">No potential challenges identified.</p>
                )}
              </div>
            </div>

            {recommendedImprovements.length > 0 && (
              <div>
                <h4 className="font-semibold text-blue-700 mb-3 flex items-center space-x-2">
                  <TrendingUp className="w-4 h-4" />
                  <span>Recommended Improvements</span>
                </h4>
                <ul className="space-y-2">
                  {recommendedImprovements.map((improvement, index) => (
                    <li key={index} className="flex items-start space-x-2">
                      <div className="w-2 h-2 bg-blue-500 rounded-full mt-2 flex-shrink-0"></div>
                      <span className="text-sm text-gray-700">{improvement}</span>
                    </li>
                  ))}
                </ul>
              </div>
            )}
          </div>
        </CardContent>
      </Card>

      {/* Skills */}
      <Card>
        <CardHeader>
          <CardTitle className="flex items-center space-x-2">
            <Code className="w-5 h-5" />
            <span>Extracted Skills</span>
            <Badge variant="outline" className={getScoreColor(toPercentage(skills.confidence))}>
              {toPercentage(skills.confidence)}% confidence
            </Badge>
          </CardTitle>
          <CardDescription>Skills identified from your resume</CardDescription>
        </CardHeader>
        <CardContent>
          <div className="space-y-6">
            {skills.canadianWorkplaceRelevance && (
              <div className="p-3 rounded-lg border">
                <span className="text-sm font-medium">Canadian Workplace Relevance: </span>
                <Badge className={getRelevanceColor(skills.canadianWorkplaceRelevance)}>
                  {skills.canadianWorkplaceRelevance}
                </Badge>
              </div>
            )}
            
            {Array.isArray(skills.technical) && skills.technical.length > 0 && (
              <div>
                <h4 className="font-semibold text-gray-800 mb-3">Technical Skills</h4>
                <div className="flex flex-wrap gap-2">
                  {skills.technical.map((skill, index) => (
                    <Badge key={index} variant="secondary" className="bg-blue-50 text-blue-700 border-blue-200">
                      {skill}
                    </Badge>
                  ))}
                </div>
              </div>
            )}

            {Array.isArray(skills.soft) && skills.soft.length > 0 && (
              <div>
                <h4 className="font-semibold text-gray-800 mb-3">Soft Skills</h4>
                <div className="flex flex-wrap gap-2">
                  {skills.soft.map((skill, index) => (
                    <Badge key={index} variant="secondary" className="bg-green-50 text-green-700 border-green-200">
                      {skill}
                    </Badge>
                  ))}
                </div>
              </div>
            )}

            {Array.isArray(skills.languages) && skills.languages.length > 0 && (
              <div>
                <h4 className="font-semibold text-gray-800 mb-3 flex items-center space-x-2">
                  <Languages className="w-4 h-4" />
                  <span>Languages</span>
                </h4>
                <div className="grid grid-cols-1 md:grid-cols-2 gap-3">
                  {skills.languages.map((lang, index) => (
                    <div key={index} className="flex items-center justify-between p-3 bg-gray-50 rounded-lg">
                      <span className="font-medium">{lang.language}</span>
                      <Badge variant="outline">{lang.proficiency}</Badge>
                    </div>
                  ))}
                </div>
              </div>
            )}
          </div>
        </CardContent>
      </Card>

      {/* Work Experience */}
      {workExperience.length > 0 && (
        <Card>
          <CardHeader>
            <CardTitle className="flex items-center space-x-2">
              <Briefcase className="w-5 h-5" />
              <span>Work Experience</span>
            </CardTitle>
            <CardDescription>Professional experience extracted from your resume</CardDescription>
          </CardHeader>
          <CardContent>
            <div className="space-y-6">
              {workExperience.map((exp, index) => (
                <div key={index} className="border-l-4 border-blue-200 pl-4 py-3 bg-gray-50 rounded-r-lg">
                  <div className="flex items-start justify-between mb-2">
                    <div>
                      <h4 className="font-semibold text-gray-900">{exp.title}</h4>
                      <p className="text-sm text-gray-600 font-medium">{exp.company}</p>
                      {exp.location && (
                        <p className="text-sm text-gray-500">{exp.location}</p>
                      )}
                    </div>
                    <div className="text-right">
                      <Badge variant="outline">
                        {exp.startDate} - {exp.endDate || 'Present'}
                      </Badge>
                      {exp.canadianRelevance && (
                        <div className="mt-1">
                          <Badge className={getRelevanceColor(exp.canadianRelevance)}>
                            {exp.canadianRelevance} relevance
                          </Badge>
                        </div>
                      )}
                      <div className="mt-1">
                        <Badge variant="outline" className={getScoreColor(toPercentage(exp.confidence))}>
                          {toPercentage(exp.confidence)}% confidence
                        </Badge>
                      </div>
                    </div>
                  </div>
                  
                  {Array.isArray(exp.responsibilities) && exp.responsibilities.length > 0 && (
                    <div className="mt-3">
                      <h5 className="font-medium text-gray-800 mb-2">Key Responsibilities:</h5>
                      <ul className="space-y-1">
                        {exp.responsibilities.map((resp, respIndex) => (
                          <li key={respIndex} className="flex items-start space-x-2">
                            <div className="w-1.5 h-1.5 bg-blue-500 rounded-full mt-2 flex-shrink-0"></div>
                            <span className="text-sm text-gray-700">{resp}</span>
                          </li>
                        ))}
                      </ul>
                    </div>
                  )}

                  {Array.isArray(exp.achievements) && exp.achievements.length > 0 && (
                    <div className="mt-3">
                      <h5 className="font-medium text-gray-800 mb-2">Key Achievements:</h5>
                      <ul className="space-y-1">
                        {exp.achievements.map((achievement, achIndex) => (
                          <li key={achIndex} className="flex items-start space-x-2">
                            <div className="w-1.5 h-1.5 bg-green-500 rounded-full mt-2 flex-shrink-0"></div>
                            <span className="text-sm text-gray-700">{achievement}</span>
                          </li>
                        ))}
                      </ul>
                    </div>
                  )}
                </div>
              ))}
            </div>
          </CardContent>
        </Card>
      )}

      {/* Education */}
      {education.length > 0 && (
        <Card>
          <CardHeader>
            <CardTitle className="flex items-center space-x-2">
              <GraduationCap className="w-5 h-5" />
              <span>Education</span>
            </CardTitle>
            <CardDescription>Educational background extracted from your resume</CardDescription>
          </CardHeader>
          <CardContent>
            <div className="space-y-4">
              {education.map((edu, index) => (
                <div key={index} className="border-l-4 border-green-200 pl-4 py-3 bg-gray-50 rounded-r-lg">
                  <div className="flex items-start justify-between mb-2">
                    <div>
                      <h4 className="font-semibold text-gray-900">{edu.degree}</h4>
                      <p className="text-sm text-gray-600">{edu.institution}</p>
                      {edu.location && (
                        <p className="text-sm text-gray-500">{edu.location}</p>
                      )}
                    </div>
                    <div className="text-right">
                      <Badge variant="outline">{edu.year}</Badge>
                      {edu.gpa && (
                        <div className="mt-1">
                          <Badge variant="secondary">GPA: {edu.gpa}</Badge>
                        </div>
                      )}
                      {edu.canadianEquivalency && (
                        <div className="mt-1">
                          <Badge className="bg-blue-100 text-blue-800 border-blue-200">
                            {edu.canadianEquivalency}
                          </Badge>
                        </div>
                      )}
                      <div className="mt-1">
                        <Badge variant="outline" className={getScoreColor(toPercentage(edu.confidence))}>
                          {toPercentage(edu.confidence)}% confidence
                        </Badge>
                      </div>
                    </div>
                  </div>
                  
                  {Array.isArray(edu.relevantCoursework) && edu.relevantCoursework.length > 0 && (
                    <div className="mt-3">
                      <h5 className="font-medium text-gray-800 mb-2">Relevant Coursework:</h5>
                      <div className="flex flex-wrap gap-1">
                        {edu.relevantCoursework.map((course, courseIndex) => (
                          <Badge key={courseIndex} variant="outline" className="text-xs">
                            {course}
                          </Badge>
                        ))}
                      </div>
                    </div>
                  )}
                </div>
              ))}
            </div>
          </CardContent>
        </Card>
      )}

      {/* Certifications */}
      {certifications.length > 0 && (
        <Card>
          <CardHeader>
            <CardTitle>Certifications</CardTitle>
            <CardDescription>Professional certifications and their Canadian recognition</CardDescription>
          </CardHeader>
          <CardContent>
            <div className="space-y-3">
              {certifications.map((cert, index) => (
                <div key={index} className="border-l-4 border-purple-200 pl-4 py-2 bg-gray-50 rounded-r-lg">
                  <div className="flex items-center justify-between">
                    <div>
                      <h4 className="font-semibold text-gray-900">{cert.name}</h4>
                      <p className="text-sm text-gray-600">{cert.issuer}</p>
                    </div>
                    <div className="text-right">
                      <Badge variant="outline">{cert.year}</Badge>
                      {cert.expiryDate && (
                        <div className="mt-1">
                          <Badge variant="secondary">Expires: {cert.expiryDate}</Badge>
                        </div>
                      )}
                      {cert.canadianRecognition && (
                        <div className="mt-1">
                          <Badge className={
                            cert.canadianRecognition === 'Recognized' ? 'bg-green-100 text-green-800 border-green-200' :
                            cert.canadianRecognition === 'Partially' ? 'bg-yellow-100 text-yellow-800 border-yellow-200' :
                            'bg-red-100 text-red-800 border-red-200'
                          }>
                            {cert.canadianRecognition}
                          </Badge>
                        </div>
                      )}
                    </div>
                  </div>
                </div>
              ))}
            </div>
          </CardContent>
        </Card>
      )}

      {/* Projects */}
      {projects.length > 0 && (
        <Card>
          <CardHeader>
            <CardTitle>Projects</CardTitle>
            <CardDescription>Notable projects extracted from your resume</CardDescription>
          </CardHeader>
          <CardContent>
            <div className="space-y-4">
              {projects.map((project, index) => (
                <div key={index} className="border-l-4 border-indigo-200 pl-4 py-3 bg-gray-50 rounded-r-lg">
                  <div className="flex items-start justify-between mb-2">
                    <div>
                      <h4 className="font-semibold text-gray-900">{project.name}</h4>
                      <p className="text-sm text-gray-600">{project.role}</p>
                      <p className="text-sm text-gray-700 mt-1">{project.description}</p>
                    </div>
                    <div className="text-right">
                      <Badge variant="outline">{project.year}</Badge>
                      <div className="mt-1">
                        <Badge variant="outline" className={getScoreColor(toPercentage(project.confidence))}>
                          {toPercentage(project.confidence)}% confidence
                        </Badge>
                      </div>
                    </div>
                  </div>
                  
                  {Array.isArray(project.technologies) && project.technologies.length > 0 && (
                    <div className="mt-3">
                      <h5 className="font-medium text-gray-800 mb-2">Technologies Used:</h5>
                      <div className="flex flex-wrap gap-1">
                        {project.technologies.map((tech, techIndex) => (
                          <Badge key={techIndex} variant="secondary" className="text-xs bg-indigo-50 text-indigo-700 border-indigo-200">
                            {tech}
                          </Badge>
                        ))}
                      </div>
                    </div>
                  )}
                </div>
              ))}
            </div>
          </CardContent>
        </Card>
      )}

      {/* Actions */}
      <Card className="bg-blue-50 border-blue-200">
        <CardContent className="p-6">
          <h3 className="font-semibold text-blue-900 mb-4">Next Steps</h3>
          <div className="flex flex-wrap gap-3">
            <Button 
              onClick={handleGenerateCareerProfile}
              className="bg-blue-600 hover:bg-blue-700"
              disabled={loadingPositions || (targetIndustries.length === 0 && (!analysis.positionRecommendations || analysis.positionRecommendations.length === 0))}
            >
              {loadingPositions ? (
                <>
                  <Loader2 className="w-4 h-4 mr-2 animate-spin" />
                  Generating Recommendations...
                </>
              ) : (
                <>
                  <Target className="w-4 h-4 mr-2" />
                  View Career Profile
                </>
              )}
            </Button>
            <Button 
              variant="outline"
              onClick={() => window.location.href = '/dashboard/resume'}
              className="border-blue-600 text-blue-600 hover:bg-blue-50"
            >
              Upload New Resume
            </Button>
            <Button 
              variant="outline"
              onClick={onBack}
            >
              Back to Analyses
            </Button>
          </div>
        </CardContent>
      </Card>

      {/* Position Recommendations Modal */}
      {showPositionModal && (
        <div className="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50">
          <div className="bg-white rounded-lg max-w-6xl w-full max-h-[90vh] overflow-y-auto">
            <div className="sticky top-0 bg-white border-b px-6 py-4 flex items-center justify-between">
              <h2 className="text-2xl font-bold text-gray-900">Career Path Recommendations</h2>
              <Button onClick={closeModal} variant="ghost" size="sm">
                <X className="w-4 h-4" />
              </Button>
            </div>

            <div className="p-6">
              {!enhancedProfile ? (
                <>
                  <p className="text-gray-600 mb-6">
                    Based on your resume analysis, here are the most suitable career paths in Canada:
                  </p>

                  {loadingPositions ? (
                    <div className="text-center py-12">
                      <Loader2 className="w-8 h-8 animate-spin mx-auto mb-4" />
                      <p className="text-gray-600">Analyzing your profile and generating recommendations...</p>
                    </div>
                  ) : (
                    <div className="grid gap-4">
                      {positions.map((position, index) => (
                        <Card key={index} className="hover:shadow-lg transition-shadow">
                          <CardContent className="p-6">
                            <div className="flex items-start justify-between mb-4">
                              <div className="flex-1">
                                <h3 className="text-xl font-semibold text-gray-900 mb-2">{position.position}</h3>
                                <div className="flex flex-wrap gap-2 mb-3">
                                  {position.immigrantFriendly && (
                                    <Badge className="bg-green-100 text-green-800">
                                      <Globe className="w-3 h-3 mr-1" />
                                      Immigrant Friendly
                                    </Badge>
                                  )}
                                  <Badge className={getDemandColor(position.marketDemand)}>
                                    {position.marketDemand} Demand
                                  </Badge>
                                  <Badge variant="outline">
                                    <DollarSign className="w-3 h-3 mr-1" />
                                    {position.salaryRange}
                                  </Badge>
                                </div>
                              </div>
                              <div className="text-right ml-4">
                                <div className="text-3xl font-bold text-blue-600 mb-1">
                                  {position.successProbability}%
                                </div>
                                <p className="text-sm text-gray-500">Success Rate</p>
                              </div>
                            </div>

                            <div className="grid md:grid-cols-2 gap-4 mb-4">
                              <div>
                                <h4 className="font-medium text-gray-900 mb-2">Why This Matches:</h4>
                                <ul className="text-sm text-gray-600 space-y-1">
                                  {position.reasons.slice(0, 3).map((reason, idx) => (
                                    <li key={idx} className="flex items-start">
                                      <CheckCircle className="w-4 h-4 text-green-500 mr-2 mt-0.5 flex-shrink-0" />
                                      {reason}
                                    </li>
                                  ))}
                                </ul>
                              </div>
                              <div>
                                <h4 className="font-medium text-gray-900 mb-2">Key Skills Match:</h4>
                                <div className="flex items-center mb-2">
                                  <Progress value={position.skillMatch} className="flex-1 mr-3" />
                                  <span className="text-sm font-medium">{position.skillMatch}%</span>
                                </div>
                                <div className="flex flex-wrap gap-1">
                                  {position.requiredSkills.slice(0, 4).map((skill, idx) => (
                                    <Badge key={idx} variant="secondary" className="text-xs">
                                      {skill}
                                    </Badge>
                                  ))}
                                </div>
                              </div>
                            </div>

                            <div className="flex flex-col gap-2 pt-4 border-t">
                              <div className="flex gap-2">
                                <Button 
                                  onClick={() => handleSelectPosition(position)}
                                  variant="default"
                                  className="flex-1 bg-blue-600 hover:bg-blue-700 text-white"
                                >
                                  <Target className="w-4 h-4 mr-2" />
                                  Generate Career Profile
                                </Button>
                                <Button 
                                  onClick={(e) => {
                                    e.stopPropagation();
                                    handleJobSearch(position);
                                  }}
                                  variant="outline"
                                  className="flex-1 border-green-600 text-green-700 hover:bg-green-50"
                                >
                                  <Search className="w-4 h-4 mr-2" />
                                  Jobs Related to {position.position}
                                </Button>
                              </div>
                            </div>
                          </CardContent>
                        </Card>
                      ))}
                    </div>
                  )}
                </>
              ) : (
                <div className="space-y-6">
                  {loadingProfile ? (
                    <div className="text-center py-12">
                      <Loader2 className="w-8 h-8 animate-spin mx-auto mb-4" />
                      <p className="text-gray-600">Generating your personalized career profile...</p>
                    </div>
                  ) : (
                    <>
                      <div className="text-center mb-6">
                        <h3 className="text-2xl font-bold text-gray-900 mb-2">
                          Career Profile: {enhancedProfile.optimized_profile?.professional_title}
                        </h3>
                        <p className="text-gray-600">{enhancedProfile.optimized_profile?.elevator_pitch}</p>
                      </div>

                      <div className="grid md:grid-cols-2 gap-6">
                        <Card>
                          <CardHeader>
                            <CardTitle className="flex items-center space-x-2">
                              <CheckCircle className="w-5 h-5 text-green-600" />
                              <span>Your Current Strengths</span>
                            </CardTitle>
                          </CardHeader>
                          <CardContent>
                            <ul className="space-y-2">
                              {enhancedProfile.skills_positioning?.primary_skills?.map((skill, index) => (
                                <li key={index} className="flex items-start space-x-2">
                                  <div className="w-2 h-2 bg-green-500 rounded-full mt-2 flex-shrink-0"></div>
                                  <span className="text-sm">{skill.skill}</span>
                                </li>
                              ))}
                            </ul>
                          </CardContent>
                        </Card>

                        <Card>
                          <CardHeader>
                            <CardTitle className="flex items-center space-x-2">
                              <AlertCircle className="w-5 h-5 text-orange-600" />
                              <span>Skills to Develop</span>
                            </CardTitle>
                          </CardHeader>
                          <CardContent>
                            <ul className="space-y-2">
                              {enhancedProfile.skills_positioning?.skill_development_plan?.map((skill, index) => (
                                <li key={index} className="flex items-start space-x-2">
                                  <div className="w-2 h-2 bg-orange-500 rounded-full mt-2 flex-shrink-0"></div>
                                  <span className="text-sm">{skill.skill}</span>
                                </li>
                              ))}
                            </ul>
                          </CardContent>
                        </Card>

                        <Card>
                          <CardHeader>
                            <CardTitle className="flex items-center space-x-2">
                              <Target className="w-5 h-5 text-blue-600" />
                              <span>Action Plan</span>
                            </CardTitle>
                          </CardHeader>
                          <CardContent>
                            <ul className="space-y-2">
                              {enhancedProfile["90_day_action_plan"]?.week_1_2?.map((action, index) => (
                                <li key={index} className="flex items-start space-x-2">
                                  <div className="w-2 h-2 bg-blue-500 rounded-full mt-2 flex-shrink-0"></div>
                                  <span className="text-sm">{action}</span>
                                </li>
                              ))}
                            </ul>
                          </CardContent>
                        </Card>

                        <Card>
                          <CardHeader>
                            <CardTitle className="flex items-center space-x-2">
                              <Award className="w-5 h-5 text-purple-600" />
                              <span>Canadian Certifications</span>
                            </CardTitle>
                          </CardHeader>
                          <CardContent>
                            <ul className="space-y-2">
                              {enhancedProfile.skills_positioning?.primary_skills?.map((skill, index) => (
                                <li key={index} className="flex items-start space-x-2">
                                  <div className="w-2 h-2 bg-purple-500 rounded-full mt-2 flex-shrink-0"></div>
                                  <span className="text-sm">{skill.skill}</span>
                                </li>
                              ))}
                            </ul>
                          </CardContent>
                        </Card>
                      </div>

                      <div className="grid md:grid-cols-2 gap-6">
                        <Card>
                          <CardHeader>
                            <CardTitle>Timeline & Salary Progression</CardTitle>
                          </CardHeader>
                          <CardContent>
                            <div className="space-y-3">
                              <div>
                                <p className="text-sm font-medium text-gray-700">Expected Timeline:</p>
                                <p className="text-sm text-gray-600">{enhancedProfile["90_day_action_plan"]?.month_1}</p>
                              </div>
                              <div>
                                <p className="text-sm font-medium text-gray-700">Salary Progression:</p>
                                <p className="text-sm text-gray-600">{enhancedProfile.optimized_profile?.value_proposition}</p>
                              </div>
                            </div>
                          </CardContent>
                        </Card>

                        <Card>
                          <CardHeader>
                            <CardTitle>Market Outlook</CardTitle>
                          </CardHeader>
                          <CardContent>
                            <p className="text-sm text-gray-600">{enhancedProfile.optimized_profile?.value_proposition}</p>
                          </CardContent>
                        </Card>
                      </div>

                      <Card>
                        <CardHeader>
                          <CardTitle>Networking Strategy</CardTitle>
                        </CardHeader>
                        <CardContent>
                          <ul className="space-y-2">
                            {enhancedProfile.application_strategy?.networking_approach?.target_professionals?.map((strategy, index) => (
                              <li key={index} className="flex items-start space-x-2">
                                <div className="w-2 h-2 bg-indigo-500 rounded-full mt-2 flex-shrink-0"></div>
                                <span className="text-sm">{strategy}</span>
                              </li>
                            ))}
                          </ul>
                        </CardContent>
                      </Card>

                      <div className="flex justify-center">
                        <Button onClick={closeModal} className="bg-blue-600 hover:bg-blue-700">
                          Done
                        </Button>
                      </div>
                    </>
                  )}
                </div>
              )}
            </div>
          </div>
        </div>
      )}

      {/* Job Search Modal */}
      <JobSearchModal
        isOpen={jobSearchModalOpen}
        onClose={() => setJobSearchModalOpen(false)}
        careerPath={jobSearchCareerPath || { title: '' }}
      />
    </div>
  );
};

export default ResumeAnalysisDetail;
```

## File: src/components/features/resume/ResumeAnalysisList.tsx
```typescript
'use client';

import React, { useState, useEffect } from 'react';
import { Card, CardContent, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { FileText, Calendar, TrendingUp, Eye, Clock, AlertCircle } from 'lucide-react';
import { auth } from '@/lib/auth';

interface ResumeAnalysis {
  id: string;
  originalFileName: string;
  createdAt: string;
  personalInfo?: {
    name?: string;
    email?: string;
  };
  canadianMarketAnalysis?: {
    overallRelevance?: string;
    strengthsForCanadianMarket?: string[];
    potentialChallenges?: string[];
    recommendedImprovements?: string[];
    targetIndustries?: string[];
    confidence?: number;
  };
  confidenceScores?: {
    overall?: number;
  };
  metadata?: {
    processingMethod?: string;
    fileSize?: number;
  };
}

interface ResumeAnalysisListProps {
  onAnalysisSelect: (analysis: ResumeAnalysis) => void;
}

const ResumeAnalysisList: React.FC<ResumeAnalysisListProps> = ({ onAnalysisSelect }) => {
  const [analyses, setAnalyses] = useState<ResumeAnalysis[]>([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);

  useEffect(() => {
    fetchAnalyses();
  }, []);

  const fetchAnalyses = async () => {
    try {
      setLoading(true);
      
      // Use auth token or guest token for fetching analyses
      const token = auth.getAuthToken() || 'guest-token';
      const currentUser = auth.getCurrentUser();
      
      console.log('🔐 Frontend - Using token for history access:', token ? 'authenticated' : 'guest');
      console.log('👤 Frontend - Current user:', currentUser);
      console.log('🔐 Frontend - Token type:', typeof token);
      console.log('🔐 Frontend - Token length:', token ? token.length : 0);
      
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/protected/ai-local/resume/analyses`, {
        headers: {
          'Authorization': `Bearer ${token}`
        }
      });

      console.log('📥 Frontend - Response status:', response.status);
      console.log('📥 Frontend - Response headers:', Object.fromEntries(response.headers.entries()));

      const result = await response.json();
      console.log('📥 Frontend - Response data:', result);
      
      if (result.success && result.data) {
        console.log('📊 Frontend - Sample analysis structure:', result.data[0]);
        console.log('📊 Frontend - Canadian market analysis:', result.data[0]?.canadianMarketAnalysis);
        setAnalyses(result.data);
      } else {
        console.error('❌ Frontend - API Error:', result.message);
        setError(result.message || 'Failed to fetch analyses');
      }
    } catch (err: any) {
      console.error('❌ Frontend - Fetch Error:', err);
      setError(err.message || 'Failed to fetch analyses');
    } finally {
      setLoading(false);
    }
  };

  const formatDate = (dateString: string) => {
    return new Date(dateString).toLocaleDateString('en-CA', {
      year: 'numeric',
      month: 'short',
      day: 'numeric',
      hour: '2-digit',
      minute: '2-digit'
    });
  };

  const formatFileSize = (bytes: number) => {
    return (bytes / (1024 * 1024)).toFixed(2) + ' MB';
  };

  const toPercentage = (value: number) => {
    if (value <= 1) {
      return Math.round(value * 100);
    }
    return Math.round(value);
  };

  const getMarketRelevanceScore = (relevance?: string): number => {
    switch (relevance?.toLowerCase()) {
      case 'high': return 85;
      case 'medium': return 65;
      case 'low': return 35;
      default: return 0;
    }
  };

  const getScoreColor = (score: number) => {
    const percentage = toPercentage(score);
    if (percentage >= 80) return 'text-green-600 bg-green-50 border-green-200';
    if (percentage >= 60) return 'text-yellow-600 bg-yellow-50 border-yellow-200';
    return 'text-red-600 bg-red-50 border-red-200';
  };

  if (loading) {
    return (
      <div className="flex items-center justify-center py-12">
        <div className="text-center space-y-4">
          <Clock className="w-8 h-8 animate-spin mx-auto text-blue-500" />
          <p className="text-gray-600">Loading your resume analyses...</p>
        </div>
      </div>
    );
  }

  if (error) {
    return (
      <div className="flex flex-col items-center justify-center h-64 space-y-4">
        <AlertCircle className="h-12 w-12 text-red-500" />
        <div className="text-center">
          <h3 className="text-lg font-semibold text-gray-900">Unable to Load Resume Analyses</h3>
          <p className="text-gray-600 mt-2">{error}</p>
          {error.includes('log in') && (
            <Button 
              onClick={() => window.location.href = '/dashboard'}
              className="mt-4"
            >
              Back to Dashboard
            </Button>
          )}
          <Button 
            variant="outline"
            onClick={() => {
              setError(null);
              fetchAnalyses();
            }}
            className="mt-2 ml-2"
          >
            Retry
          </Button>
        </div>
      </div>
    );
  }

  if (analyses.length === 0) {
    return (
      <div className="text-center py-12">
        <div className="bg-gray-50 border border-gray-200 rounded-lg p-8 max-w-md mx-auto">
          <FileText className="w-12 h-12 mx-auto text-gray-400 mb-4" />
          <h3 className="text-lg font-semibold text-gray-900 mb-2">No Resume Analyses Yet</h3>
          <p className="text-gray-600 mb-6">
            Upload your first resume to get started with AI-powered analysis and insights.
          </p>
          <Button onClick={() => window.location.href = '/dashboard/resume'}>
            Upload Resume
          </Button>
        </div>
      </div>
    );
  }

  return (
    <div className="space-y-6">
      <div className="flex items-center justify-between">
        <div>
          <h2 className="text-2xl font-bold text-gray-900">Your Resume Analyses</h2>
          <p className="text-gray-600">Click on any analysis to view detailed insights</p>
        </div>
        <Badge variant="secondary" className="text-sm">
          {analyses.length} {analyses.length === 1 ? 'Analysis' : 'Analyses'}
        </Badge>
      </div>

      <div className="grid gap-4">
        {analyses.map((analysis) => (
          <Card 
            key={analysis.id}
            className="cursor-pointer hover:shadow-lg transition-all duration-200 hover:border-blue-300"
            onClick={() => onAnalysisSelect(analysis)}
          >
            <CardHeader className="pb-3">
              <div className="flex items-start justify-between">
                <div className="flex items-center space-x-3">
                  <div className="p-2 bg-blue-100 rounded-lg">
                    <FileText className="w-5 h-5 text-blue-600" />
                  </div>
                  <div>
                    <CardTitle className="text-lg text-gray-900">
                      {analysis.originalFileName}
                    </CardTitle>
                    <div className="flex items-center space-x-4 text-sm text-gray-500 mt-1">
                      <div className="flex items-center space-x-1">
                        <Calendar className="w-3 h-3" />
                        <span>{formatDate(analysis.createdAt)}</span>
                      </div>
                      <div className="flex items-center space-x-1">
                        <span>{formatFileSize(analysis.metadata?.fileSize || 0)}</span>
                      </div>
                      <div className="flex items-center space-x-1">
                        <Badge variant="outline" className="text-xs">
                          {analysis.metadata?.processingMethod === 'direct_pdf' ? 'Direct PDF' : 'Text Extract'}
                        </Badge>
                      </div>
                    </div>
                  </div>
                </div>
                <Button size="sm" variant="ghost" className="ml-2">
                  <Eye className="w-4 h-4" />
                </Button>
              </div>
            </CardHeader>

            <CardContent className="pt-0">
              <div className="space-y-3">
                <div className="flex items-center justify-between">
                  <div>
                    <p className="font-medium text-gray-900">
                      {analysis.personalInfo?.name || 'Name not extracted'}
                    </p>
                    <p className="text-sm text-gray-600">
                      {analysis.personalInfo?.email || 'Email not found'}
                    </p>
                  </div>
                </div>

                <div className="grid grid-cols-2 gap-4">
                  <div className={`p-3 rounded-lg border ${getScoreColor(analysis.confidenceScores?.overall || 0)}`}>
                    <div className="flex items-center justify-between">
                      <span className="text-sm font-medium">Extraction Quality</span>
                      <TrendingUp className="w-4 h-4" />
                    </div>
                    <div className="text-lg font-bold mt-1">
                      {toPercentage(analysis.confidenceScores?.overall || 0)}%
                    </div>
                  </div>

                  <div className={`p-3 rounded-lg border ${getScoreColor(getMarketRelevanceScore(analysis.canadianMarketAnalysis?.overallRelevance))}`}>
                    <div className="flex items-center justify-between">
                      <span className="text-sm font-medium">Market Alignment</span>
                      <TrendingUp className="w-4 h-4" />
                    </div>
                    <div className="text-lg font-bold mt-1">
                      {getMarketRelevanceScore(analysis.canadianMarketAnalysis?.overallRelevance)}%
                    </div>
                  </div>
                </div>

                <div className="grid grid-cols-2 gap-4 text-xs">
                  <div>
                    <span className="font-medium text-green-700">Strengths:</span>
                    <p className="text-gray-600 mt-1 line-clamp-2">
                      {analysis.canadianMarketAnalysis?.strengthsForCanadianMarket && Array.isArray(analysis.canadianMarketAnalysis.strengthsForCanadianMarket) 
                        ? analysis.canadianMarketAnalysis.strengthsForCanadianMarket.slice(0, 2).join(', ')
                        : 'No strengths available'}
                    </p>
                  </div>
                  <div>
                    <span className="font-medium text-orange-700">Improve:</span>
                    <p className="text-gray-600 mt-1 line-clamp-2">
                      {analysis.canadianMarketAnalysis?.recommendedImprovements && Array.isArray(analysis.canadianMarketAnalysis.recommendedImprovements)
                        ? analysis.canadianMarketAnalysis.recommendedImprovements.slice(0, 2).join(', ')
                        : 'No improvement areas available'}
                    </p>
                  </div>
                </div>

                <div className="pt-2 border-t border-gray-100">
                  <Button 
                    size="sm" 
                    className="w-full"
                    onClick={(e) => {
                      e.stopPropagation();
                      onAnalysisSelect(analysis);
                    }}
                  >
                    View Full Analysis
                  </Button>
                </div>
              </div>
            </CardContent>
          </Card>
        ))}
      </div>

      <Card className="bg-blue-50 border-blue-200">
        <CardContent className="p-6">
          <div className="flex items-center justify-between">
            <div>
              <h3 className="font-semibold text-blue-900 mb-1">Ready for more insights?</h3>
              <p className="text-sm text-blue-700">
                Upload a new resume or enhance your existing analysis with additional features.
              </p>
            </div>
            <div className="flex space-x-2">
              <Button 
                size="sm"
                onClick={() => window.location.href = '/dashboard/resume'}
                className="bg-blue-600 hover:bg-blue-700"
              >
                Upload New Resume
              </Button>
            </div>
          </div>
        </CardContent>
      </Card>
    </div>
  );
};

export default ResumeAnalysisList;
```

## File: src/components/features/resume/ResumeUpload.tsx
```typescript
import React, { useState, useCallback } from 'react';
import { useDropzone } from 'react-dropzone';
import { Upload, FileText, CheckCircle, AlertCircle, Clock, Zap, Globe, TrendingUp, Award, Briefcase } from 'lucide-react';

interface AnalysisResult {
  analysisId: string;
  analysis: {
    personalInfo: any;
    professionalSummary: string;
    skills: any[];
    workExperience: any[];
    education: any[];
    certifications: any[];
    projects: any[];
    canadianMarketAnalysis: any;
    confidenceScores: any;
    metadata: any;
  };
  rateLimitStatus: {
    minuteRemaining: number;
    dailyRemaining: number;
    nextResetTime: string;
  };
  processingMethod: 'direct_pdf' | 'text_extraction';
}

interface EnhancedResumeUploadProps {
  onAnalysisComplete?: (result: AnalysisResult) => void;
}

const EnhancedResumeUpload: React.FC<EnhancedResumeUploadProps> = ({ onAnalysisComplete }) => {
  const [uploading, setUploading] = useState(false);
  const [analysisResult, setAnalysisResult] = useState<AnalysisResult | null>(null);
  const [error, setError] = useState<string | null>(null);
  const [progress, setProgress] = useState(0);

  const onDrop = useCallback(async (acceptedFiles: File[]) => {
    const file = acceptedFiles[0];
    if (!file) return;

    setUploading(true);
    setError(null);
    setProgress(0);

    const formData = new FormData();
    formData.append('resume', file);

    try {
      // Simulate progress updates
      const progressInterval = setInterval(() => {
        setProgress(prev => {
          if (prev >= 90) {
            clearInterval(progressInterval);
            return 90;
          }
          return prev + 10;
        });
      }, 200);

      const response = await fetch('/api/resume/upload', {
        method: 'POST',
        body: formData,
        headers: {
          'Authorization': `Bearer ${localStorage.getItem('token')}`
        }
      });

      clearInterval(progressInterval);
      setProgress(100);

      const result = await response.json();

      if (result.success) {
        setAnalysisResult(result.data);
        onAnalysisComplete?.(result.data);
      } else {
        setError(result.message || 'Analysis failed');
      }
    } catch (err: any) {
      setError(err.message || 'Upload failed');
    } finally {
      setUploading(false);
    }
  }, [onAnalysisComplete]);

  const { getRootProps, getInputProps, isDragActive } = useDropzone({
    onDrop,
    accept: {
      'application/pdf': ['.pdf'],
      'application/vnd.openxmlformats-officedocument.wordprocessingml.document': ['.docx'],
      'image/jpeg': ['.jpg', '.jpeg'],
      'image/png': ['.png']
    },
    maxSize: 10 * 1024 * 1024, // 10MB
    disabled: uploading
  });

  const renderUploadArea = () => (
    <div
      {...getRootProps()}
      className={`
        border-2 border-dashed rounded-xl p-8 text-center cursor-pointer transition-all duration-300
        ${isDragActive 
          ? 'border-blue-500 bg-blue-50 scale-[1.02]' 
          : 'border-gray-300 hover:border-gray-400 hover:bg-gray-50'
        }
        ${uploading ? 'pointer-events-none opacity-50' : ''}
      `}
    >
      <input {...getInputProps()} />
      
      <div className="flex flex-col items-center space-y-4">
        <div className="relative">
          <Upload className="w-12 h-12 text-gray-400" />
          <Zap className="w-6 h-6 text-yellow-500 absolute -top-1 -right-1" />
        </div>
        
        <div>
          <h3 className="text-lg font-semibold text-gray-900 mb-2">
            Enhanced Resume Analysis with Gemini AI
          </h3>
          <p className="text-gray-600 mb-4">
            {isDragActive 
              ? 'Drop your resume here...' 
              : 'Drag & drop your resume or click to select'
            }
          </p>
          
          <div className="flex flex-wrap justify-center gap-2 text-sm text-gray-500">
            <span className="bg-green-100 text-green-700 px-2 py-1 rounded">PDF Direct Processing</span>
            <span className="bg-blue-100 text-blue-700 px-2 py-1 rounded">Up to 10MB</span>
            <span className="bg-purple-100 text-purple-700 px-2 py-1 rounded">Canadian Market Focus</span>
          </div>
        </div>

        <div className="grid grid-cols-2 gap-4 text-xs text-gray-600 max-w-md">
          <div className="flex items-center space-x-2">
            <Zap className="w-4 h-4 text-yellow-500" />
            <span>67x Faster Processing</span>
          </div>
          <div className="flex items-center space-x-2">
            <Globe className="w-4 h-4 text-blue-500" />
            <span>Canadian Job Market</span>
          </div>
          <div className="flex items-center space-x-2">
            <TrendingUp className="w-4 h-4 text-green-500" />
            <span>1000 req/min Limit</span>
          </div>
          <div className="flex items-center space-x-2">
            <FileText className="w-4 h-4 text-purple-500" />
            <span>Direct PDF Reading</span>
          </div>
        </div>
      </div>
    </div>
  );

  const renderProgress = () => (
    <div className="text-center space-y-4">
      <div className="flex items-center justify-center space-x-2">
        <Clock className="w-5 h-5 text-blue-500 animate-spin" />
        <span className="text-lg font-medium">Analyzing with Gemini AI...</span>
      </div>
      
      <div className="w-full bg-gray-200 rounded-full h-3">
        <div 
          className="bg-gradient-to-r from-blue-500 to-purple-600 h-3 rounded-full transition-all duration-300"
          style={{ width: `${progress}%` }}
        />
      </div>
      
      <p className="text-sm text-gray-600">
        Using {progress < 50 ? 'direct PDF processing' : 'Canadian market analysis'}...
      </p>
    </div>
  );

  const renderResults = () => {
    if (!analysisResult) return null;

    const { analysis, processingMethod, rateLimitStatus } = analysisResult;

    return (
      <div className="space-y-6">
        {/* Success Header */}
        <div className="flex items-center space-x-3 p-4 bg-green-50 rounded-lg border border-green-200">
          <CheckCircle className="w-6 h-6 text-green-600" />
          <div>
            <h3 className="font-semibold text-green-900">Analysis Complete!</h3>
            <p className="text-sm text-green-700">
              Processed using {processingMethod === 'direct_pdf' ? 'Direct PDF Reading' : 'Text Extraction'}
            </p>
          </div>
        </div>

        {/* Rate Limit Status */}
        <div className="grid grid-cols-3 gap-4 p-4 bg-blue-50 rounded-lg border border-blue-200">
          <div className="text-center">
            <div className="text-2xl font-bold text-blue-600">{rateLimitStatus.minuteRemaining}</div>
            <div className="text-sm text-blue-800">Requests Left/Min</div>
          </div>
          <div className="text-center">
            <div className="text-2xl font-bold text-purple-600">{rateLimitStatus.dailyRemaining}</div>
            <div className="text-sm text-purple-800">Requests Left/Day</div>
          </div>
          <div className="text-center">
            <div className="text-lg font-bold text-green-600">✓</div>
            <div className="text-sm text-green-800">Processing Method</div>
          </div>
        </div>

        {/* Analysis Summary */}
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {/* Professional Summary */}
          {analysis.professionalSummary && (
            <div className="p-4 border rounded-lg">
              <div className="flex items-center space-x-2 mb-3">
                <Briefcase className="w-5 h-5 text-blue-500" />
                <h4 className="font-semibold">Professional Summary</h4>
              </div>
              <p className="text-sm text-gray-700 leading-relaxed">
                {analysis.professionalSummary}
              </p>
            </div>
          )}

          {/* Skills Overview */}
          <div className="p-4 border rounded-lg">
            <div className="flex items-center space-x-2 mb-3">
              <Award className="w-5 h-5 text-purple-500" />
              <h4 className="font-semibold">Skills Identified</h4>
            </div>
            <div className="flex flex-wrap gap-2">
              {analysis.skills.slice(0, 8).map((skill: any, index: number) => (
                <span 
                  key={index}
                  className="px-2 py-1 bg-purple-100 text-purple-700 text-xs rounded"
                >
                  {typeof skill === 'string' ? skill : skill.name}
                </span>
              ))}
              {analysis.skills.length > 8 && (
                <span className="px-2 py-1 bg-gray-100 text-gray-600 text-xs rounded">
                  +{analysis.skills.length - 8} more
                </span>
              )}
            </div>
          </div>

          {/* Canadian Market Analysis */}
          {analysis.canadianMarketAnalysis && (
            <div className="p-4 border rounded-lg md:col-span-2">
              <div className="flex items-center space-x-2 mb-3">
                <Globe className="w-5 h-5 text-green-500" />
                <h4 className="font-semibold">Canadian Market Insights</h4>
              </div>
              <div className="grid grid-cols-1 md:grid-cols-3 gap-4 text-sm">
                <div>
                  <span className="font-medium text-gray-700">Market Fit:</span>
                  <div className="text-green-600 font-semibold">
                    {analysis.canadianMarketAnalysis.marketFitScore || 'Analyzing...'}
                  </div>
                </div>
                <div>
                  <span className="font-medium text-gray-700">In-Demand Skills:</span>
                  <div className="text-blue-600 font-semibold">
                    {analysis.canadianMarketAnalysis.inDemandSkills?.length || 0} identified
                  </div>
                </div>
                <div>
                  <span className="font-medium text-gray-700">Improvement Areas:</span>
                  <div className="text-orange-600 font-semibold">
                    {analysis.canadianMarketAnalysis.improvementAreas?.length || 0} suggestions
                  </div>
                </div>
              </div>
            </div>
          )}
        </div>

        {/* Confidence Scores */}
        <div className="p-4 bg-gray-50 rounded-lg">
          <h4 className="font-semibold mb-3">Analysis Confidence</h4>
          <div className="grid grid-cols-2 md:grid-cols-4 gap-4 text-sm">
            {Object.entries(analysis.confidenceScores || {}).map(([key, value]: [string, any]) => (
              <div key={key} className="text-center">
                <div className="text-lg font-bold text-indigo-600">{Math.round(value * 100)}%</div>
                <div className="text-gray-600 capitalize">{key.replace(/([A-Z])/g, ' $1').trim()}</div>
              </div>
            ))}
          </div>
        </div>
      </div>
    );
  };

  const renderError = () => (
    <div className="flex items-center space-x-3 p-4 bg-red-50 rounded-lg border border-red-200">
      <AlertCircle className="w-6 h-6 text-red-600" />
      <div>
        <h3 className="font-semibold text-red-900">Analysis Failed</h3>
        <p className="text-sm text-red-700">{error}</p>
      </div>
    </div>
  );

  return (
    <div className="max-w-4xl mx-auto p-6">
      <div className="mb-6">
        <h2 className="text-2xl font-bold text-gray-900 mb-2">
          Enhanced Resume Analysis
        </h2>
        <p className="text-gray-600">
          Powered by Gemini Developer API with 67x faster processing and Canadian market focus
        </p>
      </div>

      {error && renderError()}
      
      {!analysisResult && !uploading && !error && renderUploadArea()}
      
      {uploading && renderProgress()}
      
      {analysisResult && renderResults()}
    </div>
  );
};

export default EnhancedResumeUpload;
```

## File: src/components/features/resume/templates/CanadianPDFTemplate.tsx
```typescript
"use client";

import React from 'react';
import { Badge } from '@/components/ui/badge';
import { 
  Mail, 
  Phone, 
  MapPin, 
  Globe, 
  Linkedin,
  Calendar,
  Star,
  Award,
  GraduationCap,
  Briefcase,
  User,
  Target,
  CheckCircle
} from 'lucide-react';

export interface TemplateProps {
  resume: any;
  template: 'professional' | 'modern' | 'classic' | 'minimal';
  className?: string;
}

export interface TemplateStyle {
  name: string;
  description: string;
  className: string;
  headerStyle: string;
  sectionStyle: string;
  accentColor: string;
}

export const TEMPLATE_STYLES: Record<string, TemplateStyle> = {
  professional: {
    name: 'Professional',
    description: 'Clean and traditional Canadian format',
    className: 'template-professional',
    headerStyle: 'bg-blue-50 border-b-4 border-blue-600',
    sectionStyle: 'border-l-4 border-blue-500',
    accentColor: '#2563eb'
  },
  modern: {
    name: 'Modern',
    description: 'Contemporary design with visual elements',
    className: 'template-modern',
    headerStyle: 'bg-gradient-to-r from-purple-600 to-blue-600 text-white',
    sectionStyle: 'border-l-4 border-purple-500',
    accentColor: '#7c3aed'
  },
  classic: {
    name: 'Classic',
    description: 'Timeless and elegant format',
    className: 'template-classic',
    headerStyle: 'bg-gray-50 border-b-2 border-gray-800',
    sectionStyle: 'border-l-3 border-gray-800',
    accentColor: '#1f2937'
  },
  minimal: {
    name: 'Minimal',
    description: 'Simple and clean design',
    className: 'template-minimal',
    headerStyle: 'border-b-2 border-gray-300',
    sectionStyle: 'border-l-2 border-gray-400',
    accentColor: '#6b7280'
  }
};

export default function CanadianPDFTemplate({ 
  resume, 
  template = 'professional',
  className = '' 
}: TemplateProps) {
  const resumeData = resume?.resumeData || {};
  const personalInfo = resumeData.personalInfo || {};
  const professionalSummary = resumeData.professionalSummary || {};
  const workExperience = resumeData.workExperience || [];
  const education = resumeData.education || [];
  const skills = resumeData.skills || [];
  const certifications = resumeData.certifications || [];
  const languages = resumeData.languages || [];

  const templateStyle = TEMPLATE_STYLES[template];

  const formatDate = (date: string) => {
    if (!date) return '';
    return new Date(date).toLocaleDateString('en-CA', {
      year: 'numeric',
      month: 'short'
    });
  };

  const getSkillLevel = (level: string) => {
    switch (level) {
      case 'expert': return 'Expert';
      case 'advanced': return 'Advanced';
      case 'intermediate': return 'Intermediate';
      case 'beginner': return 'Beginner';
      default: return level;
    }
  };

  const getSkillLevelColor = (level: string) => {
    switch (level) {
      case 'expert': return 'bg-green-100 text-green-800';
      case 'advanced': return 'bg-blue-100 text-blue-800';
      case 'intermediate': return 'bg-yellow-100 text-yellow-800';
      case 'beginner': return 'bg-gray-100 text-gray-800';
      default: return 'bg-gray-100 text-gray-800';
    }
  };

  const renderHeader = () => {
    switch (template) {
      case 'modern':
        return (
          <div className={`${templateStyle.headerStyle} p-6 rounded-lg mb-6`}>
            <h1 className="text-3xl font-bold mb-2">
              {personalInfo.name || 'Your Name'}
            </h1>
            <div className="flex items-center justify-center gap-4 text-sm opacity-90">
              {personalInfo.email && (
                <div className="flex items-center gap-1">
                  <Mail className="h-4 w-4" />
                  <span>{personalInfo.email}</span>
                </div>
              )}
              {personalInfo.phone && (
                <div className="flex items-center gap-1">
                  <Phone className="h-4 w-4" />
                  <span>{personalInfo.phone}</span>
                </div>
              )}
              {personalInfo.location && (
                <div className="flex items-center gap-1">
                  <MapPin className="h-4 w-4" />
                  <span>{personalInfo.location}</span>
                </div>
              )}
            </div>
            <div className="flex items-center justify-center gap-4 text-sm opacity-90 mt-2">
              {personalInfo.linkedin && (
                <div className="flex items-center gap-1">
                  <Linkedin className="h-4 w-4" />
                  <span>{personalInfo.linkedin}</span>
                </div>
              )}
              {personalInfo.website && (
                <div className="flex items-center gap-1">
                  <Globe className="h-4 w-4" />
                  <span>{personalInfo.website}</span>
                </div>
              )}
            </div>
          </div>
        );

      default:
        return (
          <div className={`${templateStyle.headerStyle} p-6 mb-6`}>
            <h1 className="text-3xl font-bold text-gray-900 mb-2">
              {personalInfo.name || 'Your Name'}
            </h1>
            <div className="flex items-center justify-center gap-4 text-sm text-gray-600 mb-2">
              {personalInfo.email && (
                <div className="flex items-center gap-1">
                  <Mail className="h-4 w-4" />
                  <span>{personalInfo.email}</span>
                </div>
              )}
              {personalInfo.phone && (
                <div className="flex items-center gap-1">
                  <Phone className="h-4 w-4" />
                  <span>{personalInfo.phone}</span>
                </div>
              )}
              {personalInfo.location && (
                <div className="flex items-center gap-1">
                  <MapPin className="h-4 w-4" />
                  <span>{personalInfo.location}</span>
                </div>
              )}
            </div>
            <div className="flex items-center justify-center gap-4 text-sm text-gray-600">
              {personalInfo.linkedin && (
                <div className="flex items-center gap-1">
                  <Linkedin className="h-4 w-4" />
                  <span>{personalInfo.linkedin}</span>
                </div>
              )}
              {personalInfo.website && (
                <div className="flex items-center gap-1">
                  <Globe className="h-4 w-4" />
                  <span>{personalInfo.website}</span>
                </div>
              )}
            </div>
          </div>
        );
    }
  };

  const renderSectionTitle = (title: string, icon: React.ReactNode) => {
    switch (template) {
      case 'modern':
        return (
          <h2 className="text-xl font-bold text-gray-900 mb-4 flex items-center gap-2">
            <div className="p-2 bg-purple-100 rounded-lg">
              {icon}
            </div>
            {title}
          </h2>
        );

      case 'classic':
        return (
          <h2 className="text-xl font-bold text-gray-900 mb-4 flex items-center gap-2 border-b-2 border-gray-800 pb-2">
            {icon}
            {title}
          </h2>
        );

      default:
        return (
          <h2 className="text-xl font-bold text-gray-900 mb-4 flex items-center gap-2">
            {icon}
            {title}
          </h2>
        );
    }
  };

  return (
    <div className={`bg-white shadow-lg ${templateStyle.className} ${className}`} style={{ 
      width: '210mm', 
      minHeight: '297mm',
      padding: '20mm',
      boxSizing: 'border-box'
    }}>
      {/* Header */}
      {renderHeader()}

      {/* Professional Summary */}
      {professionalSummary.summary && (
        <div className="mb-6">
          {renderSectionTitle('Professional Summary', <User className="h-5 w-5" />)}
          <p className="text-gray-700 leading-relaxed">
            {professionalSummary.summary}
          </p>
        </div>
      )}

      {/* Work Experience */}
      {workExperience.length > 0 && (
        <div className="mb-6">
          {renderSectionTitle('Professional Experience', <Briefcase className="h-5 w-5" />)}
          <div className="space-y-4">
            {workExperience.map((job: any, index: number) => (
              <div key={index} className={`${templateStyle.sectionStyle} pl-4`}>
                <div className="flex justify-between items-start mb-1">
                  <h3 className="font-semibold text-gray-900">
                    {job.title}
                  </h3>
                  <span className="text-sm text-gray-600">
                    {formatDate(job.startDate)} - {job.current ? 'Present' : formatDate(job.endDate)}
                  </span>
                </div>
                <div className="text-gray-700 mb-2">
                  <span className="font-medium">{job.company}</span>
                  {job.location && (
                    <span className="text-gray-600"> • {job.location}</span>
                  )}
                </div>
                {job.description && (
                  <p className="text-gray-700 text-sm mb-2">
                    {job.description}
                  </p>
                )}
                {job.achievements && job.achievements.length > 0 && (
                  <ul className="list-disc list-inside text-sm text-gray-700 space-y-1">
                    {job.achievements.map((achievement: string, idx: number) => (
                      <li key={idx}>{achievement}</li>
                    ))}
                  </ul>
                )}
              </div>
            ))}
          </div>
        </div>
      )}

      {/* Skills */}
      {skills.length > 0 && (
        <div className="mb-6">
          {renderSectionTitle('Skills & Competencies', <Target className="h-5 w-5" />)}
          <div className="grid grid-cols-2 gap-4">
            {skills.map((skill: any, index: number) => (
              <div key={index} className="flex justify-between items-center">
                <span className="font-medium text-gray-900">
                  {skill.name}
                  {skill.canadianEquivalent && (
                    <span className="text-xs text-gray-500 ml-1">
                      ({skill.canadianEquivalent})
                    </span>
                  )}
                </span>
                <Badge 
                  variant="outline" 
                  className={`text-xs ${getSkillLevelColor(skill.level)}`}
                >
                  {getSkillLevel(skill.level)}
                </Badge>
              </div>
            ))}
          </div>
        </div>
      )}

      {/* Education */}
      {education.length > 0 && (
        <div className="mb-6">
          {renderSectionTitle('Education', <GraduationCap className="h-5 w-5" />)}
          <div className="space-y-3">
            {education.map((edu: any, index: number) => (
              <div key={index} className={`${templateStyle.sectionStyle} pl-4`}>
                <div className="flex justify-between items-start mb-1">
                  <h3 className="font-semibold text-gray-900">
                    {edu.degree}
                  </h3>
                  <span className="text-sm text-gray-600">
                    {formatDate(edu.startDate)} - {edu.current ? 'Present' : formatDate(edu.endDate)}
                  </span>
                </div>
                <div className="text-gray-700 mb-1">
                  <span className="font-medium">{edu.institution}</span>
                  {edu.location && (
                    <span className="text-gray-600"> • {edu.location}</span>
                  )}
                </div>
                {edu.gpa && (
                  <div className="text-sm text-gray-600">
                    GPA: {edu.gpa}
                  </div>
                )}
                {edu.relevantCourses && edu.relevantCourses.length > 0 && (
                  <div className="text-sm text-gray-700 mt-1">
                    <span className="font-medium">Relevant Courses:</span> {edu.relevantCourses.join(', ')}
                  </div>
                )}
              </div>
            ))}
          </div>
        </div>
      )}

      {/* Certifications */}
      {certifications.length > 0 && (
        <div className="mb-6">
          {renderSectionTitle('Certifications', <Award className="h-5 w-5" />)}
          <div className="space-y-2">
            {certifications.map((cert: any, index: number) => (
              <div key={index} className="flex justify-between items-center">
                <div>
                  <span className="font-medium text-gray-900">{cert.name}</span>
                  {cert.issuer && (
                    <span className="text-gray-600 text-sm ml-2">• {cert.issuer}</span>
                  )}
                </div>
                <span className="text-sm text-gray-600">
                  {formatDate(cert.date)}
                </span>
              </div>
            ))}
          </div>
        </div>
      )}

      {/* Languages */}
      {languages.length > 0 && (
        <div className="mb-6">
          {renderSectionTitle('Languages', <Globe className="h-5 w-5" />)}
          <div className="grid grid-cols-2 gap-4">
            {languages.map((lang: any, index: number) => (
              <div key={index} className="flex justify-between items-center">
                <span className="font-medium text-gray-900">{lang.language}</span>
                <Badge variant="outline" className="text-xs">
                  {lang.proficiency}
                </Badge>
              </div>
            ))}
          </div>
        </div>
      )}

      {/* Additional Information */}
      {resumeData.additionalInfo && (
        <div className="mb-6">
          {renderSectionTitle('Additional Information', <Star className="h-5 w-5" />)}
          <p className="text-gray-700 leading-relaxed">
            {resumeData.additionalInfo}
          </p>
        </div>
      )}

      {/* Footer */}
      <div className="mt-8 pt-4 border-t border-gray-200 text-center text-xs text-gray-500">
        <div className="flex items-center justify-center gap-2 mb-1">
          <CheckCircle className="h-3 w-3 text-green-600" />
          <span>Generated by ImmiGrowAI - Optimized for Canadian Job Market</span>
        </div>
        {resume.atsScore && (
          <div className="flex items-center justify-center gap-2">
            <span>ATS Score:</span>
            <Badge className="bg-green-600 text-white text-xs">
              {resume.atsScore}/100
            </Badge>
          </div>
        )}
      </div>
    </div>
  );
}

// Export template selector component
export function TemplateSelector({ 
  selectedTemplate, 
  onTemplateChange 
}: { 
  selectedTemplate: string; 
  onTemplateChange: (template: string) => void;
}) {
  return (
    <div className="space-y-4">
      <h3 className="text-lg font-semibold">Choose Template</h3>
      <div className="grid grid-cols-2 gap-4">
        {Object.entries(TEMPLATE_STYLES).map(([key, style]) => (
          <div
            key={key}
            onClick={() => onTemplateChange(key)}
            className={`
              p-4 border-2 rounded-lg cursor-pointer transition-all
              ${selectedTemplate === key 
                ? 'border-blue-500 bg-blue-50' 
                : 'border-gray-200 hover:border-gray-300'
              }
            `}
          >
            <div className="font-medium text-gray-900">{style.name}</div>
            <div className="text-sm text-gray-600">{style.description}</div>
            <div 
              className="w-4 h-4 rounded mt-2" 
              style={{ backgroundColor: style.accentColor }}
            />
          </div>
        ))}
      </div>
    </div>
  );
}
```

## File: src/components/forms/BaseForm.tsx
```typescript
import React from 'react';
import { cn } from '@/lib/utils';
import { FormError } from './FormError';
import { FormSubmitButton } from './FormSubmitButton';

export interface BaseFormProps {
  children: React.ReactNode;
  onSubmit: (e: React.FormEvent<HTMLFormElement>) => void | Promise<void>;
  loading?: boolean;
  error?: string | null;
  className?: string;
  submitText?: string;
  disabled?: boolean;
  showSubmitButton?: boolean;
}

export const BaseForm: React.FC<BaseFormProps> = ({
  children,
  onSubmit,
  loading = false,
  error = null,
  className,
  submitText = 'Submit',
  disabled = false,
  showSubmitButton = true,
}) => {
  const handleSubmit = async (e: React.FormEvent<HTMLFormElement>) => {
    e.preventDefault();
    if (loading || disabled) return;
    
    try {
      await onSubmit(e);
    } catch (err) {
      console.error('Form submission error:', err);
    }
  };

  return (
    <form
      onSubmit={handleSubmit}
      className={cn('space-y-6', className)}
      noValidate
    >
      {error && <FormError error={error} />}
      
      <div className="space-y-4">
        {children}
      </div>

      {showSubmitButton && (
        <FormSubmitButton
          loading={loading}
          disabled={disabled}
          text={submitText}
        />
      )}
    </form>
  );
};
```

## File: src/components/forms/FormError.tsx
```typescript
import React from 'react';
import { Alert, AlertDescription } from '@/components/ui/alert';
import { AlertCircle } from 'lucide-react';
import { cn } from '@/lib/utils';

export interface FormErrorProps {
  error: string;
  className?: string;
  variant?: 'default' | 'destructive' | 'warning';
}

export const FormError: React.FC<FormErrorProps> = ({
  error,
  className,
  variant = 'destructive',
}) => {
  if (!error) return null;

  return (
    <Alert variant={variant} className={cn('mb-4', className)}>
      <AlertCircle className="h-4 w-4" />
      <AlertDescription>{error}</AlertDescription>
    </Alert>
  );
};
```

## File: src/components/forms/FormField.tsx
```typescript
import React from 'react';
import { cn } from '@/lib/utils';
import { Label } from '@/components/ui/label';
import { Input } from '@/components/ui/input';
import { Textarea } from '@/components/ui/textarea';
import { Select, SelectContent, SelectItem, SelectTrigger, SelectValue } from '@/components/ui/select';
import { Checkbox } from '@/components/ui/checkbox';
import { RadioGroup, RadioGroupItem } from '@/components/ui/radio-group';

export type FieldType = 'text' | 'email' | 'password' | 'number' | 'tel' | 'url' | 'textarea' | 'select' | 'checkbox' | 'radio';

export interface SelectOption {
  value: string;
  label: string;
  disabled?: boolean;
}

export interface FormFieldProps {
  name: string;
  label?: string;
  type?: FieldType;
  placeholder?: string;
  value?: string | number | boolean;
  onChange?: (value: any) => void;
  onBlur?: () => void;
  error?: string;
  required?: boolean;
  disabled?: boolean;
  className?: string;
  options?: SelectOption[];
  rows?: number;
  min?: number;
  max?: number;
  step?: number;
  autoComplete?: string;
  autoFocus?: boolean;
  readOnly?: boolean;
  helpText?: string;
}

export const FormField: React.FC<FormFieldProps> = ({
  name,
  label,
  type = 'text',
  placeholder,
  value,
  onChange,
  onBlur,
  error,
  required = false,
  disabled = false,
  className,
  options = [],
  rows = 3,
  min,
  max,
  step,
  autoComplete,
  autoFocus = false,
  readOnly = false,
  helpText,
}) => {
  const fieldId = `field-${name}`;
  const errorId = `error-${name}`;
  const helpId = `help-${name}`;

  const renderField = () => {
    const commonProps = {
      id: fieldId,
      name,
      value: value as string,
      onChange: (e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => {
        onChange?.(e.target.value);
      },
      onBlur,
      placeholder,
      disabled,
      readOnly,
      autoComplete,
      autoFocus,
      'aria-describedby': cn(
        error && errorId,
        helpText && helpId
      ),
      'aria-invalid': !!error,
    };

    switch (type) {
      case 'textarea':
        return (
          <Textarea
            {...commonProps}
            rows={rows}
            value={value as string}
            onChange={(e) => onChange?.(e.target.value)}
          />
        );

      case 'select':
        return (
          <Select
            value={value as string}
            onValueChange={onChange}
            disabled={disabled}
          >
            <SelectTrigger className={cn(error && 'border-destructive')}>
              <SelectValue placeholder={placeholder} />
            </SelectTrigger>
            <SelectContent>
              {options.map((option) => (
                <SelectItem
                  key={option.value}
                  value={option.value}
                  disabled={option.disabled}
                >
                  {option.label}
                </SelectItem>
              ))}
            </SelectContent>
          </Select>
        );

      case 'checkbox':
        return (
          <Checkbox
            id={fieldId}
            checked={value as boolean}
            onCheckedChange={onChange}
            disabled={disabled}
            aria-describedby={cn(
              error && errorId,
              helpText && helpId
            )}
          />
        );

      case 'radio':
        return (
          <RadioGroup
            value={value as string}
            onValueChange={onChange}
            disabled={disabled}
            aria-describedby={cn(
              error && errorId,
              helpText && helpId
            )}
          >
            {options.map((option) => (
              <div key={option.value} className="flex items-center space-x-2">
                <RadioGroupItem
                  value={option.value}
                  id={`${fieldId}-${option.value}`}
                  disabled={option.disabled}
                />
                <Label htmlFor={`${fieldId}-${option.value}`}>
                  {option.label}
                </Label>
              </div>
            ))}
          </RadioGroup>
        );

      default:
        return (
          <Input
            {...commonProps}
            type={type}
            min={min}
            max={max}
            step={step}
          />
        );
    }
  };

  return (
    <div className={cn('space-y-2', className)}>
      {label && (
        <Label htmlFor={fieldId} className={cn(required && 'after:content-["*"] after:ml-0.5 after:text-destructive')}>
          {label}
        </Label>
      )}
      
      {renderField()}
      
      {helpText && (
        <p id={helpId} className="text-sm text-muted-foreground">
          {helpText}
        </p>
      )}
      
      {error && (
        <p id={errorId} className="text-sm text-destructive">
          {error}
        </p>
      )}
    </div>
  );
};
```

## File: src/components/forms/FormSubmitButton.tsx
```typescript
import React from 'react';
import { Button } from '@/components/ui/button';
import { Loader2 } from 'lucide-react';
import { cn } from '@/lib/utils';

export interface FormSubmitButtonProps {
  loading?: boolean;
  disabled?: boolean;
  text?: string;
  className?: string;
  variant?: 'default' | 'destructive' | 'outline' | 'secondary' | 'ghost' | 'link';
  size?: 'default' | 'sm' | 'lg' | 'icon';
  type?: 'submit' | 'button' | 'reset';
}

export const FormSubmitButton: React.FC<FormSubmitButtonProps> = ({
  loading = false,
  disabled = false,
  text = 'Submit',
  className,
  variant = 'default',
  size = 'default',
  type = 'submit',
}) => {
  return (
    <Button
      type={type}
      disabled={disabled || loading}
      className={cn('w-full', className)}
      variant={variant}
      size={size}
    >
      {loading && <Loader2 className="mr-2 h-4 w-4 animate-spin" />}
      {text}
    </Button>
  );
};
```

## File: src/components/forms/index.ts
```typescript
// Form components exports
export * from './validation';
```

## File: src/components/forms/validation/auth.ts
```typescript
import { z } from 'zod';

export const loginSchema = z.object({
  email: z
    .string()
    .min(1, 'Email is required')
    .email('Please enter a valid email address'),
  password: z
    .string()
    .min(1, 'Password is required')
    .min(6, 'Password must be at least 6 characters'),
  rememberMe: z.boolean().optional(),
});

export const registerSchema = z.object({
  firstName: z
    .string()
    .min(1, 'First name is required')
    .min(2, 'First name must be at least 2 characters')
    .max(50, 'First name must be less than 50 characters'),
  lastName: z
    .string()
    .min(1, 'Last name is required')
    .min(2, 'Last name must be at least 2 characters')
    .max(50, 'Last name must be less than 50 characters'),
  email: z
    .string()
    .min(1, 'Email is required')
    .email('Please enter a valid email address'),
  password: z
    .string()
    .min(1, 'Password is required')
    .min(8, 'Password must be at least 8 characters')
    .regex(
      /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)/,
      'Password must contain at least one uppercase letter, one lowercase letter, and one number'
    ),
  confirmPassword: z
    .string()
    .min(1, 'Please confirm your password'),
  acceptTerms: z
    .boolean()
    .refine((val) => val === true, 'You must accept the terms and conditions'),
}).refine((data) => data.password === data.confirmPassword, {
  message: "Passwords don't match",
  path: ["confirmPassword"],
});

export const forgotPasswordSchema = z.object({
  email: z
    .string()
    .min(1, 'Email is required')
    .email('Please enter a valid email address'),
});

export const resetPasswordSchema = z.object({
  password: z
    .string()
    .min(1, 'Password is required')
    .min(8, 'Password must be at least 8 characters')
    .regex(
      /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)/,
      'Password must contain at least one uppercase letter, one lowercase letter, and one number'
    ),
  confirmPassword: z
    .string()
    .min(1, 'Please confirm your password'),
}).refine((data) => data.password === data.confirmPassword, {
  message: "Passwords don't match",
  path: ["confirmPassword"],
});

export const changePasswordSchema = z.object({
  currentPassword: z
    .string()
    .min(1, 'Current password is required'),
  newPassword: z
    .string()
    .min(1, 'New password is required')
    .min(8, 'New password must be at least 8 characters')
    .regex(
      /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)/,
      'New password must contain at least one uppercase letter, one lowercase letter, and one number'
    ),
  confirmNewPassword: z
    .string()
    .min(1, 'Please confirm your new password'),
}).refine((data) => data.newPassword === data.confirmNewPassword, {
  message: "New passwords don't match",
  path: ["confirmNewPassword"],
});

export type LoginFormData = z.infer<typeof loginSchema>;
export type RegisterFormData = z.infer<typeof registerSchema>;
export type ForgotPasswordFormData = z.infer<typeof forgotPasswordSchema>;
export type ResetPasswordFormData = z.infer<typeof resetPasswordSchema>;
export type ChangePasswordFormData = z.infer<typeof changePasswordSchema>;
```

## File: src/components/forms/validation/career.ts
```typescript
import { z } from 'zod';

export const careerProfileSchema = z.object({
  title: z
    .string()
    .min(1, 'Job title is required')
    .max(100, 'Title must be less than 100 characters'),
  industry: z
    .string()
    .min(1, 'Industry is required')
    .max(100, 'Industry must be less than 100 characters'),
  experienceLevel: z.enum(['entry', 'mid', 'senior', 'executive']),
  skills: z
    .array(z.string())
    .min(1, 'At least one skill is required')
    .max(20, 'Maximum 20 skills allowed'),
  preferredLocation: z
    .string()
    .max(100, 'Location must be less than 100 characters')
    .optional(),
  salaryRange: z.object({
    min: z.number().min(0, 'Minimum salary must be positive'),
    max: z.number().min(0, 'Maximum salary must be positive'),
  }).refine((data) => data.max >= data.min, {
    message: 'Maximum salary must be greater than or equal to minimum salary',
    path: ['max'],
  }).optional(),
  remotePreference: z.enum(['on-site', 'hybrid', 'remote']).optional(),
  workAuthorization: z
    .array(z.string())
    .min(1, 'At least one work authorization is required')
    .optional(),
  languages: z
    .array(z.object({
      language: z.string().min(1, 'Language is required'),
      proficiency: z.enum(['basic', 'conversational', 'fluent', 'native']),
    }))
    .optional(),
  education: z
    .array(z.object({
      degree: z.string().min(1, 'Degree is required'),
      institution: z.string().min(1, 'Institution is required'),
      year: z.number().min(1900).max(new Date().getFullYear()),
      field: z.string().min(1, 'Field of study is required'),
    }))
    .optional(),
  certifications: z
    .array(z.object({
      name: z.string().min(1, 'Certification name is required'),
      issuer: z.string().min(1, 'Issuer is required'),
      year: z.number().min(1900).max(new Date().getFullYear()),
      expiryDate: z.date().optional(),
    }))
    .optional(),
});

export const jobSearchSchema = z.object({
  keywords: z
    .string()
    .min(1, 'Search keywords are required')
    .max(200, 'Keywords must be less than 200 characters'),
  location: z
    .string()
    .max(100, 'Location must be less than 100 characters')
    .optional(),
  radius: z
    .number()
    .min(1, 'Radius must be at least 1 mile')
    .max(100, 'Radius must be less than 100 miles')
    .optional(),
  jobType: z
    .array(z.enum(['full-time', 'part-time', 'contract', 'internship', 'temporary']))
    .optional(),
  experienceLevel: z
    .array(z.enum(['entry', 'mid', 'senior', 'executive']))
    .optional(),
  remote: z.boolean().optional(),
  salaryMin: z
    .number()
    .min(0, 'Minimum salary must be positive')
    .optional(),
  salaryMax: z
    .number()
    .min(0, 'Maximum salary must be positive')
    .optional(),
  datePosted: z.enum(['1', '3', '7', '14', '30']).optional(),
  sortBy: z.enum(['relevance', 'date', 'salary']).optional(),
});

export const jobApplicationSchema = z.object({
  jobId: z
    .string()
    .min(1, 'Job ID is required'),
  resumeId: z
    .string()
    .min(1, 'Resume is required'),
  coverLetter: z
    .string()
    .max(2000, 'Cover letter must be less than 2000 characters')
    .optional(),
  expectedSalary: z
    .number()
    .min(0, 'Expected salary must be positive')
    .optional(),
  availability: z
    .string()
    .max(200, 'Availability must be less than 200 characters')
    .optional(),
  additionalQuestions: z
    .array(z.object({
      question: z.string().min(1, 'Question is required'),
      answer: z.string().min(1, 'Answer is required'),
    }))
    .optional(),
});

export const careerGoalSchema = z.object({
  shortTermGoal: z
    .string()
    .min(1, 'Short-term goal is required')
    .max(500, 'Short-term goal must be less than 500 characters'),
  longTermGoal: z
    .string()
    .min(1, 'Long-term goal is required')
    .max(500, 'Long-term goal must be less than 500 characters'),
  targetPosition: z
    .string()
    .min(1, 'Target position is required')
    .max(100, 'Target position must be less than 100 characters'),
  targetCompany: z
    .string()
    .max(100, 'Target company must be less than 100 characters')
    .optional(),
  timeline: z.enum(['6-months', '1-year', '2-years', '3-years', '5-years']),
  prioritySkills: z
    .array(z.string())
    .min(1, 'At least one priority skill is required')
    .max(10, 'Maximum 10 priority skills allowed'),
});

export type CareerProfileFormData = z.infer<typeof careerProfileSchema>;
export type JobSearchFormData = z.infer<typeof jobSearchSchema>;
export type JobApplicationFormData = z.infer<typeof jobApplicationSchema>;
export type CareerGoalFormData = z.infer<typeof careerGoalSchema>;
```

## File: src/components/forms/validation/resume.ts
```typescript
import { z } from 'zod';

export const resumeUploadSchema = z.object({
  file: z
    .instanceof(File)
    .refine((file) => file.size > 0, 'File is required')
    .refine(
      (file) => file.size <= 5 * 1024 * 1024, // 5MB
      'File size must be less than 5MB'
    )
    .refine(
      (file) => {
        const allowedTypes = [
          'application/pdf',
          'application/msword',
          'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
          'text/plain'
        ];
        return allowedTypes.includes(file.type);
      },
      'File must be a PDF, DOC, DOCX, or TXT file'
    ),
  title: z
    .string()
    .min(1, 'Resume title is required')
    .max(100, 'Title must be less than 100 characters'),
  description: z
    .string()
    .max(500, 'Description must be less than 500 characters')
    .optional(),
  isPublic: z.boolean().optional(),
});

export const resumeAnalysisSchema = z.object({
  resumeId: z
    .string()
    .min(1, 'Resume ID is required'),
  analysisType: z.enum(['general', 'job-specific', 'skills', 'improvements']),
  jobDescription: z
    .string()
    .max(2000, 'Job description must be less than 2000 characters')
    .optional(),
  focusAreas: z
    .array(z.string())
    .min(1, 'At least one focus area is required')
    .max(5, 'Maximum 5 focus areas allowed')
    .optional(),
});

export const resumeUpdateSchema = z.object({
  title: z
    .string()
    .min(1, 'Resume title is required')
    .max(100, 'Title must be less than 100 characters'),
  description: z
    .string()
    .max(500, 'Description must be less than 500 characters')
    .optional(),
  isPublic: z.boolean().optional(),
  tags: z
    .array(z.string())
    .max(10, 'Maximum 10 tags allowed')
    .optional(),
});

export const resumeFeedbackSchema = z.object({
  resumeId: z
    .string()
    .min(1, 'Resume ID is required'),
  feedback: z
    .string()
    .min(1, 'Feedback is required')
    .max(1000, 'Feedback must be less than 1000 characters'),
  rating: z
    .number()
    .min(1, 'Rating is required')
    .max(5, 'Rating must be between 1 and 5'),
  category: z.enum(['content', 'format', 'skills', 'overall']),
});

export type ResumeUploadFormData = z.infer<typeof resumeUploadSchema>;
export type ResumeAnalysisFormData = z.infer<typeof resumeAnalysisSchema>;
export type ResumeUpdateFormData = z.infer<typeof resumeUpdateSchema>;
export type ResumeFeedbackFormData = z.infer<typeof resumeFeedbackSchema>;
```

## File: src/components/forms/validation/user.ts
```typescript
import { z } from 'zod';

export const userProfileSchema = z.object({
  firstName: z
    .string()
    .min(1, 'First name is required')
    .min(2, 'First name must be at least 2 characters')
    .max(50, 'First name must be less than 50 characters'),
  lastName: z
    .string()
    .min(1, 'Last name is required')
    .min(2, 'Last name must be at least 2 characters')
    .max(50, 'Last name must be less than 50 characters'),
  email: z
    .string()
    .min(1, 'Email is required')
    .email('Please enter a valid email address'),
  phone: z
    .string()
    .regex(/^\+?[\d\s\-\(\)]+$/, 'Please enter a valid phone number')
    .optional(),
  dateOfBirth: z
    .date()
    .max(new Date(), 'Date of birth cannot be in the future')
    .optional(),
  location: z.object({
    city: z.string().max(100, 'City must be less than 100 characters').optional(),
    state: z.string().max(100, 'State must be less than 100 characters').optional(),
    country: z.string().max(100, 'Country must be less than 100 characters').optional(),
    zipCode: z.string().max(20, 'Zip code must be less than 20 characters').optional(),
  }).optional(),
  bio: z
    .string()
    .max(500, 'Bio must be less than 500 characters')
    .optional(),
  website: z
    .string()
    .url('Please enter a valid URL')
    .optional()
    .or(z.literal('')),
  socialLinks: z.object({
    linkedin: z.string().url('Please enter a valid LinkedIn URL').optional().or(z.literal('')),
    github: z.string().url('Please enter a valid GitHub URL').optional().or(z.literal('')),
    twitter: z.string().url('Please enter a valid Twitter URL').optional().or(z.literal('')),
    portfolio: z.string().url('Please enter a valid portfolio URL').optional().or(z.literal('')),
  }).optional(),
  preferences: z.object({
    emailNotifications: z.boolean().optional(),
    pushNotifications: z.boolean().optional(),
    marketingEmails: z.boolean().optional(),
    jobAlerts: z.boolean().optional(),
    newsletter: z.boolean().optional(),
  }).optional(),
});

export const userSettingsSchema = z.object({
  theme: z.enum(['light', 'dark', 'system']).optional(),
  language: z.enum(['en', 'es', 'fr', 'de', 'zh', 'ja']).optional(),
  timezone: z.string().optional(),
  dateFormat: z.enum(['MM/DD/YYYY', 'DD/MM/YYYY', 'YYYY-MM-DD']).optional(),
  timeFormat: z.enum(['12h', '24h']).optional(),
  currency: z.enum(['USD', 'EUR', 'GBP', 'CAD', 'AUD']).optional(),
  privacy: z.object({
    profileVisibility: z.enum(['public', 'private', 'connections']).optional(),
    resumeVisibility: z.enum(['public', 'private', 'connections']).optional(),
    showEmail: z.boolean().optional(),
    showPhone: z.boolean().optional(),
    showLocation: z.boolean().optional(),
  }).optional(),
  security: z.object({
    twoFactorEnabled: z.boolean().optional(),
    sessionTimeout: z.number().min(5).max(1440).optional(), // minutes
    loginNotifications: z.boolean().optional(),
  }).optional(),
});

export const userPreferencesSchema = z.object({
  jobPreferences: z.object({
    preferredJobTypes: z
      .array(z.enum(['full-time', 'part-time', 'contract', 'internship', 'temporary']))
      .optional(),
    preferredIndustries: z
      .array(z.string())
      .max(10, 'Maximum 10 preferred industries')
      .optional(),
    preferredLocations: z
      .array(z.string())
      .max(10, 'Maximum 10 preferred locations')
      .optional(),
    salaryExpectations: z.object({
      min: z.number().min(0).optional(),
      max: z.number().min(0).optional(),
      currency: z.enum(['USD', 'EUR', 'GBP', 'CAD', 'AUD']).optional(),
    }).optional(),
    remotePreference: z.enum(['on-site', 'hybrid', 'remote']).optional(),
    workAuthorization: z
      .array(z.string())
      .optional(),
  }).optional(),
  communicationPreferences: z.object({
    preferredContactMethod: z.enum(['email', 'phone', 'linkedin']).optional(),
    contactTime: z.enum(['morning', 'afternoon', 'evening', 'anytime']).optional(),
    timezone: z.string().optional(),
  }).optional(),
  notificationPreferences: z.object({
    jobAlerts: z.boolean().optional(),
    applicationUpdates: z.boolean().optional(),
    profileViews: z.boolean().optional(),
    connectionRequests: z.boolean().optional(),
    marketingEmails: z.boolean().optional(),
    newsletter: z.boolean().optional(),
    systemUpdates: z.boolean().optional(),
  }).optional(),
});

export const userAccountSchema = z.object({
  currentPassword: z
    .string()
    .min(1, 'Current password is required'),
  newEmail: z
    .string()
    .min(1, 'New email is required')
    .email('Please enter a valid email address'),
  confirmPassword: z
    .string()
    .min(1, 'Please confirm your password'),
}).refine((data) => data.currentPassword !== data.confirmPassword, {
  message: 'New email confirmation password must match current password',
  path: ['confirmPassword'],
});

export type UserProfileFormData = z.infer<typeof userProfileSchema>;
export type UserSettingsFormData = z.infer<typeof userSettingsSchema>;
export type UserPreferencesFormData = z.infer<typeof userPreferencesSchema>;
export type UserAccountFormData = z.infer<typeof userAccountSchema>;
```

## File: src/components/index.ts
```typescript
// Component barrel exports
export * from './common';
export * from './features/resume';
export * from './features/career';
export * from './features/auth';
export * from './forms';
export * from './providers';
export * from './ui';
```

## File: src/components/providers/api-provider.tsx
```typescript
"use client";

import React, { createContext, useContext, useState, useCallback } from 'react';

export interface ApiConfig {
  baseUrl: string;
  timeout: number;
  retries: number;
  headers: Record<string, string>;
}

export interface ApiState {
  loading: boolean;
  error: string | null;
  lastRequest: string | null;
  requestCount: number;
}

export interface ApiContextType {
  config: ApiConfig;
  state: ApiState;
  updateConfig: (config: Partial<ApiConfig>) => void;
  setLoading: (loading: boolean) => void;
  setError: (error: string | null) => void;
  clearError: () => void;
  incrementRequestCount: () => void;
  resetState: () => void;
}

const ApiContext = createContext<ApiContextType | undefined>(undefined);

const defaultConfig: ApiConfig = {
  baseUrl: process.env.NEXT_PUBLIC_API_URL || 'http://localhost:3001',
  timeout: 10000,
  retries: 3,
  headers: {
    'Content-Type': 'application/json',
  },
};

const defaultState: ApiState = {
  loading: false,
  error: null,
  lastRequest: null,
  requestCount: 0,
};

export interface ApiProviderProps {
  children: React.ReactNode;
  config?: Partial<ApiConfig>;
}

export const ApiProvider: React.FC<ApiProviderProps> = ({
  children,
  config: initialConfig = {},
}) => {
  const [config, setConfig] = useState<ApiConfig>({
    ...defaultConfig,
    ...initialConfig,
  });
  
  const [state, setState] = useState<ApiState>(defaultState);

  const updateConfig = useCallback((newConfig: Partial<ApiConfig>) => {
    setConfig(prev => ({
      ...prev,
      ...newConfig,
    }));
  }, []);

  const setLoading = useCallback((loading: boolean) => {
    setState(prev => ({
      ...prev,
      loading,
    }));
  }, []);

  const setError = useCallback((error: string | null) => {
    setState(prev => ({
      ...prev,
      error,
    }));
  }, []);

  const clearError = useCallback(() => {
    setState(prev => ({
      ...prev,
      error: null,
    }));
  }, []);

  const incrementRequestCount = useCallback(() => {
    setState(prev => ({
      ...prev,
      requestCount: prev.requestCount + 1,
    }));
  }, []);

  const resetState = useCallback(() => {
    setState(defaultState);
  }, []);

  const value: ApiContextType = {
    config,
    state,
    updateConfig,
    setLoading,
    setError,
    clearError,
    incrementRequestCount,
    resetState,
  };

  return (
    <ApiContext.Provider value={value}>
      {children}
    </ApiContext.Provider>
  );
};

export const useApi = (): ApiContextType => {
  const context = useContext(ApiContext);
  if (context === undefined) {
    throw new Error('useApi must be used within an ApiProvider');
  }
  return context;
};
```

## File: src/components/providers/auth-provider.tsx
```typescript
"use client";

import React, { createContext, useContext, useEffect, useState } from 'react';
import { useRouter } from 'next/navigation';
import { User } from '@/types/auth';

export interface AuthContextType {
  user: User | null;
  loading: boolean;
  error: string | null;
  login: (email: string, password: string) => Promise<void>;
  register: (userData: any) => Promise<void>;
  logout: () => Promise<void>;
  updateUser: (userData: Partial<User>) => Promise<void>;
  clearError: () => void;
}

const AuthContext = createContext<AuthContextType | undefined>(undefined);

export interface AuthProviderProps {
  children: React.ReactNode;
  initialUser?: User | null;
}

export const AuthProvider: React.FC<AuthProviderProps> = ({
  children,
  initialUser = null,
}) => {
  const [user, setUser] = useState<User | null>(initialUser);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);
  const router = useRouter();

  useEffect(() => {
    // Check for existing session/token
    const checkAuth = async () => {
      try {
        const token = localStorage.getItem('auth_token');
        if (token) {
          // Validate token with backend
          const response = await fetch('/api/auth/me', {
            headers: {
              'Authorization': `Bearer ${token}`,
            },
          });
          
          if (response.ok) {
            const userData = await response.json();
            setUser(userData);
          } else {
            localStorage.removeItem('auth_token');
          }
        }
      } catch (err) {
        console.error('Auth check failed:', err);
      } finally {
        setLoading(false);
      }
    };

    checkAuth();
  }, []);

  const login = async (email: string, password: string) => {
    try {
      setLoading(true);
      setError(null);

      const response = await fetch('/api/auth/login', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify({ email, password }),
      });

      const data = await response.json();

      if (!response.ok) {
        throw new Error(data.message || 'Login failed');
      }

      localStorage.setItem('auth_token', data.token);
      setUser(data.user);
      router.push('/dashboard');
    } catch (err) {
      setError(err instanceof Error ? err.message : 'Login failed');
      throw err;
    } finally {
      setLoading(false);
    }
  };

  const register = async (userData: any) => {
    try {
      setLoading(true);
      setError(null);

      const response = await fetch('/api/auth/register', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify(userData),
      });

      const data = await response.json();

      if (!response.ok) {
        throw new Error(data.message || 'Registration failed');
      }

      localStorage.setItem('auth_token', data.token);
      setUser(data.user);
      router.push('/dashboard');
    } catch (err) {
      setError(err instanceof Error ? err.message : 'Registration failed');
      throw err;
    } finally {
      setLoading(false);
    }
  };

  const logout = async () => {
    try {
      setLoading(true);
      
      // Call logout endpoint
      const token = localStorage.getItem('auth_token');
      if (token) {
        await fetch('/api/auth/logout', {
          method: 'POST',
          headers: {
            'Authorization': `Bearer ${token}`,
          },
        });
      }
    } catch (err) {
      console.error('Logout error:', err);
    } finally {
      localStorage.removeItem('auth_token');
      setUser(null);
      setLoading(false);
      router.push('/auth/login');
    }
  };

  const updateUser = async (userData: Partial<User>) => {
    try {
      setLoading(true);
      setError(null);

      const token = localStorage.getItem('auth_token');
      const response = await fetch('/api/user/profile', {
        method: 'PUT',
        headers: {
          'Content-Type': 'application/json',
          'Authorization': `Bearer ${token}`,
        },
        body: JSON.stringify(userData),
      });

      const data = await response.json();

      if (!response.ok) {
        throw new Error(data.message || 'Update failed');
      }

      setUser(data.user);
    } catch (err) {
      setError(err instanceof Error ? err.message : 'Update failed');
      throw err;
    } finally {
      setLoading(false);
    }
  };

  const clearError = () => {
    setError(null);
  };

  const value: AuthContextType = {
    user,
    loading,
    error,
    login,
    register,
    logout,
    updateUser,
    clearError,
  };

  return (
    <AuthContext.Provider value={value}>
      {children}
    </AuthContext.Provider>
  );
};

export const useAuth = (): AuthContextType => {
  const context = useContext(AuthContext);
  if (context === undefined) {
    throw new Error('useAuth must be used within an AuthProvider');
  }
  return context;
};
```

## File: src/components/providers/index.ts
```typescript
// Provider components exports
export * from './theme-provider';
export * from './auth-provider';
export * from './api-provider';
export * from './toast-provider';
```

## File: src/components/providers/theme-provider.tsx
```typescript
"use client";

import * as React from "react";
import { ThemeProvider as NextThemesProvider } from "next-themes";

export interface ThemeProviderProps {
  children: React.ReactNode;
  attribute?: string;
  defaultTheme?: string;
  enableSystem?: boolean;
  disableTransitionOnChange?: boolean;
  storageKey?: string;
  themes?: string[];
}

export function ThemeProvider({
  children,
  attribute = "class",
  defaultTheme = "system",
  enableSystem = true,
  disableTransitionOnChange = false,
  storageKey = "theme",
  themes = ["light", "dark", "system"],
  ...props
}: ThemeProviderProps) {
  return (
    <NextThemesProvider
      attribute={attribute}
      defaultTheme={defaultTheme}
      enableSystem={enableSystem}
      disableTransitionOnChange={disableTransitionOnChange}
      storageKey={storageKey}
      themes={themes}
      {...props}
    >
      {children}
    </NextThemesProvider>
  );
}
```

## File: src/components/providers/toast-provider.tsx
```typescript
"use client";

import React, { createContext, useContext, useState, useCallback } from 'react';
import { Toaster } from '@/components/ui/toaster';
import { useToast } from '@/hooks/useToast';

export interface ToastMessage {
  id: string;
  title: string;
  description?: string;
  variant?: 'default' | 'destructive' | 'success' | 'warning';
  duration?: number;
  action?: {
    label: string;
    onClick: () => void;
  };
}

export interface ToastContextType {
  toasts: ToastMessage[];
  addToast: (toast: Omit<ToastMessage, 'id'>) => void;
  removeToast: (id: string) => void;
  clearToasts: () => void;
  success: (title: string, description?: string) => void;
  error: (title: string, description?: string) => void;
  warning: (title: string, description?: string) => void;
  info: (title: string, description?: string) => void;
}

const ToastContext = createContext<ToastContextType | undefined>(undefined);

export interface ToastProviderProps {
  children: React.ReactNode;
  maxToasts?: number;
}

export const ToastProvider: React.FC<ToastProviderProps> = ({
  children,
  maxToasts = 5,
}) => {
  const [toasts, setToasts] = useState<ToastMessage[]>([]);
  const { toast } = useToast();

  const addToast = useCallback((toastData: Omit<ToastMessage, 'id'>) => {
    const id = Math.random().toString(36).substr(2, 9);
    const newToast: ToastMessage = {
      id,
      duration: 5000,
      variant: 'default',
      ...toastData,
    };

    setToasts(prev => {
      const updated = [newToast, ...prev];
      if (updated.length > maxToasts) {
        return updated.slice(0, maxToasts);
      }
      return updated;
    });

    // Auto-remove toast after duration
    if (newToast.duration && newToast.duration > 0) {
      setTimeout(() => {
        removeToast(id);
      }, newToast.duration);
    }
  }, [maxToasts]);

  const removeToast = useCallback((id: string) => {
    setToasts(prev => prev.filter(toast => toast.id !== id));
  }, []);

  const clearToasts = useCallback(() => {
    setToasts([]);
  }, []);

  const success = useCallback((title: string, description?: string) => {
    addToast({
      title,
      description,
      variant: 'success',
    });
  }, [addToast]);

  const error = useCallback((title: string, description?: string) => {
    addToast({
      title,
      description,
      variant: 'destructive',
    });
  }, [addToast]);

  const warning = useCallback((title: string, description?: string) => {
    addToast({
      title,
      description,
      variant: 'warning',
    });
  }, [addToast]);

  const info = useCallback((title: string, description?: string) => {
    addToast({
      title,
      description,
      variant: 'default',
    });
  }, [addToast]);

  const value: ToastContextType = {
    toasts,
    addToast,
    removeToast,
    clearToasts,
    success,
    error,
    warning,
    info,
  };

  return (
    <ToastContext.Provider value={value}>
      {children}
      <Toaster />
    </ToastContext.Provider>
  );
};

export const useToastContext = (): ToastContextType => {
  const context = useContext(ToastContext);
  if (context === undefined) {
    throw new Error('useToastContext must be used within a ToastProvider');
  }
  return context;
};
```

## File: src/components/ui/alert.tsx
```typescript
import * as React from "react"
import { cva, type VariantProps } from "class-variance-authority"

import { cn } from "@/lib/utils"

const alertVariants = cva(
  "relative w-full rounded-lg border px-4 py-3 text-sm [&>svg+div]:translate-y-[-3px] [&>svg]:absolute [&>svg]:left-4 [&>svg]:top-4 [&>svg]:text-foreground [&>svg~*]:pl-7",
  {
    variants: {
      variant: {
        default: "bg-background text-foreground",
        destructive:
          "border-destructive/50 text-destructive dark:border-destructive [&>svg]:text-destructive",
      },
    },
    defaultVariants: {
      variant: "default",
    },
  }
)

const Alert = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement> & VariantProps<typeof alertVariants>
>(({ className, variant, ...props }, ref) => (
  <div
    ref={ref}
    role="alert"
    className={cn(alertVariants({ variant }), className)}
    {...props}
  />
))
Alert.displayName = "Alert"

const AlertTitle = React.forwardRef<
  HTMLParagraphElement,
  React.HTMLAttributes<HTMLHeadingElement>
>(({ className, ...props }, ref) => (
  <h5
    ref={ref}
    className={cn("mb-1 font-medium leading-none tracking-tight", className)}
    {...props}
  />
))
AlertTitle.displayName = "AlertTitle"

const AlertDescription = React.forwardRef<
  HTMLParagraphElement,
  React.HTMLAttributes<HTMLParagraphElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("text-sm [&_p]:leading-relaxed", className)}
    {...props}
  />
))
AlertDescription.displayName = "AlertDescription"

export { Alert, AlertTitle, AlertDescription }
```

## File: src/components/ui/avatar.tsx
```typescript
"use client"

import * as React from "react"
import * as AvatarPrimitive from "@radix-ui/react-avatar"

import { cn } from "@/lib/utils"

const Avatar = React.forwardRef<
  React.ElementRef<typeof AvatarPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof AvatarPrimitive.Root>
>(({ className, ...props }, ref) => (
  <AvatarPrimitive.Root
    ref={ref}
    className={cn(
      "relative flex h-10 w-10 shrink-0 overflow-hidden rounded-full",
      className
    )}
    {...props}
  />
))
Avatar.displayName = AvatarPrimitive.Root.displayName

const AvatarImage = React.forwardRef<
  React.ElementRef<typeof AvatarPrimitive.Image>,
  React.ComponentPropsWithoutRef<typeof AvatarPrimitive.Image>
>(({ className, ...props }, ref) => (
  <AvatarPrimitive.Image
    ref={ref}
    className={cn("aspect-square h-full w-full", className)}
    {...props}
  />
))
AvatarImage.displayName = AvatarPrimitive.Image.displayName

const AvatarFallback = React.forwardRef<
  React.ElementRef<typeof AvatarPrimitive.Fallback>,
  React.ComponentPropsWithoutRef<typeof AvatarPrimitive.Fallback>
>(({ className, ...props }, ref) => (
  <AvatarPrimitive.Fallback
    ref={ref}
    className={cn(
      "flex h-full w-full items-center justify-center rounded-full bg-muted",
      className
    )}
    {...props}
  />
))
AvatarFallback.displayName = AvatarPrimitive.Fallback.displayName

export { Avatar, AvatarImage, AvatarFallback }
```

## File: src/components/ui/badge.tsx
```typescript
import * as React from "react"
import { cva, type VariantProps } from "class-variance-authority"

import { cn } from "@/lib/utils"

const badgeVariants = cva(
  "inline-flex items-center rounded-full border px-2.5 py-0.5 text-xs font-semibold transition-colors focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2",
  {
    variants: {
      variant: {
        default:
          "border-transparent bg-primary text-primary-foreground hover:bg-primary/80",
        secondary:
          "border-transparent bg-secondary text-secondary-foreground hover:bg-secondary/80",
        destructive:
          "border-transparent bg-destructive text-destructive-foreground hover:bg-destructive/80",
        outline: "text-foreground",
      },
    },
    defaultVariants: {
      variant: "default",
    },
  }
)

export interface BadgeProps
  extends React.HTMLAttributes<HTMLDivElement>,
    VariantProps<typeof badgeVariants> {}

function Badge({ className, variant, ...props }: BadgeProps) {
  return (
    <div className={cn(badgeVariants({ variant }), className)} {...props} />
  )
}

export { Badge, badgeVariants }
```

## File: src/components/ui/button.tsx
```typescript
import * as React from "react"
import { Slot } from "@radix-ui/react-slot"
import { cva, type VariantProps } from "class-variance-authority"

import { cn } from "@/lib/utils"

const buttonVariants = cva(
  "inline-flex items-center justify-center gap-2 whitespace-nowrap rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:pointer-events-none disabled:opacity-50 [&_svg]:pointer-events-none [&_svg]:size-4 [&_svg]:shrink-0",
  {
    variants: {
      variant: {
        default:
          "bg-primary text-primary-foreground shadow hover:bg-primary/90",
        destructive:
          "bg-destructive text-destructive-foreground shadow-sm hover:bg-destructive/90",
        outline:
          "border border-input bg-background shadow-sm hover:bg-accent hover:text-accent-foreground",
        secondary:
          "bg-secondary text-secondary-foreground shadow-sm hover:bg-secondary/80",
        ghost: "hover:bg-accent hover:text-accent-foreground",
        link: "text-primary underline-offset-4 hover:underline",
      },
      size: {
        default: "h-9 px-4 py-2",
        sm: "h-8 rounded-md px-3 text-xs",
        lg: "h-10 rounded-md px-8",
        icon: "h-9 w-9",
      },
    },
    defaultVariants: {
      variant: "default",
      size: "default",
    },
  }
)

export interface ButtonProps
  extends React.ButtonHTMLAttributes<HTMLButtonElement>,
    VariantProps<typeof buttonVariants> {
  asChild?: boolean
}

const Button = React.forwardRef<HTMLButtonElement, ButtonProps>(
  ({ className, variant, size, asChild = false, ...props }, ref) => {
    const Comp = asChild ? Slot : "button"
    return (
      <Comp
        className={cn(buttonVariants({ variant, size, className }))}
        ref={ref}
        {...props}
      />
    )
  }
)
Button.displayName = "Button"

export { Button, buttonVariants }
```

## File: src/components/ui/calendar.tsx
```typescript
"use client";

import * as React from "react";
import { ChevronLeft, ChevronRight } from "lucide-react";
import { DayPicker, DropdownProps } from "react-day-picker";

import { cn } from "@/lib/utils";
import { buttonVariants } from "@/components/ui/button";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "./select";
import { ScrollArea } from "@/components/ui/scroll-area";

export type CalendarProps = React.ComponentProps<typeof DayPicker>;

function Calendar({
  className,
  classNames,
  showOutsideDays = true,
  ...props
}: CalendarProps) {
  return (
    <DayPicker
      showOutsideDays={showOutsideDays}
      className={cn("p-3", className)}
      classNames={{
        month: "space-y-4",
        months: "flex flex-col sm:flex-row space-y-4 sm:space-y-0 relative",
        month_caption: "flex justify-center pt-1 relative items-center",
        month_grid: "w-full border-collapse space-y-1",

        // TEST
        dropdowns: "flex justify-center gap-1",
        nav: "flex items-center justify-between absolute inset-x-0 top-2",
        button_previous: cn(
          buttonVariants({ variant: "outline" }),
          "h-7 w-7 bg-transparent p-0 opacity-50 hover:opacity-100 z-10"
        ),
        button_next: cn(
          buttonVariants({ variant: "outline" }),
          "h-7 w-7 bg-transparent p-0 opacity-50 hover:opacity-100 z-10"
        ),
        // TEST

        weeks: "w-full border-collapse space-y-",
        weekdays: "flex",
        weekday:
          "text-muted-foreground rounded-md w-9 font-normal text-[0.8rem]",
        week: "flex w-full mt-2",
        day_button:
          "h-9 w-9 text-center text-sm p-0 relative [&:has([aria-selected].day-range-end)]:rounded-r-md [&:has([aria-selected].day-outside)]:bg-accent/50 [&:has([aria-selected])]:bg-accent first:[&:has([aria-selected])]:rounded-l-md last:[&:has([aria-selected])]:rounded-r-md focus-within:relative focus-within:z-20",
        day: cn(
          buttonVariants({ variant: "ghost" }),
          "h-9 w-9 p-0 font-normal aria-selected:opacity-100"
        ),
        range_end: "day-range-end",
        selected:
          "bg-primary text-primary-foreground hover:bg-primary hover:text-primary-foreground focus:bg-primary focus:text-primary-foreground",
        outside:
          "day-outside text-muted-foreground opacity-50 aria-selected:bg-accent/50 aria-selected:text-muted-foreground aria-selected:opacity-30",
        disabled: "text-muted-foreground opacity-50",
        range_middle:
          "aria-selected:bg-accent aria-selected:text-accent-foreground",
        hidden: "invisible",
        ...classNames,
      }}
      components={{
        Dropdown: ({ value, onChange, options }: DropdownProps) => {
          const selected = options?.find((child) => child.value === value);
          const handleChange = (value: string) => {
            const changeEvent = {
              target: { value },
            } as React.ChangeEvent<HTMLSelectElement>;
            onChange?.(changeEvent);
          };
          return (
            <Select
              value={value?.toString()}
              onValueChange={(value) => {
                handleChange(value);
              }}
            >
              <SelectTrigger className="pr-1.5 focus:ring-0">
                <SelectValue>{selected?.label}</SelectValue>
              </SelectTrigger>
              <SelectContent position="popper">
                <ScrollArea className="h-80">
                  {options?.map((option, id: number) => (
                    <SelectItem
                      key={`${option.value}-${id}`}
                      value={option.value?.toString() ?? ""}
                    >
                      {option.label}
                    </SelectItem>
                  ))}
                </ScrollArea>
              </SelectContent>
            </Select>
          );
        },
        Chevron: ({ ...props }) =>
          props.orientation === "left" ? (
            <ChevronLeft {...props} className="h-4 w-4" />
          ) : (
            <ChevronRight {...props} className="h-4 w-4" />
          ),
      }}
      {...props}
    />
  );
}
Calendar.displayName = "Calendar";

export { Calendar };
```

## File: src/components/ui/card.tsx
```typescript
import * as React from "react"

import { cn } from "@/lib/utils"

const Card = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn(
      "rounded-xl border bg-card text-card-foreground shadow",
      className
    )}
    {...props}
  />
))
Card.displayName = "Card"

const CardHeader = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("flex flex-col space-y-1.5 p-6", className)}
    {...props}
  />
))
CardHeader.displayName = "CardHeader"

const CardTitle = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("font-semibold leading-none tracking-tight", className)}
    {...props}
  />
))
CardTitle.displayName = "CardTitle"

const CardDescription = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props}
  />
))
CardDescription.displayName = "CardDescription"

const CardContent = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div ref={ref} className={cn("p-6 pt-0", className)} {...props} />
))
CardContent.displayName = "CardContent"

const CardFooter = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("flex items-center p-6 pt-0", className)}
    {...props}
  />
))
CardFooter.displayName = "CardFooter"

export { Card, CardHeader, CardFooter, CardTitle, CardDescription, CardContent }
```

## File: src/components/ui/chart.tsx
```typescript
"use client"

import * as React from "react"
import * as RechartsPrimitive from "recharts"

import { cn } from "@/lib/utils"

// Format: { THEME_NAME: CSS_SELECTOR }
const THEMES = { light: "", dark: ".dark" } as const

export type ChartConfig = {
  [k in string]: {
    label?: React.ReactNode
    icon?: React.ComponentType
  } & (
    | { color?: string; theme?: never }
    | { color?: never; theme: Record<keyof typeof THEMES, string> }
  )
}

type ChartContextProps = {
  config: ChartConfig
}

const ChartContext = React.createContext<ChartContextProps | null>(null)

function useChart() {
  const context = React.useContext(ChartContext)

  if (!context) {
    throw new Error("useChart must be used within a <ChartContainer />")
  }

  return context
}

const ChartContainer = React.forwardRef<
  HTMLDivElement,
  React.ComponentProps<"div"> & {
    config: ChartConfig
    children: React.ComponentProps<
      typeof RechartsPrimitive.ResponsiveContainer
    >["children"]
  }
>(({ id, className, children, config, ...props }, ref) => {
  const uniqueId = React.useId()
  const chartId = `chart-${id || uniqueId.replace(/:/g, "")}`

  return (
    <ChartContext.Provider value={{ config }}>
      <div
        data-chart={chartId}
        ref={ref}
        className={cn(
          "flex aspect-video justify-center text-xs [&_.recharts-cartesian-axis-tick_text]:fill-muted-foreground [&_.recharts-cartesian-grid_line[stroke='#ccc']]:stroke-border/50 [&_.recharts-curve.recharts-tooltip-cursor]:stroke-border [&_.recharts-dot[stroke='#fff']]:stroke-transparent [&_.recharts-layer]:outline-none [&_.recharts-polar-grid_[stroke='#ccc']]:stroke-border [&_.recharts-radial-bar-background-sector]:fill-muted [&_.recharts-rectangle.recharts-tooltip-cursor]:fill-muted [&_.recharts-reference-line_[stroke='#ccc']]:stroke-border [&_.recharts-sector[stroke='#fff']]:stroke-transparent [&_.recharts-sector]:outline-none [&_.recharts-surface]:outline-none",
          className
        )}
        {...props}
      >
        <ChartStyle id={chartId} config={config} />
        <RechartsPrimitive.ResponsiveContainer>
          {children}
        </RechartsPrimitive.ResponsiveContainer>
      </div>
    </ChartContext.Provider>
  )
})
ChartContainer.displayName = "Chart"

const ChartStyle = ({ id, config }: { id: string; config: ChartConfig }) => {
  const colorConfig = Object.entries(config).filter(
    ([, config]) => config.theme || config.color
  )

  if (!colorConfig.length) {
    return null
  }

  return (
    <style
      dangerouslySetInnerHTML={{
        __html: Object.entries(THEMES)
          .map(
            ([theme, prefix]) => `
${prefix} [data-chart=${id}] {
${colorConfig
  .map(([key, itemConfig]) => {
    const color =
      itemConfig.theme?.[theme as keyof typeof itemConfig.theme] ||
      itemConfig.color
    return color ? `  --color-${key}: ${color};` : null
  })
  .join("\n")}
}
`
          )
          .join("\n"),
      }}
    />
  )
}

const ChartTooltip = RechartsPrimitive.Tooltip

const ChartTooltipContent = React.forwardRef<
  HTMLDivElement,
  React.ComponentProps<typeof RechartsPrimitive.Tooltip> &
    React.ComponentProps<"div"> & {
      hideLabel?: boolean
      hideIndicator?: boolean
      indicator?: "line" | "dot" | "dashed"
      nameKey?: string
      labelKey?: string
    }
>(
  (
    {
      active,
      payload,
      className,
      indicator = "dot",
      hideLabel = false,
      hideIndicator = false,
      label,
      labelFormatter,
      labelClassName,
      formatter,
      color,
      nameKey,
      labelKey,
    },
    ref
  ) => {
    const { config } = useChart()

    const tooltipLabel = React.useMemo(() => {
      if (hideLabel || !payload?.length) {
        return null
      }

      const [item] = payload
      const key = `${labelKey || item?.dataKey || item?.name || "value"}`
      const itemConfig = getPayloadConfigFromPayload(config, item, key)
      const value =
        !labelKey && typeof label === "string"
          ? config[label as keyof typeof config]?.label || label
          : itemConfig?.label

      if (labelFormatter) {
        return (
          <div className={cn("font-medium", labelClassName)}>
            {labelFormatter(value, payload)}
          </div>
        )
      }

      if (!value) {
        return null
      }

      return <div className={cn("font-medium", labelClassName)}>{value}</div>
    }, [
      label,
      labelFormatter,
      payload,
      hideLabel,
      labelClassName,
      config,
      labelKey,
    ])

    if (!active || !payload?.length) {
      return null
    }

    const nestLabel = payload.length === 1 && indicator !== "dot"

    return (
      <div
        ref={ref}
        className={cn(
          "grid min-w-[8rem] items-start gap-1.5 rounded-lg border border-border/50 bg-background px-2.5 py-1.5 text-xs shadow-xl",
          className
        )}
      >
        {!nestLabel ? tooltipLabel : null}
        <div className="grid gap-1.5">
          {payload.map((item, index) => {
            const key = `${nameKey || item.name || item.dataKey || "value"}`
            const itemConfig = getPayloadConfigFromPayload(config, item, key)
            const indicatorColor = color || item.payload.fill || item.color

            return (
              <div
                key={item.dataKey}
                className={cn(
                  "flex w-full flex-wrap items-stretch gap-2 [&>svg]:h-2.5 [&>svg]:w-2.5 [&>svg]:text-muted-foreground",
                  indicator === "dot" && "items-center"
                )}
              >
                {formatter && item?.value !== undefined && item.name ? (
                  formatter(item.value, item.name, item, index, item.payload)
                ) : (
                  <>
                    {itemConfig?.icon ? (
                      <itemConfig.icon />
                    ) : (
                      !hideIndicator && (
                        <div
                          className={cn(
                            "shrink-0 rounded-[2px] border-[--color-border] bg-[--color-bg]",
                            {
                              "h-2.5 w-2.5": indicator === "dot",
                              "w-1": indicator === "line",
                              "w-0 border-[1.5px] border-dashed bg-transparent":
                                indicator === "dashed",
                              "my-0.5": nestLabel && indicator === "dashed",
                            }
                          )}
                          style={
                            {
                              "--color-bg": indicatorColor,
                              "--color-border": indicatorColor,
                            } as React.CSSProperties
                          }
                        />
                      )
                    )}
                    <div
                      className={cn(
                        "flex flex-1 justify-between leading-none",
                        nestLabel ? "items-end" : "items-center"
                      )}
                    >
                      <div className="grid gap-1.5">
                        {nestLabel ? tooltipLabel : null}
                        <span className="text-muted-foreground">
                          {itemConfig?.label || item.name}
                        </span>
                      </div>
                      {item.value && (
                        <span className="font-mono font-medium tabular-nums text-foreground">
                          {item.value.toLocaleString()}
                        </span>
                      )}
                    </div>
                  </>
                )}
              </div>
            )
          })}
        </div>
      </div>
    )
  }
)
ChartTooltipContent.displayName = "ChartTooltip"

const ChartLegend = RechartsPrimitive.Legend

const ChartLegendContent = React.forwardRef<
  HTMLDivElement,
  React.ComponentProps<"div"> &
    Pick<RechartsPrimitive.LegendProps, "payload" | "verticalAlign"> & {
      hideIcon?: boolean
      nameKey?: string
    }
>(
  (
    { className, hideIcon = false, payload, verticalAlign = "bottom", nameKey },
    ref
  ) => {
    const { config } = useChart()

    if (!payload?.length) {
      return null
    }

    return (
      <div
        ref={ref}
        className={cn(
          "flex items-center justify-center gap-4",
          verticalAlign === "top" ? "pb-3" : "pt-3",
          className
        )}
      >
        {payload.map((item) => {
          const key = `${nameKey || item.dataKey || "value"}`
          const itemConfig = getPayloadConfigFromPayload(config, item, key)

          return (
            <div
              key={item.value}
              className={cn(
                "flex items-center gap-1.5 [&>svg]:h-3 [&>svg]:w-3 [&>svg]:text-muted-foreground"
              )}
            >
              {itemConfig?.icon && !hideIcon ? (
                <itemConfig.icon />
              ) : (
                <div
                  className="h-2 w-2 shrink-0 rounded-[2px]"
                  style={{
                    backgroundColor: item.color,
                  }}
                />
              )}
              {itemConfig?.label}
            </div>
          )
        })}
      </div>
    )
  }
)
ChartLegendContent.displayName = "ChartLegend"

// Helper to extract item config from a payload.
function getPayloadConfigFromPayload(
  config: ChartConfig,
  payload: unknown,
  key: string
) {
  if (typeof payload !== "object" || payload === null) {
    return undefined
  }

  const payloadPayload =
    "payload" in payload &&
    typeof payload.payload === "object" &&
    payload.payload !== null
      ? payload.payload
      : undefined

  let configLabelKey: string = key

  if (
    key in payload &&
    typeof payload[key as keyof typeof payload] === "string"
  ) {
    configLabelKey = payload[key as keyof typeof payload] as string
  } else if (
    payloadPayload &&
    key in payloadPayload &&
    typeof payloadPayload[key as keyof typeof payloadPayload] === "string"
  ) {
    configLabelKey = payloadPayload[
      key as keyof typeof payloadPayload
    ] as string
  }

  return configLabelKey in config
    ? config[configLabelKey]
    : config[key as keyof typeof config]
}

export {
  ChartContainer,
  ChartTooltip,
  ChartTooltipContent,
  ChartLegend,
  ChartLegendContent,
  ChartStyle,
}
```

## File: src/components/ui/checkbox.tsx
```typescript
"use client"

import * as React from "react"
import * as CheckboxPrimitive from "@radix-ui/react-checkbox"
import { Check } from "lucide-react"

import { cn } from "@/lib/utils"

const Checkbox = React.forwardRef<
  React.ElementRef<typeof CheckboxPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof CheckboxPrimitive.Root>
>(({ className, ...props }, ref) => (
  <CheckboxPrimitive.Root
    ref={ref}
    className={cn(
      "peer h-4 w-4 shrink-0 rounded-sm border border-primary shadow focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 data-[state=checked]:bg-primary data-[state=checked]:text-primary-foreground",
      className
    )}
    {...props}
  >
    <CheckboxPrimitive.Indicator
      className={cn("flex items-center justify-center text-current")}
    >
      <Check className="h-4 w-4" />
    </CheckboxPrimitive.Indicator>
  </CheckboxPrimitive.Root>
))
Checkbox.displayName = CheckboxPrimitive.Root.displayName

export { Checkbox }
```

## File: src/components/ui/dialog.tsx
```typescript
"use client"

import * as React from "react"
import * as DialogPrimitive from "@radix-ui/react-dialog"
import { X } from "lucide-react"

import { cn } from "@/lib/utils"

const Dialog = DialogPrimitive.Root

const DialogTrigger = DialogPrimitive.Trigger

const DialogPortal = DialogPrimitive.Portal

const DialogClose = DialogPrimitive.Close

const DialogOverlay = React.forwardRef<
  React.ElementRef<typeof DialogPrimitive.Overlay>,
  React.ComponentPropsWithoutRef<typeof DialogPrimitive.Overlay>
>(({ className, ...props }, ref) => (
  <DialogPrimitive.Overlay
    ref={ref}
    className={cn(
      "fixed inset-0 z-50 bg-black/80  data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0",
      className
    )}
    {...props}
  />
))
DialogOverlay.displayName = DialogPrimitive.Overlay.displayName

const DialogContent = React.forwardRef<
  React.ElementRef<typeof DialogPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof DialogPrimitive.Content>
>(({ className, children, ...props }, ref) => (
  <DialogPortal>
    <DialogOverlay />
    <DialogPrimitive.Content
      ref={ref}
      className={cn(
        "fixed left-[50%] top-[50%] z-50 grid w-full max-w-lg translate-x-[-50%] translate-y-[-50%] gap-4 border bg-background p-6 shadow-lg duration-200 data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[state=closed]:slide-out-to-left-1/2 data-[state=closed]:slide-out-to-top-[48%] data-[state=open]:slide-in-from-left-1/2 data-[state=open]:slide-in-from-top-[48%] sm:rounded-lg",
        className
      )}
      {...props}
    >
      {children}
      <DialogPrimitive.Close className="absolute right-4 top-4 rounded-sm opacity-70 ring-offset-background transition-opacity hover:opacity-100 focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 disabled:pointer-events-none data-[state=open]:bg-accent data-[state=open]:text-muted-foreground">
        <X className="h-4 w-4" />
        <span className="sr-only">Close</span>
      </DialogPrimitive.Close>
    </DialogPrimitive.Content>
  </DialogPortal>
))
DialogContent.displayName = DialogPrimitive.Content.displayName

const DialogHeader = ({
  className,
  ...props
}: React.HTMLAttributes<HTMLDivElement>) => (
  <div
    className={cn(
      "flex flex-col space-y-1.5 text-center sm:text-left",
      className
    )}
    {...props}
  />
)
DialogHeader.displayName = "DialogHeader"

const DialogFooter = ({
  className,
  ...props
}: React.HTMLAttributes<HTMLDivElement>) => (
  <div
    className={cn(
      "flex flex-col-reverse sm:flex-row sm:justify-end sm:space-x-2",
      className
    )}
    {...props}
  />
)
DialogFooter.displayName = "DialogFooter"

const DialogTitle = React.forwardRef<
  React.ElementRef<typeof DialogPrimitive.Title>,
  React.ComponentPropsWithoutRef<typeof DialogPrimitive.Title>
>(({ className, ...props }, ref) => (
  <DialogPrimitive.Title
    ref={ref}
    className={cn(
      "text-lg font-semibold leading-none tracking-tight",
      className
    )}
    {...props}
  />
))
DialogTitle.displayName = DialogPrimitive.Title.displayName

const DialogDescription = React.forwardRef<
  React.ElementRef<typeof DialogPrimitive.Description>,
  React.ComponentPropsWithoutRef<typeof DialogPrimitive.Description>
>(({ className, ...props }, ref) => (
  <DialogPrimitive.Description
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props}
  />
))
DialogDescription.displayName = DialogPrimitive.Description.displayName

export {
  Dialog,
  DialogPortal,
  DialogOverlay,
  DialogTrigger,
  DialogClose,
  DialogContent,
  DialogHeader,
  DialogFooter,
  DialogTitle,
  DialogDescription,
}
```

## File: src/components/ui/dropdown-menu.tsx
```typescript
"use client"

import * as React from "react"
import * as DropdownMenuPrimitive from "@radix-ui/react-dropdown-menu"
import { Check, ChevronRight, Circle } from "lucide-react"

import { cn } from "@/lib/utils"

const DropdownMenu = DropdownMenuPrimitive.Root

const DropdownMenuTrigger = DropdownMenuPrimitive.Trigger

const DropdownMenuGroup = DropdownMenuPrimitive.Group

const DropdownMenuPortal = DropdownMenuPrimitive.Portal

const DropdownMenuSub = DropdownMenuPrimitive.Sub

const DropdownMenuRadioGroup = DropdownMenuPrimitive.RadioGroup

const DropdownMenuSubTrigger = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.SubTrigger>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.SubTrigger> & {
    inset?: boolean
  }
>(({ className, inset, children, ...props }, ref) => (
  <DropdownMenuPrimitive.SubTrigger
    ref={ref}
    className={cn(
      "flex cursor-default select-none items-center gap-2 rounded-sm px-2 py-1.5 text-sm outline-none focus:bg-accent data-[state=open]:bg-accent [&_svg]:pointer-events-none [&_svg]:size-4 [&_svg]:shrink-0",
      inset && "pl-8",
      className
    )}
    {...props}
  >
    {children}
    <ChevronRight className="ml-auto" />
  </DropdownMenuPrimitive.SubTrigger>
))
DropdownMenuSubTrigger.displayName =
  DropdownMenuPrimitive.SubTrigger.displayName

const DropdownMenuSubContent = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.SubContent>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.SubContent>
>(({ className, ...props }, ref) => (
  <DropdownMenuPrimitive.SubContent
    ref={ref}
    className={cn(
      "z-50 min-w-[8rem] overflow-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-lg data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
      className
    )}
    {...props}
  />
))
DropdownMenuSubContent.displayName =
  DropdownMenuPrimitive.SubContent.displayName

const DropdownMenuContent = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.Content>
>(({ className, sideOffset = 4, ...props }, ref) => (
  <DropdownMenuPrimitive.Portal>
    <DropdownMenuPrimitive.Content
      ref={ref}
      sideOffset={sideOffset}
      className={cn(
        "z-50 max-h-[var(--radix-dropdown-menu-content-available-height)] min-w-[8rem] overflow-y-auto overflow-x-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-md",
        "data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props}
    />
  </DropdownMenuPrimitive.Portal>
))
DropdownMenuContent.displayName = DropdownMenuPrimitive.Content.displayName

const DropdownMenuItem = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.Item>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.Item> & {
    inset?: boolean
  }
>(({ className, inset, ...props }, ref) => (
  <DropdownMenuPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center gap-2 rounded-sm px-2 py-1.5 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50 [&>svg]:size-4 [&>svg]:shrink-0",
      inset && "pl-8",
      className
    )}
    {...props}
  />
))
DropdownMenuItem.displayName = DropdownMenuPrimitive.Item.displayName

const DropdownMenuCheckboxItem = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.CheckboxItem>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.CheckboxItem>
>(({ className, children, checked, ...props }, ref) => (
  <DropdownMenuPrimitive.CheckboxItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    checked={checked}
    {...props}
  >
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <DropdownMenuPrimitive.ItemIndicator>
        <Check className="h-4 w-4" />
      </DropdownMenuPrimitive.ItemIndicator>
    </span>
    {children}
  </DropdownMenuPrimitive.CheckboxItem>
))
DropdownMenuCheckboxItem.displayName =
  DropdownMenuPrimitive.CheckboxItem.displayName

const DropdownMenuRadioItem = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.RadioItem>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.RadioItem>
>(({ className, children, ...props }, ref) => (
  <DropdownMenuPrimitive.RadioItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    {...props}
  >
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <DropdownMenuPrimitive.ItemIndicator>
        <Circle className="h-2 w-2 fill-current" />
      </DropdownMenuPrimitive.ItemIndicator>
    </span>
    {children}
  </DropdownMenuPrimitive.RadioItem>
))
DropdownMenuRadioItem.displayName = DropdownMenuPrimitive.RadioItem.displayName

const DropdownMenuLabel = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.Label>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.Label> & {
    inset?: boolean
  }
>(({ className, inset, ...props }, ref) => (
  <DropdownMenuPrimitive.Label
    ref={ref}
    className={cn(
      "px-2 py-1.5 text-sm font-semibold",
      inset && "pl-8",
      className
    )}
    {...props}
  />
))
DropdownMenuLabel.displayName = DropdownMenuPrimitive.Label.displayName

const DropdownMenuSeparator = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.Separator>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.Separator>
>(({ className, ...props }, ref) => (
  <DropdownMenuPrimitive.Separator
    ref={ref}
    className={cn("-mx-1 my-1 h-px bg-muted", className)}
    {...props}
  />
))
DropdownMenuSeparator.displayName = DropdownMenuPrimitive.Separator.displayName

const DropdownMenuShortcut = ({
  className,
  ...props
}: React.HTMLAttributes<HTMLSpanElement>) => {
  return (
    <span
      className={cn("ml-auto text-xs tracking-widest opacity-60", className)}
      {...props}
    />
  )
}
DropdownMenuShortcut.displayName = "DropdownMenuShortcut"

export {
  DropdownMenu,
  DropdownMenuTrigger,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuCheckboxItem,
  DropdownMenuRadioItem,
  DropdownMenuLabel,
  DropdownMenuSeparator,
  DropdownMenuShortcut,
  DropdownMenuGroup,
  DropdownMenuPortal,
  DropdownMenuSub,
  DropdownMenuSubContent,
  DropdownMenuSubTrigger,
  DropdownMenuRadioGroup,
}
```

## File: src/components/ui/form.tsx
```typescript
"use client"

import * as React from "react"
import * as LabelPrimitive from "@radix-ui/react-label"
import { Slot } from "@radix-ui/react-slot"
import {
  Controller,
  ControllerProps,
  FieldPath,
  FieldValues,
  FormProvider,
  useFormContext,
} from "react-hook-form"

import { cn } from "@/lib/utils"
import { Label } from "@/components/ui/label"

const Form = FormProvider

type FormFieldContextValue<
  TFieldValues extends FieldValues = FieldValues,
  TName extends FieldPath<TFieldValues> = FieldPath<TFieldValues>
> = {
  name: TName
}

const FormFieldContext = React.createContext<FormFieldContextValue>(
  {} as FormFieldContextValue
)

const FormField = <
  TFieldValues extends FieldValues = FieldValues,
  TName extends FieldPath<TFieldValues> = FieldPath<TFieldValues>
>({
  ...props
}: ControllerProps<TFieldValues, TName>) => {
  return (
    <FormFieldContext.Provider value={{ name: props.name }}>
      <Controller {...props} />
    </FormFieldContext.Provider>
  )
}

const useFormField = () => {
  const fieldContext = React.useContext(FormFieldContext)
  const itemContext = React.useContext(FormItemContext)
  const { getFieldState, formState } = useFormContext()

  const fieldState = getFieldState(fieldContext.name, formState)

  if (!fieldContext) {
    throw new Error("useFormField should be used within <FormField>")
  }

  const { id } = itemContext

  return {
    id,
    name: fieldContext.name,
    formItemId: `${id}-form-item`,
    formDescriptionId: `${id}-form-item-description`,
    formMessageId: `${id}-form-item-message`,
    ...fieldState,
  }
}

type FormItemContextValue = {
  id: string
}

const FormItemContext = React.createContext<FormItemContextValue>(
  {} as FormItemContextValue
)

const FormItem = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => {
  const id = React.useId()

  return (
    <FormItemContext.Provider value={{ id }}>
      <div ref={ref} className={cn("space-y-2", className)} {...props} />
    </FormItemContext.Provider>
  )
})
FormItem.displayName = "FormItem"

const FormLabel = React.forwardRef<
  React.ElementRef<typeof LabelPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof LabelPrimitive.Root>
>(({ className, ...props }, ref) => {
  const { error, formItemId } = useFormField()

  return (
    <Label
      ref={ref}
      className={cn(error && "text-destructive", className)}
      htmlFor={formItemId}
      {...props}
    />
  )
})
FormLabel.displayName = "FormLabel"

const FormControl = React.forwardRef<
  React.ElementRef<typeof Slot>,
  React.ComponentPropsWithoutRef<typeof Slot>
>(({ ...props }, ref) => {
  const { error, formItemId, formDescriptionId, formMessageId } = useFormField()

  return (
    <Slot
      ref={ref}
      id={formItemId}
      aria-describedby={
        !error
          ? `${formDescriptionId}`
          : `${formDescriptionId} ${formMessageId}`
      }
      aria-invalid={!!error}
      {...props}
    />
  )
})
FormControl.displayName = "FormControl"

const FormDescription = React.forwardRef<
  HTMLParagraphElement,
  React.HTMLAttributes<HTMLParagraphElement>
>(({ className, ...props }, ref) => {
  const { formDescriptionId } = useFormField()

  return (
    <p
      ref={ref}
      id={formDescriptionId}
      className={cn("text-[0.8rem] text-muted-foreground", className)}
      {...props}
    />
  )
})
FormDescription.displayName = "FormDescription"

const FormMessage = React.forwardRef<
  HTMLParagraphElement,
  React.HTMLAttributes<HTMLParagraphElement>
>(({ className, children, ...props }, ref) => {
  const { error, formMessageId } = useFormField()
  const body = error ? String(error?.message) : children

  if (!body) {
    return null
  }

  return (
    <p
      ref={ref}
      id={formMessageId}
      className={cn("text-[0.8rem] font-medium text-destructive", className)}
      {...props}
    >
      {body}
    </p>
  )
})
FormMessage.displayName = "FormMessage"

export {
  useFormField,
  Form,
  FormItem,
  FormLabel,
  FormControl,
  FormDescription,
  FormMessage,
  FormField,
}
```

## File: src/components/ui/index.ts
```typescript
// UI components exports
export * from './alert';
export * from './avatar';
export * from './badge';
export * from './button';
export * from './calendar';
export * from './card';
export * from './chart';
export * from './checkbox';
export * from './dialog';
export * from './dropdown-menu';
export * from './form';
export * from './input';
export * from './label';
export * from './popover';
export * from './progress';
export * from './radio-group';
export * from './scroll-area';
export * from './select';
export * from './skeleton';
export * from './table';
export * from './tabs';
export * from './textarea';
export * from './toast';
export * from './toaster';
```

## File: src/components/ui/input.tsx
```typescript
import * as React from "react"

import { cn } from "@/lib/utils"

const Input = React.forwardRef<HTMLInputElement, React.ComponentProps<"input">>(
  ({ className, type, ...props }, ref) => {
    return (
      <input
        type={type}
        className={cn(
          "flex h-9 w-full rounded-md border border-input bg-transparent px-3 py-1 text-base shadow-sm transition-colors file:border-0 file:bg-transparent file:text-sm file:font-medium file:text-foreground placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 md:text-sm",
          className
        )}
        ref={ref}
        {...props}
      />
    )
  }
)
Input.displayName = "Input"

export { Input }
```

## File: src/components/ui/label.tsx
```typescript
"use client"

import * as React from "react"
import * as LabelPrimitive from "@radix-ui/react-label"
import { cva, type VariantProps } from "class-variance-authority"

import { cn } from "@/lib/utils"

const labelVariants = cva(
  "text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
)

const Label = React.forwardRef<
  React.ElementRef<typeof LabelPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof LabelPrimitive.Root> &
    VariantProps<typeof labelVariants>
>(({ className, ...props }, ref) => (
  <LabelPrimitive.Root
    ref={ref}
    className={cn(labelVariants(), className)}
    {...props}
  />
))
Label.displayName = LabelPrimitive.Root.displayName

export { Label }
```

## File: src/components/ui/popover.tsx
```typescript
"use client"

import * as React from "react"
import * as PopoverPrimitive from "@radix-ui/react-popover"

import { cn } from "@/lib/utils"

const Popover = PopoverPrimitive.Root

const PopoverTrigger = PopoverPrimitive.Trigger

const PopoverAnchor = PopoverPrimitive.Anchor

const PopoverContent = React.forwardRef<
  React.ElementRef<typeof PopoverPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof PopoverPrimitive.Content>
>(({ className, align = "center", sideOffset = 4, ...props }, ref) => (
  <PopoverPrimitive.Portal>
    <PopoverPrimitive.Content
      ref={ref}
      align={align}
      sideOffset={sideOffset}
      className={cn(
        "z-50 w-72 rounded-md border bg-popover p-4 text-popover-foreground shadow-md outline-none data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props}
    />
  </PopoverPrimitive.Portal>
))
PopoverContent.displayName = PopoverPrimitive.Content.displayName

export { Popover, PopoverTrigger, PopoverContent, PopoverAnchor }
```

## File: src/components/ui/progress.tsx
```typescript
"use client"

import * as React from "react"
import * as ProgressPrimitive from "@radix-ui/react-progress"

import { cn } from "@/lib/utils"

const Progress = React.forwardRef<
  React.ElementRef<typeof ProgressPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof ProgressPrimitive.Root>
>(({ className, value, ...props }, ref) => (
  <ProgressPrimitive.Root
    ref={ref}
    className={cn(
      "relative h-4 w-full overflow-hidden rounded-full bg-secondary",
      className
    )}
    {...props}
  >
    <ProgressPrimitive.Indicator
      className="h-full w-full flex-1 bg-primary transition-all"
      style={{ transform: `translateX(-${100 - (value || 0)}%)` }}
    />
  </ProgressPrimitive.Root>
))
Progress.displayName = ProgressPrimitive.Root.displayName

export { Progress }
```

## File: src/components/ui/radio-group.tsx
```typescript
"use client"

import * as React from "react"
import * as RadioGroupPrimitive from "@radix-ui/react-radio-group"
import { Circle } from "lucide-react"

import { cn } from "@/lib/utils"

const RadioGroup = React.forwardRef<
  React.ElementRef<typeof RadioGroupPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof RadioGroupPrimitive.Root>
>(({ className, ...props }, ref) => {
  return (
    <RadioGroupPrimitive.Root
      className={cn("grid gap-2", className)}
      {...props}
      ref={ref}
    />
  )
})
RadioGroup.displayName = RadioGroupPrimitive.Root.displayName

const RadioGroupItem = React.forwardRef<
  React.ElementRef<typeof RadioGroupPrimitive.Item>,
  React.ComponentPropsWithoutRef<typeof RadioGroupPrimitive.Item>
>(({ className, ...props }, ref) => {
  return (
    <RadioGroupPrimitive.Item
      ref={ref}
      className={cn(
        "aspect-square h-4 w-4 rounded-full border border-primary text-primary shadow focus:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50",
        className
      )}
      {...props}
    >
      <RadioGroupPrimitive.Indicator className="flex items-center justify-center">
        <Circle className="h-3.5 w-3.5 fill-primary" />
      </RadioGroupPrimitive.Indicator>
    </RadioGroupPrimitive.Item>
  )
})
RadioGroupItem.displayName = RadioGroupPrimitive.Item.displayName

export { RadioGroup, RadioGroupItem }
```

## File: src/components/ui/scroll-area.tsx
```typescript
"use client"

import * as React from "react"
import * as ScrollAreaPrimitive from "@radix-ui/react-scroll-area"

import { cn } from "@/lib/utils"

const ScrollArea = React.forwardRef<
  React.ElementRef<typeof ScrollAreaPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof ScrollAreaPrimitive.Root>
>(({ className, children, ...props }, ref) => (
  <ScrollAreaPrimitive.Root
    ref={ref}
    className={cn("relative overflow-hidden", className)}
    {...props}
  >
    <ScrollAreaPrimitive.Viewport className="h-full w-full rounded-[inherit]">
      {children}
    </ScrollAreaPrimitive.Viewport>
    <ScrollBar />
    <ScrollAreaPrimitive.Corner />
  </ScrollAreaPrimitive.Root>
))
ScrollArea.displayName = ScrollAreaPrimitive.Root.displayName

const ScrollBar = React.forwardRef<
  React.ElementRef<typeof ScrollAreaPrimitive.ScrollAreaScrollbar>,
  React.ComponentPropsWithoutRef<typeof ScrollAreaPrimitive.ScrollAreaScrollbar>
>(({ className, orientation = "vertical", ...props }, ref) => (
  <ScrollAreaPrimitive.ScrollAreaScrollbar
    ref={ref}
    orientation={orientation}
    className={cn(
      "flex touch-none select-none transition-colors",
      orientation === "vertical" &&
        "h-full w-2.5 border-l border-l-transparent p-[1px]",
      orientation === "horizontal" &&
        "h-2.5 flex-col border-t border-t-transparent p-[1px]",
      className
    )}
    {...props}
  >
    <ScrollAreaPrimitive.ScrollAreaThumb className="relative flex-1 rounded-full bg-border" />
  </ScrollAreaPrimitive.ScrollAreaScrollbar>
))
ScrollBar.displayName = ScrollAreaPrimitive.ScrollAreaScrollbar.displayName

export { ScrollArea, ScrollBar }
```

## File: src/components/ui/select.tsx
```typescript
"use client"

import * as React from "react"
import * as SelectPrimitive from "@radix-ui/react-select"
import { Check, ChevronDown, ChevronUp } from "lucide-react"

import { cn } from "@/lib/utils"

const Select = SelectPrimitive.Root

const SelectGroup = SelectPrimitive.Group

const SelectValue = SelectPrimitive.Value

const SelectTrigger = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Trigger>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Trigger>
>(({ className, children, ...props }, ref) => (
  <SelectPrimitive.Trigger
    ref={ref}
    className={cn(
      "flex h-9 w-full items-center justify-between whitespace-nowrap rounded-md border border-input bg-transparent px-3 py-2 text-sm shadow-sm ring-offset-background placeholder:text-muted-foreground focus:outline-none focus:ring-1 focus:ring-ring disabled:cursor-not-allowed disabled:opacity-50 [&>span]:line-clamp-1",
      className
    )}
    {...props}
  >
    {children}
    <SelectPrimitive.Icon asChild>
      <ChevronDown className="h-4 w-4 opacity-50" />
    </SelectPrimitive.Icon>
  </SelectPrimitive.Trigger>
))
SelectTrigger.displayName = SelectPrimitive.Trigger.displayName

const SelectScrollUpButton = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.ScrollUpButton>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.ScrollUpButton>
>(({ className, ...props }, ref) => (
  <SelectPrimitive.ScrollUpButton
    ref={ref}
    className={cn(
      "flex cursor-default items-center justify-center py-1",
      className
    )}
    {...props}
  >
    <ChevronUp className="h-4 w-4" />
  </SelectPrimitive.ScrollUpButton>
))
SelectScrollUpButton.displayName = SelectPrimitive.ScrollUpButton.displayName

const SelectScrollDownButton = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.ScrollDownButton>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.ScrollDownButton>
>(({ className, ...props }, ref) => (
  <SelectPrimitive.ScrollDownButton
    ref={ref}
    className={cn(
      "flex cursor-default items-center justify-center py-1",
      className
    )}
    {...props}
  >
    <ChevronDown className="h-4 w-4" />
  </SelectPrimitive.ScrollDownButton>
))
SelectScrollDownButton.displayName =
  SelectPrimitive.ScrollDownButton.displayName

const SelectContent = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Content>
>(({ className, children, position = "popper", ...props }, ref) => (
  <SelectPrimitive.Portal>
    <SelectPrimitive.Content
      ref={ref}
      className={cn(
        "relative z-50 max-h-96 min-w-[8rem] overflow-hidden rounded-md border bg-popover text-popover-foreground shadow-md data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        position === "popper" &&
          "data-[side=bottom]:translate-y-1 data-[side=left]:-translate-x-1 data-[side=right]:translate-x-1 data-[side=top]:-translate-y-1",
        className
      )}
      position={position}
      {...props}
    >
      <SelectScrollUpButton />
      <SelectPrimitive.Viewport
        className={cn(
          "p-1",
          position === "popper" &&
            "h-[var(--radix-select-trigger-height)] w-full min-w-[var(--radix-select-trigger-width)]"
        )}
      >
        {children}
      </SelectPrimitive.Viewport>
      <SelectScrollDownButton />
    </SelectPrimitive.Content>
  </SelectPrimitive.Portal>
))
SelectContent.displayName = SelectPrimitive.Content.displayName

const SelectLabel = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Label>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Label>
>(({ className, ...props }, ref) => (
  <SelectPrimitive.Label
    ref={ref}
    className={cn("px-2 py-1.5 text-sm font-semibold", className)}
    {...props}
  />
))
SelectLabel.displayName = SelectPrimitive.Label.displayName

const SelectItem = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Item>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Item>
>(({ className, children, ...props }, ref) => (
  <SelectPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex w-full cursor-default select-none items-center rounded-sm py-1.5 pl-2 pr-8 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    {...props}
  >
    <span className="absolute right-2 flex h-3.5 w-3.5 items-center justify-center">
      <SelectPrimitive.ItemIndicator>
        <Check className="h-4 w-4" />
      </SelectPrimitive.ItemIndicator>
    </span>
    <SelectPrimitive.ItemText>{children}</SelectPrimitive.ItemText>
  </SelectPrimitive.Item>
))
SelectItem.displayName = SelectPrimitive.Item.displayName

const SelectSeparator = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Separator>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Separator>
>(({ className, ...props }, ref) => (
  <SelectPrimitive.Separator
    ref={ref}
    className={cn("-mx-1 my-1 h-px bg-muted", className)}
    {...props}
  />
))
SelectSeparator.displayName = SelectPrimitive.Separator.displayName

export {
  Select,
  SelectGroup,
  SelectValue,
  SelectTrigger,
  SelectContent,
  SelectLabel,
  SelectItem,
  SelectSeparator,
  SelectScrollUpButton,
  SelectScrollDownButton,
}
```

## File: src/components/ui/skeleton.tsx
```typescript
import React from 'react';
import { cn } from "@/lib/utils";

export interface SkeletonProps extends React.HTMLAttributes<HTMLDivElement> {
  variant?: 'default' | 'text' | 'circular' | 'rectangular';
  size?: 'sm' | 'default' | 'lg' | 'xl';
  width?: string | number;
  height?: string | number;
  lines?: number;
  showAnimation?: boolean;
}

export const Skeleton: React.FC<SkeletonProps> = ({
  className,
  variant = 'default',
  size = 'default',
  width,
  height,
  lines = 1,
  showAnimation = true,
  ...props
}) => {
  const sizeClasses = {
    sm: 'h-4',
    default: 'h-6',
    lg: 'h-8',
    xl: 'h-12',
  };

  const variantClasses = {
    default: 'rounded-md',
    text: 'rounded',
    circular: 'rounded-full',
    rectangular: 'rounded-none',
  };

  const animationClass = showAnimation ? 'animate-pulse' : '';

  const style: React.CSSProperties = {
    width: width,
    height: height,
  };

  if (lines > 1) {
    return (
      <div className="space-y-2" role="status" aria-label="Loading content">
        {Array.from({ length: lines }).map((_, index) => (
          <div
            key={index}
            className={cn(
              'bg-muted',
              variantClasses[variant],
              animationClass,
              sizeClasses[size],
              className
            )}
            style={index === lines - 1 ? { width: '60%' } : undefined}
            {...props}
          />
        ))}
      </div>
    );
  }

  return (
    <div
      className={cn(
        'bg-muted',
        variantClasses[variant],
        animationClass,
        sizeClasses[size],
        className
      )}
      style={style}
      role="status"
      aria-label="Loading content"
      {...props}
    />
  );
};
```

## File: src/components/ui/table.tsx
```typescript
import * as React from "react"

import { cn } from "@/lib/utils"

const Table = React.forwardRef<
  HTMLTableElement,
  React.HTMLAttributes<HTMLTableElement>
>(({ className, ...props }, ref) => (
  <div className="relative w-full overflow-auto">
    <table
      ref={ref}
      className={cn("w-full caption-bottom text-sm", className)}
      {...props}
    />
  </div>
))
Table.displayName = "Table"

const TableHeader = React.forwardRef<
  HTMLTableSectionElement,
  React.HTMLAttributes<HTMLTableSectionElement>
>(({ className, ...props }, ref) => (
  <thead ref={ref} className={cn("[&_tr]:border-b", className)} {...props} />
))
TableHeader.displayName = "TableHeader"

const TableBody = React.forwardRef<
  HTMLTableSectionElement,
  React.HTMLAttributes<HTMLTableSectionElement>
>(({ className, ...props }, ref) => (
  <tbody
    ref={ref}
    className={cn("[&_tr:last-child]:border-0", className)}
    {...props}
  />
))
TableBody.displayName = "TableBody"

const TableFooter = React.forwardRef<
  HTMLTableSectionElement,
  React.HTMLAttributes<HTMLTableSectionElement>
>(({ className, ...props }, ref) => (
  <tfoot
    ref={ref}
    className={cn(
      "border-t bg-muted/50 font-medium [&>tr]:last:border-b-0",
      className
    )}
    {...props}
  />
))
TableFooter.displayName = "TableFooter"

const TableRow = React.forwardRef<
  HTMLTableRowElement,
  React.HTMLAttributes<HTMLTableRowElement>
>(({ className, ...props }, ref) => (
  <tr
    ref={ref}
    className={cn(
      "border-b transition-colors hover:bg-muted/50 data-[state=selected]:bg-muted",
      className
    )}
    {...props}
  />
))
TableRow.displayName = "TableRow"

const TableHead = React.forwardRef<
  HTMLTableCellElement,
  React.ThHTMLAttributes<HTMLTableCellElement>
>(({ className, ...props }, ref) => (
  <th
    ref={ref}
    className={cn(
      "h-10 px-2 text-left align-middle font-medium text-muted-foreground [&:has([role=checkbox])]:pr-0 [&>[role=checkbox]]:translate-y-[2px]",
      className
    )}
    {...props}
  />
))
TableHead.displayName = "TableHead"

const TableCell = React.forwardRef<
  HTMLTableCellElement,
  React.TdHTMLAttributes<HTMLTableCellElement>
>(({ className, ...props }, ref) => (
  <td
    ref={ref}
    className={cn(
      "p-2 align-middle [&:has([role=checkbox])]:pr-0 [&>[role=checkbox]]:translate-y-[2px]",
      className
    )}
    {...props}
  />
))
TableCell.displayName = "TableCell"

const TableCaption = React.forwardRef<
  HTMLTableCaptionElement,
  React.HTMLAttributes<HTMLTableCaptionElement>
>(({ className, ...props }, ref) => (
  <caption
    ref={ref}
    className={cn("mt-4 text-sm text-muted-foreground", className)}
    {...props}
  />
))
TableCaption.displayName = "TableCaption"

export {
  Table,
  TableHeader,
  TableBody,
  TableFooter,
  TableHead,
  TableRow,
  TableCell,
  TableCaption,
}
```

## File: src/components/ui/tabs.tsx
```typescript
"use client"

import * as React from "react"
import * as TabsPrimitive from "@radix-ui/react-tabs"

import { cn } from "@/lib/utils"

const Tabs = TabsPrimitive.Root

const TabsList = React.forwardRef<
  React.ElementRef<typeof TabsPrimitive.List>,
  React.ComponentPropsWithoutRef<typeof TabsPrimitive.List>
>(({ className, ...props }, ref) => (
  <TabsPrimitive.List
    ref={ref}
    className={cn(
      "inline-flex h-9 items-center justify-center rounded-lg bg-muted p-1 text-muted-foreground",
      className
    )}
    {...props}
  />
))
TabsList.displayName = TabsPrimitive.List.displayName

const TabsTrigger = React.forwardRef<
  React.ElementRef<typeof TabsPrimitive.Trigger>,
  React.ComponentPropsWithoutRef<typeof TabsPrimitive.Trigger>
>(({ className, ...props }, ref) => (
  <TabsPrimitive.Trigger
    ref={ref}
    className={cn(
      "inline-flex items-center justify-center whitespace-nowrap rounded-md px-3 py-1 text-sm font-medium ring-offset-background transition-all focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 data-[state=active]:bg-background data-[state=active]:text-foreground data-[state=active]:shadow",
      className
    )}
    {...props}
  />
))
TabsTrigger.displayName = TabsPrimitive.Trigger.displayName

const TabsContent = React.forwardRef<
  React.ElementRef<typeof TabsPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof TabsPrimitive.Content>
>(({ className, ...props }, ref) => (
  <TabsPrimitive.Content
    ref={ref}
    className={cn(
      "mt-2 ring-offset-background focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2",
      className
    )}
    {...props}
  />
))
TabsContent.displayName = TabsPrimitive.Content.displayName

export { Tabs, TabsList, TabsTrigger, TabsContent }
```

## File: src/components/ui/textarea.tsx
```typescript
import * as React from "react"

import { cn } from "@/lib/utils"

const Textarea = React.forwardRef<
  HTMLTextAreaElement,
  React.ComponentProps<"textarea">
>(({ className, ...props }, ref) => {
  return (
    <textarea
      className={cn(
        "flex min-h-[60px] w-full rounded-md border border-input bg-transparent px-3 py-2 text-base shadow-sm placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 md:text-sm",
        className
      )}
      ref={ref}
      {...props}
    />
  )
})
Textarea.displayName = "Textarea"

export { Textarea }
```

## File: src/components/ui/toast.tsx
```typescript
"use client"

import * as React from "react"
import * as ToastPrimitives from "@radix-ui/react-toast"
import { cva, type VariantProps } from "class-variance-authority"
import { X } from "lucide-react"

import { cn } from "@/lib/utils"

const ToastProvider = ToastPrimitives.Provider

const ToastViewport = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Viewport>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Viewport>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Viewport
    ref={ref}
    className={cn(
      "fixed top-0 z-[100] flex max-h-screen w-full flex-col-reverse p-4 sm:bottom-0 sm:right-0 sm:top-auto sm:flex-col md:max-w-[420px]",
      className
    )}
    {...props}
  />
))
ToastViewport.displayName = ToastPrimitives.Viewport.displayName

const toastVariants = cva(
  "group pointer-events-auto relative flex w-full items-center justify-between space-x-2 overflow-hidden rounded-md border p-4 pr-6 shadow-lg transition-all data-[swipe=cancel]:translate-x-0 data-[swipe=end]:translate-x-[var(--radix-toast-swipe-end-x)] data-[swipe=move]:translate-x-[var(--radix-toast-swipe-move-x)] data-[swipe=move]:transition-none data-[state=open]:animate-in data-[state=closed]:animate-out data-[swipe=end]:animate-out data-[state=closed]:fade-out-80 data-[state=closed]:slide-out-to-right-full data-[state=open]:slide-in-from-top-full data-[state=open]:sm:slide-in-from-bottom-full",
  {
    variants: {
      variant: {
        default: "border bg-background text-foreground",
        destructive:
          "destructive group border-destructive bg-destructive text-destructive-foreground",
      },
    },
    defaultVariants: {
      variant: "default",
    },
  }
)

const Toast = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Root>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Root> &
    VariantProps<typeof toastVariants>
>(({ className, variant, ...props }, ref) => {
  return (
    <ToastPrimitives.Root
      ref={ref}
      className={cn(toastVariants({ variant }), className)}
      {...props}
    />
  )
})
Toast.displayName = ToastPrimitives.Root.displayName

const ToastAction = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Action>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Action>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Action
    ref={ref}
    className={cn(
      "inline-flex h-8 shrink-0 items-center justify-center rounded-md border bg-transparent px-3 text-sm font-medium transition-colors hover:bg-secondary focus:outline-none focus:ring-1 focus:ring-ring disabled:pointer-events-none disabled:opacity-50 group-[.destructive]:border-muted/40 group-[.destructive]:hover:border-destructive/30 group-[.destructive]:hover:bg-destructive group-[.destructive]:hover:text-destructive-foreground group-[.destructive]:focus:ring-destructive",
      className
    )}
    {...props}
  />
))
ToastAction.displayName = ToastPrimitives.Action.displayName

const ToastClose = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Close>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Close>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Close
    ref={ref}
    className={cn(
      "absolute right-1 top-1 rounded-md p-1 text-foreground/50 opacity-0 transition-opacity hover:text-foreground focus:opacity-100 focus:outline-none focus:ring-1 group-hover:opacity-100 group-[.destructive]:text-red-300 group-[.destructive]:hover:text-red-50 group-[.destructive]:focus:ring-red-400 group-[.destructive]:focus:ring-offset-red-600",
      className
    )}
    toast-close=""
    {...props}
  >
    <X className="h-4 w-4" />
  </ToastPrimitives.Close>
))
ToastClose.displayName = ToastPrimitives.Close.displayName

const ToastTitle = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Title>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Title>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Title
    ref={ref}
    className={cn("text-sm font-semibold [&+div]:text-xs", className)}
    {...props}
  />
))
ToastTitle.displayName = ToastPrimitives.Title.displayName

const ToastDescription = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Description>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Description>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Description
    ref={ref}
    className={cn("text-sm opacity-90", className)}
    {...props}
  />
))
ToastDescription.displayName = ToastPrimitives.Description.displayName

type ToastProps = React.ComponentPropsWithoutRef<typeof Toast>

type ToastActionElement = React.ReactElement<typeof ToastAction>

export {
  type ToastProps,
  type ToastActionElement,
  ToastProvider,
  ToastViewport,
  Toast,
  ToastTitle,
  ToastDescription,
  ToastClose,
  ToastAction,
}
```

## File: src/components/ui/toaster.tsx
```typescript
"use client"

import { useToast } from "@/hooks/use-toast"
import {
  Toast,
  ToastClose,
  ToastDescription,
  ToastProvider,
  ToastTitle,
  ToastViewport,
} from "@/components/ui/toast"

export function Toaster() {
  const { toasts } = useToast()

  return (
    <ToastProvider>
      {toasts.map(function ({ id, title, description, action, ...props }) {
        return (
          <Toast key={id} {...props}>
            <div className="grid gap-1">
              {title && <ToastTitle>{title}</ToastTitle>}
              {description && (
                <ToastDescription>{description}</ToastDescription>
              )}
            </div>
            {action}
            <ToastClose />
          </Toast>
        )
      })}
      <ToastViewport />
    </ToastProvider>
  )
}
```

## File: src/hooks/index.ts
```typescript
// Custom hooks exports
export * from './useAuth';
export * from './useApi';
export * from './useResumeAnalysis';
export * from './useLocalStorage';
export * from './useToast';
export * from './useForm';
export * from './use-toast';
```

## File: src/hooks/use-toast.ts
```typescript
"use client"

// Inspired by react-hot-toast library
import * as React from "react"

import type {
  ToastActionElement,
  ToastProps,
} from "@/components/ui/toast"

const TOAST_LIMIT = 1
const TOAST_REMOVE_DELAY = 1000000

type ToasterToast = ToastProps & {
  id: string
  title?: React.ReactNode
  description?: React.ReactNode
  action?: ToastActionElement
}

const actionTypes = {
  ADD_TOAST: "ADD_TOAST",
  UPDATE_TOAST: "UPDATE_TOAST",
  DISMISS_TOAST: "DISMISS_TOAST",
  REMOVE_TOAST: "REMOVE_TOAST",
} as const

let count = 0

function genId() {
  count = (count + 1) % Number.MAX_SAFE_INTEGER
  return count.toString()
}

type ActionType = typeof actionTypes

type Action =
  | {
      type: ActionType["ADD_TOAST"]
      toast: ToasterToast
    }
  | {
      type: ActionType["UPDATE_TOAST"]
      toast: Partial<ToasterToast>
    }
  | {
      type: ActionType["DISMISS_TOAST"]
      toastId?: ToasterToast["id"]
    }
  | {
      type: ActionType["REMOVE_TOAST"]
      toastId?: ToasterToast["id"]
    }

interface State {
  toasts: ToasterToast[]
}

const toastTimeouts = new Map<string, ReturnType<typeof setTimeout>>()

const addToRemoveQueue = (toastId: string) => {
  if (toastTimeouts.has(toastId)) {
    return
  }

  const timeout = setTimeout(() => {
    toastTimeouts.delete(toastId)
    dispatch({
      type: "REMOVE_TOAST",
      toastId: toastId,
    })
  }, TOAST_REMOVE_DELAY)

  toastTimeouts.set(toastId, timeout)
}

export const reducer = (state: State, action: Action): State => {
  switch (action.type) {
    case "ADD_TOAST":
      return {
        ...state,
        toasts: [action.toast, ...state.toasts].slice(0, TOAST_LIMIT),
      }

    case "UPDATE_TOAST":
      return {
        ...state,
        toasts: state.toasts.map((t) =>
          t.id === action.toast.id ? { ...t, ...action.toast } : t
        ),
      }

    case "DISMISS_TOAST": {
      const { toastId } = action

      // ! Side effects ! - This could be extracted into a dismissToast() action,
      // but I'll keep it here for simplicity
      if (toastId) {
        addToRemoveQueue(toastId)
      } else {
        state.toasts.forEach((toast) => {
          addToRemoveQueue(toast.id)
        })
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
      }
    }
    case "REMOVE_TOAST":
      if (action.toastId === undefined) {
        return {
          ...state,
          toasts: [],
        }
      }
      return {
        ...state,
        toasts: state.toasts.filter((t) => t.id !== action.toastId),
      }
  }
}

const listeners: Array<(state: State) => void> = []

let memoryState: State = { toasts: [] }

function dispatch(action: Action) {
  memoryState = reducer(memoryState, action)
  listeners.forEach((listener) => {
    listener(memoryState)
  })
}

type Toast = Omit<ToasterToast, "id">

function toast({ ...props }: Toast) {
  const id = genId()

  const update = (props: ToasterToast) =>
    dispatch({
      type: "UPDATE_TOAST",
      toast: { ...props, id },
    })
  const dismiss = () => dispatch({ type: "DISMISS_TOAST", toastId: id })

  dispatch({
    type: "ADD_TOAST",
    toast: {
      ...props,
      id,
      open: true,
      onOpenChange: (open) => {
        if (!open) dismiss()
      },
    },
  })

  return {
    id: id,
    dismiss,
    update,
  }
}

function useToast() {
  const [state, setState] = React.useState<State>(memoryState)

  React.useEffect(() => {
    listeners.push(setState)
    return () => {
      const index = listeners.indexOf(setState)
      if (index > -1) {
        listeners.splice(index, 1)
      }
    }
  }, [state])

  return {
    ...state,
    toast,
    dismiss: (toastId?: string) => dispatch({ type: "DISMISS_TOAST", toastId }),
  }
}

export { useToast, toast }
```

## File: src/hooks/useApi.ts
```typescript
import { useState, useCallback } from 'react'
import { ApiResponse, ApiError } from '@/types/api'

interface UseApiOptions<T> {
  onSuccess?: (data: T) => void
  onError?: (error: ApiError) => void
  immediate?: boolean
}

export const useApi = <T>(endpoint: string, options: UseApiOptions<T> = {}) => {
  const [data, setData] = useState<T | null>(null)
  const [loading, setLoading] = useState(false)
  const [error, setError] = useState<ApiError | null>(null)

  const fetchData = useCallback(async () => {
    setLoading(true)
    setError(null)
    
    try {
      const token = localStorage.getItem('token')
      const headers: Record<string, string> = {
        'Content-Type': 'application/json'
      }
      
      if (token) {
        headers['Authorization'] = `Bearer ${token}`
      }

      const response = await fetch(endpoint, { headers })
      const result: ApiResponse<T> = await response.json()

      if (response.ok && result.success) {
        setData(result.data!)
        options.onSuccess?.(result.data!)
      } else {
        const apiError: ApiError = {
          message: result.error || result.message || 'Request failed',
          status: response.status
        }
        setError(apiError)
        options.onError?.(apiError)
      }
    } catch (err) {
      const apiError: ApiError = {
        message: 'Network error',
        status: 0
      }
      setError(apiError)
      options.onError?.(apiError)
    } finally {
      setLoading(false)
    }
  }, [endpoint, options])

  const postData = useCallback(async (body: any) => {
    setLoading(true)
    setError(null)
    
    try {
      const token = localStorage.getItem('token')
      const headers: Record<string, string> = {
        'Content-Type': 'application/json'
      }
      
      if (token) {
        headers['Authorization'] = `Bearer ${token}`
      }

      const response = await fetch(endpoint, {
        method: 'POST',
        headers,
        body: JSON.stringify(body)
      })

      const result: ApiResponse<T> = await response.json()

      if (response.ok && result.success) {
        setData(result.data!)
        options.onSuccess?.(result.data!)
      } else {
        const apiError: ApiError = {
          message: result.error || result.message || 'Request failed',
          status: response.status
        }
        setError(apiError)
        options.onError?.(apiError)
      }
    } catch (err) {
      const apiError: ApiError = {
        message: 'Network error',
        status: 0
      }
      setError(apiError)
      options.onError?.(apiError)
    } finally {
      setLoading(false)
    }
  }, [endpoint, options])

  return {
    data,
    loading,
    error,
    fetchData,
    postData,
    refetch: fetchData
  }
}
```

## File: src/hooks/useAuth.ts
```typescript
import { useState, useEffect, useCallback } from 'react'
import { User, LoginCredentials, RegisterCredentials } from '@/types/auth'

export const useAuth = () => {
  const [user, setUser] = useState<User | null>(null)
  const [isAuthenticated, setIsAuthenticated] = useState(false)
  const [isLoading, setIsLoading] = useState(true)
  const [error, setError] = useState<string | null>(null)

  // Check if user is authenticated on mount
  useEffect(() => {
    const checkAuth = async () => {
      try {
        const token = localStorage.getItem('token')
        if (token) {
          // Verify token with backend
          const response = await fetch('/api/auth/verify', {
            headers: {
              'Authorization': `Bearer ${token}`
            }
          })
          
          if (response.ok) {
            const userData = await response.json()
            setUser(userData.user)
            setIsAuthenticated(true)
          } else {
            localStorage.removeItem('token')
          }
        }
      } catch (err) {
        console.error('Auth check failed:', err)
      } finally {
        setIsLoading(false)
      }
    }

    checkAuth()
  }, [])

  const login = useCallback(async (credentials: LoginCredentials) => {
    setIsLoading(true)
    setError(null)
    
    try {
      const response = await fetch('/api/auth/login', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(credentials)
      })

      const data = await response.json()

      if (response.ok) {
        localStorage.setItem('token', data.token)
        setUser(data.user)
        setIsAuthenticated(true)
      } else {
        setError(data.message || 'Login failed')
      }
    } catch (err) {
      setError('Network error')
    } finally {
      setIsLoading(false)
    }
  }, [])

  const register = useCallback(async (credentials: RegisterCredentials) => {
    setIsLoading(true)
    setError(null)
    
    try {
      const response = await fetch('/api/auth/register', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(credentials)
      })

      const data = await response.json()

      if (response.ok) {
        localStorage.setItem('token', data.token)
        setUser(data.user)
        setIsAuthenticated(true)
      } else {
        setError(data.message || 'Registration failed')
      }
    } catch (err) {
      setError('Network error')
    } finally {
      setIsLoading(false)
    }
  }, [])

  const logout = useCallback(() => {
    localStorage.removeItem('token')
    setUser(null)
    setIsAuthenticated(false)
    setError(null)
  }, [])

  const clearError = useCallback(() => {
    setError(null)
  }, [])

  return {
    user,
    isAuthenticated,
    isLoading,
    error,
    login,
    register,
    logout,
    clearError
  }
}
```

## File: src/hooks/useForm.ts
```typescript
import { useState, useCallback } from 'react'
import { FormState, FormValidationRule } from '@/types/forms'

export function useForm<T extends Record<string, any>>(initialValues: T, validationRules?: Record<keyof T, FormValidationRule>) {
  const [state, setState] = useState<FormState<T>>({
    values: initialValues,
    errors: {},
    touched: {},
    isSubmitting: false,
    isValid: true
  })

  const validateField = useCallback((name: keyof T, value: any): string | undefined => {
    if (!validationRules || !validationRules[name]) return undefined

    const rule = validationRules[name]
    
    if (rule.required && !value) {
      return `${String(name)} is required`
    }
    
    if (rule.minLength && value && value.length < rule.minLength) {
      return `${String(name)} must be at least ${rule.minLength} characters`
    }
    
    if (rule.maxLength && value && value.length > rule.maxLength) {
      return `${String(name)} must be no more than ${rule.maxLength} characters`
    }
    
    if (rule.pattern && value && !rule.pattern.test(value)) {
      return `${String(name)} format is invalid`
    }
    
    if (rule.custom) {
      return rule.custom(value)
    }
    
    return undefined
  }, [validationRules])

  const setFieldValue = useCallback((name: keyof T, value: any) => {
    setState(prev => {
      const newValues = { ...prev.values, [name]: value }
      const error = validateField(name, value)
      const newErrors = { ...prev.errors }
      
      if (error) {
        newErrors[name] = error
      } else {
        delete newErrors[name]
      }
      
      return {
        ...prev,
        values: newValues,
        errors: newErrors,
        touched: { ...prev.touched, [name]: true },
        isValid: Object.keys(newErrors).length === 0
      }
    })
  }, [validateField])

  const setFieldTouched = useCallback((name: keyof T, touched: boolean = true) => {
    setState(prev => ({
      ...prev,
      touched: { ...prev.touched, [name]: touched }
    }))
  }, [])

  const validateForm = useCallback((): boolean => {
    const errors: Partial<Record<keyof T, string>> = {}
    
    Object.keys(state.values).forEach(key => {
      const fieldKey = key as keyof T
      const error = validateField(fieldKey, state.values[fieldKey])
      if (error) {
        errors[fieldKey] = error
      }
    })
    
    setState(prev => ({
      ...prev,
      errors,
      isValid: Object.keys(errors).length === 0
    }))
    
    return Object.keys(errors).length === 0
  }, [state.values, validateField])

  const resetForm = useCallback(() => {
    setState({
      values: initialValues,
      errors: {},
      touched: {},
      isSubmitting: false,
      isValid: true
    })
  }, [initialValues])

  const setSubmitting = useCallback((isSubmitting: boolean) => {
    setState(prev => ({ ...prev, isSubmitting }))
  }, [])

  return {
    values: state.values,
    errors: state.errors,
    touched: state.touched,
    isSubmitting: state.isSubmitting,
    isValid: state.isValid,
    setFieldValue,
    setFieldTouched,
    validateForm,
    resetForm,
    setSubmitting
  }
}
```

## File: src/hooks/useLocalStorage.ts
```typescript
import { useState, useEffect } from 'react'

export function useLocalStorage<T>(key: string, initialValue: T) {
  // Get from local storage then parse stored json or return initialValue
  const [storedValue, setStoredValue] = useState<T>(() => {
    if (typeof window === 'undefined') {
      return initialValue
    }
    try {
      const item = window.localStorage.getItem(key)
      return item ? JSON.parse(item) : initialValue
    } catch (error) {
      console.log(error)
      return initialValue
    }
  })

  // Return a wrapped version of useState's setter function that persists the new value to localStorage
  const setValue = (value: T | ((val: T) => T)) => {
    try {
      // Allow value to be a function so we have the same API as useState
      const valueToStore = value instanceof Function ? value(storedValue) : value
      setStoredValue(valueToStore)
      if (typeof window !== 'undefined') {
        window.localStorage.setItem(key, JSON.stringify(valueToStore))
      }
    } catch (error) {
      console.log(error)
    }
  }

  return [storedValue, setValue] as const
}
```

## File: src/hooks/useResumeAnalysis.ts
```typescript
import { useApi } from './useApi'
import { ResumeAnalysis } from '@/types/ai'

export const useResumeAnalysis = () => {
  const { data: analyses, loading, error, fetchData, postData } = useApi<ResumeAnalysis[]>('/api/resume/analyses')

  const uploadResume = async (file: File) => {
    const formData = new FormData()
    formData.append('resume', file)
    
    const response = await fetch('/api/resume/upload', {
      method: 'POST',
      headers: {
        'Authorization': `Bearer ${localStorage.getItem('token')}`
      },
      body: formData
    })
    
    if (response.ok) {
      await fetchData() // Refresh analyses
      return await response.json()
    } else {
      throw new Error('Upload failed')
    }
  }

  const getAnalysis = async (id: string) => {
    const response = await fetch(`/api/resume/analyses/${id}`, {
      headers: {
        'Authorization': `Bearer ${localStorage.getItem('token')}`
      }
    })
    
    if (response.ok) {
      return await response.json()
    } else {
      throw new Error('Failed to fetch analysis')
    }
  }

  return {
    analyses,
    loading,
    error,
    uploadResume,
    getAnalysis,
    refetch: fetchData
  }
}
```

## File: src/hooks/useToast.ts
```typescript
import { useToast as useToastOriginal } from "@/hooks/use-toast"

export const useToast = useToastOriginal
```

## File: src/lib/api.ts
```typescript
import axios, { AxiosInstance, AxiosRequestConfig, AxiosResponse, AxiosError } from 'axios'
import { useAuthStore } from '@/stores/authStore'

// API Configuration
const API_BASE_URL = process.env.NEXT_PUBLIC_API_URL || 'http://localhost:3001/api'
const API_TIMEOUT = 30000 // 30 seconds

// ============================================================================
// API ENDPOINTS
// ============================================================================

export const API_ENDPOINTS = {
  // Authentication endpoints
  auth: {
    login: '/auth/login',
    register: '/auth/register',
    logout: '/auth/logout',
    refresh: '/auth/refresh',
    forgotPassword: '/auth/forgot-password',
    resetPassword: '/auth/reset-password',
    verifyEmail: '/auth/verify-email',
    resendVerification: '/auth/resend-verification',
    changePassword: '/auth/change-password',
    profile: '/auth/profile',
  },

  // User endpoints
  user: {
    profile: '/user/profile',
    settings: '/user/settings',
    preferences: '/user/preferences',
    notifications: '/user/notifications',
    avatar: '/user/avatar',
    deleteAccount: '/user/delete-account',
  },

  // Career endpoints
  career: {
    profile: '/career/profile',
    updateProfile: '/career/profile',
    skills: '/career/skills',
    experience: '/career/experience',
    education: '/career/education',
    certifications: '/career/certifications',
    languages: '/career/languages',
  },

  // Job search endpoints
  jobs: {
    search: '/jobs/search',
    details: (id: string) => `/jobs/${id}`,
    save: (id: string) => `/jobs/${id}/save`,
    unsave: (id: string) => `/jobs/${id}/unsave`,
    apply: (id: string) => `/jobs/${id}/apply`,
    recommendations: '/jobs/recommendations',
    saved: '/jobs/saved',
    applications: '/jobs/applications',
    application: (id: string) => `/jobs/applications/${id}`,
  },

  // Resume endpoints
  resume: {
    upload: '/resume/upload',
    analyze: '/resume/analyze',
    list: '/resume/list',
    details: (id: string) => `/resume/${id}`,
    delete: (id: string) => `/resume/${id}`,
    download: (id: string) => `/resume/${id}/download`,
    update: (id: string) => `/resume/${id}`,
    generate: '/resume/generate',
    templates: '/resume/templates',
  },

  // AI endpoints
  ai: {
    resumeAnalysis: '/ai/resume/analysis',
    careerRecommendations: '/ai/career/recommendations',
    jobMatching: '/ai/jobs/matching',
    skillGap: '/ai/skills/gap-analysis',
    interviewPrep: '/ai/interview/prep',
    coverLetter: '/ai/cover-letter/generate',
    profileOptimization: '/ai/profile/optimize',
  },

  // File upload endpoints
  upload: {
    resume: '/upload/resume',
    avatar: '/upload/avatar',
    document: '/upload/document',
  },

  // Health check endpoints
  health: {
    check: '/health',
    status: '/health/status',
  },

  // Analytics endpoints
  analytics: {
    dashboard: '/analytics/dashboard',
    userActivity: '/analytics/user-activity',
    jobViews: '/analytics/job-views',
    applications: '/analytics/applications',
  },
} as const

// Helper function to build full URLs
export const buildApiUrl = (endpoint: string, baseUrl?: string): string => {
  const apiBaseUrl = baseUrl || process.env.NEXT_PUBLIC_API_URL || 'http://localhost:3001'
  
  // If endpoint already starts with /api, use it as is
  if (endpoint.startsWith('/api/')) {
    return `${apiBaseUrl}${endpoint}`
  }
  
  // Otherwise, append to the base URL
  return `${apiBaseUrl}${endpoint}`
}

// Helper function to build endpoint with parameters
export const buildEndpoint = (template: string, ...params: string[]): string => {
  return params.reduce((url, param, index) => {
    return url.replace(`{${index}}`, param)
  }, template)
}

// Type-safe endpoint access
export type EndpointKey = keyof typeof API_ENDPOINTS
export type EndpointPath = string

// Endpoint validation
export const isValidEndpoint = (endpoint: string): boolean => {
  return Object.values(API_ENDPOINTS)
    .flatMap(category => Object.values(category))
    .some(path => path === endpoint || path.includes('{'))
}

// Export individual endpoint categories for easier imports
export const { auth, user, career, jobs, resume, ai, upload, health, analytics } = API_ENDPOINTS

// ============================================================================
// API TYPES
// ============================================================================

// Base API response structure
export interface APIResponse<T = any> {
  success: boolean
  data: T
  message?: string
  errors?: string[]
  timestamp: string
}

// Paginated response structure
export interface PaginatedResponse<T = any> extends APIResponse<T[]> {
  pagination: {
    page: number
    limit: number
    total: number
    totalPages: number
    hasNext: boolean
    hasPrev: boolean
  }
}

// Error response structure
export interface APIErrorResponse {
  success: false
  error: {
    code: string
    message: string
    details?: any
  }
  timestamp: string
}

// Authentication types
export interface AuthResponse {
  user: {
    id: string
    email: string
    name: string
    avatar?: string
    role: 'user' | 'admin'
    emailVerified: boolean
    createdAt: string
    updatedAt: string
  }
  token: string
  refreshToken: string
  expiresIn: number
}

export interface LoginRequest {
  email: string
  password: string
}

export interface RegisterRequest {
  email: string
  password: string
  name: string
  confirmPassword: string
}

export interface ForgotPasswordRequest {
  email: string
}

export interface ResetPasswordRequest {
  token: string
  password: string
  confirmPassword: string
}

// User types
export interface UserProfileResponse {
  id: string
  userId: string
  firstName: string
  lastName: string
  avatar?: string
  bio?: string
  phone?: string
  location?: string
  website?: string
  socialLinks: {
    linkedin?: string
    github?: string
    twitter?: string
  }
  createdAt: string
  updatedAt: string
}

export interface UserPreferencesResponse {
  theme: 'light' | 'dark' | 'system'
  language: string
  timezone: string
  emailNotifications: boolean
  pushNotifications: boolean
  privacySettings: {
    profileVisibility: 'public' | 'private' | 'connections'
    showEmail: boolean
    showPhone: boolean
  }
}

// Career types
export interface CareerProfileResponse {
  id: string
  userId: string
  title: string
  summary: string
  skills: string[]
  experience: ExperienceResponse[]
  education: EducationResponse[]
  certifications: CertificationResponse[]
  languages: LanguageResponse[]
  createdAt: string
  updatedAt: string
}

export interface ExperienceResponse {
  id: string
  title: string
  company: string
  location: string
  startDate: string
  endDate?: string
  current: boolean
  description: string
}

export interface EducationResponse {
  id: string
  degree: string
  institution: string
  field: string
  startDate: string
  endDate?: string
  current: boolean
  gpa?: number
}

export interface CertificationResponse {
  id: string
  name: string
  issuer: string
  issueDate: string
  expiryDate?: string
  credentialId?: string
  url?: string
}

export interface LanguageResponse {
  id: string
  name: string
  proficiency: 'beginner' | 'intermediate' | 'advanced' | 'native'
}

// Job search types
export interface JobSearchRequest {
  query?: string
  location?: string
  type?: 'full-time' | 'part-time' | 'contract' | 'internship'
  remote?: boolean
  experience?: 'entry' | 'mid' | 'senior' | 'executive'
  salary?: {
    min?: number
    max?: number
    currency?: string
  }
  skills?: string[]
  page?: number
  limit?: number
}

export interface JobSearchResponse {
  id: string
  title: string
  company: string
  location: string
  description: string
  requirements: string[]
  salary?: {
    min: number
    max: number
    currency: string
  }
  type: 'full-time' | 'part-time' | 'contract' | 'internship'
  remote: boolean
  postedAt: string
  applicationDeadline?: string
  companyLogo?: string
  benefits?: string[]
  skills?: string[]
}

export interface JobApplicationRequest {
  jobId: string
  coverLetter?: string
  resumeId?: string
  additionalInfo?: string
}

export interface JobApplicationResponse {
  id: string
  jobId: string
  userId: string
  status: 'pending' | 'reviewed' | 'interviewed' | 'accepted' | 'rejected'
  appliedAt: string
  updatedAt: string
  job: JobSearchResponse
}

// Resume types
export interface ResumeUploadRequest {
  file: File
  title?: string
  description?: string
}

export interface ResumeUploadResponse {
  id: string
  userId: string
  title: string
  description?: string
  filename: string
  fileSize: number
  fileType: string
  uploadDate: string
  isPublic: boolean
  downloadUrl: string
}

export interface ResumeAnalysisRequest {
  resumeId: string
  analysisType?: 'general' | 'skills' | 'experience' | 'education' | 'comprehensive'
  jobDescription?: string
}

export interface ResumeAnalysisResponse {
  id: string
  resumeId: string
  analysisType: string
  score: number
  feedback: {
    strengths: string[]
    weaknesses: string[]
    suggestions: string[]
  }
  skills: {
    detected: string[]
    missing: string[]
    score: number
  }
  experience: {
    years: number
    relevance: number
    suggestions: string[]
  }
  education: {
    level: string
    relevance: number
    suggestions: string[]
  }
  createdAt: string
}

// AI types
export interface AIAnalysisRequest {
  resumeId: string
  analysisType: 'general' | 'skills' | 'experience' | 'education' | 'comprehensive'
  jobDescription?: string
}

export interface CareerRecommendationsRequest {
  skills?: string[]
  experience?: number
  interests?: string[]
  location?: string
}

export interface CareerRecommendationsResponse {
  careers: {
    title: string
    description: string
    matchScore: number
    requiredSkills: string[]
    salary: {
      min: number
      max: number
      currency: string
    }
    growth: number
  }[]
}

export interface JobMatchingRequest {
  resumeId?: string
  skills?: string[]
  experience?: number
  location?: string
  limit?: number
}

export interface CoverLetterRequest {
  jobTitle: string
  companyName: string
  jobDescription: string
  resumeId?: string
  tone?: 'professional' | 'friendly' | 'enthusiastic' | 'formal'
}

export interface CoverLetterResponse {
  content: string
  suggestions: string[]
  wordCount: number
  estimatedReadTime: number
}

// File upload types
export interface FileUploadRequest {
  file: File
  type: 'resume' | 'avatar' | 'document'
  description?: string
}

export interface FileUploadResponse {
  id: string
  filename: string
  originalName: string
  fileSize: number
  fileType: string
  url: string
  uploadDate: string
}

// Notification types
export interface NotificationResponse {
  id: string
  userId: string
  type: 'info' | 'success' | 'warning' | 'error'
  title: string
  message: string
  read: boolean
  createdAt: string
  actionUrl?: string
}

// Analytics types
export interface AnalyticsResponse {
  userActivity: {
    totalLogins: number
    lastLogin: string
    totalSearches: number
    totalApplications: number
  }
  jobViews: {
    total: number
    thisWeek: number
    thisMonth: number
    topJobs: Array<{
      jobId: string
      title: string
      views: number
    }>
  }
  applications: {
    total: number
    pending: number
    reviewed: number
    interviewed: number
    accepted: number
    rejected: number
    recent: Array<{
      id: string
      jobTitle: string
      company: string
      status: string
      appliedAt: string
    }>
  }
}

// ============================================================================
// API CLIENT
// ============================================================================

// Request/Response interceptors
const requestInterceptor = (config: AxiosRequestConfig) => {
  // Add auth token if available
  const token = useAuthStore.getState().token
  if (token) {
    config.headers = {
      ...config.headers,
      Authorization: `Bearer ${token}`,
    }
  }

  // Add content type
  if (!config.headers?.['Content-Type']) {
    config.headers = {
      ...config.headers,
      'Content-Type': 'application/json',
    }
  }

  // Add request timestamp for caching
  ;(config as any).metadata = {
    startTime: new Date(),
  }

  return config
}

const responseInterceptor = (response: AxiosResponse) => {
  // Calculate request duration
  const endTime = new Date()
  const startTime = (response.config as any).metadata?.startTime
  const duration = startTime ? endTime.getTime() - startTime.getTime() : 0

  // Log successful requests in development
  if (process.env.NODE_ENV === 'development') {
    console.log(`✅ ${response.config.method?.toUpperCase()} ${response.config.url} - ${response.status} (${duration}ms)`)
  }

  return response
}

const errorInterceptor = (error: AxiosError) => {
  // Calculate request duration
  const endTime = new Date()
  const startTime = (error.config as any)?.metadata?.startTime
  const duration = startTime ? endTime.getTime() - startTime.getTime() : 0

  // Log errors in development
  if (process.env.NODE_ENV === 'development') {
    console.error(`❌ ${error.config?.method?.toUpperCase()} ${error.config?.url} - ${error.response?.status} (${duration}ms)`, error)
  }

  // Handle authentication errors
  if (error.response?.status === 401) {
    // Clear auth state and redirect to login
    useAuthStore.getState().logout()
    window.location.href = '/auth/login'
  }

  // Handle network errors
  if (!error.response) {
    console.error('Network error:', error.message)
  }

  return Promise.reject(error)
}

// Create axios instance
const apiClient: AxiosInstance = axios.create({
  baseURL: API_BASE_URL,
  timeout: API_TIMEOUT,
  headers: {
    'Content-Type': 'application/json',
  },
})

// Add interceptors
apiClient.interceptors.request.use(requestInterceptor)
apiClient.interceptors.response.use(responseInterceptor, errorInterceptor)

// Request retry logic
const retryRequest = async (
  config: AxiosRequestConfig,
  retries: number = 3,
  delay: number = 1000
): Promise<AxiosResponse> => {
  try {
    return await apiClient(config)
  } catch (error) {
    if (retries > 0 && error instanceof AxiosError && error.response?.status >= 500) {
      await new Promise(resolve => setTimeout(resolve, delay))
      return retryRequest(config, retries - 1, delay * 2)
    }
    throw error
  }
}

// Enhanced request methods with retry logic
export const api = {
  get: <T = any>(url: string, config?: AxiosRequestConfig) =>
    retryRequest({ ...config, method: 'GET', url }) as Promise<AxiosResponse<T>>,

  post: <T = any>(url: string, data?: any, config?: AxiosRequestConfig) =>
    retryRequest({ ...config, method: 'POST', url, data }) as Promise<AxiosResponse<T>>,

  put: <T = any>(url: string, data?: any, config?: AxiosRequestConfig) =>
    retryRequest({ ...config, method: 'PUT', url, data }) as Promise<AxiosResponse<T>>,

  patch: <T = any>(url: string, data?: any, config?: AxiosRequestConfig) =>
    retryRequest({ ...config, method: 'PATCH', url, data }) as Promise<AxiosResponse<T>>,

  delete: <T = any>(url: string, config?: AxiosRequestConfig) =>
    retryRequest({ ...config, method: 'DELETE', url }) as Promise<AxiosResponse<T>>,

  // File upload method
  upload: <T = any>(url: string, file: File, config?: AxiosRequestConfig) => {
    const formData = new FormData()
    formData.append('file', file)
    
    return retryRequest({
      ...config,
      method: 'POST',
      url,
      data: formData,
      headers: {
        ...config?.headers,
        'Content-Type': 'multipart/form-data',
      },
    }) as Promise<AxiosResponse<T>>
  },

  // Download method
  download: (url: string, filename?: string, config?: AxiosRequestConfig) =>
    retryRequest({
      ...config,
      method: 'GET',
      url,
      responseType: 'blob',
    }).then(response => {
      const blob = new Blob([response.data])
      const downloadUrl = window.URL.createObjectURL(blob)
      const link = document.createElement('a')
      link.href = downloadUrl
      link.download = filename || 'download'
      document.body.appendChild(link)
      link.click()
      document.body.removeChild(link)
      window.URL.revokeObjectURL(downloadUrl)
      return response
    }),
}

// Error handling utilities
export class APIError extends Error {
  constructor(
    message: string,
    public status: number,
    public code?: string,
    public data?: any
  ) {
    super(message)
    this.name = 'APIError'
  }
}

export const handleAPIError = (error: AxiosError): APIError => {
  if (error.response) {
    return new APIError(
      error.response.data?.message || error.message,
      error.response.status,
      error.response.data?.code,
      error.response.data
    )
  }
  
  return new APIError(
    error.message || 'Network error',
    0,
    'NETWORK_ERROR'
  )
}

// Export the axios instance for advanced usage
export { apiClient }

// Export types
export type { AxiosInstance, AxiosRequestConfig, AxiosResponse, AxiosError }
```

## File: src/lib/api/resumeGenerator.ts
```typescript
import axios, { AxiosResponse } from 'axios'
import { 
  GenerateResumeRequest, 
  GenerateResumeResponse, 
  UpdateResumeRequest, 
  AutoSaveRequest, 
  SearchResumesRequest,
  GeneratedResume,
  JobAnalysis,
  SkillsTranslation,
  ATSScore,
  ExportOptions,
  ExportResult,
  ApiResponse,
  PaginatedResponse,
  GenerationProgress
} from '@/types/resume-generator'
import { buildApiUrl } from '../api'

// ========================================
// API ENDPOINTS
// ========================================

const RESUME_GENERATOR_ENDPOINTS = {
  // Core resume generation
  generate: '/api/v1/resume/generate',
  
  // Generated resume management
  generated: '/api/v1/resume/generated',
  generatedById: (id: string) => `/api/v1/resume/generated/${id}`,
  updateGenerated: (id: string) => `/api/v1/resume/generated/${id}`,
  deleteGenerated: (id: string) => `/api/v1/resume/generated/${id}`,
  
  // Auto-save functionality
  autoSave: (id: string) => `/api/v1/resume/generated/${id}/auto-save`,
  
  // Download tracking
  trackDownload: (id: string) => `/api/v1/resume/generated/${id}/track-download`,
  
  // Search and statistics
  search: '/api/v1/resume/generated/search',
  statistics: '/api/v1/resume/generated/statistics',
  
  // AI analysis and translation
  analyzeJobTargeting: '/api/v1/resume/analyze-job-targeting',
  translateSkills: '/api/v1/resume/translate-skills',
  
  // Export functionality
  export: (id: string) => `/api/v1/resume/generated/${id}/export`,
  downloadPDF: (id: string) => `/api/v1/resume/generated/${id}/download-pdf`,
} as const

// ========================================
// API CONFIGURATION
// ========================================

const API_CONFIG = {
  timeout: 60000, // 60 seconds for generation
  retries: 3,
  retryDelay: 1000,
}

// ========================================
// HELPER FUNCTIONS
// ========================================

/**
 * Get authentication headers
 */
const getAuthHeaders = () => {
  try {
    const sessionStr = localStorage.getItem('session');
    const session = sessionStr ? JSON.parse(sessionStr) : null;
    const token = session?.access_token;
    return token ? { Authorization: `Bearer ${token}` } : {};
  } catch (error) {
    console.error('Error getting auth headers:', error);
    return {};
  }
}

/**
 * Handle API errors
 */
const handleApiError = (error: any): never => {
  if (error.response) {
    const { status, data } = error.response
    throw new Error(data?.message || `API Error: ${status}`)
  } else if (error.request) {
    throw new Error('Network error: Unable to connect to server')
  } else {
    throw new Error(error.message || 'Unknown error occurred')
  }
}

/**
 * Retry function for API calls
 */
const retryApiCall = async <T>(
  apiCall: () => Promise<T>,
  retries: number = API_CONFIG.retries,
  delay: number = API_CONFIG.retryDelay
): Promise<T> => {
  try {
    return await apiCall()
  } catch (error) {
    if (retries > 0 && error.message.includes('Network error')) {
      await new Promise(resolve => setTimeout(resolve, delay))
      return retryApiCall(apiCall, retries - 1, delay * 2)
    }
    throw error
  }
}

// ========================================
// CORE RESUME GENERATION API
// ========================================

/**
 * Generate a new Canadian resume using AI
 */
export const generateCanadianResume = async (
  request: GenerateResumeRequest
): Promise<GenerateResumeResponse> => {
  try {
    const response: AxiosResponse<GenerateResumeResponse> = await retryApiCall(() =>
      axios.post(
        buildApiUrl(RESUME_GENERATOR_ENDPOINTS.generate),
        request,
        {
          headers: {
            'Content-Type': 'application/json',
            ...getAuthHeaders(),
          },
          timeout: API_CONFIG.timeout,
        }
      )
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Get user's generated resumes with pagination
 */
export const getUserGeneratedResumes = async (
  page: number = 1,
  limit: number = 20,
  sortBy: string = 'createdAt',
  sortOrder: 'asc' | 'desc' = 'desc'
): Promise<PaginatedResponse<GeneratedResume>> => {
  try {
    const response: AxiosResponse<PaginatedResponse<GeneratedResume>> = await axios.get(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.generated),
      {
        headers: getAuthHeaders(),
        params: { page, limit, sortBy, sortOrder },
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Get a specific generated resume by ID
 */
export const getGeneratedResumeById = async (
  resumeId: string
): Promise<ApiResponse<GeneratedResume>> => {
  try {
    const response: AxiosResponse<ApiResponse<GeneratedResume>> = await axios.get(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.generatedById(resumeId)),
      {
        headers: getAuthHeaders(),
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Update a generated resume
 */
export const updateGeneratedResume = async (
  request: UpdateResumeRequest
): Promise<ApiResponse<GeneratedResume>> => {
  try {
    const response: AxiosResponse<ApiResponse<GeneratedResume>> = await axios.put(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.updateGenerated(request.resumeId)),
      request.updates,
      {
        headers: {
          'Content-Type': 'application/json',
          ...getAuthHeaders(),
        },
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Delete a generated resume
 */
export const deleteGeneratedResume = async (
  resumeId: string
): Promise<ApiResponse<void>> => {
  try {
    const response: AxiosResponse<ApiResponse<void>> = await axios.delete(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.deleteGenerated(resumeId)),
      {
        headers: getAuthHeaders(),
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// AUTO-SAVE FUNCTIONALITY
// ========================================

/**
 * Auto-save user edits to a resume
 */
export const autoSaveUserEdits = async (
  request: AutoSaveRequest
): Promise<ApiResponse<void>> => {
  try {
    const response: AxiosResponse<ApiResponse<void>> = await axios.patch(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.autoSave(request.resumeId)),
      { userEdits: request.userEdits },
      {
        headers: {
          'Content-Type': 'application/json',
          ...getAuthHeaders(),
        },
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// DOWNLOAD TRACKING
// ========================================

/**
 * Track PDF download for analytics
 */
export const trackPDFDownload = async (
  resumeId: string
): Promise<ApiResponse<void>> => {
  try {
    const response: AxiosResponse<ApiResponse<void>> = await axios.post(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.trackDownload(resumeId)),
      {},
      {
        headers: getAuthHeaders(),
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// SEARCH AND STATISTICS
// ========================================

/**
 * Search generated resumes with filters
 */
export const searchGeneratedResumes = async (
  request: SearchResumesRequest
): Promise<PaginatedResponse<GeneratedResume>> => {
  try {
    const response: AxiosResponse<PaginatedResponse<GeneratedResume>> = await axios.get(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.search),
      {
        headers: getAuthHeaders(),
        params: request,
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Get generated resume statistics
 */
export const getGeneratedResumeStatistics = async (): Promise<ApiResponse<any>> => {
  try {
    const response: AxiosResponse<ApiResponse<any>> = await axios.get(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.statistics),
      {
        headers: getAuthHeaders(),
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// AI ANALYSIS AND TRANSLATION
// ========================================

/**
 * Analyze job targeting for optimization
 */
export const analyzeJobTargeting = async (
  jobDescription: string,
  userProfile?: any
): Promise<ApiResponse<JobAnalysis>> => {
  try {
    const response: AxiosResponse<ApiResponse<JobAnalysis>> = await axios.post(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.analyzeJobTargeting),
      { jobDescription, userProfile },
      {
        headers: {
          'Content-Type': 'application/json',
          ...getAuthHeaders(),
        },
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Translate skills for Canadian market
 */
export const translateSkillsForCanadianMarket = async (
  skills: string[],
  targetIndustry?: string,
  sourceCountry?: string,
  experienceLevel?: string
): Promise<ApiResponse<SkillsTranslation[]>> => {
  try {
    const response: AxiosResponse<ApiResponse<SkillsTranslation[]>> = await axios.post(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.translateSkills),
      { skills, targetIndustry, sourceCountry, experienceLevel },
      {
        headers: {
          'Content-Type': 'application/json',
          ...getAuthHeaders(),
        },
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// EXPORT FUNCTIONALITY
// ========================================

/**
 * Export resume in various formats
 */
export const exportResume = async (
  resumeId: string,
  options: ExportOptions
): Promise<ApiResponse<ExportResult>> => {
  try {
    const response: AxiosResponse<ApiResponse<ExportResult>> = await axios.post(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.export(resumeId)),
      options,
      {
        headers: {
          'Content-Type': 'application/json',
          ...getAuthHeaders(),
        },
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Download resume as PDF
 */
export const downloadResumePDF = async (
  resumeId: string,
  template?: string
): Promise<Blob> => {
  try {
    const response: AxiosResponse<Blob> = await axios.get(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.downloadPDF(resumeId)),
      {
        headers: getAuthHeaders(),
        params: { template },
        responseType: 'blob',
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// STREAMING GENERATION PROGRESS
// ========================================

/**
 * Stream generation progress updates
 */
export const streamGenerationProgress = (
  resumeId: string,
  onProgress: (progress: GenerationProgress) => void,
  onComplete: (result: GeneratedResume) => void,
  onError: (error: string) => void
): (() => void) => {
  const eventSource = new EventSource(
    `${buildApiUrl(`/resume/generate/${resumeId}/progress`)}`,
    {
      headers: getAuthHeaders(),
    }
  )

  eventSource.onmessage = (event) => {
    try {
      const data = JSON.parse(event.data)
      
      if (data.type === 'progress') {
        onProgress(data.progress)
      } else if (data.type === 'complete') {
        onComplete(data.result)
        eventSource.close()
      } else if (data.type === 'error') {
        onError(data.error)
        eventSource.close()
      }
    } catch (error) {
      onError('Failed to parse progress update')
    }
  }

  eventSource.onerror = () => {
    onError('Connection lost')
    eventSource.close()
  }

  // Return cleanup function
  return () => {
    eventSource.close()
  }
}

// ========================================
// BULK OPERATIONS
// ========================================

/**
 * Bulk delete generated resumes
 */
export const bulkDeleteGeneratedResumes = async (
  resumeIds: string[]
): Promise<ApiResponse<{ success: number; failed: number }>> => {
  try {
    const response: AxiosResponse<ApiResponse<{ success: number; failed: number }>> = await axios.delete(
      buildApiUrl(RESUME_GENERATOR_ENDPOINTS.generated),
      {
        headers: getAuthHeaders(),
        data: { resumeIds },
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Bulk export resumes
 */
export const bulkExportResumes = async (
  resumeIds: string[],
  options: ExportOptions
): Promise<ApiResponse<ExportResult[]>> => {
  try {
    const response: AxiosResponse<ApiResponse<ExportResult[]>> = await axios.post(
      buildApiUrl('/resume/generated/bulk-export'),
      { resumeIds, options },
      {
        headers: {
          'Content-Type': 'application/json',
          ...getAuthHeaders(),
        },
        timeout: API_CONFIG.timeout * 2, // Longer timeout for bulk operations
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// UTILITY FUNCTIONS
// ========================================

/**
 * Check if resume generation is supported
 */
export const checkGenerationSupport = async (): Promise<ApiResponse<{
  supported: boolean
  features: string[]
  limitations: string[]
}>> => {
  try {
    const response: AxiosResponse<ApiResponse<{
      supported: boolean
      features: string[]
      limitations: string[]
    }>> = await axios.get(
      buildApiUrl('/api/v1/resume/generate/support'),
      {
        headers: getAuthHeaders(),
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

/**
 * Get generation templates
 */
export const getGenerationTemplates = async (): Promise<ApiResponse<{
  templates: Array<{
    id: string
    name: string
    description: string
    preview: string
    category: string
  }>
}>> => {
  try {
    const response: AxiosResponse<ApiResponse<{
      templates: Array<{
        id: string
        name: string
        description: string
        preview: string
        category: string
      }>
    }>> = await axios.get(
      buildApiUrl('/api/v1/resume/generate/templates'),
      {
        headers: getAuthHeaders(),
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// RESUME ANALYSES FUNCTIONS
// ========================================

/**
 * Get user's uploaded resume analyses
 */
export const getUserResumeAnalyses = async (): Promise<ApiResponse<any[]>> => {
  try {
    const response: AxiosResponse<ApiResponse<any[]>> = await axios.get(
      buildApiUrl('/api/v1/resume/analyses'),
      {
        headers: getAuthHeaders(),
        timeout: API_CONFIG.timeout,
      }
    )

    return response.data
  } catch (error) {
    handleApiError(error)
  }
}

// ========================================
// EXPORT ALL FUNCTIONS
// ========================================

export {
  RESUME_GENERATOR_ENDPOINTS,
  API_CONFIG,
  getAuthHeaders,
  handleApiError,
  retryApiCall,
}
```

## File: src/lib/auth.ts
```typescript
import { createClient } from '@supabase/supabase-js';

// Create Supabase client
const supabaseUrl = process.env.NEXT_PUBLIC_SUPABASE_URL!;
const supabaseAnonKey = process.env.NEXT_PUBLIC_SUPABASE_ANON_KEY!;

export const supabase = createClient(supabaseUrl, supabaseAnonKey);

export interface User {
  id: string;
  email: string;
  fullName: string;
  role?: string;
}

export interface AuthResponse {
  success: boolean;
  message: string;
  user?: User;
  session?: any;
}

// Authentication functions
export const auth = {
  // Register new user
  async register(email: string, password: string, fullName: string, additionalData?: any): Promise<AuthResponse> {
    try {
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/auth/register`, {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify({
          email,
          password,
          fullName,
          ...additionalData
        }),
      });

      const data = await response.json();
      
      if (data.success && data.session) {
        // Store session in localStorage
        localStorage.setItem('session', JSON.stringify(data.session));
        localStorage.setItem('user', JSON.stringify(data.user));
      }

      return data;
    } catch (error) {
      console.error('Registration error:', error);
      return {
        success: false,
        message: 'Registration failed. Please try again.'
      };
    }
  },

  // Login user
  async login(email: string, password: string): Promise<AuthResponse> {
    try {
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/auth/login`, {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify({ email, password }),
      });

      const data = await response.json();
      
      if (data.success && data.session) {
        // Store session in localStorage
        localStorage.setItem('session', JSON.stringify(data.session));
        localStorage.setItem('user', JSON.stringify(data.user));
      }

      return data;
    } catch (error) {
      console.error('Login error:', error);
      return {
        success: false,
        message: 'Login failed. Please try again.'
      };
    }
  },

  // Logout user
  async logout(): Promise<AuthResponse> {
    try {
      const session = this.getSession();
      if (session?.access_token) {
        await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/auth/logout`, {
          method: 'POST',
          headers: {
            'Authorization': `Bearer ${session.access_token}`,
            'Content-Type': 'application/json',
          },
        });
      }

      // Clear localStorage
      localStorage.removeItem('session');
      localStorage.removeItem('user');

      return {
        success: true,
        message: 'Logged out successfully'
      };
    } catch (error) {
      console.error('Logout error:', error);
      // Clear localStorage even if API call fails
      localStorage.removeItem('session');
      localStorage.removeItem('user');
      
      return {
        success: true,
        message: 'Logged out successfully'
      };
    }
  },

  // Get current session
  getSession() {
    try {
      const sessionStr = localStorage.getItem('session');
      return sessionStr ? JSON.parse(sessionStr) : null;
    } catch (error) {
      console.error('Error parsing session:', error);
      return null;
    }
  },

  // Get current user
  getCurrentUser(): User | null {
    try {
      const userStr = localStorage.getItem('user');
      return userStr ? JSON.parse(userStr) : null;
    } catch (error) {
      console.error('Error parsing user:', error);
      return null;
    }
  },

  // Check if user is authenticated
  isAuthenticated(): boolean {
    const session = this.getSession();
    const user = this.getCurrentUser();
    return !!(session?.access_token && user);
  },

  // Get auth token for API calls
  getAuthToken(): string | null {
    const session = this.getSession();
    return session?.access_token || null;
  },

  // Refresh token
  async refreshToken(): Promise<boolean> {
    try {
      const session = this.getSession();
      if (!session?.refresh_token) {
        return false;
      }

      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/auth/refresh`, {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify({
          refresh_token: session.refresh_token
        }),
      });

      const data = await response.json();
      
      if (data.success && data.session) {
        localStorage.setItem('session', JSON.stringify(data.session));
        return true;
      }

      return false;
    } catch (error) {
      console.error('Token refresh error:', error);
      return false;
    }
  },

  // Update user profile
  async updateProfile(profileData: any): Promise<AuthResponse> {
    try {
      const session = this.getSession();
      if (!session?.access_token) {
        return {
          success: false,
          message: 'Not authenticated'
        };
      }

      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/auth/profile`, {
        method: 'PUT',
        headers: {
          'Authorization': `Bearer ${session.access_token}`,
          'Content-Type': 'application/json',
        },
        body: JSON.stringify(profileData),
      });

      const data = await response.json();
      
      if (data.success && data.user) {
        localStorage.setItem('user', JSON.stringify(data.user));
      }

      return data;
    } catch (error) {
      console.error('Profile update error:', error);
      return {
        success: false,
        message: 'Profile update failed. Please try again.'
      };
    }
  },

  // Get user profile
  async getProfile(): Promise<AuthResponse> {
    try {
      const session = this.getSession();
      if (!session?.access_token) {
        return {
          success: false,
          message: 'Not authenticated'
        };
      }

      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/api/auth/profile`, {
        method: 'GET',
        headers: {
          'Authorization': `Bearer ${session.access_token}`,
          'Content-Type': 'application/json',
        },
      });

      const data = await response.json();
      
      if (data.success && data.user) {
        localStorage.setItem('user', JSON.stringify(data.user));
      }

      return data;
    } catch (error) {
      console.error('Profile fetch error:', error);
      return {
        success: false,
        message: 'Failed to fetch profile'
      };
    }
  }
};
```

## File: src/lib/config.ts
```typescript
// ============================================================================
// APPLICATION CONFIGURATION
// ============================================================================

// API Configuration
export const API_CONFIG = {
  BASE_URL: process.env.NEXT_PUBLIC_API_URL || 'http://localhost:3001',
  TIMEOUT: 10000,
  RETRY_ATTEMPTS: 3,
  RETRY_DELAY: 1000
} as const

// UI Configuration
export const UI_CONFIG = {
  THEMES: {
    LIGHT: 'light',
    DARK: 'dark',
    SYSTEM: 'system'
  },
  BREAKPOINTS: {
    SM: 640,
    MD: 768,
    LG: 1024,
    XL: 1280,
    '2XL': 1536
  },
  ANIMATIONS: {
    DURATION: {
      FAST: 150,
      NORMAL: 300,
      SLOW: 500
    },
    EASING: {
      DEFAULT: 'cubic-bezier(0.4, 0, 0.2, 1)',
      LINEAR: 'linear',
      IN: 'cubic-bezier(0.4, 0, 1, 1)',
      OUT: 'cubic-bezier(0, 0, 0.2, 1)',
      IN_OUT: 'cubic-bezier(0.4, 0, 0.2, 1)'
    }
  }
} as const

export const COMPONENT_SIZES = {
  SM: 'sm',
  DEFAULT: 'default',
  LG: 'lg',
  XL: 'xl'
} as const

// ============================================================================
// ROUTES CONFIGURATION
// ============================================================================

export const ROUTES = {
  HOME: '/',
  AUTH: {
    LOGIN: '/auth',
    REGISTER: '/auth/register',
    FORGOT_PASSWORD: '/auth/forgot-password'
  },
  DASHBOARD: {
    ROOT: '/dashboard',
    USER: '/dashboard/user',
    AI: {
      ROOT: '/dashboard/user/ai',
      RESUME: '/dashboard/user/ai/resume',
      CAREER_PROFILE: '/dashboard/user/ai/career-profile',
      HISTORY: '/dashboard/user/ai/history'
    },
    CAREER: '/dashboard/user/career',
    PROFILE: '/dashboard/user/profile',
    SETTINGS: '/dashboard/user/profile/settings'
  },
  API: {
    AUTH: {
      LOGIN: '/api/auth/login',
      REGISTER: '/api/auth/register',
      LOGOUT: '/api/auth/logout',
      VERIFY: '/api/auth/verify'
    },
    AI: {
      RESUME: {
        UPLOAD: '/api/resume/upload',
        ANALYSES: '/api/resume/analyses'
      },
      CAREER_PROFILE: '/api/career/profile'
    },
    CAREER: {
      SEARCH_JOBS: '/api/career/search',
      RECOMMENDATIONS: '/api/career/recommendations'
    },
    USER: {
      PROFILE: '/api/user/profile',
      SETTINGS: '/api/user/settings'
    }
  }
} as const

// ============================================================================
// MESSAGE CONSTANTS
// ============================================================================

export const MESSAGES = {
  SUCCESS: {
    LOGIN: 'Successfully logged in',
    REGISTER: 'Successfully registered',
    LOGOUT: 'Successfully logged out',
    PROFILE_UPDATED: 'Profile updated successfully',
    RESUME_UPLOADED: 'Resume uploaded successfully',
    ANALYSIS_COMPLETED: 'Analysis completed successfully'
  },
  ERROR: {
    LOGIN_FAILED: 'Login failed. Please check your credentials.',
    REGISTER_FAILED: 'Registration failed. Please try again.',
    NETWORK_ERROR: 'Network error. Please check your connection.',
    UPLOAD_FAILED: 'Upload failed. Please try again.',
    ANALYSIS_FAILED: 'Analysis failed. Please try again.',
    UNAUTHORIZED: 'You are not authorized to perform this action.',
    NOT_FOUND: 'The requested resource was not found.',
    SERVER_ERROR: 'Server error. Please try again later.'
  },
  VALIDATION: {
    REQUIRED: 'This field is required',
    EMAIL_INVALID: 'Please enter a valid email address',
    PASSWORD_MIN: 'Password must be at least 8 characters',
    PASSWORD_MATCH: 'Passwords must match',
    FILE_SIZE: 'File size must be less than 5MB',
    FILE_TYPE: 'Please upload a PDF file'
  }
} as const

// ============================================================================
// FEATURE FLAGS
// ============================================================================

export const FEATURES = {
  AI_RESUME_ANALYSIS: true,
  CAREER_RECOMMENDATIONS: true,
  JOB_SEARCH: true,
  USER_PROFILES: true,
  FILE_UPLOADS: true,
  NOTIFICATIONS: true,
  ANALYTICS: true
} as const

// ============================================================================
// ENVIRONMENT CONFIGURATION
// ============================================================================

export const ENV_CONFIG = {
  IS_DEVELOPMENT: process.env.NODE_ENV === 'development',
  IS_PRODUCTION: process.env.NODE_ENV === 'production',
  IS_TEST: process.env.NODE_ENV === 'test',
  API_URL: process.env.NEXT_PUBLIC_API_URL,
  APP_URL: process.env.NEXT_PUBLIC_APP_URL,
  AUTH_SECRET: process.env.NEXTAUTH_SECRET,
  GOOGLE_CLIENT_ID: process.env.GOOGLE_CLIENT_ID,
  GOOGLE_CLIENT_SECRET: process.env.GOOGLE_CLIENT_SECRET
} as const

// ============================================================================
// VALIDATION RULES
// ============================================================================

export const VALIDATION_RULES = {
  PASSWORD: {
    MIN_LENGTH: 8,
    REQUIRE_UPPERCASE: true,
    REQUIRE_LOWERCASE: true,
    REQUIRE_NUMBERS: true,
    REQUIRE_SPECIAL_CHARS: false
  },
  FILE: {
    MAX_SIZE: 5 * 1024 * 1024, // 5MB
    ALLOWED_TYPES: ['application/pdf', 'text/plain'],
    ALLOWED_EXTENSIONS: ['.pdf', '.txt']
  },
  EMAIL: {
    MAX_LENGTH: 254
  },
  NAME: {
    MIN_LENGTH: 2,
    MAX_LENGTH: 50
  }
} as const

// ============================================================================
// CACHE CONFIGURATION
// ============================================================================

export const CACHE_CONFIG = {
  TTL: {
    SHORT: 5 * 60 * 1000, // 5 minutes
    MEDIUM: 30 * 60 * 1000, // 30 minutes
    LONG: 24 * 60 * 60 * 1000, // 24 hours
    VERY_LONG: 7 * 24 * 60 * 60 * 1000 // 7 days
  },
  KEYS: {
    USER_PROFILE: 'user_profile',
    RESUME_ANALYSIS: 'resume_analysis',
    CAREER_RECOMMENDATIONS: 'career_recommendations',
    JOB_SEARCH: 'job_search'
  }
} as const

// ============================================================================
// EXPORT ALL CONFIGURATIONS
// ============================================================================

export default {
  API_CONFIG,
  UI_CONFIG,
  COMPONENT_SIZES,
  ROUTES,
  MESSAGES,
  FEATURES,
  ENV_CONFIG,
  VALIDATION_RULES,
  CACHE_CONFIG
}
```

## File: src/lib/config/constants.ts
```typescript
// Global Constants Configuration
// Centralized constants for the application

// Application constants
export const APP_CONSTANTS = {
  NAME: 'ImmiGrowAI',
  VERSION: '1.0.0',
  DESCRIPTION: 'AI-powered career growth platform',
  AUTHOR: 'ImmiGrowAI Team',
  WEBSITE: 'https://immigrowai.com',
  SUPPORT_EMAIL: 'support@immigrowai.com',
} as const

// API constants
export const API_CONSTANTS = {
  TIMEOUT: 30000, // 30 seconds
  RETRY_ATTEMPTS: 3,
  RETRY_DELAY: 1000, // 1 second
  MAX_FILE_SIZE: 10 * 1024 * 1024, // 10MB
  RATE_LIMIT: {
    REQUESTS_PER_MINUTE: 60,
    REQUESTS_PER_HOUR: 1000,
  },
} as const

// Authentication constants
export const AUTH_CONSTANTS = {
  TOKEN_EXPIRY: 24 * 60 * 60 * 1000, // 24 hours
  REFRESH_TOKEN_EXPIRY: 7 * 24 * 60 * 60 * 1000, // 7 days
  PASSWORD_MIN_LENGTH: 8,
  PASSWORD_MAX_LENGTH: 128,
  SESSION_TIMEOUT: 30 * 60 * 1000, // 30 minutes
} as const

// File upload constants
export const UPLOAD_CONSTANTS = {
  MAX_FILE_SIZE: 10 * 1024 * 1024, // 10MB
  ALLOWED_RESUME_TYPES: [
    'application/pdf',
    'application/msword',
    'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
  ],
  ALLOWED_IMAGE_TYPES: [
    'image/jpeg',
    'image/png',
    'image/webp',
  ],
  ALLOWED_DOCUMENT_TYPES: [
    'application/pdf',
    'application/msword',
    'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
    'text/plain',
  ],
} as const

// UI constants
export const UI_CONSTANTS = {
  BREAKPOINTS: {
    MOBILE: 768,
    TABLET: 1024,
    DESKTOP: 1280,
    LARGE_DESKTOP: 1536,
  },
  ANIMATION_DURATION: {
    FAST: 150,
    NORMAL: 300,
    SLOW: 500,
  },
  Z_INDEX: {
    DROPDOWN: 1000,
    STICKY: 1020,
    FIXED: 1030,
    MODAL_BACKDROP: 1040,
    MODAL: 1050,
    POPOVER: 1060,
    TOOLTIP: 1070,
  },
  COLORS: {
    PRIMARY: '#3B82F6',
    SECONDARY: '#6B7280',
    SUCCESS: '#10B981',
    WARNING: '#F59E0B',
    ERROR: '#EF4444',
    INFO: '#3B82F6',
  },
} as const

// Form constants
export const FORM_CONSTANTS = {
  VALIDATION: {
    EMAIL_REGEX: /^[^\s@]+@[^\s@]+\.[^\s@]+$/,
    PHONE_REGEX: /^\+?[\d\s\-\(\)]+$/,
    URL_REGEX: /^https?:\/\/.+/,
    PASSWORD_REGEX: /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$/,
  },
  LIMITS: {
    NAME_MAX_LENGTH: 100,
    BIO_MAX_LENGTH: 500,
    DESCRIPTION_MAX_LENGTH: 1000,
    COVER_LETTER_MAX_LENGTH: 2000,
    SKILLS_MAX_COUNT: 20,
    EXPERIENCE_MAX_COUNT: 20,
    EDUCATION_MAX_COUNT: 10,
    CERTIFICATIONS_MAX_COUNT: 10,
    LANGUAGES_MAX_COUNT: 10,
  },
} as const

// Job search constants
export const JOB_CONSTANTS = {
  SEARCH: {
    DEFAULT_PAGE_SIZE: 10,
    MAX_PAGE_SIZE: 50,
    DEFAULT_RADIUS: 25, // miles
    MAX_RADIUS: 100,
  },
  TYPES: ['full-time', 'part-time', 'contract', 'internship'] as const,
  EXPERIENCE_LEVELS: ['entry', 'mid', 'senior', 'executive'] as const,
  SALARY_CURRENCIES: ['USD', 'EUR', 'GBP', 'CAD', 'AUD'] as const,
  APPLICATION_STATUSES: ['pending', 'reviewed', 'interviewed', 'accepted', 'rejected'] as const,
} as const

// Resume constants
export const RESUME_CONSTANTS = {
  ANALYSIS_TYPES: ['general', 'skills', 'experience', 'education', 'comprehensive'] as const,
  SCORE_RANGES: {
    EXCELLENT: { min: 90, max: 100 },
    GOOD: { min: 70, max: 89 },
    AVERAGE: { min: 50, max: 69 },
    POOR: { min: 0, max: 49 },
  },
  TEMPLATES: {
    PROFESSIONAL: 'professional',
    CREATIVE: 'creative',
    MINIMAL: 'minimal',
    MODERN: 'modern',
  },
} as const

// Career constants
export const CAREER_CONSTANTS = {
  SKILL_CATEGORIES: [
    'programming',
    'design',
    'marketing',
    'sales',
    'management',
    'communication',
    'analytics',
    'languages',
    'tools',
    'soft-skills',
  ] as const,
  PROFICIENCY_LEVELS: ['beginner', 'intermediate', 'advanced', 'native'] as const,
  EDUCATION_LEVELS: [
    'high-school',
    'associate',
    'bachelor',
    'master',
    'doctorate',
    'certification',
  ] as const,
} as const

// Notification constants
export const NOTIFICATION_CONSTANTS = {
  TYPES: ['info', 'success', 'warning', 'error'] as const,
  AUTO_DISMISS_DELAY: 5000, // 5 seconds
  MAX_VISIBLE: 5,
  STORAGE_KEY: 'notifications',
} as const

// Storage constants
export const STORAGE_CONSTANTS = {
  KEYS: {
    AUTH_TOKEN: 'auth-token',
    REFRESH_TOKEN: 'refresh-token',
    USER_PREFERENCES: 'user-preferences',
    THEME: 'theme',
    LANGUAGE: 'language',
    SIDEBAR_STATE: 'sidebar-state',
    NOTIFICATIONS: 'notifications',
    CART: 'cart',
    RECENT_SEARCHES: 'recent-searches',
    SAVED_JOBS: 'saved-jobs',
  },
  PREFIX: 'immigrowai_',
} as const

// Error constants
export const ERROR_CONSTANTS = {
  MESSAGES: {
    NETWORK_ERROR: 'Network error. Please check your connection.',
    UNAUTHORIZED: 'You are not authorized to perform this action.',
    FORBIDDEN: 'Access denied.',
    NOT_FOUND: 'The requested resource was not found.',
    VALIDATION_ERROR: 'Please check your input and try again.',
    SERVER_ERROR: 'Server error. Please try again later.',
    TIMEOUT_ERROR: 'Request timed out. Please try again.',
    UNKNOWN_ERROR: 'An unexpected error occurred.',
  },
  CODES: {
    NETWORK_ERROR: 'NETWORK_ERROR',
    UNAUTHORIZED: 'UNAUTHORIZED',
    FORBIDDEN: 'FORBIDDEN',
    NOT_FOUND: 'NOT_FOUND',
    VALIDATION_ERROR: 'VALIDATION_ERROR',
    SERVER_ERROR: 'SERVER_ERROR',
    TIMEOUT_ERROR: 'TIMEOUT_ERROR',
    UNKNOWN_ERROR: 'UNKNOWN_ERROR',
  },
} as const

// Date and time constants
export const DATE_CONSTANTS = {
  FORMATS: {
    DATE: 'YYYY-MM-DD',
    DATETIME: 'YYYY-MM-DD HH:mm:ss',
    TIME: 'HH:mm:ss',
    DISPLAY_DATE: 'MMM DD, YYYY',
    DISPLAY_DATETIME: 'MMM DD, YYYY HH:mm',
    DISPLAY_TIME: 'HH:mm',
  },
  TIMEZONES: {
    UTC: 'UTC',
    EST: 'America/New_York',
    PST: 'America/Los_Angeles',
    GMT: 'Europe/London',
    CET: 'Europe/Paris',
  },
} as const

// Pagination constants
export const PAGINATION_CONSTANTS = {
  DEFAULT_PAGE: 1,
  DEFAULT_LIMIT: 10,
  MAX_LIMIT: 100,
  PAGE_SIZE_OPTIONS: [10, 20, 50, 100],
} as const

// Export all constants
export const CONSTANTS = {
  APP: APP_CONSTANTS,
  API: API_CONSTANTS,
  AUTH: AUTH_CONSTANTS,
  UPLOAD: UPLOAD_CONSTANTS,
  UI: UI_CONSTANTS,
  FORM: FORM_CONSTANTS,
  JOB: JOB_CONSTANTS,
  RESUME: RESUME_CONSTANTS,
  CAREER: CAREER_CONSTANTS,
  NOTIFICATION: NOTIFICATION_CONSTANTS,
  STORAGE: STORAGE_CONSTANTS,
  ERROR: ERROR_CONSTANTS,
  DATE: DATE_CONSTANTS,
  PAGINATION: PAGINATION_CONSTANTS,
} as const

// Export individual constants for easier imports

export default CONSTANTS
```

## File: src/lib/config/environment.ts
```typescript
import { z } from 'zod'

// Environment schema validation
const environmentSchema = z.object({
  // API Configuration
  NEXT_PUBLIC_API_URL: z.string().url().optional(),
  NEXT_PUBLIC_API_TIMEOUT: z.string().transform(Number).pipe(z.number().min(1000).max(60000)).optional(),
  
  // Authentication
  NEXT_PUBLIC_AUTH_DOMAIN: z.string().optional(),
  NEXT_PUBLIC_AUTH_CLIENT_ID: z.string().optional(),
  
  // Database
  NEXT_PUBLIC_DATABASE_URL: z.string().optional(),
  
  // File Storage
  NEXT_PUBLIC_STORAGE_URL: z.string().url().optional(),
  NEXT_PUBLIC_UPLOAD_MAX_SIZE: z.string().transform(Number).pipe(z.number().min(1).max(100)).optional(),
  
  // Analytics
  NEXT_PUBLIC_ANALYTICS_ID: z.string().optional(),
  NEXT_PUBLIC_ANALYTICS_ENABLED: z.string().transform(val => val === 'true').optional(),
  
  // Monitoring
  NEXT_PUBLIC_SENTRY_DSN: z.string().optional(),
  NEXT_PUBLIC_SENTRY_ENVIRONMENT: z.string().optional(),
  
  // Feature Flags
  NEXT_PUBLIC_FEATURE_AI_ENABLED: z.string().transform(val => val === 'true').optional(),
  NEXT_PUBLIC_FEATURE_JOB_SEARCH_ENABLED: z.string().transform(val => val === 'true').optional(),
  NEXT_PUBLIC_FEATURE_RESUME_ANALYSIS_ENABLED: z.string().transform(val => val === 'true').optional(),
  NEXT_PUBLIC_FEATURE_CAREER_PROFILE_ENABLED: z.string().transform(val => val === 'true').optional(),
  
  // Development
  NODE_ENV: z.enum(['development', 'production', 'test']).default('development'),
  NEXT_PUBLIC_DEBUG_MODE: z.string().transform(val => val === 'true').optional(),
  
  // App Configuration
  NEXT_PUBLIC_APP_NAME: z.string().default('ImmiGrowAI'),
  NEXT_PUBLIC_APP_VERSION: z.string().default('1.0.0'),
  NEXT_PUBLIC_APP_DESCRIPTION: z.string().default('AI-powered career growth platform'),
  
  // Contact Information
  NEXT_PUBLIC_CONTACT_EMAIL: z.string().email().optional(),
  NEXT_PUBLIC_SUPPORT_URL: z.string().url().optional(),
  
  // Social Media
  NEXT_PUBLIC_SOCIAL_LINKEDIN: z.string().url().optional(),
  NEXT_PUBLIC_SOCIAL_TWITTER: z.string().url().optional(),
  NEXT_PUBLIC_SOCIAL_GITHUB: z.string().url().optional(),
})

// Environment type
export type Environment = z.infer<typeof environmentSchema>

// Parse and validate environment variables
const parseEnvironment = (): Environment => {
  try {
    const env = environmentSchema.parse(process.env)
    return env
  } catch (error) {
    if (error instanceof z.ZodError) {
      console.error('❌ Environment validation failed:')
      error.errors.forEach(err => {
        console.error(`  - ${err.path.join('.')}: ${err.message}`)
      })
    }
    
    // Return default values for development
    if (process.env.NODE_ENV === 'development') {
      console.warn('⚠️ Using default environment values for development')
      return {
        NODE_ENV: 'development',
        NEXT_PUBLIC_APP_NAME: 'ImmiGrowAI',
        NEXT_PUBLIC_APP_VERSION: '1.0.0',
        NEXT_PUBLIC_APP_DESCRIPTION: 'AI-powered career growth platform',
        NEXT_PUBLIC_API_URL: 'http://localhost:3001/api',
        NEXT_PUBLIC_API_TIMEOUT: 30000,
        NEXT_PUBLIC_UPLOAD_MAX_SIZE: 10,
        NEXT_PUBLIC_FEATURE_AI_ENABLED: true,
        NEXT_PUBLIC_FEATURE_JOB_SEARCH_ENABLED: true,
        NEXT_PUBLIC_FEATURE_RESUME_ANALYSIS_ENABLED: true,
        NEXT_PUBLIC_FEATURE_CAREER_PROFILE_ENABLED: true,
        NEXT_PUBLIC_DEBUG_MODE: true,
      }
    }
    
    throw new Error('Environment validation failed')
  }
}

// Get validated environment
export const env = parseEnvironment()

// Environment helpers
export const isDevelopment = env.NODE_ENV === 'development'
export const isProduction = env.NODE_ENV === 'production'
export const isTest = env.NODE_ENV === 'test'

// API Configuration
export const apiConfig = {
  baseUrl: env.NEXT_PUBLIC_API_URL || 'http://localhost:3001/api',
  timeout: env.NEXT_PUBLIC_API_TIMEOUT || 30000,
  retries: 3,
  retryDelay: 1000,
}

// File Upload Configuration
export const uploadConfig = {
  maxSize: (env.NEXT_PUBLIC_UPLOAD_MAX_SIZE || 10) * 1024 * 1024, // Convert MB to bytes
  allowedTypes: {
    resume: ['application/pdf', 'application/msword', 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'],
    avatar: ['image/jpeg', 'image/png', 'image/webp'],
    document: ['application/pdf', 'application/msword', 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'],
  },
  storageUrl: env.NEXT_PUBLIC_STORAGE_URL,
}

// Feature Flags
export const features = {
  ai: env.NEXT_PUBLIC_FEATURE_AI_ENABLED ?? true,
  jobSearch: env.NEXT_PUBLIC_FEATURE_JOB_SEARCH_ENABLED ?? true,
  resumeAnalysis: env.NEXT_PUBLIC_FEATURE_RESUME_ANALYSIS_ENABLED ?? true,
  careerProfile: env.NEXT_PUBLIC_FEATURE_CAREER_PROFILE_ENABLED ?? true,
}

// Analytics Configuration
export const analyticsConfig = {
  enabled: env.NEXT_PUBLIC_ANALYTICS_ENABLED ?? !isDevelopment,
  id: env.NEXT_PUBLIC_ANALYTICS_ID,
}

// Monitoring Configuration
export const monitoringConfig = {
  sentry: {
    dsn: env.NEXT_PUBLIC_SENTRY_DSN,
    environment: env.NEXT_PUBLIC_SENTRY_ENVIRONMENT || env.NODE_ENV,
  },
}

// App Configuration
export const appConfig = {
  name: env.NEXT_PUBLIC_APP_NAME,
  version: env.NEXT_PUBLIC_APP_VERSION,
  description: env.NEXT_PUBLIC_APP_DESCRIPTION,
  debug: env.NEXT_PUBLIC_DEBUG_MODE ?? isDevelopment,
  contact: {
    email: env.NEXT_PUBLIC_CONTACT_EMAIL,
    support: env.NEXT_PUBLIC_SUPPORT_URL,
  },
  social: {
    linkedin: env.NEXT_PUBLIC_SOCIAL_LINKEDIN,
    twitter: env.NEXT_PUBLIC_SOCIAL_TWITTER,
    github: env.NEXT_PUBLIC_SOCIAL_GITHUB,
  },
}

// Export configuration objects
export default {
  env,
  isDevelopment,
  isProduction,
  isTest,
  apiConfig,
  uploadConfig,
  features,
  analyticsConfig,
  monitoringConfig,
  appConfig,
}
```

## File: src/lib/config/features.ts
```typescript
// Feature Flags Configuration
// Centralized feature flag management for enabling/disabling features

import { features as envFeatures } from './environment'

// Feature flag types
export interface FeatureFlag {
  name: string
  description: string
  enabled: boolean
  category: 'core' | 'ai' | 'premium' | 'experimental' | 'deprecated'
  version?: string
  dependencies?: string[]
}

// Feature flag categories
export const FEATURE_CATEGORIES = {
  CORE: 'core',
  AI: 'ai',
  PREMIUM: 'premium',
  EXPERIMENTAL: 'experimental',
  DEPRECATED: 'deprecated',
} as const

// Define all feature flags
export const FEATURE_FLAGS: Record<string, FeatureFlag> = {
  // Core Features
  AUTHENTICATION: {
    name: 'authentication',
    description: 'User authentication and authorization',
    enabled: true,
    category: FEATURE_CATEGORIES.CORE,
  },

  USER_PROFILE: {
    name: 'user_profile',
    description: 'User profile management',
    enabled: true,
    category: FEATURE_CATEGORIES.CORE,
  },

  NOTIFICATIONS: {
    name: 'notifications',
    description: 'In-app notifications system',
    enabled: true,
    category: FEATURE_CATEGORIES.CORE,
  },

  // AI Features
  AI_RESUME_ANALYSIS: {
    name: 'ai_resume_analysis',
    description: 'AI-powered resume analysis and feedback',
    enabled: envFeatures.ai,
    category: FEATURE_CATEGORIES.AI,
    dependencies: ['authentication', 'user_profile'],
  },

  AI_CAREER_RECOMMENDATIONS: {
    name: 'ai_career_recommendations',
    description: 'AI-powered career path recommendations',
    enabled: envFeatures.ai,
    category: FEATURE_CATEGORIES.AI,
    dependencies: ['authentication', 'user_profile'],
  },

  AI_JOB_MATCHING: {
    name: 'ai_job_matching',
    description: 'AI-powered job matching algorithm',
    enabled: envFeatures.ai,
    category: FEATURE_CATEGORIES.AI,
    dependencies: ['authentication', 'job_search'],
  },

  AI_COVER_LETTER_GENERATOR: {
    name: 'ai_cover_letter_generator',
    description: 'AI-powered cover letter generation',
    enabled: envFeatures.ai,
    category: FEATURE_CATEGORIES.AI,
    dependencies: ['authentication', 'resume_management'],
  },

  AI_INTERVIEW_PREP: {
    name: 'ai_interview_prep',
    description: 'AI-powered interview preparation tools',
    enabled: envFeatures.ai,
    category: FEATURE_CATEGORIES.AI,
    dependencies: ['authentication', 'user_profile'],
  },

  AI_SKILL_GAP_ANALYSIS: {
    name: 'ai_skill_gap_analysis',
    description: 'AI-powered skill gap analysis',
    enabled: envFeatures.ai,
    category: FEATURE_CATEGORIES.AI,
    dependencies: ['authentication', 'career_profile'],
  },

  // Job Search Features
  JOB_SEARCH: {
    name: 'job_search',
    description: 'Job search and browsing functionality',
    enabled: envFeatures.jobSearch,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication'],
  },

  JOB_APPLICATIONS: {
    name: 'job_applications',
    description: 'Job application tracking',
    enabled: envFeatures.jobSearch,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'job_search'],
  },

  SAVED_JOBS: {
    name: 'saved_jobs',
    description: 'Save and manage favorite jobs',
    enabled: envFeatures.jobSearch,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'job_search'],
  },

  JOB_RECOMMENDATIONS: {
    name: 'job_recommendations',
    description: 'Personalized job recommendations',
    enabled: envFeatures.jobSearch,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'job_search'],
  },

  // Resume Features
  RESUME_MANAGEMENT: {
    name: 'resume_management',
    description: 'Resume upload and management',
    enabled: envFeatures.resumeAnalysis,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication'],
  },

  RESUME_ANALYSIS: {
    name: 'resume_analysis',
    description: 'Resume analysis and feedback',
    enabled: envFeatures.resumeAnalysis,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'resume_management'],
  },

  RESUME_TEMPLATES: {
    name: 'resume_templates',
    description: 'Resume templates and builder',
    enabled: envFeatures.resumeAnalysis,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'resume_management'],
  },

  // Career Profile Features
  CAREER_PROFILE: {
    name: 'career_profile',
    description: 'Career profile management',
    enabled: envFeatures.careerProfile,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'user_profile'],
  },

  SKILL_MANAGEMENT: {
    name: 'skill_management',
    description: 'Skill tracking and management',
    enabled: envFeatures.careerProfile,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'career_profile'],
  },

  EXPERIENCE_TRACKING: {
    name: 'experience_tracking',
    description: 'Work experience tracking',
    enabled: envFeatures.careerProfile,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'career_profile'],
  },

  EDUCATION_TRACKING: {
    name: 'education_tracking',
    description: 'Education and certification tracking',
    enabled: envFeatures.careerProfile,
    category: FEATURE_CATEGORIES.CORE,
    dependencies: ['authentication', 'career_profile'],
  },

  // Premium Features
  ADVANCED_ANALYTICS: {
    name: 'advanced_analytics',
    description: 'Advanced analytics and insights',
    enabled: false,
    category: FEATURE_CATEGORIES.PREMIUM,
    dependencies: ['authentication'],
  },

  PRIORITY_SUPPORT: {
    name: 'priority_support',
    description: 'Priority customer support',
    enabled: false,
    category: FEATURE_CATEGORIES.PREMIUM,
    dependencies: ['authentication'],
  },

  CUSTOM_BRANDING: {
    name: 'custom_branding',
    description: 'Custom branding options',
    enabled: false,
    category: FEATURE_CATEGORIES.PREMIUM,
    dependencies: ['authentication'],
  },

  // Experimental Features
  BETA_FEATURES: {
    name: 'beta_features',
    description: 'Access to beta features',
    enabled: false,
    category: FEATURE_CATEGORIES.EXPERIMENTAL,
    dependencies: ['authentication'],
  },

  VOICE_INTERFACE: {
    name: 'voice_interface',
    description: 'Voice-controlled interface',
    enabled: false,
    category: FEATURE_CATEGORIES.EXPERIMENTAL,
    dependencies: ['authentication'],
  },

  AR_VISUALIZATION: {
    name: 'ar_visualization',
    description: 'AR-powered career visualization',
    enabled: false,
    category: FEATURE_CATEGORIES.EXPERIMENTAL,
    dependencies: ['authentication'],
  },
}

// Feature flag management
export class FeatureFlagManager {
  private flags: Record<string, FeatureFlag>

  constructor(flags: Record<string, FeatureFlag> = FEATURE_FLAGS) {
    this.flags = flags
  }

  // Check if a feature is enabled
  isEnabled(featureName: string): boolean {
    const flag = this.flags[featureName]
    if (!flag) {
      console.warn(`Feature flag not found: ${featureName}`)
      return false
    }

    // Check if the feature itself is enabled
    if (!flag.enabled) {
      return false
    }

    // Check dependencies
    if (flag.dependencies) {
      for (const dependency of flag.dependencies) {
        if (!this.isEnabled(dependency)) {
          return false
        }
      }
    }

    return true
  }

  // Get all enabled features
  getEnabledFeatures(): string[] {
    return Object.keys(this.flags).filter(feature => this.isEnabled(feature))
  }

  // Get features by category
  getFeaturesByCategory(category: string): FeatureFlag[] {
    return Object.values(this.flags).filter(flag => flag.category === category)
  }

  // Get all feature flags
  getAllFlags(): Record<string, FeatureFlag> {
    return { ...this.flags }
  }

  // Update a feature flag
  updateFlag(featureName: string, updates: Partial<FeatureFlag>): void {
    if (this.flags[featureName]) {
      this.flags[featureName] = { ...this.flags[featureName], ...updates }
    }
  }

  // Add a new feature flag
  addFlag(featureName: string, flag: FeatureFlag): void {
    this.flags[featureName] = flag
  }

  // Remove a feature flag
  removeFlag(featureName: string): void {
    delete this.flags[featureName]
  }
}

// Create global feature flag manager instance
export const featureFlags = new FeatureFlagManager()

// Helper functions
export const isFeatureEnabled = (featureName: string): boolean => {
  return featureFlags.isEnabled(featureName)
}

export const getEnabledFeatures = (): string[] => {
  return featureFlags.getEnabledFeatures()
}

export const getFeaturesByCategory = (category: string): FeatureFlag[] => {
  return featureFlags.getFeaturesByCategory(category)
}

// Feature-specific helper functions
export const isAIFeatureEnabled = (featureName: string): boolean => {
  return isFeatureEnabled('ai_resume_analysis') && isFeatureEnabled(featureName)
}

export const isJobSearchEnabled = (): boolean => {
  return isFeatureEnabled('job_search')
}

export const isResumeAnalysisEnabled = (): boolean => {
  return isFeatureEnabled('resume_analysis')
}

export const isCareerProfileEnabled = (): boolean => {
  return isFeatureEnabled('career_profile')
}

// Export feature flag manager and helper functions
export default featureFlags
```

## File: src/lib/config/index.ts
```typescript
// Configuration exports
export * from './environment'
export * from './features'
export * from './constants'

// Re-export commonly used items
export {
  env,
  isDevelopment,
  isProduction,
  isTest,
  apiConfig,
  uploadConfig,
  features,
  analyticsConfig,
  monitoringConfig,
  appConfig,
} from './environment'

export {
  featureFlags,
  isFeatureEnabled,
  getEnabledFeatures,
  getFeaturesByCategory,
  isAIFeatureEnabled,
  isJobSearchEnabled,
  isResumeAnalysisEnabled,
  isCareerProfileEnabled,
  FEATURE_CATEGORIES,
  FEATURE_FLAGS,
} from './features'

export {
  CONSTANTS,
  APP_CONSTANTS,
  API_CONSTANTS,
  AUTH_CONSTANTS,
  UPLOAD_CONSTANTS,
  UI_CONSTANTS,
  FORM_CONSTANTS,
  JOB_CONSTANTS,
  RESUME_CONSTANTS,
  CAREER_CONSTANTS,
  NOTIFICATION_CONSTANTS,
  STORAGE_CONSTANTS,
  ERROR_CONSTANTS,
  DATE_CONSTANTS,
  PAGINATION_CONSTANTS,
} from './constants'

// Export types
export type { Environment } from './environment'
export type { FeatureFlag } from './features'
```

## File: src/lib/index.ts
```typescript
// Library utilities exports
export * from './api';
export * from './auth';
export * from './utils';
export * from './config';
```

## File: src/lib/pdfGenerator.ts
```typescript
import puppeteer from 'puppeteer';
import { JSDOM } from 'jsdom';

export interface PDFOptions {
  format?: 'A4' | 'Letter';
  margin?: {
    top?: string;
    right?: string;
    bottom?: string;
    left?: string;
  };
  printBackground?: boolean;
  preferCSSPageSize?: boolean;
  displayHeaderFooter?: boolean;
  headerTemplate?: string;
  footerTemplate?: string;
  landscape?: boolean;
}

export interface ResumePDFData {
  personalInfo: any;
  professionalSummary: any;
  workExperience: any[];
  education: any[];
  skills: any[];
  certifications: any[];
  languages: any[];
  additionalInfo?: string;
  atsScore?: number;
}

export class PDFGenerator {
  private browser: puppeteer.Browser | null = null;

  /**
   * Initialize the PDF generator
   */
  async initialize(): Promise<void> {
    if (!this.browser) {
      this.browser = await puppeteer.launch({
        headless: 'new',
        args: [
          '--no-sandbox',
          '--disable-setuid-sandbox',
          '--disable-dev-shm-usage',
          '--disable-accelerated-2d-canvas',
          '--no-first-run',
          '--no-zygote',
          '--disable-gpu'
        ]
      });
    }
  }

  /**
   * Close the browser instance
   */
  async close(): Promise<void> {
    if (this.browser) {
      await this.browser.close();
      this.browser = null;
    }
  }

  /**
   * Generate PDF from HTML content
   */
  async generatePDFFromHTML(
    htmlContent: string,
    options: PDFOptions = {}
  ): Promise<Buffer> {
    await this.initialize();

    if (!this.browser) {
      throw new Error('Browser not initialized');
    }

    const page = await this.browser.newPage();
    
    try {
      // Set content and wait for network idle
      await page.setContent(htmlContent, {
        waitUntil: 'networkidle0',
        timeout: 30000
      });

      // Generate PDF with options
      const pdfBuffer = await page.pdf({
        format: options.format || 'A4',
        margin: options.margin || {
          top: '20mm',
          right: '20mm',
          bottom: '20mm',
          left: '20mm'
        },
        printBackground: options.printBackground ?? true,
        preferCSSPageSize: options.preferCSSPageSize ?? true,
        displayHeaderFooter: options.displayHeaderFooter ?? false,
        headerTemplate: options.headerTemplate,
        footerTemplate: options.footerTemplate,
        landscape: options.landscape ?? false
      });

      return pdfBuffer;
    } finally {
      await page.close();
    }
  }

  /**
   * Generate PDF from resume data using Canadian template
   */
  async generateResumePDF(
    resumeData: ResumePDFData,
    options: PDFOptions = {}
  ): Promise<Buffer> {
    const htmlContent = this.generateResumeHTML(resumeData);
    return this.generatePDFFromHTML(htmlContent, options);
  }

  /**
   * Generate HTML content for resume
   */
  private generateResumeHTML(resumeData: ResumePDFData): string {
    const {
      personalInfo,
      professionalSummary,
      workExperience,
      education,
      skills,
      certifications,
      languages,
      additionalInfo,
      atsScore
    } = resumeData;

    const formatDate = (date: string) => {
      if (!date) return '';
      return new Date(date).toLocaleDateString('en-CA', {
        year: 'numeric',
        month: 'short'
      });
    };

    const getSkillLevel = (level: string) => {
      switch (level) {
        case 'expert': return 'Expert';
        case 'advanced': return 'Advanced';
        case 'intermediate': return 'Intermediate';
        case 'beginner': return 'Beginner';
        default: return level;
      }
    };

    return `
      <!DOCTYPE html>
      <html lang="en">
      <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>${personalInfo?.name || 'Resume'}</title>
        <style>
          @page {
            size: A4;
            margin: 20mm;
          }
          
          body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            margin: 0;
            padding: 0;
            background: white;
          }
          
          .container {
            max-width: 210mm;
            margin: 0 auto;
            padding: 0;
          }
          
          .header {
            text-align: center;
            margin-bottom: 30px;
            border-bottom: 2px solid #2563eb;
            padding-bottom: 20px;
          }
          
          .name {
            font-size: 28px;
            font-weight: bold;
            color: #1f2937;
            margin-bottom: 10px;
          }
          
          .contact-info {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            font-size: 14px;
            color: #6b7280;
            margin-bottom: 10px;
          }
          
          .contact-item {
            display: flex;
            align-items: center;
            gap: 5px;
          }
          
          .section {
            margin-bottom: 25px;
          }
          
          .section-title {
            font-size: 18px;
            font-weight: bold;
            color: #1f2937;
            border-bottom: 1px solid #e5e7eb;
            padding-bottom: 5px;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 8px;
          }
          
          .section-title::before {
            content: '';
            width: 4px;
            height: 20px;
            background: #2563eb;
            border-radius: 2px;
          }
          
          .summary {
            font-size: 14px;
            line-height: 1.6;
            color: #374151;
            text-align: justify;
          }
          
          .experience-item, .education-item {
            margin-bottom: 20px;
            padding-left: 15px;
            border-left: 3px solid #2563eb;
          }
          
          .experience-header, .education-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 8px;
          }
          
          .job-title, .degree {
            font-weight: bold;
            color: #1f2937;
            font-size: 16px;
          }
          
          .date-range {
            font-size: 12px;
            color: #6b7280;
            white-space: nowrap;
          }
          
          .company, .institution {
            font-weight: 600;
            color: #374151;
            font-size: 14px;
          }
          
          .location {
            color: #6b7280;
            font-size: 12px;
          }
          
          .description {
            font-size: 13px;
            color: #374151;
            margin-bottom: 8px;
            line-height: 1.5;
          }
          
          .achievements {
            list-style-type: disc;
            margin-left: 20px;
            font-size: 12px;
            color: #374151;
          }
          
          .achievements li {
            margin-bottom: 3px;
          }
          
          .skills-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px;
          }
          
          .skill-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 5px 0;
            border-bottom: 1px solid #f3f4f6;
          }
          
          .skill-name {
            font-weight: 500;
            color: #374151;
            font-size: 13px;
          }
          
          .skill-level {
            font-size: 11px;
            color: #6b7280;
            background: #f3f4f6;
            padding: 2px 6px;
            border-radius: 3px;
          }
          
          .canadian-equivalent {
            font-size: 10px;
            color: #9ca3af;
            margin-left: 5px;
          }
          
          .certifications-list, .languages-list {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 5px 0;
            border-bottom: 1px solid #f3f4f6;
          }
          
          .cert-name, .language-name {
            font-weight: 500;
            color: #374151;
            font-size: 13px;
          }
          
          .cert-issuer {
            color: #6b7280;
            font-size: 11px;
          }
          
          .cert-date, .language-level {
            font-size: 11px;
            color: #6b7280;
          }
          
          .additional-info {
            font-size: 13px;
            color: #374151;
            line-height: 1.5;
            text-align: justify;
          }
          
          .footer {
            margin-top: 30px;
            padding-top: 15px;
            border-top: 1px solid #e5e7eb;
            text-align: center;
            font-size: 10px;
            color: #9ca3af;
          }
          
          .ats-score {
            display: inline-block;
            background: #10b981;
            color: white;
            padding: 2px 8px;
            border-radius: 3px;
            font-size: 10px;
            margin-left: 10px;
          }
          
          @media print {
            body {
              -webkit-print-color-adjust: exact;
              color-adjust: exact;
            }
          }
        </style>
      </head>
      <body>
        <div class="container">
          <!-- Header -->
          <div class="header">
            <div class="name">${personalInfo?.name || 'Your Name'}</div>
            <div class="contact-info">
              ${personalInfo?.email ? `<div class="contact-item">📧 ${personalInfo.email}</div>` : ''}
              ${personalInfo?.phone ? `<div class="contact-item">📞 ${personalInfo.phone}</div>` : ''}
              ${personalInfo?.location ? `<div class="contact-item">📍 ${personalInfo.location}</div>` : ''}
            </div>
            <div class="contact-info">
              ${personalInfo?.linkedin ? `<div class="contact-item">🔗 ${personalInfo.linkedin}</div>` : ''}
              ${personalInfo?.website ? `<div class="contact-item">🌐 ${personalInfo.website}</div>` : ''}
            </div>
          </div>

          <!-- Professional Summary -->
          ${professionalSummary?.summary ? `
            <div class="section">
              <div class="section-title">Professional Summary</div>
              <div class="summary">${professionalSummary.summary}</div>
            </div>
          ` : ''}

          <!-- Work Experience -->
          ${workExperience && workExperience.length > 0 ? `
            <div class="section">
              <div class="section-title">Professional Experience</div>
              ${workExperience.map(job => `
                <div class="experience-item">
                  <div class="experience-header">
                    <div class="job-title">${job.title || ''}</div>
                    <div class="date-range">${formatDate(job.startDate)} - ${job.current ? 'Present' : formatDate(job.endDate)}</div>
                  </div>
                  <div class="company">${job.company || ''}${job.location ? ` • ${job.location}` : ''}</div>
                  ${job.description ? `<div class="description">${job.description}</div>` : ''}
                  ${job.achievements && job.achievements.length > 0 ? `
                    <ul class="achievements">
                      ${job.achievements.map(achievement => `<li>${achievement}</li>`).join('')}
                    </ul>
                  ` : ''}
                </div>
              `).join('')}
            </div>
          ` : ''}

          <!-- Skills -->
          ${skills && skills.length > 0 ? `
            <div class="section">
              <div class="section-title">Skills & Competencies</div>
              <div class="skills-grid">
                ${skills.map(skill => `
                  <div class="skill-item">
                    <div class="skill-name">
                      ${skill.name}
                      ${skill.canadianEquivalent ? `<span class="canadian-equivalent">(${skill.canadianEquivalent})</span>` : ''}
                    </div>
                    <div class="skill-level">${getSkillLevel(skill.level)}</div>
                  </div>
                `).join('')}
              </div>
            </div>
          ` : ''}

          <!-- Education -->
          ${education && education.length > 0 ? `
            <div class="section">
              <div class="section-title">Education</div>
              ${education.map(edu => `
                <div class="education-item">
                  <div class="education-header">
                    <div class="degree">${edu.degree || ''}</div>
                    <div class="date-range">${formatDate(edu.startDate)} - ${edu.current ? 'Present' : formatDate(edu.endDate)}</div>
                  </div>
                  <div class="institution">${edu.institution || ''}${edu.location ? ` • ${edu.location}` : ''}</div>
                  ${edu.gpa ? `<div class="description">GPA: ${edu.gpa}</div>` : ''}
                  ${edu.relevantCourses && edu.relevantCourses.length > 0 ? `
                    <div class="description">
                      <strong>Relevant Courses:</strong> ${edu.relevantCourses.join(', ')}
                    </div>
                  ` : ''}
                </div>
              `).join('')}
            </div>
          ` : ''}

          <!-- Certifications -->
          ${certifications && certifications.length > 0 ? `
            <div class="section">
              <div class="section-title">Certifications</div>
              ${certifications.map(cert => `
                <div class="certifications-list">
                  <div>
                    <div class="cert-name">${cert.name}</div>
                    ${cert.issuer ? `<div class="cert-issuer">${cert.issuer}</div>` : ''}
                  </div>
                  <div class="cert-date">${formatDate(cert.date)}</div>
                </div>
              `).join('')}
            </div>
          ` : ''}

          <!-- Languages -->
          ${languages && languages.length > 0 ? `
            <div class="section">
              <div class="section-title">Languages</div>
              ${languages.map(lang => `
                <div class="languages-list">
                  <div class="language-name">${lang.language}</div>
                  <div class="language-level">${lang.proficiency}</div>
                </div>
              `).join('')}
            </div>
          ` : ''}

          <!-- Additional Information -->
          ${additionalInfo ? `
            <div class="section">
              <div class="section-title">Additional Information</div>
              <div class="additional-info">${additionalInfo}</div>
            </div>
          ` : ''}

          <!-- Footer -->
          <div class="footer">
            <div>Generated by ImmiGrowAI - Optimized for Canadian Job Market</div>
            ${atsScore ? `<div>ATS Score: <span class="ats-score">${atsScore}/100</span></div>` : ''}
          </div>
        </div>
      </body>
      </html>
    `;
  }

  /**
   * Generate PDF from URL
   */
  async generatePDFFromURL(url: string, options: PDFOptions = {}): Promise<Buffer> {
    await this.initialize();

    if (!this.browser) {
      throw new Error('Browser not initialized');
    }

    const page = await this.browser.newPage();
    
    try {
      await page.goto(url, {
        waitUntil: 'networkidle0',
        timeout: 30000
      });

      const pdfBuffer = await page.pdf({
        format: options.format || 'A4',
        margin: options.margin || {
          top: '20mm',
          right: '20mm',
          bottom: '20mm',
          left: '20mm'
        },
        printBackground: options.printBackground ?? true,
        preferCSSPageSize: options.preferCSSPageSize ?? true,
        displayHeaderFooter: options.displayHeaderFooter ?? false,
        headerTemplate: options.headerTemplate,
        footerTemplate: options.footerTemplate,
        landscape: options.landscape ?? false
      });

      return pdfBuffer;
    } finally {
      await page.close();
    }
  }

  /**
   * Validate HTML content
   */
  validateHTML(htmlContent: string): boolean {
    try {
      const dom = new JSDOM(htmlContent);
      return dom.window.document.body !== null;
    } catch (error) {
      return false;
    }
  }
}

// Export singleton instance
export const pdfGenerator = new PDFGenerator();
```

## File: src/lib/utils.ts
```typescript
// Consolidated utility functions
import { clsx, type ClassValue } from 'clsx'
import { twMerge } from 'tailwind-merge'

// ===== CLASS NAME UTILITY =====

/**
 * Utility for constructing className strings conditionally
 */
export function cn(...inputs: ClassValue[]) {
  return twMerge(clsx(inputs))
}

// ===== GENERAL HELPERS =====

/**
 * Generate a random ID
 */
export const generateId = (): string => {
  return Math.random().toString(36).substr(2, 9);
};

/**
 * Generate a UUID
 */
export const generateUUID = (): string => {
  return 'xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx'.replace(/[xy]/g, function(c) {
    const r = Math.random() * 16 | 0;
    const v = c == 'x' ? r : (r & 0x3 | 0x8);
    return v.toString(16);
  });
};

/**
 * Deep clone an object
 */
export const deepClone = <T>(obj: T): T => {
  if (obj === null || typeof obj !== 'object') return obj;
  if (obj instanceof Date) return new Date(obj.getTime()) as T;
  if (obj instanceof Array) return obj.map(item => deepClone(item)) as T;
  if (typeof obj === 'object') {
    const clonedObj = {} as T;
    for (const key in obj) {
      if (obj.hasOwnProperty(key)) {
        clonedObj[key] = deepClone(obj[key]);
      }
    }
    return clonedObj;
  }
  return obj;
};

/**
 * Check if object is empty
 */
export const isEmpty = (obj: any): boolean => {
  if (obj == null) return true;
  if (Array.isArray(obj) || typeof obj === 'string') return obj.length === 0;
  if (obj instanceof Map || obj instanceof Set) return obj.size === 0;
  if (typeof obj === 'object') return Object.keys(obj).length === 0;
  return false;
};

/**
 * Get nested object property safely
 */
export const getNestedValue = (obj: any, path: string, defaultValue?: any): any => {
  const keys = path.split('.');
  let result = obj;
  
  for (const key of keys) {
    if (result == null || typeof result !== 'object') {
      return defaultValue;
    }
    result = result[key];
  }
  
  return result !== undefined ? result : defaultValue;
};

// ===== PERFORMANCE HELPERS =====

/**
 * Debounce function
 */
export const debounce = <T extends (...args: any[]) => any>(
  func: T,
  wait: number
): ((...args: Parameters<T>) => void) => {
  let timeout: NodeJS.Timeout;
  return (...args: Parameters<T>) => {
    clearTimeout(timeout);
    timeout = setTimeout(() => func(...args), wait);
  };
};

/**
 * Throttle function
 */
export const throttle = <T extends (...args: any[]) => any>(
  func: T,
  limit: number
): ((...args: Parameters<T>) => void) => {
  let inThrottle: boolean;
  return (...args: Parameters<T>) => {
    if (!inThrottle) {
      func(...args);
      inThrottle = true;
      setTimeout(() => inThrottle = false, limit);
    }
  };
};

/**
 * Memoize function results
 */
export const memoize = <T extends (...args: any[]) => any>(
  func: T
): T => {
  const cache = new Map();
  return ((...args: Parameters<T>) => {
    const key = JSON.stringify(args);
    if (cache.has(key)) {
      return cache.get(key);
    }
    const result = func(...args);
    cache.set(key, result);
    return result;
  }) as T;
};

// ===== STRING HELPERS =====

/**
 * Capitalize first letter
 */
export const capitalize = (str: string): string => {
  return str.charAt(0).toUpperCase() + str.slice(1);
};

/**
 * Convert to title case
 */
export const toTitleCase = (str: string): string => {
  return str.replace(/\w\S*/g, (txt) => 
    txt.charAt(0).toUpperCase() + txt.substr(1).toLowerCase()
  );
};

/**
 * Truncate string with ellipsis
 */
export const truncate = (str: string, length: number): string => {
  if (str.length <= length) return str;
  return str.slice(0, length) + '...';
};

/**
 * Convert string to slug
 */
export const toSlug = (str: string): string => {
  return str
    .toLowerCase()
    .replace(/[^\w ]+/g, '')
    .replace(/ +/g, '-');
};

// ===== DATE HELPERS =====

/**
 * Format date to readable string
 */
export const formatDate = (date: Date | string): string => {
  const d = new Date(date);
  return d.toLocaleDateString('en-US', {
    year: 'numeric',
    month: 'long',
    day: 'numeric'
  });
};

/**
 * Format date to relative time
 */
export const formatRelativeTime = (date: Date | string): string => {
  const now = new Date();
  const d = new Date(date);
  const diffInSeconds = Math.floor((now.getTime() - d.getTime()) / 1000);

  if (diffInSeconds < 60) return 'just now';
  if (diffInSeconds < 3600) return `${Math.floor(diffInSeconds / 60)}m ago`;
  if (diffInSeconds < 86400) return `${Math.floor(diffInSeconds / 3600)}h ago`;
  if (diffInSeconds < 2592000) return `${Math.floor(diffInSeconds / 86400)}d ago`;
  if (diffInSeconds < 31536000) return `${Math.floor(diffInSeconds / 2592000)}mo ago`;
  return `${Math.floor(diffInSeconds / 31536000)}y ago`;
};

/**
 * Check if date is today
 */
export const isToday = (date: Date | string): boolean => {
  const today = new Date();
  const d = new Date(date);
  return d.toDateString() === today.toDateString();
};

// ===== VALIDATION HELPERS =====

/**
 * Validate email format
 */
export const isValidEmail = (email: string): boolean => {
  const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  return emailRegex.test(email);
};

/**
 * Validate URL format
 */
export const isValidUrl = (url: string): boolean => {
  try {
    new URL(url);
    return true;
  } catch {
    return false;
  }
};

/**
 * Validate phone number format
 */
export const isValidPhone = (phone: string): boolean => {
  const phoneRegex = /^[\+]?[1-9][\d]{0,15}$/;
  return phoneRegex.test(phone.replace(/\s/g, ''));
};

// ===== ARRAY HELPERS =====

/**
 * Remove duplicates from array
 */
export const unique = <T>(arr: T[]): T[] => {
  return [...new Set(arr)];
};

/**
 * Group array by key
 */
export const groupBy = <T>(arr: T[], key: keyof T): Record<string, T[]> => {
  return arr.reduce((groups, item) => {
    const group = String(item[key]);
    groups[group] = groups[group] || [];
    groups[group].push(item);
    return groups;
  }, {} as Record<string, T[]>);
};

/**
 * Sort array by key
 */
export const sortBy = <T>(arr: T[], key: keyof T, direction: 'asc' | 'desc' = 'asc'): T[] => {
  return [...arr].sort((a, b) => {
    const aVal = a[key];
    const bVal = b[key];
    
    if (aVal < bVal) return direction === 'asc' ? -1 : 1;
    if (aVal > bVal) return direction === 'asc' ? 1 : -1;
    return 0;
  });
};

/**
 * Chunk array into smaller arrays
 */
export const chunk = <T>(arr: T[], size: number): T[][] => {
  const chunks: T[][] = [];
  for (let i = 0; i < arr.length; i += size) {
    chunks.push(arr.slice(i, i + size));
  }
  return chunks;
};

// ===== OBJECT HELPERS =====

/**
 * Pick specific keys from object
 */
export const pick = <T, K extends keyof T>(obj: T, keys: K[]): Pick<T, K> => {
  const result = {} as Pick<T, K>;
  keys.forEach(key => {
    if (key in obj) {
      result[key] = obj[key];
    }
  });
  return result;
};

/**
 * Omit specific keys from object
 */
export const omit = <T, K extends keyof T>(obj: T, keys: K[]): Omit<T, K> => {
  const result = { ...obj };
  keys.forEach(key => {
    delete result[key];
  });
  return result;
};

/**
 * Merge objects deeply
 */
export const merge = <T extends Record<string, any>>(target: T, ...sources: Partial<T>[]): T => {
  const result = { ...target };
  
  sources.forEach(source => {
    Object.keys(source).forEach(key => {
      const value = source[key];
      if (value && typeof value === 'object' && !Array.isArray(value)) {
        result[key] = merge(result[key] || {}, value);
      } else {
        result[key] = value;
      }
    });
  });
  
  return result;
};

// ===== FILE HELPERS =====

/**
 * Format file size
 */
export const formatFileSize = (bytes: number): string => {
  if (bytes === 0) return '0 Bytes';
  
  const k = 1024;
  const sizes = ['Bytes', 'KB', 'MB', 'GB', 'TB'];
  const i = Math.floor(Math.log(bytes) / Math.log(k));
  
  return parseFloat((bytes / Math.pow(k, i)).toFixed(2)) + ' ' + sizes[i];
};

/**
 * Get file extension
 */
export const getFileExtension = (filename: string): string => {
  return filename.slice((filename.lastIndexOf('.') - 1 >>> 0) + 2);
};

/**
 * Check if file is image
 */
export const isImageFile = (filename: string): boolean => {
  const imageExtensions = ['jpg', 'jpeg', 'png', 'gif', 'webp', 'svg'];
  const ext = getFileExtension(filename).toLowerCase();
  return imageExtensions.includes(ext);
};

// ===== COLOR HELPERS =====

/**
 * Convert hex to RGB
 */
export const hexToRgb = (hex: string): { r: number; g: number; b: number } | null => {
  const result = /^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i.exec(hex);
  return result ? {
    r: parseInt(result[1], 16),
    g: parseInt(result[2], 16),
    b: parseInt(result[3], 16)
  } : null;
};

/**
 * Convert RGB to hex
 */
export const rgbToHex = (r: number, g: number, b: number): string => {
  return '#' + [r, g, b].map(x => {
    const hex = x.toString(16);
    return hex.length === 1 ? '0' + hex : hex;
  }).join('');
};

// ===== ERROR HANDLING =====

/**
 * Safe JSON parse
 */
export const safeJsonParse = <T>(str: string, fallback: T): T => {
  try {
    return JSON.parse(str);
  } catch {
    return fallback;
  }
};

/**
 * Safe function execution
 */
export const safeExecute = <T>(fn: () => T, fallback: T): T => {
  try {
    return fn();
  } catch {
    return fallback;
  }
};

// ===== BROWSER HELPERS =====

/**
 * Copy text to clipboard
 */
export const copyToClipboard = async (text: string): Promise<boolean> => {
  try {
    await navigator.clipboard.writeText(text);
    return true;
  } catch {
    // Fallback for older browsers
    const textArea = document.createElement('textarea');
    textArea.value = text;
    document.body.appendChild(textArea);
    textArea.select();
    const success = document.execCommand('copy');
    document.body.removeChild(textArea);
    return success;
  }
};

/**
 * Download file
 */
export const downloadFile = (url: string, filename: string): void => {
  const link = document.createElement('a');
  link.href = url;
  link.download = filename;
  document.body.appendChild(link);
  link.click();
  document.body.removeChild(link);
};

/**
 * Check if element is in viewport
 */
export const isInViewport = (element: Element): boolean => {
  const rect = element.getBoundingClientRect();
  return (
    rect.top >= 0 &&
    rect.left >= 0 &&
    rect.bottom <= (window.innerHeight || document.documentElement.clientHeight) &&
    rect.right <= (window.innerWidth || document.documentElement.clientWidth)
  );
};
```

## File: src/middleware.ts
```typescript
import { NextResponse } from 'next/server'
import type { NextRequest } from 'next/server'

// Simplified middleware - no authentication required
export async function middleware(request: NextRequest) {
  // Allow all requests to pass through without authentication
  return NextResponse.next()
}
 
export const config = {
  matcher: [
    // Empty matcher - no routes require authentication
  ],
}
```

## File: src/stores/authStore.ts
```typescript
import { create } from 'zustand'
import { persist, subscribeWithSelector } from 'zustand/middleware'
import { AuthStore, RegisterData } from './types'
import type { User, LoginCredentials } from '@/types/auth'

// Default user preferences
const defaultUserPreferences = {
  theme: 'system' as const,
  language: 'en',
  timezone: 'UTC',
  emailNotifications: true,
  pushNotifications: true,
  privacySettings: {
    profileVisibility: 'public' as const,
    showEmail: false,
    showPhone: false,
  },
}

// Initial state
const initialState = {
  user: null,
  isAuthenticated: false,
  isLoading: false,
  error: null,
  token: null,
}

// Auth store implementation
export const useAuthStore = create<AuthStore>()(
  subscribeWithSelector(
    persist(
      (set, get) => ({
        ...initialState,

        // Actions
        login: async (credentials: LoginCredentials) => {
          set({ isLoading: true, error: null })
          
          try {
            // TODO: Replace with actual API call
            const response = await fetch('/api/auth/login', {
              method: 'POST',
              headers: {
                'Content-Type': 'application/json',
              },
              body: JSON.stringify(credentials),
            })

            if (!response.ok) {
              throw new Error('Login failed')
            }

            const data = await response.json()
            
            set({
              user: data.user,
              token: data.token,
              isAuthenticated: true,
              isLoading: false,
              error: null,
            })
          } catch (error) {
            set({
              isLoading: false,
              error: error instanceof Error ? error.message : 'Login failed',
            })
            throw error
          }
        },

        logout: () => {
          set({
            user: null,
            token: null,
            isAuthenticated: false,
            error: null,
          })
          
          // Clear any stored data
          localStorage.removeItem('auth-token')
          sessionStorage.clear()
        },

        register: async (userData: RegisterData) => {
          set({ isLoading: true, error: null })
          
          try {
            // TODO: Replace with actual API call
            const response = await fetch('/api/auth/register', {
              method: 'POST',
              headers: {
                'Content-Type': 'application/json',
              },
              body: JSON.stringify(userData),
            })

            if (!response.ok) {
              throw new Error('Registration failed')
            }

            const data = await response.json()
            
            set({
              user: data.user,
              token: data.token,
              isAuthenticated: true,
              isLoading: false,
              error: null,
            })
          } catch (error) {
            set({
              isLoading: false,
              error: error instanceof Error ? error.message : 'Registration failed',
            })
            throw error
          }
        },

        setUser: (user: User | null) => {
          set({
            user,
            isAuthenticated: !!user,
          })
        },

        setToken: (token: string | null) => {
          set({ token })
          
          if (token) {
            localStorage.setItem('auth-token', token)
          } else {
            localStorage.removeItem('auth-token')
          }
        },

        setLoading: (loading: boolean) => {
          set({ isLoading: loading })
        },

        setError: (error: string | null) => {
          set({ error })
        },

        clearError: () => {
          set({ error: null })
        },
      }),
      {
        name: 'auth-storage',
        partialize: (state) => ({
          user: state.user,
          token: state.token,
          isAuthenticated: state.isAuthenticated,
        }),
        onRehydrateStorage: () => (state) => {
          // Rehydrate token from localStorage if not in state
          if (state && !state.token) {
            const storedToken = localStorage.getItem('auth-token')
            if (storedToken) {
              state.setToken(storedToken)
            }
          }
        },
      }
    )
  )
)

// Selectors for better performance
export const useAuthUser = () => useAuthStore((state) => state.user)
export const useAuthToken = () => useAuthStore((state) => state.token)
export const useIsAuthenticated = () => useAuthStore((state) => state.isAuthenticated)
export const useAuthLoading = () => useAuthStore((state) => state.isLoading)
export const useAuthError = () => useAuthStore((state) => state.error)

// Actions
export const useAuthActions = () => useAuthStore((state) => ({
  login: state.login,
  logout: state.logout,
  register: state.register,
  setUser: state.setUser,
  setToken: state.setToken,
  setLoading: state.setLoading,
  setError: state.setError,
  clearError: state.clearError,
}))
```

## File: src/stores/index.ts
```typescript
// State management stores exports
export * from './authStore';
export * from './userStore';
export * from './types';

// Main store hooks for easy access
export { useAuthStore } from './authStore'
export { useUIStore } from './uiStore'
export { useCareerStore } from './careerStore'
export { useUserStore } from './userStore'

// Re-export commonly used hooks
export {
  // Auth hooks
  useAuthUser,
  useAuthToken,
  useIsAuthenticated,
  useAuthLoading,
  useAuthError,
  useAuthActions,
} from './authStore'

export {
  // UI hooks
  useTheme,
  useSidebarOpen,
  useModals,
  useToasts,
  useLoadingStates,
  useModal,
  useLoading,
  useUIActions,
  useThemeActions,
  useSidebarActions,
  useModalActions,
  useToastActions,
  useLoadingActions,
} from './uiStore'

export {
  // Career hooks
  useCareerProfile,
  useJobSearchResults,
  useSavedJobs,
  useApplications,
  useCareerLoading,
  useCareerError,
  useSavedJob,
  useApplication,
  useJobApplication,
  useCareerActions,
  useCareerProfileActions,
  useJobSearchActions,
  useSavedJobActions,
  useApplicationActions,
} from './careerStore'

export {
  // User hooks
  useUserProfile,
  useUserPreferences,
  useNotifications,
  useUserLoading,
  useUserError,
  useUnreadNotifications,
  useNotificationCount,
  useUnreadNotificationCount,
  useUserTheme,
  useUserLanguage,
  useUserTimezone,
  useEmailNotifications,
  usePushNotifications,
  usePrivacySettings,
  useUserActions,
  useUserProfileActions,
  useUserPreferencesActions,
  useNotificationActions,
} from './userStore'
```

## File: src/stores/resumeGeneratorStore.ts
```typescript
import { create } from 'zustand'
import { persist, subscribeWithSelector } from 'zustand/middleware'
import { ResumeGeneratorState, ResumeGeneratorActions, ResumeGeneratorStore } from './types'

// Initial state
const initialState: ResumeGeneratorState = {
  // Resume selection state
  selectedResumeId: null,
  availableResumes: [],
  
  // Job targeting state
  jobTargeting: {
    jobTitle: '',
    companyName: '',
    jobDescription: '',
    industry: '',
    location: '',
    salaryRange: null,
    requiredSkills: [],
    preferredSkills: [],
    experienceLevel: null
  },
  
  // Generation state
  isGenerating: false,
  generationProgress: 0,
  generationStatus: '',
  generationError: null,
  
  // Generated resumes
  generatedResumes: [],
  currentResume: null,
  
  // Editor state
  isEditing: false,
  userEdits: {},
  autoSaveStatus: 'idle', // 'idle' | 'saving' | 'saved' | 'error'
  lastSaved: null,
  
  // AI suggestions
  aiSuggestions: [],
  appliedSuggestions: [],
  
  // Search and filters
  searchQuery: '',
  filters: {
    jobTitle: '',
    companyName: '',
    industry: '',
    status: 'all',
    dateRange: null
  },
  
  // Pagination
  pagination: {
    page: 1,
    limit: 20,
    total: 0,
    totalPages: 0
  },
  
  // Loading states
  isLoading: false,
  error: null
}

// Resume generator store implementation
export const useResumeGeneratorStore = create<ResumeGeneratorStore>()(
  subscribeWithSelector(
    persist(
      (set, get) => ({
        ...initialState,

        // Resume Selection Actions
        setSelectedResumeId: (resumeId: string | null) => {
          set({ selectedResumeId: resumeId })
        },

        setAvailableResumes: (resumes: any[]) => {
          set({ availableResumes: resumes })
        },

        // Job Targeting Actions
        setJobTargeting: (targeting: Partial<typeof initialState.jobTargeting>) => {
          set(state => ({
            jobTargeting: { ...state.jobTargeting, ...targeting }
          }))
        },

        resetJobTargeting: () => {
          set({ jobTargeting: initialState.jobTargeting })
        },

        validateJobTargeting: () => {
          const state = get()
          const { jobTargeting } = state
          
          const errors: string[] = []
          
          // Required fields
          if (!jobTargeting.jobTitle?.trim()) {
            errors.push('Job title is required')
          }
          
          if (!jobTargeting.jobDescription?.trim()) {
            errors.push('Job description is required')
          }
          
          if (!jobTargeting.industry?.trim()) {
            errors.push('Industry is required')
          }
          
          if (!jobTargeting.location?.trim()) {
            errors.push('Location is required')
          }
          
          if (!jobTargeting.experienceLevel) {
            errors.push('Experience level is required')
          }
          
          return {
            isValid: errors.length === 0,
            errors,
            warnings: []
          }
        },

        // Generation Actions
        startGeneration: () => {
          set({
            isGenerating: true,
            generationProgress: 0,
            generationStatus: 'Starting generation...',
            generationError: null
          })
        },

        updateGenerationProgress: (progress: number, status: string) => {
          set({
            generationProgress: progress,
            generationStatus: status
          })
        },

        completeGeneration: (resume: any) => {
          set({
            isGenerating: false,
            generationProgress: 100,
            generationStatus: 'Generation completed!',
            currentResume: resume,
            generatedResumes: [resume, ...get().generatedResumes]
          })
        },

        failGeneration: (error: string) => {
          set({
            isGenerating: false,
            generationError: error,
            generationStatus: 'Generation failed'
          })
        },

        resetGeneration: () => {
          set({
            isGenerating: false,
            generationProgress: 0,
            generationStatus: '',
            generationError: null
          })
        },

        // Additional generation helpers
        setGenerationProgress: (progress: number) => {
          set({ generationProgress: progress })
        },

        setGenerationStatus: (status: string) => {
          set({ generationStatus: status })
        },

        setGenerationError: (error: string | null) => {
          set({ generationError: error })
        },

        setIsGenerating: (isGenerating: boolean) => {
          set({ isGenerating })
        },

        // Generated Resumes Actions
        setGeneratedResumes: (resumes: any[]) => {
          set({ generatedResumes: resumes })
        },

        addGeneratedResume: (resume: any) => {
          set(state => ({
            generatedResumes: [resume, ...state.generatedResumes]
          }))
        },

        updateGeneratedResume: (resumeId: string, updates: any) => {
          set(state => ({
            generatedResumes: state.generatedResumes.map(resume =>
              resume.id === resumeId ? { ...resume, ...updates } : resume
            ),
            currentResume: state.currentResume?.id === resumeId
              ? { ...state.currentResume, ...updates }
              : state.currentResume
          }))
        },

        deleteGeneratedResume: (resumeId: string) => {
          set(state => ({
            generatedResumes: state.generatedResumes.filter(resume => resume.id !== resumeId),
            currentResume: state.currentResume?.id === resumeId ? null : state.currentResume
          }))
        },

        setCurrentResume: (resume: any) => {
          set({ currentResume: resume })
        },

        // Editor Actions
        startEditing: () => {
          set({ isEditing: true })
        },

        stopEditing: () => {
          set({ isEditing: false })
        },

        updateUserEdits: (edits: any) => {
          set(state => ({
            userEdits: { ...state.userEdits, ...edits }
          }))
        },

        resetUserEdits: () => {
          set({ userEdits: {} })
        },

        setAutoSaveStatus: (status: 'idle' | 'saving' | 'saved' | 'error') => {
          set({ autoSaveStatus: status })
        },

        setLastSaved: (timestamp: Date) => {
          set({ lastSaved: timestamp })
        },

        // AI Suggestions Actions
        setAISuggestions: (suggestions: any[]) => {
          set({ aiSuggestions: suggestions })
        },

        applySuggestion: (suggestionId: string) => {
          const suggestion = get().aiSuggestions.find(s => s.id === suggestionId)
          if (suggestion) {
            set(state => ({
              appliedSuggestions: [...state.appliedSuggestions, suggestion],
              userEdits: { ...state.userEdits, ...suggestion.changes }
            }))
          }
        },

        rejectSuggestion: (suggestionId: string) => {
          set(state => ({
            aiSuggestions: state.aiSuggestions.filter(s => s.id !== suggestionId)
          }))
        },

        clearSuggestions: () => {
          set({ aiSuggestions: [], appliedSuggestions: [] })
        },

        // Search and Filter Actions
        setSearchQuery: (query: string) => {
          set({ searchQuery: query })
        },

        setFilters: (filters: Partial<typeof initialState.filters>) => {
          set(state => ({
            filters: { ...state.filters, ...filters }
          }))
        },

        resetFilters: () => {
          set({ filters: initialState.filters })
        },

        // Pagination Actions
        setPagination: (pagination: Partial<typeof initialState.pagination>) => {
          set(state => ({
            pagination: { ...state.pagination, ...pagination }
          }))
        },

        setPage: (page: number) => {
          set(state => ({
            pagination: { ...state.pagination, page }
          }))
        },

        // Loading and Error Actions
        setLoading: (loading: boolean) => {
          set({ isLoading: loading })
        },

        setError: (error: string | null) => {
          set({ error })
        },

        clearError: () => {
          set({ error: null })
        },

        // Utility Actions
        reset: () => {
          set(initialState)
        },

        // Persistence helpers
        saveToLocalStorage: () => {
          const state = get()
          localStorage.setItem('resumeGeneratorState', JSON.stringify({
            selectedResumeId: state.selectedResumeId,
            jobTargeting: state.jobTargeting,
            userEdits: state.userEdits,
            filters: state.filters
          }))
        },

        loadFromLocalStorage: () => {
          try {
            const saved = localStorage.getItem('resumeGeneratorState')
            if (saved) {
              const parsed = JSON.parse(saved)
              set(parsed)
            }
          } catch (error) {
            console.error('Failed to load resume generator state:', error)
          }
        }
      }),
      {
        name: 'resume-generator-store',
        partialize: (state) => ({
          selectedResumeId: state.selectedResumeId,
          jobTargeting: state.jobTargeting,
          userEdits: state.userEdits,
          filters: state.filters,
          pagination: state.pagination
        })
      }
    )
  )
)

// Export store hooks for specific functionality
export const useResumeSelection = () => useResumeGeneratorStore(state => ({
  selectedResumeId: state.selectedResumeId,
  availableResumes: state.availableResumes,
  setSelectedResumeId: state.setSelectedResumeId,
  setAvailableResumes: state.setAvailableResumes
}))

export const useJobTargeting = () => useResumeGeneratorStore(state => ({
  jobTargeting: state.jobTargeting,
  setJobTargeting: state.setJobTargeting,
  resetJobTargeting: state.resetJobTargeting
}))

export const useGeneration = () => useResumeGeneratorStore(state => ({
  isGenerating: state.isGenerating,
  generationProgress: state.generationProgress,
  generationStatus: state.generationStatus,
  generationError: state.generationError,
  startGeneration: state.startGeneration,
  updateGenerationProgress: state.updateGenerationProgress,
  completeGeneration: state.completeGeneration,
  failGeneration: state.failGeneration,
  resetGeneration: state.resetGeneration
}))

export const useGeneratedResumes = () => useResumeGeneratorStore(state => ({
  generatedResumes: state.generatedResumes,
  currentResume: state.currentResume,
  setGeneratedResumes: state.setGeneratedResumes,
  addGeneratedResume: state.addGeneratedResume,
  updateGeneratedResume: state.updateGeneratedResume,
  deleteGeneratedResume: state.deleteGeneratedResume,
  setCurrentResume: state.setCurrentResume
}))

export const useEditor = () => useResumeGeneratorStore(state => ({
  isEditing: state.isEditing,
  userEdits: state.userEdits,
  autoSaveStatus: state.autoSaveStatus,
  lastSaved: state.lastSaved,
  startEditing: state.startEditing,
  stopEditing: state.stopEditing,
  updateUserEdits: state.updateUserEdits,
  resetUserEdits: state.resetUserEdits,
  setAutoSaveStatus: state.setAutoSaveStatus,
  setLastSaved: state.setLastSaved
}))

export const useAISuggestions = () => useResumeGeneratorStore(state => ({
  aiSuggestions: state.aiSuggestions,
  appliedSuggestions: state.appliedSuggestions,
  setAISuggestions: state.setAISuggestions,
  applySuggestion: state.applySuggestion,
  rejectSuggestion: state.rejectSuggestion,
  clearSuggestions: state.clearSuggestions
}))

export const useSearchAndFilters = () => useResumeGeneratorStore(state => ({
  searchQuery: state.searchQuery,
  filters: state.filters,
  pagination: state.pagination,
  setSearchQuery: state.setSearchQuery,
  setFilters: state.setFilters,
  resetFilters: state.resetFilters,
  setPagination: state.setPagination,
  setPage: state.setPage
}))
```

## File: src/stores/types.ts
```typescript
// Store type definitions for Zustand stores
import type { User, LoginCredentials } from '@/types/auth'

// Auth Store Types
export interface AuthState {
  user: User | null
  isAuthenticated: boolean
  isLoading: boolean
  error: string | null
  token: string | null
}

export interface AuthActions {
  login: (credentials: LoginCredentials) => Promise<void>
  logout: () => void
  register: (userData: RegisterData) => Promise<void>
  setUser: (user: User | null) => void
  setToken: (token: string | null) => void
  setLoading: (loading: boolean) => void
  setError: (error: string | null) => void
  clearError: () => void
}

export interface AuthStore extends AuthState, AuthActions {}

// UI Store Types
export interface UIState {
  theme: 'light' | 'dark' | 'system'
  sidebarOpen: boolean
  modals: {
    [key: string]: boolean
  }
  toasts: Toast[]
  loadingStates: {
    [key: string]: boolean
  }
}

export interface UIActions {
  setTheme: (theme: 'light' | 'dark' | 'system') => void
  toggleSidebar: () => void
  setSidebarOpen: (open: boolean) => void
  openModal: (modalId: string) => void
  closeModal: (modalId: string) => void
  addToast: (toast: Omit<Toast, 'id'>) => void
  removeToast: (id: string) => void
  setLoading: (key: string, loading: boolean) => void
  clearLoading: (key: string) => void
}

export interface UIStore extends UIState, UIActions {}

// Career Store Types
export interface CareerState {
  careerProfile: CareerProfile | null
  jobSearchResults: JobSearchResult[]
  savedJobs: SavedJob[]
  applications: JobApplication[]
  isLoading: boolean
  error: string | null
}

export interface CareerActions {
  setCareerProfile: (profile: CareerProfile | null) => void
  updateCareerProfile: (updates: Partial<CareerProfile>) => void
  setJobSearchResults: (results: JobSearchResult[]) => void
  addSavedJob: (job: SavedJob) => void
  removeSavedJob: (jobId: string) => void
  addApplication: (application: JobApplication) => void
  setLoading: (loading: boolean) => void
  setError: (error: string | null) => void
  clearError: () => void
}

export interface CareerStore extends CareerState, CareerActions {}

// User Store Types
export interface UserState {
  profile: UserProfile | null
  preferences: UserPreferences
  notifications: Notification[]
  isLoading: boolean
  error: string | null
}

export interface UserActions {
  setProfile: (profile: UserProfile | null) => void
  updateProfile: (updates: Partial<UserProfile>) => void
  setPreferences: (preferences: UserPreferences) => void
  addNotification: (notification: Notification) => void
  removeNotification: (id: string) => void
  markNotificationAsRead: (id: string) => void
  setLoading: (loading: boolean) => void
  setError: (error: string | null) => void
  clearError: () => void
}

export interface UserStore extends UserState, UserActions {}

// Resume Generator Store Types
export interface ResumeGeneratorState {
  // Resume selection state
  selectedResumeId: string | null
  availableResumes: any[]
  
  // Job targeting state
  jobTargeting: {
    jobTitle: string
    companyName: string
    jobDescription: string
    industry: string
    location: string
    salaryRange: { min: number; max: number } | null
    requiredSkills: string[]
    preferredSkills: string[]
    experienceLevel: 'entry' | 'mid' | 'senior' | 'executive' | null
  }
  
  // Generation state
  isGenerating: boolean
  generationProgress: number
  generationStatus: string
  generationError: string | null
  
  // Generated resumes
  generatedResumes: any[]
  currentResume: any | null
  
  // Editor state
  isEditing: boolean
  userEdits: Record<string, any>
  autoSaveStatus: 'idle' | 'saving' | 'saved' | 'error'
  lastSaved: Date | null
  
  // AI suggestions
  aiSuggestions: any[]
  appliedSuggestions: any[]
  
  // Search and filters
  searchQuery: string
  filters: {
    jobTitle: string
    companyName: string
    industry: string
    status: string
    dateRange: { start: Date; end: Date } | null
  }
  
  // Pagination
  pagination: {
    page: number
    limit: number
    total: number
    totalPages: number
  }
  
  // Loading states
  isLoading: boolean
  error: string | null
}

export interface ResumeGeneratorActions {
  // Resume Selection Actions
  setSelectedResumeId: (resumeId: string | null) => void
  setAvailableResumes: (resumes: any[]) => void
  
  // Job Targeting Actions
  setJobTargeting: (targeting: Partial<ResumeGeneratorState['jobTargeting']>) => void
  resetJobTargeting: () => void
  validateJobTargeting: () => { isValid: boolean; errors: string[]; warnings: string[] }
  
  // Generation Actions
  startGeneration: () => void
  updateGenerationProgress: (progress: number, status: string) => void
  completeGeneration: (resume: any) => void
  failGeneration: (error: string) => void
  resetGeneration: () => void
  setGenerationProgress: (progress: number) => void
  setGenerationStatus: (status: string) => void
  setGenerationError: (error: string | null) => void
  setIsGenerating: (isGenerating: boolean) => void
  
  // Generated Resumes Actions
  setGeneratedResumes: (resumes: any[]) => void
  addGeneratedResume: (resume: any) => void
  updateGeneratedResume: (resumeId: string, updates: any) => void
  deleteGeneratedResume: (resumeId: string) => void
  setCurrentResume: (resume: any) => void
  
  // Editor Actions
  startEditing: () => void
  stopEditing: () => void
  updateUserEdits: (edits: any) => void
  resetUserEdits: () => void
  setAutoSaveStatus: (status: 'idle' | 'saving' | 'saved' | 'error') => void
  setLastSaved: (timestamp: Date) => void
  
  // AI Suggestions Actions
  setAISuggestions: (suggestions: any[]) => void
  applySuggestion: (suggestionId: string) => void
  rejectSuggestion: (suggestionId: string) => void
  clearSuggestions: () => void
  
  // Search and Filter Actions
  setSearchQuery: (query: string) => void
  setFilters: (filters: Partial<ResumeGeneratorState['filters']>) => void
  resetFilters: () => void
  
  // Pagination Actions
  setPagination: (pagination: Partial<ResumeGeneratorState['pagination']>) => void
  setPage: (page: number) => void
  
  // Loading and Error Actions
  setLoading: (loading: boolean) => void
  setError: (error: string | null) => void
  clearError: () => void
  
  // Utility Actions
  reset: () => void
  saveToLocalStorage: () => void
  loadFromLocalStorage: () => void
}

export interface ResumeGeneratorStore extends ResumeGeneratorState, ResumeGeneratorActions {}

// Common Types
export interface User {
  id: string
  email: string
  name: string
  avatar?: string
  role: 'user' | 'admin'
  createdAt: string
  updatedAt: string
}

export interface LoginCredentials {
  email: string
  password: string
}

export interface RegisterData {
  email: string
  password: string
  name: string
}

export interface Toast {
  id: string
  type: 'success' | 'error' | 'warning' | 'info'
  title: string
  message?: string
  duration?: number
}

export interface CareerProfile {
  id: string
  userId: string
  title: string
  summary: string
  skills: string[]
  experience: Experience[]
  education: Education[]
  certifications: Certification[]
  languages: Language[]
  createdAt: string
  updatedAt: string
}

export interface JobSearchResult {
  id: string
  title: string
  company: string
  location: string
  description: string
  requirements: string[]
  salary?: {
    min: number
    max: number
    currency: string
  }
  type: 'full-time' | 'part-time' | 'contract' | 'internship'
  remote: boolean
  postedAt: string
  applicationDeadline?: string
}

export interface SavedJob {
  id: string
  jobId: string
  userId: string
  savedAt: string
  job: JobSearchResult
}

export interface JobApplication {
  id: string
  jobId: string
  userId: string
  status: 'pending' | 'reviewed' | 'interviewed' | 'accepted' | 'rejected'
  appliedAt: string
  updatedAt: string
  job: JobSearchResult
}

export interface UserProfile {
  id: string
  userId: string
  firstName: string
  lastName: string
  avatar?: string
  bio?: string
  phone?: string
  location?: string
  website?: string
  socialLinks: {
    linkedin?: string
    github?: string
    twitter?: string
  }
  createdAt: string
  updatedAt: string
}

export interface UserPreferences {
  theme: 'light' | 'dark' | 'system'
  language: string
  timezone: string
  emailNotifications: boolean
  pushNotifications: boolean
  privacySettings: {
    profileVisibility: 'public' | 'private' | 'connections'
    showEmail: boolean
    showPhone: boolean
  }
}

export interface Notification {
  id: string
  userId: string
  type: 'info' | 'success' | 'warning' | 'error'
  title: string
  message: string
  read: boolean
  createdAt: string
  actionUrl?: string
}

export interface Experience {
  id: string
  title: string
  company: string
  location: string
  startDate: string
  endDate?: string
  current: boolean
  description: string
}

export interface Education {
  id: string
  degree: string
  institution: string
  field: string
  startDate: string
  endDate?: string
  current: boolean
  gpa?: number
}

export interface Certification {
  id: string
  name: string
  issuer: string
  issueDate: string
  expiryDate?: string
  credentialId?: string
  url?: string
}

export interface Language {
  id: string
  name: string
  proficiency: 'beginner' | 'intermediate' | 'advanced' | 'native'
}
```

## File: src/stores/userStore.ts
```typescript
import { create } from 'zustand'
import { persist, subscribeWithSelector } from 'zustand/middleware'
import { UserStore, UserProfile, UserPreferences, Notification } from './types'

// Default user preferences
const defaultUserPreferences: UserPreferences = {
  theme: 'system',
  language: 'en',
  timezone: 'UTC',
  emailNotifications: true,
  pushNotifications: true,
  privacySettings: {
    profileVisibility: 'public',
    showEmail: false,
    showPhone: false,
  },
}

// Initial state
const initialState = {
  profile: null,
  preferences: defaultUserPreferences,
  notifications: [],
  isLoading: false,
  error: null,
}

// User store implementation
export const useUserStore = create<UserStore>()(
  subscribeWithSelector(
    persist(
      (set, get) => ({
        ...initialState,

        // Profile actions
        setProfile: (profile: UserProfile | null) => {
          set({ profile })
        },

        updateProfile: (updates: Partial<UserProfile>) => {
          set((state) => ({
            profile: state.profile
              ? { ...state.profile, ...updates }
              : null,
          }))
        },

        // Preferences actions
        setPreferences: (preferences: UserPreferences) => {
          set({ preferences })
        },

        // Notification actions
        addNotification: (notification: Notification) => {
          set((state) => ({
            notifications: [notification, ...state.notifications],
          }))
        },

        removeNotification: (id: string) => {
          set((state) => ({
            notifications: state.notifications.filter((notification) => notification.id !== id),
          }))
        },

        markNotificationAsRead: (id: string) => {
          set((state) => ({
            notifications: state.notifications.map((notification) =>
              notification.id === id
                ? { ...notification, read: true }
                : notification
            ),
          }))
        },

        // Loading and error actions
        setLoading: (loading: boolean) => {
          set({ isLoading: loading })
        },

        setError: (error: string | null) => {
          set({ error })
        },

        clearError: () => {
          set({ error: null })
        },
      }),
      {
        name: 'user-storage',
        partialize: (state) => ({
          profile: state.profile,
          preferences: state.preferences,
          notifications: state.notifications,
        }),
      }
    )
  )
)

// Selectors for better performance
export const useUserProfile = () => useUserStore((state) => state.profile)
export const useUserPreferences = () => useUserStore((state) => state.preferences)
export const useNotifications = () => useUserStore((state) => state.notifications)
export const useUserLoading = () => useUserStore((state) => state.isLoading)
export const useUserError = () => useUserStore((state) => state.error)

// Specific selectors
export const useUnreadNotifications = () => 
  useUserStore((state) => state.notifications.filter(notification => !notification.read))

export const useNotificationCount = () => 
  useUserStore((state) => state.notifications.length)

export const useUnreadNotificationCount = () => 
  useUserStore((state) => state.notifications.filter(notification => !notification.read).length)

export const useUserTheme = () => 
  useUserStore((state) => state.preferences.theme)

export const useUserLanguage = () => 
  useUserStore((state) => state.preferences.language)

export const useUserTimezone = () => 
  useUserStore((state) => state.preferences.timezone)

export const useEmailNotifications = () => 
  useUserStore((state) => state.preferences.emailNotifications)

export const usePushNotifications = () => 
  useUserStore((state) => state.preferences.pushNotifications)

export const usePrivacySettings = () => 
  useUserStore((state) => state.preferences.privacySettings)

// Actions
export const useUserActions = () => useUserStore((state) => ({
  setProfile: state.setProfile,
  updateProfile: state.updateProfile,
  setPreferences: state.setPreferences,
  addNotification: state.addNotification,
  removeNotification: state.removeNotification,
  markNotificationAsRead: state.markNotificationAsRead,
  setLoading: state.setLoading,
  setError: state.setError,
  clearError: state.clearError,
}))

// Convenience hooks for specific actions
export const useUserProfileActions = () => useUserStore((state) => ({
  setProfile: state.setProfile,
  updateProfile: state.updateProfile,
}))

export const useUserPreferencesActions = () => useUserStore((state) => ({
  setPreferences: state.setPreferences,
}))

export const useNotificationActions = () => useUserStore((state) => ({
  addNotification: state.addNotification,
  removeNotification: state.removeNotification,
  markNotificationAsRead: state.markNotificationAsRead,
}))
```

## File: src/styles/globals.css
```css
@tailwind base;
@tailwind components;
@tailwind utilities;

body {
  font-family: Arial, Helvetica, sans-serif;
}

@layer base {
  :root {
    --background: 0 0% 100%;
    --foreground: 240 10% 3.9%;
    --card: 0 0% 100%;
    --card-foreground: 240 10% 3.9%;
    --popover: 0 0% 100%;
    --popover-foreground: 240 10% 3.9%;
    --primary: 240 5.9% 10%;
    --primary-foreground: 0 0% 98%;
    --secondary: 240 4.8% 95.9%;
    --secondary-foreground: 240 5.9% 10%;
    --muted: 240 4.8% 95.9%;
    --muted-foreground: 240 3.8% 46.1%;
    --accent: 240 4.8% 95.9%;
    --accent-foreground: 240 5.9% 10%;
    --destructive: 0 84.2% 60.2%;
    --destructive-foreground: 0 0% 98%;
    --border: 240 5.9% 90%;
    --input: 240 5.9% 90%;
    --ring: 240 10% 3.9%;
    --chart-1: 12 76% 61%;
    --chart-2: 173 58% 39%;
    --chart-3: 197 37% 24%;
    --chart-4: 43 74% 66%;
    --chart-5: 27 87% 67%;
    --radius: 0.5rem;
  }
  .dark {
    --background: 240 10% 3.9%;
    --foreground: 0 0% 98%;
    --card: 240 10% 3.9%;
    --card-foreground: 0 0% 98%;
    --popover: 240 10% 3.9%;
    --popover-foreground: 0 0% 98%;
    --primary: 0 0% 98%;
    --primary-foreground: 240 5.9% 10%;
    --secondary: 240 3.7% 15.9%;
    --secondary-foreground: 0 0% 98%;
    --muted: 240 3.7% 15.9%;
    --muted-foreground: 240 5% 64.9%;
    --accent: 240 3.7% 15.9%;
    --accent-foreground: 0 0% 98%;
    --destructive: 0 62.8% 30.6%;
    --destructive-foreground: 0 0% 98%;
    --border: 240 3.7% 15.9%;
    --input: 240 3.7% 15.9%;
    --ring: 240 4.9% 83.9%;
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

## File: src/types/api.ts
```typescript
// ============================================================================
// API TYPES - Consolidated from ai.ts and career.ts
// ============================================================================

// AI Types
export interface ResumeAnalysis {
  id: string
  userId: string
  fileName: string
  analysis: {
    skills: string[]
    experience: string[]
    education: string[]
    recommendations: string[]
    score: number
  }
  createdAt: string
  updatedAt: string
}

export interface CareerProfile {
  id: string
  userId: string
  title: string
  summary: string
  skills: string[]
  experience: string[]
  education: string[]
  interests: string[]
  createdAt: string
  updatedAt: string
}

export interface JobRecommendation {
  id: string
  title: string
  company: string
  location: string
  description: string
  requirements: string[]
  salary?: string
  matchScore: number
  url?: string
}

// Career Types
export interface Job {
  id: string
  title: string
  company: string
  location: string
  description: string
  requirements: string[]
  salary?: string
  type: 'full-time' | 'part-time' | 'contract' | 'internship'
  remote: boolean
  postedAt: string
  url?: string
}

export interface JobSearchFilters {
  query?: string
  location?: string
  type?: string[]
  remote?: boolean
  salary?: {
    min?: number
    max?: number
  }
  experience?: string[]
}

export interface CareerPath {
  id: string
  title: string
  description: string
  steps: CareerStep[]
  estimatedDuration: string
  difficulty: 'beginner' | 'intermediate' | 'advanced'
}

export interface CareerStep {
  id: string
  title: string
  description: string
  order: number
  completed: boolean
  resources?: string[]
}
```

## File: src/types/auth.ts
```typescript
export interface User {
  id: string
  email: string
  name?: string
  avatar?: string
  createdAt: string
  updatedAt: string
}

export interface LoginCredentials {
  email: string
  password: string
}

export interface RegisterCredentials extends LoginCredentials {
  name: string
  confirmPassword: string
}

export interface AuthState {
  user: User | null
  isAuthenticated: boolean
  isLoading: boolean
  error: string | null
}

export interface AuthContextType extends AuthState {
  login: (credentials: LoginCredentials) => Promise<void>
  register: (credentials: RegisterCredentials) => Promise<void>
  logout: () => void
  clearError: () => void
}
```

## File: src/types/components.ts
```typescript
// ============================================================================
// COMPONENT TYPES - Consolidated from core.ts, store.ts, and user.ts
// ============================================================================

// ===== COMMON TYPES =====

export type LoadingState = 'idle' | 'loading' | 'success' | 'error'

export interface BaseEntity {
  id: string
  createdAt: string
  updatedAt: string
}

export interface SelectOption {
  value: string
  label: string
  disabled?: boolean
}

export interface FormField {
  name: string
  label: string
  type: 'text' | 'email' | 'password' | 'number' | 'textarea' | 'select' | 'checkbox' | 'radio'
  required?: boolean
  placeholder?: string
  options?: SelectOption[]
  validation?: any
}

export interface ToastMessage {
  id: string
  type: 'success' | 'error' | 'warning' | 'info'
  title: string
  description?: string
  duration?: number
}

// ===== FORM TYPES =====

export interface FormState<T = any> {
  values: T
  errors: Partial<Record<keyof T, string>>
  touched: Partial<Record<keyof T, boolean>>
  isSubmitting: boolean
  isValid: boolean
}

export interface FormFieldProps {
  name: string
  label: string
  type?: 'text' | 'email' | 'password' | 'number' | 'textarea' | 'select' | 'checkbox' | 'radio'
  placeholder?: string
  required?: boolean
  disabled?: boolean
  options?: Array<{ value: string; label: string }>
  validation?: any
}

export interface FormValidationRule {
  required?: boolean
  minLength?: number
  maxLength?: number
  pattern?: RegExp
  custom?: (value: any) => string | undefined
}

// ===== API TYPES =====

export interface ApiResponse<T = any> {
  success: boolean
  data?: T
  message?: string
  error?: string
}

export interface PaginatedResponse<T> extends ApiResponse<T[]> {
  pagination: {
    page: number
    limit: number
    total: number
    totalPages: number
  }
}

export interface ApiError {
  message: string
  code?: string
  status?: number
}

// ===== STORE TYPES =====

export interface RootState {
  auth: AuthState
  ui: UIState
  career: CareerState
  user: UserState
}

export interface UIState {
  theme: 'light' | 'dark' | 'system'
  sidebarOpen: boolean
  notifications: ToastMessage[]
  loadingStates: Record<string, boolean>
}

export interface CareerState {
  jobs: Job[]
  filters: JobSearchFilters
  selectedJob: Job | null
  isLoading: boolean
  error: string | null
}

export interface UserState {
  profile: UserProfile | null
  settings: UserSettings | null
  isLoading: boolean
  error: string | null
}

export interface StoreAction<T = any> {
  type: string
  payload?: T
}

// ===== USER TYPES =====

export interface UserProfile {
  id: string
  email: string
  name: string
  avatar?: string
  bio?: string
  location?: string
  website?: string
  socialLinks?: {
    linkedin?: string
    github?: string
    twitter?: string
  }
  preferences?: {
    theme: 'light' | 'dark' | 'system'
    notifications: boolean
    emailUpdates: boolean
  }
  createdAt: string
  updatedAt: string
}

export interface UserSettings {
  theme: 'light' | 'dark' | 'system'
  notifications: boolean
  emailUpdates: boolean
  privacy: {
    profileVisibility: 'public' | 'private'
    showEmail: boolean
    showLocation: boolean
  }
}

// ===== IMPORTED TYPES =====

// Import types from api.ts to avoid circular dependencies
export interface Job {
  id: string
  title: string
  company: string
  location: string
  description: string
  requirements: string[]
  salary?: string
  type: 'full-time' | 'part-time' | 'contract' | 'internship'
  remote: boolean
  postedAt: string
  url?: string
}

export interface JobSearchFilters {
  query?: string
  location?: string
  type?: string[]
  remote?: boolean
  salary?: {
    min?: number
    max?: number
  }
  experience?: string[]
}

// Import types from auth.ts
export interface User {
  id: string
  email: string
  name?: string
  avatar?: string
  createdAt: string
  updatedAt: string
}

export interface AuthState {
  user: User | null
  isAuthenticated: boolean
  isLoading: boolean
  error: string | null
}
```

## File: src/types/index.ts
```typescript
// Type exports
export * from './auth';
export * from './api';
export * from './components';
```

## File: src/types/resume-generator.ts
```typescript
/**
 * Resume Generator TypeScript Types
 * Comprehensive type definitions for the AI-powered resume generator
 */

// ========================================
// CORE RESUME TYPES
// ========================================

export interface PersonalInfo {
  name: string
  email: string
  phone: string
  location: string
  linkedin?: string
  website?: string
  confidence: number
}

export interface ProfessionalSummary {
  summary: string
  confidence: number
  suggestions?: string[]
}

export interface Skill {
  name: string
  level: 'beginner' | 'intermediate' | 'advanced' | 'expert'
  category: string
  confidence: number
  canadianEquivalent?: string
}

export interface WorkExperience {
  title: string
  company: string
  location: string
  startDate: string
  endDate?: string
  current: boolean
  description: string
  achievements: string[]
  confidence: number
  canadianAdaptations?: string[]
}

export interface Education {
  degree: string
  institution: string
  location: string
  graduationDate: string
  gpa?: number
  relevantCourses: string[]
  confidence: number
  canadianEquivalency?: string
}

export interface Certification {
  name: string
  issuer: string
  issueDate: string
  expiryDate?: string
  credentialId?: string
  confidence: number
  canadianRecognition?: string
}

export interface Project {
  name: string
  description: string
  technologies: string[]
  url?: string
  startDate: string
  endDate?: string
  confidence: number
}

export interface GeneratedResume {
  id: string
  userId: string
  originalAnalysisId: string
  jobTargeting: JobTargeting
  personalInfo: PersonalInfo
  professionalSummary: ProfessionalSummary
  skills: Skill[]
  workExperience: WorkExperience[]
  education: Education[]
  certifications: Certification[]
  projects: Project[]
  atsScore: number
  status: 'draft' | 'final' | 'archived'
  createdAt: string
  updatedAt: string
  lastEditedAt?: string
  downloadCount: number
  metadata: Record<string, any>
}

// ========================================
// JOB TARGETING TYPES
// ========================================

export interface JobTargeting {
  jobTitle: string
  companyName: string
  jobDescription?: string
  industry?: string
  location?: string
  salaryRange?: {
    min: number
    max: number
    currency: string
  }
  requiredSkills: string[]
  preferredSkills: string[]
  experienceLevel: 'entry' | 'mid' | 'senior' | 'executive'
  keywords: string[]
  companyCulture?: string[]
  benefits?: string[]
}

export interface JobAnalysis {
  keyRequirements: string[]
  preferredQualifications: string[]
  companyValues: string[]
  industryTrends: string[]
  salaryInsights: {
    range: { min: number; max: number }
    currency: string
    market: string
  }
  skillGaps: {
    missing: string[]
    suggested: string[]
  }
  optimizationSuggestions: string[]
}

// ========================================
// AI GENERATION TYPES
// ========================================

export interface GenerationProgress {
  stage: 'analyzing' | 'generating' | 'optimizing' | 'finalizing'
  progress: number
  status: string
  estimatedTimeRemaining?: number
}

export interface AISuggestion {
  id: string
  type: 'content' | 'format' | 'keyword' | 'style'
  category: 'personal_info' | 'summary' | 'skills' | 'experience' | 'education'
  title: string
  description: string
  changes: Record<string, any>
  confidence: number
  reasoning: string
  applied: boolean
}

export interface GenerationResult {
  resume: GeneratedResume
  suggestions: AISuggestion[]
  atsScore: number
  optimizationTips: string[]
  canadianMarketInsights: string[]
}

// ========================================
// EDITOR TYPES
// ========================================

export interface UserEdit {
  field: string
  section: string
  oldValue: any
  newValue: any
  timestamp: Date
  autoSaved: boolean
}

export interface EditorState {
  isEditing: boolean
  currentSection: string | null
  selectedField: string | null
  userEdits: UserEdit[]
  autoSaveStatus: 'idle' | 'saving' | 'saved' | 'error'
  lastSaved: Date | null
  hasUnsavedChanges: boolean
}

export interface EditableField {
  id: string
  type: 'text' | 'textarea' | 'select' | 'date' | 'array' | 'object'
  label: string
  value: any
  placeholder?: string
  required: boolean
  validation?: {
    minLength?: number
    maxLength?: number
    pattern?: string
    custom?: (value: any) => boolean
  }
  options?: Array<{ label: string; value: any }>
}

export interface EditableSection {
  id: string
  title: string
  fields: EditableField[]
  canAdd: boolean
  canRemove: boolean
  canReorder: boolean
  template?: any
}

// ========================================
// SEARCH AND FILTER TYPES
// ========================================

export interface SearchFilters {
  jobTitle?: string
  companyName?: string
  industry?: string
  status?: 'draft' | 'final' | 'archived' | 'all'
  dateRange?: {
    start: Date
    end: Date
  }
  atsScoreRange?: {
    min: number
    max: number
  }
}

export interface SearchResult {
  resumes: GeneratedResume[]
  pagination: {
    page: number
    limit: number
    total: number
    totalPages: number
  }
  filters: SearchFilters
}

// ========================================
// API TYPES
// ========================================

export interface GenerateResumeRequest {
  originalAnalysisId: string
  jobTargeting: JobTargeting
}

export interface GenerateResumeResponse {
  success: boolean
  data?: GeneratedResume
  error?: string
  progress?: GenerationProgress
}

export interface UpdateResumeRequest {
  resumeId: string
  updates: Partial<GeneratedResume>
}

export interface AutoSaveRequest {
  resumeId: string
  userEdits: Record<string, any>
}

export interface SearchResumesRequest {
  filters: SearchFilters
  pagination: {
    page: number
    limit: number
  }
  sortBy?: string
  sortOrder?: 'asc' | 'desc'
}

// ========================================
// CANADIAN MARKET TYPES
// ========================================

export interface CanadianMarketData {
  jobTitles: {
    [industry: string]: string[]
  }
  industries: string[]
  locations: {
    provinces: string[]
    cities: {
      [province: string]: string[]
    }
  }
  skills: {
    [category: string]: {
      name: string
      canadianEquivalent: string
      demand: 'high' | 'medium' | 'low'
    }[]
  }
  salaryRanges: {
    [jobTitle: string]: {
      entry: { min: number; max: number }
      mid: { min: number; max: number }
      senior: { min: number; max: number }
      currency: string
    }
  }
}

export interface SkillsTranslation {
  originalSkill: string
  canadianEquivalent: string
  confidence: number
  industry: string
  reasoning: string
}

// ========================================
// ATS SCORING TYPES
// ========================================

export interface ATSScore {
  overall: number
  breakdown: {
    keywordMatch: number
    formatCompliance: number
    contentQuality: number
    structure: number
  }
  keywords: {
    found: string[]
    missing: string[]
    suggested: string[]
  }
  formatIssues: string[]
  recommendations: string[]
}

// ========================================
// EXPORT TYPES
// ========================================

export interface ExportOptions {
  format: 'pdf' | 'docx' | 'txt'
  template: 'professional' | 'creative' | 'minimal' | 'executive'
  includeATS: boolean
  includeSuggestions: boolean
  watermark?: boolean
}

export interface ExportResult {
  url: string
  filename: string
  size: number
  format: string
  expiresAt: Date
}

// ========================================
// UTILITY TYPES
// ========================================

export type ExperienceLevel = 'entry' | 'mid' | 'senior' | 'executive'
export type ResumeStatus = 'draft' | 'final' | 'archived'
export type AutoSaveStatus = 'idle' | 'saving' | 'saved' | 'error'
export type GenerationStage = 'analyzing' | 'generating' | 'optimizing' | 'finalizing'
export type SuggestionType = 'content' | 'format' | 'keyword' | 'style'
export type FieldType = 'text' | 'textarea' | 'select' | 'date' | 'array' | 'object'

// ========================================
// EVENT TYPES
// ========================================

export interface ResumeGeneratorEvents {
  'resume:selected': { resumeId: string }
  'generation:started': { jobTargeting: JobTargeting }
  'generation:progress': GenerationProgress
  'generation:completed': { resume: GeneratedResume }
  'generation:failed': { error: string }
  'editor:started': { resumeId: string }
  'editor:saved': { resumeId: string; timestamp: Date }
  'suggestion:applied': { suggestionId: string }
  'suggestion:rejected': { suggestionId: string }
  'export:requested': { resumeId: string; options: ExportOptions }
  'export:completed': { result: ExportResult }
}

// ========================================
// VALIDATION TYPES
// ========================================

export interface ValidationRule {
  field: string
  type: 'required' | 'minLength' | 'maxLength' | 'pattern' | 'email' | 'url' | 'custom'
  value?: any
  message: string
}

export interface ValidationResult {
  isValid: boolean
  errors: {
    field: string
    message: string
  }[]
}

// ========================================
// CONFIGURATION TYPES
// ========================================

export interface ResumeGeneratorConfig {
  autoSave: {
    enabled: boolean
    interval: number // seconds
    maxRetries: number
  }
  generation: {
    maxRetries: number
    timeout: number // seconds
    progressUpdateInterval: number // seconds
  }
  editor: {
    enableRealTimeValidation: boolean
    enableAutoComplete: boolean
    enableSpellCheck: boolean
  }
  export: {
    defaultFormat: 'pdf' | 'docx' | 'txt'
    defaultTemplate: 'professional' | 'creative' | 'minimal' | 'executive'
    maxFileSize: number // bytes
  }
  ats: {
    enabled: boolean
    scoringAlgorithm: 'standard' | 'advanced'
    keywordWeight: number
    formatWeight: number
  }
}

// ========================================
// ERROR TYPES
// ========================================

export interface ResumeGeneratorError {
  code: string
  message: string
  details?: any
  timestamp: Date
  context?: {
    resumeId?: string
    userId?: string
    action?: string
  }
}

export type ResumeGeneratorErrorCode = 
  | 'GENERATION_FAILED'
  | 'INVALID_JOB_TARGETING'
  | 'RESUME_NOT_FOUND'
  | 'PERMISSION_DENIED'
  | 'VALIDATION_FAILED'
  | 'AUTO_SAVE_FAILED'
  | 'EXPORT_FAILED'
  | 'NETWORK_ERROR'
  | 'UNKNOWN_ERROR'

// ========================================
// RESPONSE TYPES
// ========================================

export interface ApiResponse<T = any> {
  success: boolean
  data?: T
  error?: string
  message?: string
  timestamp: Date
}

export interface PaginatedResponse<T = any> {
  data: T[]
  pagination: {
    page: number
    limit: number
    total: number
    totalPages: number
  }
  success: boolean
  message?: string
}

// ========================================
// EXPORT ALL TYPES
// ========================================

export type {
  PersonalInfo,
  ProfessionalSummary,
  Skill,
  WorkExperience,
  Education,
  Certification,
  Project,
  GeneratedResume,
  JobTargeting,
  JobAnalysis,
  GenerationProgress,
  AISuggestion,
  GenerationResult,
  UserEdit,
  EditorState,
  EditableField,
  EditableSection,
  SearchFilters,
  SearchResult,
  GenerateResumeRequest,
  GenerateResumeResponse,
  UpdateResumeRequest,
  AutoSaveRequest,
  SearchResumesRequest,
  CanadianMarketData,
  SkillsTranslation,
  ATSScore,
  ExportOptions,
  ExportResult,
  ValidationRule,
  ValidationResult,
  ResumeGeneratorConfig,
  ResumeGeneratorError,
  ApiResponse,
  PaginatedResponse
}
```

## File: tailwind.config.ts
```typescript
import type { Config } from "tailwindcss";
import animate from "tailwindcss-animate";

export default {
	darkMode: ["class"],
	content: [
		"./src/pages/**/*.{js,ts,jsx,tsx,mdx}",
		"./src/components/**/*.{js,ts,jsx,tsx,mdx}",
		"./src/app/**/*.{js,ts,jsx,tsx,mdx}",
	],
	theme: {
		extend: {
			colors: {
				background: 'hsl(var(--background))',
				foreground: 'hsl(var(--foreground))',
				card: {
					DEFAULT: 'hsl(var(--card))',
					foreground: 'hsl(var(--card-foreground))'
				},
				popover: {
					DEFAULT: 'hsl(var(--popover))',
					foreground: 'hsl(var(--popover-foreground))'
				},
				primary: {
					DEFAULT: 'hsl(var(--primary))',
					foreground: 'hsl(var(--primary-foreground))'
				},
				secondary: {
					DEFAULT: 'hsl(var(--secondary))',
					foreground: 'hsl(var(--secondary-foreground))'
				},
				muted: {
					DEFAULT: 'hsl(var(--muted))',
					foreground: 'hsl(var(--muted-foreground))'
				},
				accent: {
					DEFAULT: 'hsl(var(--accent))',
					foreground: 'hsl(var(--accent-foreground))'
				},
				destructive: {
					DEFAULT: 'hsl(var(--destructive))',
					foreground: 'hsl(var(--destructive-foreground))'
				},
				border: 'hsl(var(--border))',
				input: 'hsl(var(--input))',
				ring: 'hsl(var(--ring))',
				chart: {
					'1': 'hsl(var(--chart-1))',
					'2': 'hsl(var(--chart-2))',
					'3': 'hsl(var(--chart-3))',
					'4': 'hsl(var(--chart-4))',
					'5': 'hsl(var(--chart-5))'
				}
			},
			borderRadius: {
				lg: 'var(--radius)',
				md: 'calc(var(--radius) - 2px)',
				sm: 'calc(var(--radius) - 4px)'
			}
		}
	},
	plugins: [animate],
} satisfies Config;
```

## File: tsconfig.json
```json
{
  "compilerOptions": {
    "target": "ES2022",
    "lib": ["dom", "dom.iterable", "esnext"],
    "allowJs": true,
    "skipLibCheck": true,
    "strict": true,
    "noEmit": true,
    "esModuleInterop": true,
    "module": "esnext",
    "moduleResolution": "bundler",
    "resolveJsonModule": true,
    "isolatedModules": true,
    "jsx": "preserve",
    "incremental": true,
    "forceConsistentCasingInFileNames": true,
    "noImplicitAny": true,
    "noImplicitReturns": true,
    "noImplicitThis": true,
    "noUnusedLocals": true,
    "noUnusedParameters": true,
    "exactOptionalPropertyTypes": true,
    "noUncheckedIndexedAccess": true,
    "noImplicitOverride": true,
    "allowUnusedLabels": false,
    "allowUnreachableCode": false,
    "plugins": [
      {
        "name": "next"
      }
    ],
    "paths": {
      "@/*": ["./src/*"],
      "@/components/*": ["./src/components/*"],
      "@/lib/*": ["./src/lib/*"],
      "@/stores/*": ["./src/stores/*"],
      "@/hooks/*": ["./src/hooks/*"],
      "@/types/*": ["./src/types/*"],
      "@/constants/*": ["./src/constants/*"],
      "@/utils/*": ["./src/utils/*"],
      "@/styles/*": ["./src/styles/*"],
      "@/app/*": ["./src/app/*"]
    }
  },
  "include": [
    "next-env.d.ts",
    "**/*.ts",
    "**/*.tsx",
    ".next/types/**/*.ts",
    "src/**/*"
  ],
  "exclude": [
    "node_modules",
    ".next",
    "out",
    "dist",
    "build"
  ]
}
```
