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
eslint.config.mjs
next.config.ts
postcss.config.mjs
README.md
src/app/(auth)/forgot-password/page.tsx
src/app/(auth)/layout.tsx
src/app/(auth)/login/page.tsx
src/app/(auth)/onboarding/car-dealer/BusinessInformation.tsx
src/app/(auth)/onboarding/car-dealer/page.tsx
src/app/(auth)/onboarding/car-dealer/SuccessPage.tsx
src/app/(auth)/onboarding/car-dealer/types.ts
src/app/(auth)/onboarding/consultant/BusinessInformation.tsx
src/app/(auth)/onboarding/consultant/page.tsx
src/app/(auth)/onboarding/consultant/SuccessPage.tsx
src/app/(auth)/onboarding/consultant/types.ts
src/app/(auth)/onboarding/immigrant/page.tsx
src/app/(auth)/onboarding/layout.tsx
src/app/(auth)/onboarding/page.tsx
src/app/(auth)/onboarding/realtor/BusinessInformation.tsx
src/app/(auth)/onboarding/realtor/OfficeWorkSetup.tsx
src/app/(auth)/onboarding/realtor/page.tsx
src/app/(auth)/onboarding/realtor/SuccessPage.tsx
src/app/(auth)/onboarding/realtor/types.ts
src/app/(auth)/signup/page.tsx
src/app/api/ai/resume/analyses/route.ts
src/app/api/career/search-jobs/route.ts
src/app/dashboard/admin/page.tsx
src/app/dashboard/admin/user-list/page.tsx
src/app/dashboard/admin/verify-users/page.tsx
src/app/dashboard/admin/view-user/[id]/page.tsx
src/app/dashboard/car-dealer/add-listing/page.tsx
src/app/dashboard/car-dealer/availability/page.tsx
src/app/dashboard/car-dealer/bookings/page.tsx
src/app/dashboard/car-dealer/car-listings/[id]/page.tsx
src/app/dashboard/car-dealer/car-listings/page.tsx
src/app/dashboard/car-dealer/edit-listing/[id]/page.tsx
src/app/dashboard/car-dealer/page.tsx
src/app/dashboard/consultant/availability/page.tsx
src/app/dashboard/consultant/bookings/page.tsx
src/app/dashboard/consultant/page.tsx
src/app/dashboard/layout.tsx
src/app/dashboard/not-verified/page.tsx
src/app/dashboard/page.tsx
src/app/dashboard/realtor/add-listing/page.tsx
src/app/dashboard/realtor/availability/page.tsx
src/app/dashboard/realtor/bookings/page.tsx
src/app/dashboard/realtor/edit-listing/[id]/page.tsx
src/app/dashboard/realtor/house-listings/[id]/page.tsx
src/app/dashboard/realtor/house-listings/page.tsx
src/app/dashboard/realtor/page.tsx
src/app/dashboard/user/ai/career-profile/page.tsx
src/app/dashboard/user/ai/page.tsx
src/app/dashboard/user/ai/resume/page.tsx
src/app/dashboard/user/bookings/page.tsx
src/app/dashboard/user/cars/car-listings/[id]/page.tsx
src/app/dashboard/user/cars/page.tsx
src/app/dashboard/user/consultant/page.tsx
src/app/dashboard/user/favourites-car/page.tsx
src/app/dashboard/user/favourites-house/page.tsx
src/app/dashboard/user/homes/house-listings/[id]/page.tsx
src/app/dashboard/user/homes/page.tsx
src/app/dashboard/user/page.tsx
src/app/dashboard/user/profile/page.tsx
src/app/dashboard/user/saved/page.tsx
src/app/dashboard/user/slots/[listingId]/[type]/page.tsx
src/app/dashboard/user/slots/consultant/[consultantId]/page.tsx
src/app/globals.css
src/app/layout.tsx
src/app/page.tsx
src/components/ai/AIFeaturesPanel.tsx
src/components/ai/EnhancedResumeUpload.tsx
src/components/ai/JobSearchModal.tsx
src/components/ai/ResumeAnalysisDetail.tsx
src/components/ai/ResumeAnalysisList.tsx
src/components/AIFeatures.tsx
src/components/availability/AppointmentBooking.tsx
src/components/availability/AvailabilityForm.tsx
src/components/availability/AvailabilityPage.tsx
src/components/availability/BookingTable.tsx
src/components/availability/UserBooking.tsx
src/components/consultant/ConsultantCarousel.tsx
src/components/consultant/UpcomingMeetings.tsx
src/components/Filter.tsx
src/components/Footer.tsx
src/components/Header.tsx
src/components/ListingCard.tsx
src/components/Listings.tsx
src/components/Logo.tsx
src/components/onboarding/DocumentUpload.tsx
src/components/onboarding/PersonalInformation.tsx
src/components/onboarding/TermsAndConditions.tsx
src/components/providers/theme-provider.tsx
src/components/QuickLinks.tsx
src/components/Sidecard.tsx
src/components/ThemeSwitcher.tsx
src/components/ui/alert.tsx
src/components/ui/badge.tsx
src/components/ui/button.tsx
src/components/ui/calendar.tsx
src/components/ui/card.tsx
src/components/ui/chart.tsx
src/components/ui/checkbox.tsx
src/components/ui/dialog.tsx
src/components/ui/dropdown-menu.tsx
src/components/ui/form.tsx
src/components/ui/input.tsx
src/components/ui/label.tsx
src/components/ui/popover.tsx
src/components/ui/progress.tsx
src/components/ui/radio-group.tsx
src/components/ui/scroll-area.tsx
src/components/ui/select.tsx
src/components/ui/table.tsx
src/components/ui/tabs.tsx
src/components/ui/textarea.tsx
src/components/ui/toast.tsx
src/components/ui/toaster.tsx
src/components/UserProfile.tsx
src/hooks/use-toast.ts
src/lib/auth.ts
src/lib/utils.ts
src/middleware.ts
tailwind.config.ts
```

# Files

## File: .repomixignore
````
# Dependencies
node_modules/
npm-debug.log*
yarn-debug.log*
yarn-error.log*
package-lock.json
yarn.lock

# Environment files (contain sensitive data)
.env
.env.local
.env.development.local
.env.test.local
.env.production.local
*.env

# Build outputs
dist/
build/
out/
.next/
.nuxt/
.output/
.vercel/

# Cache directories
.cache/
.parcel-cache/
.eslintcache
.stylelintcache
.rpt2_cache/
.rts2_cache_cjs/
.rts2_cache_es/
.rts2_cache_umd/

# Logs
*.log
logs/
pids/
*.pid
*.seed
*.pid.lock

# Temporary files
tmp/
temp/
.tmp/
*.tmp

# Database files
*.db
*.sqlite
*.sqlite3
prisma/ai-features.db

# IDE/Editor files
.vscode/
.idea/
*.swp
*.swo
*~
.DS_Store
Thumbs.db

# OS generated files
.DS_Store?
ehthumbs.db
Icon?

# Compiled binary addons
*.node
*.dll

# TypeScript compiled files
*.tsbuildinfo

# ESLint cache
.eslintcache

# Optional npm cache directory
.npm

# Optional REPL history
.node_repl_history

# Coverage directory used by tools like istanbul
coverage/
*.lcov
.nyc_output

# Dependency directories
jspm_packages/

# Optional eslint cache
.eslintcache

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

# parcel-bundler cache
.cache
.parcel-cache

# next.js build output
.next

# nuxt.js build output
.nuxt

# vuepress build output
.vuepress/dist

# Serverless directories
.serverless

# Firebase cache
.firebase/

# TernJS port file
.tern-port

# Stores VSCode versions used for testing VSCode extensions
.vscode-test

# Generated files
*.generated.*
*-generated.*

# Archive files
*.zip
*.tar.gz
*.rar

# Key files (sensitive)
key/
*.pem
*.key
*.crt
*.json

# Upload directories with user content
uploads/

# Test output
test-results/
coverage/

# Documentation build
docs/build/
````

## File: .gitignore
````
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
````

## File: eslint.config.mjs
````
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
````

## File: next.config.ts
````typescript
import type { NextConfig } from "next";

const nextConfig: NextConfig = {
  reactStrictMode: true,
  env: {
    BASE_URL: process.env.BASE_URL, 
  },
};

export default nextConfig;
````

## File: postcss.config.mjs
````
/** @type {import('postcss-load-config').Config} */
const config = {
  plugins: {
    tailwindcss: {},
  },
};

export default config;
````

## File: src/app/(auth)/layout.tsx
````typescript
import Header from "@/components/Header";
import { Toaster } from "@/components/ui/toaster";
import React, { ReactNode } from "react";

async function Layout({ children }: { children: ReactNode }) {

  return (
    <div className="flex flex-col h-screen min-w-full bg-background">
      <Header />
      <main className="w-full h-full">{children}</main>
      <Toaster />
    </div>
  );
}

export default Layout;
````

## File: src/app/(auth)/onboarding/car-dealer/BusinessInformation.tsx
````typescript
import React from "react";
import { FormData } from "./types"; // Importing FormData interface
import { Label } from "@/components/ui/label";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import { Checkbox } from "@/components/ui/checkbox";
import {
  Select as SingleSelect,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";
import Select, { MultiValue } from "react-select";

type OptionType = { value: string; label: string };

const carBrandsOptions: OptionType[] = [
  { value: "Brand A", label: "Brand A" },
  { value: "Brand B", label: "Brand B" },
  { value: "Brand C", label: "Brand C" },
  // Add more brands as needed
];

const BusinessInformation: React.FC<{
  formData: FormData; // Use the correct type
  setFormData: React.Dispatch<React.SetStateAction<FormData>>;
  errors: { [key: string]: string }; // Use the correct type
}> = ({ formData, setFormData, errors }) => {
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Business Information</h2>
      <div className="flex justify-between items-center gap-1">
        <Label className="w-1/3">Showroom Location(s):</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.showroomLocations}
          onChange={(e) =>
            setFormData({ ...formData, showroomLocations: e.target.value })
          }
        />
      </div>
      {errors.showroomLocations && <p className="text-red-500 text-sm mb-4">{errors.showroomLocations}</p>}
      <div className="flex justify-between items-center">
        <Label>Test Drive Policy:</Label>
        <Textarea
          className="w-2/3 mb-4"
          value={formData.testDrivePolicy}
          onChange={(e) =>
            setFormData({ ...formData, testDrivePolicy: e.target.value })
          }
        />
      </div>
      {errors.testDrivePolicy && <p className="text-red-500 text-sm mb-4">{errors.testDrivePolicy}</p>}
      <div className="text-left mb-4">
        <p className="mb-2">Vehicle Financing Options:</p>
        <div className="flex justify-between items-center gap-1">
          <div className="flex gap-2">
            <Checkbox
              checked={formData.vehicleFinancingOptions.inHouseFinancing}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  vehicleFinancingOptions: {
                    ...formData.vehicleFinancingOptions,
                    inHouseFinancing: checked ? true : false,
                  },
                })
              }
            />
            <Label>In-house Financing</Label>
          </div>
          
          <div className="flex gap-2">
            <Checkbox
              checked={formData.vehicleFinancingOptions.thirdPartyBanks}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  vehicleFinancingOptions: {
                    ...formData.vehicleFinancingOptions,
                    thirdPartyBanks: checked ? true : false,
                  },
                })
              }
            />
            <Label>Third-Party Banks</Label>
          </div>

          <div className="flex gap-2">
            <Checkbox
              checked={formData.vehicleFinancingOptions.leaseOptions}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  vehicleFinancingOptions: {
                    ...formData.vehicleFinancingOptions,
                    leaseOptions: checked ? true : false,
                  },
                })
              }
            />
            <Label>Lease</Label>
          </div>
          
        </div>
      </div>
      {errors.vehicleFinancingOptions && <p className="text-red-500 text-sm mb-4">{errors.vehicleFinancingOptions}</p>}
      <div className="flex justify-between items-center">
        <Label>Trade-in Options Available:</Label>
        <SingleSelect
          value={formData.tradeInOptions ? "Yes" : "No"}
          onValueChange={(value) =>
            setFormData({
              ...formData,
              tradeInOptions: value === "Yes",
            })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select option" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="Yes">Yes</SelectItem>
            <SelectItem value="No">No</SelectItem>
          </SelectContent>
        </SingleSelect>
      </div>
      <div className="flex justify-between items-center gap-1">
        <Label className="w-1/3">Service & Warranty Information:</Label>
        <Textarea
          className="w-2/3 mb-4"
          value={formData.serviceWarrantyInfo}
          onChange={(e) =>
            setFormData({ ...formData, serviceWarrantyInfo: e.target.value })
          }
        />
      </div>
      {errors.serviceWarrantyInfo && <p className="text-red-500 text-sm mb-4">{errors.serviceWarrantyInfo}</p>}
      <div className="flex justify-between items-center">
        <Label>Registration Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessRegistrationNumber}
          onChange={(e) =>
            setFormData({
              ...formData,
              businessRegistrationNumber: e.target.value,
            })
          }
        />
      </div>
      {errors.businessRegistrationNumber && <p className="text-red-500 text-sm mb-4">{errors.businessRegistrationNumber}</p>}
      <div className="flex justify-between items-center">
        <Label>Business Name:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessName}
          onChange={(e) =>
            setFormData({ ...formData, businessName: e.target.value })
          }
        />
      </div>
      {errors.businessName && <p className="text-red-500 text-sm mb-4">{errors.businessName}</p>}
      <div className="flex justify-between items-center">
        <Label>Business Address:</Label>
        <Textarea
          className="w-2/3 mb-4"
          value={formData.businessAddress}
          onChange={(e) =>
            setFormData({ ...formData, businessAddress: e.target.value })
          }
        />
      </div>
      {errors.businessAddress && <p className="text-red-500 text-sm mb-4">{errors.businessAddress}</p>}
      <div className="flex justify-between items-center">
        <Label>Years in Business:</Label>
        <SingleSelect
          value={formData.yearsInBusiness}
          onValueChange={(value) =>
            setFormData({ ...formData, yearsInBusiness: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select years" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="1-5">1-5 years</SelectItem>
            <SelectItem value="5-10">5-10 years</SelectItem>
            <SelectItem value="10+">10+ years</SelectItem>
          </SelectContent>
        </SingleSelect>
      </div>
      {errors.yearsInBusiness && <p className="text-red-500 text-sm mb-4">{errors.yearsInBusiness}</p>}
      <div className="flex justify-between items-center">
        <Label>Dealership License Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.dealershipLicenseNumber}
          onChange={(e) =>
            setFormData({
              ...formData,
              dealershipLicenseNumber: e.target.value,
            })
          }
        />
      </div>
      {errors.dealershipLicenseNumber && <p className="text-red-500 text-sm mb-4">{errors.dealershipLicenseNumber}</p>}
      <div className="flex justify-between items-center gap-1">
        <Label className="w-1/3">Car Brands Sold:</Label>
        <Select
          isMulti
          options={carBrandsOptions}
          value={
            formData.carBrandsSold?.length
              ? carBrandsOptions.filter((option) =>
                  formData.carBrandsSold?.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              carBrandsSold: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.carBrandsSold && <p className="text-red-500 text-sm mb-4">{errors.carBrandsSold}</p>}
      <div className="text-left mb-4">
        <Label className="w-1/3">New or Used Cars?</Label>
        <div className="flex justify-between items-center gap-1">
          <div className="flex gap-2">
            <Checkbox
              checked={formData.newOrUsedCars.new}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  newOrUsedCars: {
                    ...formData.newOrUsedCars,
                    new: checked ? true : false,
                  },
                })
              }
            />
            <Label className="w-1/3">New</Label>
          </div>
          
          <div className="flex gap-2">
            <Checkbox
              checked={formData.newOrUsedCars.used}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  newOrUsedCars: {
                    ...formData.newOrUsedCars,
                    used: checked ? true : false,
                  },
                })
              }
            />
            <Label className="w-1/3">Used</Label>
          </div>
          
          <div className="flex gap-2">
            <Checkbox
              checked={formData.newOrUsedCars.both}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  newOrUsedCars: {
                    ...formData.newOrUsedCars,
                    both: checked ? true : false,
                  },
                })
              }
            />
            <Label className="w-1/3">Both</Label>
          </div>
         
        </div>
      </div>
      {/* {errors.newOrUsedCars && <p className="text-red-500 text-sm mb-4">{errors.newOrUsedCars}</p>} */}
    </div>
  );
};

export default BusinessInformation; // Ensure single default export
````

## File: src/app/(auth)/onboarding/car-dealer/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import React, { useState } from "react";
import BusinessInformation from "./BusinessInformation";
// import DocumentUpload from "./DocumentUpload";
import type { FormData } from "./types";
import PersonalInformation from "@/components/onboarding/PersonalInformation";
import TermsAndConditions from "@/components/onboarding/TermsAndConditions";
import DocumentUpload from "@/components/onboarding/DocumentUpload";
import SuccessPage from "./SuccessPage";
import { useRouter } from "next/navigation";

const CarDealer: React.FC = () => {
  const [formData, setFormData] = useState<FormData>({
    fullName: "",
    email: "",
    phoneNumber: "",
    dateOfBirth: "",
    showroomLocations: "",
    testDrivePolicy: "",
    vehicleFinancingOptions: {
      inHouseFinancing: false,
      thirdPartyBanks: false,
      leaseOptions: false,
    },
    tradeInOptions: false,
    serviceWarrantyInfo: "",
    businessRegistrationNumber: "",
    businessName: "",
    businessAddress: "",
    yearsInBusiness: "",
    dealershipLicenseNumber: "",
    carBrandsSold: [],
    newOrUsedCars: {
      new: false,
      used: false,
      both: false,
    },
    governmentId: "",
    licenseDocument: "",
    businessVerification: "",
    backgroundCheckApproved: false,
    termsAccepted: false,
  });

    const [errors, setErrors] = useState({});

  const validateForm = () => {
    const newErrors: Record<string, string> = {};

    if(currentStep===1){
           // Full Name Validation
    if (!formData.fullName || formData.fullName.length < 3) {
      newErrors.fullName = "Full Name must be at least 3 characters";
    }
  
    // Phone Number Validations
    if (!formData.phoneNumber) {
      newErrors.phoneNumber = "Phone number is required";
    } else if (!/^\d+$/.test(formData.phoneNumber)) {
      newErrors.phoneNumber = "Phone number must contain only digits";
    } else if (formData.phoneNumber.length !== 10) {
      newErrors.phoneLength = "Phone number must be exactly 10 digits";
    }
  
    // Date of Birth Validation (Minimum 15 years old)
    if (!formData.dateOfBirth) {
      newErrors.dateOfBirth = "Date of Birth is required";
    } else {
      const dob = new Date(formData.dateOfBirth);
      const today = new Date();
      const minDate = new Date();
      minDate.setFullYear(today.getFullYear() - 15); // 15 years ago
  
      if (dob > minDate) {
        newErrors.dateOfBirth = "You must be at least 15 years old";
      }
    }
    }

    else if(currentStep === 2){

        // Business Name Validation
    // Validate Showroom Location
    if (!formData.showroomLocations) {
      newErrors.showroomLocations = "Showroom Location(s) are required.";
    }
  
    // Validate Test Drive Policy
    if (!formData.testDrivePolicy) {
      newErrors.testDrivePolicy = "Test Drive Policy is required.";
    }
  
    // Validate Vehicle Financing Options (Check at least one option is selected)
    const { inHouseFinancing, thirdPartyBanks, leaseOptions } = formData.vehicleFinancingOptions;
    if (!inHouseFinancing && !thirdPartyBanks && !leaseOptions) {
      newErrors.vehicleFinancingOptions = "At least one vehicle financing option must be selected.";
    }
  
    // Validate Service & Warranty Information
    if (!formData.serviceWarrantyInfo) {
      newErrors.serviceWarrantyInfo = "Service & Warranty Information is required.";
    }
  
    // Validate Business Registration Number
    if (!formData.businessRegistrationNumber) {
      newErrors.businessRegistrationNumber = "Business Registration Number is required.";
    }
  
    // Validate Business Name
    if (!formData.businessName) {
      newErrors.businessName = "Business Name is required.";
    }
  
    // Validate Business Address
    if (!formData.businessAddress) {
      newErrors.businessAddress = "Business Address is required.";
    }
  
    // Validate Years in Business
    if (!formData.yearsInBusiness) {
      newErrors.yearsInBusiness = "Please select years in business.";
    }
  
    // Validate Dealership License Number
    if (!formData.dealershipLicenseNumber) {
      newErrors.dealershipLicenseNumber = "Dealership License Number is required.";
    }
  
    // Validate Car Brands Sold (At least one brand must be selected)
    if (formData.carBrandsSold.length === 0) {
      newErrors.carBrandsSold = "At least one car brand must be selected.";
    }
  
    // Validate New or Used Cars checkboxes (At least one should be checked)
    // const { new: isNew, used: isUsed, both: isBoth } = formData.newOrUsedCars;
    // if (!isNew && !isUsed && !isBoth) {
    //   newErrors.newOrUsedCars = "Please select at least one option (New, Used, or Both).";
    // }
  }


  else if(currentStep===3){
    if (!formData.governmentId) {
      newErrors.governmentId = "Government ID is required.";
    }
    if (!formData.businessVerification) {
      newErrors.businessVerification = "Business verification document is required.";
    }
    if (!formData.licenseDocument) {
      newErrors.licenseDocument = "License document is required.";
    
  }
}
  else if(currentStep===4){
    
    if (formData.backgroundCheckApproved === false) {
      newErrors.backgroundCheckApproved = "Please accept the background verification.";
    }
    if (formData.termsAccepted === false) {
      newErrors.termsAccepted = "Please accept the terms and conditions.";
    }

  }
 

      setErrors(newErrors);
    return Object.keys(newErrors).length === 0;
};

  const [currentStep, setCurrentStep] = useState(1);
  const router = useRouter();

  const handleNextStep = () => {
    // Validate required fields
    if (validateForm()) {
      setCurrentStep((prevStep) => prevStep + 1);
      }
  };

  const handlePreviousStep = () => {
    setCurrentStep((prevStep) => prevStep - 1);
  };

  const [isLoading, setIsLoading] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const handleSubmit = async () => {
    setIsLoading(true);

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      
      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }
      
      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataToSend = new FormData();
      formDataToSend.append("fullName", formData.fullName);
      formDataToSend.append("phoneNo", formData.phoneNumber);
      formDataToSend.append("DOB", formData.dateOfBirth);
      formDataToSend.append("rolename", "Car Dealership");
      formDataToSend.append("businessName", formData.businessName);
      formDataToSend.append("businessAddress", formData.businessAddress);
      formDataToSend.append("businessRegistration", formData.businessRegistrationNumber);
      formDataToSend.append("yearsInBusiness", formData.yearsInBusiness);
      formDataToSend.append("dealershipLicenseNumber", formData.dealershipLicenseNumber);
      formDataToSend.append("carBrandsSold", formData.carBrandsSold.join(","));
      formDataToSend.append("newOrUsedCars", JSON.stringify(formData.newOrUsedCars));
      formDataToSend.append("showroomLocations", formData.showroomLocations);
      formDataToSend.append("testDrivePolicy", formData.testDrivePolicy);
      formDataToSend.append("financingOptions", JSON.stringify(formData.vehicleFinancingOptions));
      formDataToSend.append("tradeInOptions", formData.tradeInOptions.toString());
      formDataToSend.append("serviceWarrantyInfo", formData.serviceWarrantyInfo);
      formDataToSend.append("govId", formData.governmentId);
      formDataToSend.append("licenseCert", formData.licenseDocument);
      formDataToSend.append("businessDoc", formData.businessVerification);
      formDataToSend.append("backgroundVerification", formData.backgroundCheckApproved.toString());
      formDataToSend.append("termsConditionCheck", formData.termsAccepted.toString());

      const response = await fetch(`${endpoint}api/onboarding/information`, {
        method: "POST",
        headers: {
          Authorization: `Bearer ${token}`,
        },
        body: formDataToSend,
      });

      if (!response.ok) {
        const errorData = await response.json();
        throw new Error(errorData.error || "Failed to submit form");
      }

      router.push("/dashboard/not-verified?reason=user");
    } catch (error) {
      console.error("Submission error:", error);
    } finally {
      setIsLoading(false);
    }
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl w-full min-h-[600px] h-full">
        <div className="py-8 px-6 shadow text-center w-full h-full flex flex-col justify-between">
          {currentStep === 1 && (
            <PersonalInformation
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 2 && (
            <BusinessInformation
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 3 && (
            <DocumentUpload formData={formData} setFormData={setFormData}  errors={errors} />
          )}
          {currentStep === 4 && (
            <TermsAndConditions formData={formData} setFormData={setFormData}  errors={errors} />
          )}
          {currentStep === 5 && <SuccessPage formData={formData} />}
          <div className="flex gap-4 justify-center">
            {currentStep > 1 && (
              <Button onClick={handlePreviousStep}>Back</Button>
            )}
            {currentStep == 1 && (
              <Button onClick={() => router.push("/onboarding")}>Back</Button>
            )}
            {currentStep < 5 && <Button onClick={handleNextStep}>Next</Button>}
            {currentStep === 5 && (
              <Button 
                onClick={handleSubmit}
                disabled={isLoading}
              >
                {isLoading ? "Submitting..." : "Submit"}
              </Button>
            )}
          </div>
        </div>
      </div>
    </div>
  );
};

export default CarDealer;
````

## File: src/app/(auth)/onboarding/car-dealer/SuccessPage.tsx
````typescript
import React from "react";
import { FormData } from "./types"; // Importing FormData interface

const SuccessPage: React.FC<{ formData: FormData }> = ({ formData }) => {
  return (
    <div className="flex flex-col justify-center">
      <h2 className="text-xl font-semibold mb-2">Review Details</h2>
      <p className="text-center mb-4">
        Please review the details you have provided below.
      </p>
      <span className="flex justify-between mb-1">
        <strong>Full Name:</strong> {formData.fullName}
      </span>
      {/* <span className="flex justify-between mb-1">
        <strong>Email:</strong> {formData.email}
      </span> */}
      <span className="flex justify-between mb-1">
        <strong>Phone Number:</strong> {formData.phoneNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Showroom Location(s):</strong> {formData.showroomLocations}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Test Drive Policy:</strong> {formData.testDrivePolicy}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Trade-in Options:</strong>{" "}
        {formData.tradeInOptions ? "Yes" : "No"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Registration Number:</strong>{" "}
        {formData.businessRegistrationNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Name:</strong> {formData.businessName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Address:</strong> {formData.businessAddress}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Years in Business:</strong> {formData.yearsInBusiness}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Dealership License Number:</strong>{" "}
        {formData.dealershipLicenseNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Car Brands Sold:</strong> {formData.carBrandsSold.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>New or Used Cars:</strong>{" "}
        {formData.newOrUsedCars.new ? "New" : ""}{" "}
        {formData.newOrUsedCars.used ? "Used" : ""}{" "}
        {formData.newOrUsedCars.both ? "Both" : ""}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Government ID:</strong>{" "}
        {formData.governmentId ? "Provided" : "Not provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>License Document:</strong>{" "}
        {formData.licenseDocument ? "Provided" : "Not provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Verification:</strong>{" "}
        {formData.businessVerification ? "Provided" : "Not provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Background Check Approved:</strong>{" "}
        {formData.backgroundCheckApproved? "Yes" : "No"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Terms Accepted:</strong> {formData.termsAccepted ? "Yes" : "No"}
      </span>
    </div>
  );
};

export default SuccessPage;
````

## File: src/app/(auth)/onboarding/car-dealer/types.ts
````typescript
export interface FormData {
  fullName: string;
  email: string;
  phoneNumber: string;
  dateOfBirth: string;
  showroomLocations: string;
  testDrivePolicy: string;
  vehicleFinancingOptions: {
    inHouseFinancing: boolean;
    thirdPartyBanks: boolean;
    leaseOptions: boolean;
  };
  tradeInOptions: boolean;
  serviceWarrantyInfo: string;
  businessRegistrationNumber: string;
  businessName: string;
  businessAddress: string;
  yearsInBusiness: string;
  dealershipLicenseNumber: string;
  carBrandsSold: string[];
  newOrUsedCars: {
    new: boolean;
    used: boolean;
    both: boolean;
  };
  governmentId: string | Blob;
  businessVerification: string | Blob;
  licenseDocument: string | Blob;
  backgroundCheckApproved: boolean;
  termsAccepted: boolean;
}
````

## File: src/app/(auth)/onboarding/consultant/BusinessInformation.tsx
````typescript
import React from "react";
import { FormData } from "./types";
import { Label } from "@/components/ui/label";
import { Input } from "@/components/ui/input";
import Select, { MultiValue } from "react-select";
import {
  Select as SingleSelect,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";

type OptionType = { value: string; label: string };

const immigrationServicesOptions: OptionType[] = [
  { value: "Permanant Resident", label: "Permanant Resident" },
  { value: "Study Permit", label: "Study Permit" },
  { value: "Work Permit", label: "Work Permit" },
  { value: "Citizen", label: "Citizen" },
];

const languagesSpokenOptions: OptionType[] = [
  { value: "English", label: "Enlish" },
  { value: "French", label: "French" },
  { value: "Hindi", label: "Hindi" },
];

const countriesServedOptions: OptionType[] = [
  { value: "C1", label: "C1" },
  { value: "C2", label: "C2" },
  { value: "C3", label: "C3" },
];

const BusinessInformation: React.FC<{
  formData: FormData;
  setFormData: React.Dispatch<React.SetStateAction<FormData>>;
  errors: { [key: string]: string };
}> = ({ formData, setFormData, errors }) => {
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Business Information</h2>
      <div className="flex justify-between items-center">
        <Label>Business Name:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessName}
          onChange={(e) =>
            setFormData({ ...formData, businessName: e.target.value })
          }
        />
      </div>
      {errors.businessName && (
        <p className="text-red-500 text-sm mb-4">{errors.businessName}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Business Address:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessAddress}
          onChange={(e) =>
            setFormData({ ...formData, businessAddress: e.target.value })
          }
        />
      </div>
      {errors.businessAddress && (
        <p className="text-red-500 text-sm mb-4">{errors.businessAddress}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Registration Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessRegistrationNumber}
          onChange={(e) =>
            setFormData({
              ...formData,
              businessRegistrationNumber: e.target.value,
            })
          }
        />
      </div>
      {errors.businessRegistrationNumber && (
        <p className="text-red-500 text-sm mb-4">
          {errors.businessRegistrationNumber}
        </p>
      )}
      <div className="flex justify-between items-center">
        <Label>Years of Experience:</Label>
        <SingleSelect
          value={formData.yearsOfExperience || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, yearsOfExperience: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select Years of Expereince" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="1-5">1-5 years</SelectItem>
            <SelectItem value="5-10">5-10 years</SelectItem>
            <SelectItem value="10+">10+ years</SelectItem>
          </SelectContent>
        </SingleSelect>
      </div>
      {errors.yearsOfExperience && (
        <p className="text-red-500 text-sm mb-4">{errors.yearsOfExperience}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>License Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.licenseNumber}
          onChange={(e) =>
            setFormData({
              ...formData,
              licenseNumber: e.target.value,
            })
          }
        />
      </div>
      {errors.licenseNumber && (
        <p className="text-red-500 text-sm mb-4">{errors.licenseNumber}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Countries Served:</Label>
        <Select
          isMulti
          options={countriesServedOptions}
          value={
            formData.countriesServed?.length
              ? countriesServedOptions.filter((option) =>
                  formData.countriesServed.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              countriesServed: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.countriesServed && (
        <p className="text-red-500 text-sm mb-4">{errors.countriesServed}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Consultation Fee:</Label>
        <Input
          className="w-2/3 mb-4"
          type="number"
          value={formData.consultationFee}
          onChange={(e) =>
            setFormData({
              ...formData,
              consultationFee: Number(e.target.value),
            })
          }
        />
      </div>
      {errors.consultationFee && (
        <p className="text-red-500 text-sm mb-4">{errors.consultationFee}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Partnered Legal Firms:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.partneredLegalFirms}
          onChange={(e) =>
            setFormData({ ...formData, partneredLegalFirms: e.target.value })
          }
        />
      </div>
      {errors.partneredLegalFirms && (
        <p className="text-red-500 text-sm mb-4">
          {errors.partneredLegalFirms}
        </p>
      )}
      <div className="flex justify-between items-center">
        <Label>Website Links:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.websiteLinks}
          onChange={(e) =>
            setFormData({ ...formData, websiteLinks: e.target.value })
          }
        />
      </div>
      {errors.websiteLinks && (
        <p className="text-red-500 text-sm mb-4">{errors.websiteLinks}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Immigration Services:</Label>
        <Select
          isMulti
          options={immigrationServicesOptions}
          value={
            formData.immigrationServices?.length
              ? immigrationServicesOptions.filter((option) =>
                  formData.immigrationServices.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              immigrationServices: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.immigrationServices && (
        <p className="text-red-500 text-sm mb-4">
          {errors.immigrationServices}
        </p>
      )}
      <div className="flex justify-between items-center">
        <Label>Languages Spoken:</Label>
        <Select
          isMulti
          options={languagesSpokenOptions}
          value={
            formData.languagesSpoken?.length
              ? languagesSpokenOptions.filter((option) =>
                  formData.languagesSpoken.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              languagesSpoken: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.languagesSpoken && (
        <p className="text-red-500 text-sm mb-4">{errors.languagesSpoken}</p>
      )}
    </div>
  );
};

export default BusinessInformation;
````

## File: src/app/(auth)/onboarding/consultant/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button"; // Corrected import statement
import React, { useState } from "react";
import type { FormData } from "./types";
import BusinessInformation from "./BusinessInformation";
import SuccessPage from "./SuccessPage";
import PersonalInformation from "@/components/onboarding/PersonalInformation";
import TermsAndConditions from "@/components/onboarding/TermsAndConditions";
import DocumentUpload from "@/components/onboarding/DocumentUpload";
import { useRouter } from "next/navigation";

const Consultant = () => {
  const [formData, setFormData] = useState<FormData>({
    fullName: "",
    email: "",
    phoneNumber: "",
    dateOfBirth: "",
    countriesServed: [],
    consultationFee: 0,
    businessRegistrationNumber: "",
    partneredLegalFirms: "",
    websiteLinks: "",
    businessName: "",
    businessAddress: "",
    yearsOfExperience: "",
    licenseNumber: "",
    immigrationServices: [],
    languagesSpoken: [],
    governmentId: "",
    businessVerification: "",
    licenseDocument: "",
    backgroundCheckApproved: false,
    termsAccepted: false,
  });

  const [currentStep, setCurrentStep] = useState(1);
  const router = useRouter();

  const [errors, setErrors] = useState({});

  const validateForm = () => {
    const newErrors: Record<string, string> = {};

    if (currentStep === 1) {
      // Full Name Validation
      if (!formData.fullName || formData.fullName.length < 3) {
        newErrors.fullName = "Full Name must be at least 3 characters";
      }

      // Phone Number Validations
      if (!formData.phoneNumber) {
        newErrors.phoneNumber = "Phone number is required";
      } else if (!/^\d+$/.test(formData.phoneNumber)) {
        newErrors.phoneNumber = "Phone number must contain only digits";
      } else if (formData.phoneNumber.length !== 10) {
        newErrors.phoneLength = "Phone number must be exactly 10 digits";
      }

      // Date of Birth Validation (Minimum 15 years old)
      if (!formData.dateOfBirth) {
        newErrors.dateOfBirth = "Date of Birth is required";
      } else {
        const dob = new Date(formData.dateOfBirth);
        const today = new Date();
        const minDate = new Date();
        minDate.setFullYear(today.getFullYear() - 15); // 15 years ago

        if (dob > minDate) {
          newErrors.dateOfBirth = "You must be at least 15 years old";
        }
      }
    } else if (currentStep === 2) {
      // Business Name Validation
      // Validate Business Name
      if (!formData.businessName.trim()) {
        newErrors.businessName = "Business name is required.";
      }

      // Validate Business Address
      if (!formData.businessAddress.trim()) {
        newErrors.businessAddress = "Business address is required.";
      }

      // Validate Registration Number
      if (!formData.businessRegistrationNumber.trim()) {
        newErrors.businessRegistrationNumber =
          "Registration number is required.";
      }

      // Validate Years of Experience (must be a number)
      if (!formData.yearsOfExperience.trim()) {
        newErrors.yearsOfExperience = "Years of experience is required.";
      }

      // Validate License Number
      if (!formData.licenseNumber.trim()) {
        newErrors.licenseNumber = "License number is required.";
      }

      // Validate Countries Served (must have at least one selection)
      if (!formData.countriesServed || formData.countriesServed.length === 0) {
        newErrors.countriesServed = "Please select at least one country.";
      }

      // Validate Consultation Fee (must be a valid number)
      if (!formData.consultationFee) {
        newErrors.consultationFee = "Consultation fee is required.";
      } else if (
        isNaN(Number(formData.consultationFee)) ||
        Number(formData.consultationFee) < 0
      ) {
        newErrors.consultationFee = "Please enter a valid fee.";
      }

      // Validate Partnered Legal Firms
      if (!formData.partneredLegalFirms.trim()) {
        newErrors.partneredLegalFirms = "Please enter partnered legal firms.";
      }

      // Validate Website Links (should be a valid URL)
      if (
        !formData.websiteLinks ||
        (formData.websiteLinks.trim() &&
          !/^https?:\/\/[^\s]+$/.test(formData.websiteLinks))
      ) {
        newErrors.websiteLinks = "Please enter a valid website URL.";
      }

      // Validate Immigration Services (must have at least one selection)
      if (
        !formData.immigrationServices ||
        formData.immigrationServices.length === 0
      ) {
        newErrors.immigrationServices = "Please select at least one service.";
      }

      // Validate Languages Spoken (must have at least one selection)
      if (!formData.languagesSpoken || formData.languagesSpoken.length === 0) {
        newErrors.languagesSpoken = "Please select at least one language.";
      }
    } else if (currentStep === 3) {
      if (!formData.governmentId) {
        newErrors.governmentId = "Government ID is required.";
      }
      if (!formData.businessVerification) {
        newErrors.businessVerification =
          "Business verification document is required.";
      }
      if (!formData.licenseDocument) {
        newErrors.licenseDocument = "License document is required.";
      }
    } else if (currentStep === 4) {
      if (formData.backgroundCheckApproved === false) {
        newErrors.backgroundCheckApproved =
          "Please accept the background verification.";
      }
      if (formData.termsAccepted === false) {
        newErrors.termsAccepted = "Please accept the terms and conditions.";
      }
    }

    setErrors(newErrors);
    return Object.keys(newErrors).length === 0;
  };

  const handleNextStep = () => {
    if (validateForm()) {
      setCurrentStep((prevStep) => prevStep + 1);
    }
  };

  const handlePreviousStep = () => {
    setCurrentStep((prevStep) => prevStep - 1);
  };

  const [isLoading, setIsLoading] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const handleSubmit = async () => {
    setIsLoading(true);

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataToSend = new FormData();
      formDataToSend.append("fullName", formData.fullName);
      formDataToSend.append("phoneNo", formData.phoneNumber);
      formDataToSend.append("DOB", formData.dateOfBirth);
      formDataToSend.append("rolename", "Immigration Consultant");
      formDataToSend.append("businessName", formData.businessName);
      formDataToSend.append("businessAddress", formData.businessAddress);
      formDataToSend.append(
        "businessRegistration",
        formData.businessRegistrationNumber
      );
      formDataToSend.append("yearsOfExperience", formData.yearsOfExperience);
      formDataToSend.append("licenseNumber", formData.licenseNumber);
      formDataToSend.append(
        "countriesServed",
        formData.countriesServed.join(",")
      );
      formDataToSend.append(
        "consultationFee",
        String(formData.consultationFee)
      );
      formDataToSend.append(
        "partneredLegalFirms",
        formData.partneredLegalFirms
      );
      formDataToSend.append("websiteLinks", formData.websiteLinks);
      formDataToSend.append(
        "servicesOffered",
        formData.immigrationServices.join(",")
      );
      formDataToSend.append(
        "languagesSpoken",
        formData.languagesSpoken.join(",")
      );
      formDataToSend.append("govId", formData.governmentId);
      formDataToSend.append("licenseCert", formData.licenseDocument);
      formDataToSend.append("businessDoc", formData.businessVerification);
      formDataToSend.append(
        "backgroundVerification",
        formData.backgroundCheckApproved.toString()
      );
      formDataToSend.append(
        "termsConditionCheck",
        formData.termsAccepted.toString()
      );

      const response = await fetch(`${endpoint}api/onboarding/information`, {
        method: "POST",
        headers: {
          Authorization: `Bearer ${token}`,
        },
        body: formDataToSend,
      });

      if (!response.ok) {
        const errorData = await response.json();
        throw new Error(errorData.error || "Failed to submit form");
      }

      router.push("/dashboard/not-verified?reason=user");
    } catch (error) {
      console.error("Submission error:", error);
    } finally {
      setIsLoading(false);
    }
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl w-full min-h-[600px] h-full">
        <div className="py-8 px-6 shadow text-center w-full h-full flex flex-col justify-between">
          {currentStep === 1 && (
            <div>
              <PersonalInformation
                formData={formData}
                setFormData={setFormData}
                errors={errors}
              />
            </div>
          )}
          {currentStep === 2 && (
            <div>
              <BusinessInformation
                formData={formData}
                setFormData={setFormData}
                errors={errors}
              />
            </div>
          )}
          {currentStep === 3 && (
            <div>
              <DocumentUpload
                formData={formData}
                setFormData={setFormData}
                errors={errors}
              />
            </div>
          )}
          {currentStep === 4 && (
            <div>
              <TermsAndConditions
                formData={formData}
                setFormData={setFormData}
                errors={errors}
              />
            </div>
          )}
          {currentStep === 5 && <SuccessPage formData={formData} />}
          <div className="flex gap-4 justify-center">
            {currentStep == 1 && (
              <Button onClick={() => router.push("/onboarding")}>Back</Button>
            )}
            {currentStep > 1 && (
              <Button onClick={handlePreviousStep}>Back</Button>
            )}
            {currentStep < 5 && <Button onClick={handleNextStep}>Next</Button>}
            {currentStep === 5 && (
              <Button onClick={handleSubmit} disabled={isLoading}>
                {isLoading ? "Submitting..." : "Submit"}
              </Button>
            )}
          </div>
        </div>
      </div>
    </div>
  );
};

export default Consultant;
````

## File: src/app/(auth)/onboarding/consultant/SuccessPage.tsx
````typescript
import React from "react";
import { FormData } from "./types";

const SuccessPage: React.FC<{ formData: FormData }> = ({ formData }) => {
  return (
    <div className="flex flex-col justify-center">
      <h2 className="text-xl font-semibold mb-2">Review Details</h2>
      <p className="text-center mb-4">
        Please review the details you have provided below.
      </p>
      <span className="flex justify-between mb-1">
        <strong>Full Name:</strong> {formData.fullName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Email:</strong> {formData.email}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Phone Number:</strong> {formData.phoneNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Date of Birth:</strong> {formData.dateOfBirth}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Countries Served:</strong> {formData.countriesServed.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Consultation Fee:</strong> {formData.consultationFee}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Registration Number:</strong>{" "}
        {formData.businessRegistrationNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Partnered Legal Firms:</strong> {formData.partneredLegalFirms}
      </span>
    
      <span className="flex justify-between mb-1">
        <strong>Website Links:</strong> {formData.websiteLinks}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Name:</strong> {formData.businessName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Address:</strong> {formData.businessAddress}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Years of Experience:</strong> {formData.yearsOfExperience}
      </span>
      <span className="flex justify-between mb-1">
        <strong>License Number:</strong> {formData.licenseNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Immigration Services:</strong>{" "}
        {formData.immigrationServices.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Languages Spoken:</strong> {formData.languagesSpoken.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Government ID:</strong>{" "}
        {formData.governmentId ? "Provided" : "Not Provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Verification:</strong>{" "}
        {formData.businessVerification ? "Provided" : "Not Provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>License Document:</strong>{" "}
        {formData.licenseDocument ? "Provided" : "Not Provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Background Check Approved:</strong>{" "}
        {formData.backgroundCheckApproved ? "Yes" : "No"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Terms Accepted:</strong> {formData.termsAccepted ? "Yes" : "No"}
      </span>
    </div>
  );
};

export default SuccessPage;
````

## File: src/app/(auth)/onboarding/consultant/types.ts
````typescript
export interface FormData {
  fullName: string;
  email: string;
  phoneNumber: string;
  dateOfBirth: string;
  countriesServed: string[];
  consultationFee: number;
  businessRegistrationNumber: string;
  partneredLegalFirms: string;
  websiteLinks: string;
  businessName: string;
  businessAddress: string;
  yearsOfExperience: string;
  licenseNumber: string;
  immigrationServices: string[];
  languagesSpoken: string[];
  governmentId: string | Blob;
  businessVerification: string | Blob;
  licenseDocument: string | Blob;
  backgroundCheckApproved: boolean;
  termsAccepted: boolean;
}
````

## File: src/app/(auth)/onboarding/layout.tsx
````typescript
import { getSession } from "@/lib/auth";
import { redirect } from "next/navigation";
import { ReactNode } from "react";

async function Layout({ children }: { children: ReactNode }) {
  const session = await getSession();

  if (!session) {
    redirect("/login");
  }

  return <main className="w-full h-full">{children}</main>;
}

export default Layout;
````

## File: src/app/(auth)/onboarding/realtor/BusinessInformation.tsx
````typescript
import React from "react";
import { FormData } from "./types";
import { Label } from "@/components/ui/label";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import Select, { MultiValue } from "react-select";
import {
  Select as SingleSelect,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";

type OptionType = { value: string; label: string };

const areasCoveredOptions: OptionType[] = [
  { value: "city", label: "City" },
  { value: "region", label: "Region" },
];

const specialtiesOptions: OptionType[] = [
  { value: "rentals", label: "Rentals" },
  { value: "sales", label: "Sales" },
  { value: "commercial", label: "Commercial" },
  { value: "residential", label: "Residential" },
  { value: "luxury", label: "Luxury Homes" },
];

const BusinessInformation: React.FC<{
  formData: FormData;
  setFormData: React.Dispatch<React.SetStateAction<FormData>>;
  errors: { [key: string]: string }; // Define errors as an object
}> = ({ formData, setFormData, errors }) => {

  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Business Information</h2>
      <div className="flex justify-between items-center">
        <Label>Business Name:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessName || ""}
          onChange={(e) =>
            setFormData({ ...formData, businessName: e.target.value })
          }
        />
      </div>
      {errors.businessName && <p className="text-red-500 text-sm mb-4">{errors.businessName}</p>}
      <div className="flex justify-between items-center">
        <Label>Business Address:</Label>
        <Textarea
          className="w-2/3 mb-4"
          value={formData.businessAddress || ""}
          onChange={(e) =>
            setFormData({ ...formData, businessAddress: e.target.value })
          }
        />
      </div>
      {errors.businessAddress && <p className="text-red-500 text-sm mb-4">{errors.businessAddress}</p>}
      <div className="flex justify-between items-center">
        <Label>License Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.licenseNumber || ""}
          onChange={(e) =>
            setFormData({ ...formData, licenseNumber: e.target.value })
          }
        />
      </div>
      {errors.licenseNumber && <p className="text-red-500 text-sm mb-4">{errors.licenseNumber}</p>}
      <div className="flex justify-between items-center">
        <Label>Years of Experience:</Label>
        <SingleSelect
          value={formData.yearsOfExperience || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, yearsOfExperience: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select Years of Expereince" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="1-5">1-5 years</SelectItem>
            <SelectItem value="5-10">5-10 years</SelectItem>
            <SelectItem value="10+">10+ years</SelectItem>
          </SelectContent>
        </SingleSelect>
      </div>
      {errors.yearsOfExperience && <p className="text-red-500 text-sm mb-4">{errors.yearsOfExperience}</p>}
      <div className="flex justify-between items-center">
        <Label>Affiliated Associations:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.affiliatedAssociations || ""}
          onChange={(e) =>
            setFormData({ ...formData, affiliatedAssociations: e.target.value })
          }
        />
      </div>
      {errors.affiliatedAssociations && <p className="text-red-500 text-sm mb-4">{errors.affiliatedAssociations}</p>}
      <div className="flex justify-between items-center">
        <Label>Areas Covered:</Label>
        <Select
          isMulti
          options={areasCoveredOptions}
          value={areasCoveredOptions.filter((option) =>
            formData.areasCovered?.includes(option.value)
          )}
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              areasCovered: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.areasCovered && <p className="text-red-500 text-sm mb-4">{errors.areasCovered}</p>}
      <div className="flex justify-between items-center">
        <Label>Specialties:</Label>
        <Select
          isMulti
          options={specialtiesOptions}
          value={
            formData.specialties?.length
              ? specialtiesOptions.filter((option) =>
                  formData.specialties.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              specialties: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.specialties && <p className="text-red-500 text-sm mb-4">{errors.specialties}</p>}
      <div className="flex justify-between items-center">
        <Label>Portfolio/Website Link:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.portfolioLink || ""}
          onChange={(e) =>
            setFormData({ ...formData, portfolioLink: e.target.value })
          }
        />
      </div>
      {errors.portfolioLinkRequired && <p className="text-red-500 text-sm mb-4">{errors.portfolioLinkRequired}</p>}
      {errors.portfolioLink && <p className="text-red-500 text-sm mb-4">{errors.portfolioLink}</p>}
      <div className="flex justify-between items-center">
        <Label>Registration Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.registrationNumber || ""}
          onChange={(e) =>
            setFormData({ ...formData, registrationNumber: e.target.value })
          }
        />
      </div>
      {errors.registrationNumber && <p className="text-red-500 text-sm mb-4">{errors.registrationNumber}</p>}
    </div>
  );
};

export default BusinessInformation;
````

## File: src/app/(auth)/onboarding/realtor/OfficeWorkSetup.tsx
````typescript
import React from "react";
import { FormData } from "./types";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";
import { RadioGroup, RadioGroupItem } from "@/components/ui/radio-group";

const OfficeWorkSetup: React.FC<{
  formData: FormData;
  setFormData: React.Dispatch<React.SetStateAction<FormData>>;
  errors: { [key: string]: string };
}> = ({ formData, setFormData, errors }) => {
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Office & Work Setup</h2>

      <div className="flex justify-between items-center">
        <Label>Work Type:</Label>
        <RadioGroup
          className="flex gap-4  mb-4"
          value={formData.workType || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, workType: value })
          }
        >
          <RadioGroupItem value="brokerage" id="brokerage" />
          <Label htmlFor="brokerage" className="mr-4">
            Brokerage
          </Label>

          <RadioGroupItem value="independent" id="independent" />
          <Label htmlFor="independent">Independent</Label>
        </RadioGroup>
      </div>
      {errors.workType && <p className="text-red-500 text-sm mb-4">{errors.workType}</p>}

      {formData.workType === "brokerage" && (
        <div className="flex justify-between items-center">
          <Label>Brokerage Name:</Label>
          <Input
            type="text"
            className="w-2/3 mb-4"
            value={formData.brokerageName || ""}
            onChange={(e) =>
              setFormData({ ...formData, brokerageName: e.target.value })
            }
          />
        </div>
        
      )}
      {errors.brokerageName && <p className="text-red-500 text-sm mb-4">{errors.brokerageName}</p>}

      <div className="flex justify-between items-center">
        <Label>Office Location:</Label>
        <Select
          value={formData.officeLocationAvailability || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, officeLocationAvailability: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select availability" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="yes">Yes</SelectItem>
            <SelectItem value="no">No</SelectItem>
          </SelectContent>
        </Select>
      </div>
      {errors.officeLocationAvailability && <p className="text-red-500 text-sm mb-4">{errors.officeLocationAvailability}</p>}

      <div className="flex justify-between items-center">
        <Label>Total Team Members:</Label>
        <Input
          type="number"
          className="w-2/3 mb-4"
          value={formData.numberOfTeamMembers || 1}
          onChange={(e) =>
            setFormData({
              ...formData,
              numberOfTeamMembers: parseInt(e.target.value, 10),
            })
          }
        />
      </div>
      
      <div className="flex justify-between items-center">
        <Label>Virtual Property Tour:</Label>
        <Select
          value={formData.virtualTourAvailability || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, virtualTourAvailability: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select availability" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="yes">Yes</SelectItem>
            <SelectItem value="no">No</SelectItem>
          </SelectContent>
        </Select>
      </div>
      {errors.virtualTourAvailability && <p className="text-red-500 text-sm mb-4">{errors.virtualTourAvailability}</p>}
    </div>
  );
};

export default OfficeWorkSetup;
````

## File: src/app/(auth)/onboarding/realtor/page.tsx
````typescript
"use client";

import React, { useState } from "react";
import BusinessInformation from "./BusinessInformation";
import OfficeWorkSetup from "./OfficeWorkSetup";
import SuccessPage from "./SuccessPage";
import type { FormData } from "./types";
import { Button } from "@/components/ui/button";
import PersonalInformation from "@/components/onboarding/PersonalInformation";
import TermsAndConditions from "@/components/onboarding/TermsAndConditions";
import DocumentUpload from "@/components/onboarding/DocumentUpload";
import { useRouter } from "next/navigation";

const Realtor = () => {
  const [currentStep, setCurrentStep] = useState(1);
  const router = useRouter();
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  const [errors, setErrors] = useState({});
  const [isSubmitting, setIsSubmitting] = useState(false);
  const [formData, setFormData] = useState<FormData>({
    fullName: "",
    phoneNumber: "",
    dateOfBirth: "",
    businessName: "",
    businessAddress: "",
    licenseNumber: "",
    yearsOfExperience: "",
    affiliatedAssociations: "",
    areasCovered: [],
    specialties: [],
    portfolioLink: "",
    registrationNumber: "",
    workType: "",
    brokerageName: "",
    officeLocationAvailability: "",
    numberOfTeamMembers: 0,
    virtualTourAvailability: "",
    governmentId: "",
    businessVerification: "",
    licenseDocument: "",
    backgroundCheckApproved: false,
    termsAccepted: false,
  });

  const validateForm = () => {
    const newErrors: Record<string, string> = {};

    if (currentStep === 1) {
      // Full Name Validation
      if (!formData.fullName || formData.fullName.length < 3) {
        newErrors.fullName = "Full Name must be at least 3 characters";
      }

      // Phone Number Validations
      if (!formData.phoneNumber) {
        newErrors.phoneNumber = "Phone number is required";
      } else if (!/^\d+$/.test(formData.phoneNumber)) {
        newErrors.phoneNumber = "Phone number must contain only digits";
      } else if (formData.phoneNumber.length !== 10) {
        newErrors.phoneLength = "Phone number must be exactly 10 digits";
      }

      // Date of Birth Validation (Minimum 15 years old)
      if (!formData.dateOfBirth) {
        newErrors.dateOfBirth = "Date of Birth is required";
      } else {
        const dob = new Date(formData.dateOfBirth);
        const today = new Date();
        const minDate = new Date();
        minDate.setFullYear(today.getFullYear() - 15); // 15 years ago

        if (dob > minDate) {
          newErrors.dateOfBirth = "You must be at least 15 years old";
        }
      }
    } else if (currentStep === 2) {
      // Business Name Validation
      if (!formData.businessName || formData.businessName.trim() === "") {
        newErrors.businessName = "Business name is required.";
      }

      // Business Address Validation
      if (!formData.businessAddress || formData.businessAddress.trim() === "") {
        newErrors.businessAddress = "Business address is required.";
      }

      // License Number Validation
      if (!formData.licenseNumber || formData.licenseNumber.trim() === "") {
        newErrors.licenseNumber = "License number is required.";
      }

      // Years of Experience Validation
      if (!formData.yearsOfExperience) {
        newErrors.yearsOfExperience = "Years of experience is required.";
      }

      // Affiliated Associations Validation
      if (
        !formData.affiliatedAssociations ||
        formData.affiliatedAssociations.trim() === ""
      ) {
        newErrors.affiliatedAssociations =
          "Affiliated associations are required.";
      }

      // Areas Covered Validation (at least one required)
      if (!formData.areasCovered || formData.areasCovered.length === 0) {
        newErrors.areasCovered = "At least one area must be selected.";
      }

      // Specialties Validation (at least one required)
      if (!formData.specialties || formData.specialties.length === 0) {
        newErrors.specialties = "At least one specialty must be selected.";
      }

      if (!formData.portfolioLink) {
        newErrors.portfolioLinkRequired = "Link is required";
      } else if (
        !/^https?:\/\/[^\s$.?#].[^\s]*$/.test(formData.portfolioLink)
      ) {
        newErrors.portfolioLink = "Invalid website link.";
      }

      // Registration Number Validation
      if (
        !formData.registrationNumber ||
        formData.registrationNumber.trim() === ""
      ) {
        newErrors.registrationNumber = "Registration number is required.";
      }
    } else if (currentStep === 3) {
      if (!formData.workType) {
        newErrors.workType = "Work type is required.";
      }

      if (formData.workType === "brokerage" && !formData.brokerageName) {
        newErrors.brokerageName = "Brokerage name is required.";
      }

      if (!formData.officeLocationAvailability) {
        newErrors.officeLocationAvailability =
          "Please select office location availability.";
      }

      if (!formData.virtualTourAvailability) {
        newErrors.virtualTourAvailability =
          "Please select virtual tour availability.";
      }
    } else if (currentStep === 4) {
      if (!formData.governmentId) {
        newErrors.governmentId = "Government ID is required.";
      }
      if (!formData.businessVerification) {
        newErrors.businessVerification =
          "Business verification document is required.";
      }
      if (!formData.licenseDocument) {
        newErrors.licenseDocument = "License document is required.";
      }
    } else if (currentStep === 5) {
      if (formData.backgroundCheckApproved === false) {
        newErrors.backgroundCheckApproved =
          "Please accept the background verification.";
      }
      if (formData.termsAccepted === false) {
        newErrors.termsAccepted = "Please accept the terms and conditions.";
      }
    }

    setErrors(newErrors);
    return Object.keys(newErrors).length === 0;
  };

  const handleNextStep = () => {
    if (validateForm()) {
      setCurrentStep((prevStep) => prevStep + 1);
    }
  };

  const handlePreviousStep = () => {
    setCurrentStep((prevStep) => prevStep - 1);
  };

  const handleSubmit = async () => {
    if (isSubmitting) return; // Prevent multiple submissions
    setIsSubmitting(true);
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataToSend = new FormData();
      formDataToSend.append("fullName", formData.fullName);
      formDataToSend.append("phoneNo", formData.phoneNumber);
      formDataToSend.append("DOB", formData.dateOfBirth);
      formDataToSend.append("rolename", "Realtor");
      formDataToSend.append("businessName", formData.businessName);
      formDataToSend.append("businessAddress", formData.businessAddress);
      formDataToSend.append("realEstateLicenseNumber", formData.licenseNumber);
      formDataToSend.append("experienceYears", formData.yearsOfExperience);
      formDataToSend.append(
        "affiliatedAssociations",
        formData.affiliatedAssociations
      );
      formDataToSend.append("areasCovered", formData.areasCovered.join(","));
      formDataToSend.append("specialties", formData.specialties.join(","));
      formDataToSend.append("portfolioLink", formData.portfolioLink);
      formDataToSend.append("registrationNumber", formData.registrationNumber);
      formDataToSend.append("workType", formData.workType);
      formDataToSend.append("brokerageName", formData.brokerageName);
      formDataToSend.append(
        "officeLocationAvailable",
        String(formData.officeLocationAvailability === "yes")
      );
      formDataToSend.append(
        "teamMembers",
        String(formData.numberOfTeamMembers ?? "")
      );
      formDataToSend.append(
        "virtualPropertyTour",
        String(formData.virtualTourAvailability === "yes")
      );

      formDataToSend.append("govId", formData.governmentId);
      formDataToSend.append("businessDoc", formData.businessVerification);
      formDataToSend.append("licenseCert", formData.licenseDocument);
      formDataToSend.append(
        "backgroundVerification",
        formData.backgroundCheckApproved.toString()
      );
      formDataToSend.append(
        "termsConditionCheck",
        formData.termsAccepted.toString()
      );

      const response = await fetch(`${endpoint}api/onboarding/information`, {
        method: "POST",
        headers: {
          Authorization: `Bearer ${token}`,
        },
        body: formDataToSend,
      });

      const data = await response.json();

      if (response.ok) {
        router.push("/dashboard/not-verified?reason=user");
      } else {
        console.error(
          "Failed to create user and upload documents:",
          data.error
        );
        // Handle error (e.g., show an error message)
      }
    } catch (error) {
      console.error("Error:", error);
      // Handle error (e.g., show an error message)
    } finally {
      setIsSubmitting(false);
    }
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl w-full min-h-[600px] h-full">
        <div className="py-8 px-6 shadow text-center w-full h-full flex flex-col justify-between">
          {currentStep === 1 && (
            <PersonalInformation
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 2 && (
            <BusinessInformation
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 3 && (
            <OfficeWorkSetup
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 4 && (
            <DocumentUpload
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 5 && (
            <TermsAndConditions
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 6 && <SuccessPage formData={formData} />}
          <div className="flex gap-4 justify-center">
            {currentStep > 1 && (
              <Button onClick={handlePreviousStep}>Back</Button>
            )}
            {currentStep == 1 && (
              <Button onClick={() => router.push("/onboarding")}>Back</Button>
            )}
            {currentStep < 6 && <Button onClick={handleNextStep}>Next</Button>}
            {currentStep === 6 && (
              <Button onClick={handleSubmit} disabled={isSubmitting}>
                {isSubmitting ? "Submitting..." : "Submit"}
              </Button>
            )}
          </div>
        </div>
      </div>
    </div>
  );
};

export default Realtor;
````

## File: src/app/(auth)/onboarding/realtor/SuccessPage.tsx
````typescript
import React from "react";
import { FormData } from "./types";

const SuccessPage: React.FC<{ formData: FormData }> = ({ formData }) => {
  return (
    <div className="flex flex-col justify-center">
      <h2 className="text-xl font-semibold mb-2">Review Details</h2>
      <p className="text-center mb-4">
        Please review the details you have provided below.
      </p>
      <span className="flex justify-between mb-1">
        <strong>Full Name:</strong> {formData.fullName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Phone Number:</strong> {formData.phoneNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Date of Birth:</strong> {formData.dateOfBirth}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Name:</strong> {formData.businessName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Address:</strong> {formData.businessAddress}
      </span>
      <span className="flex justify-between mb-1">
        <strong>License Number:</strong> {formData.licenseNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Years of Experience:</strong> {formData.yearsOfExperience}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Affiliated Associations:</strong>{" "}
        {formData.affiliatedAssociations}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Areas Covered:</strong> {formData.areasCovered.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Specialties:</strong> {formData.specialties.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Portfolio Link:</strong> {formData.portfolioLink}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Registration Number:</strong> {formData.registrationNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Background Check Approved:</strong>{" "}
        {formData.backgroundCheckApproved? "Yes" : "No"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Terms Accepted:</strong> {formData.termsAccepted ? "Yes" : "No"}
      </span>
    </div>
  );
};

export default SuccessPage;
````

## File: src/app/(auth)/onboarding/realtor/types.ts
````typescript
export interface FormData {
  fullName: string;
  phoneNumber: string;
  dateOfBirth: string;
  businessName: string;
  businessAddress: string;
  licenseNumber: string;
  yearsOfExperience: string;
  affiliatedAssociations: string;
  areasCovered: string[];
  specialties: string[];
  portfolioLink: string;
  registrationNumber: string;
  workType: string;
  brokerageName: string;
  officeLocationAvailability: string;
  numberOfTeamMembers: number;
  virtualTourAvailability: string;
  governmentId: string | Blob;
  businessVerification: string | Blob;
  licenseDocument: string | Blob;
  backgroundCheckApproved: boolean;
  termsAccepted: boolean;
}
````

## File: src/app/api/ai/resume/analyses/route.ts
````typescript
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
      { success: false, message: 'Failed to fetch resume analyses', error: error.message },
      { status: 500 }
    );
  }
}
````

## File: src/app/api/career/search-jobs/route.ts
````typescript
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
````

## File: src/app/dashboard/car-dealer/availability/page.tsx
````typescript
"use client";
import Availability from "@/components/availability/AvailabilityPage";
import SideCard from "@/components/Sidecard";


const services = ["Dashboard", "Listings","Availability", "Bookings"];
  const urls = ["/dashboard/car-dealer", "/dashboard/car-dealer/car-listings/", "/dashboard/car-dealer/availability/", "/dashboard/car-dealer/bookings/"];


const RealtorAvailability = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <Availability />
      </div>
    </div>
  );
};

export default RealtorAvailability;
````

## File: src/app/dashboard/car-dealer/bookings/page.tsx
````typescript
"use client";
import BookingTable from "@/components/availability/BookingTable";
import SideCard from "@/components/Sidecard";

const services = ["Dashboard", "Listings","Availability", "Bookings"];
  const urls = ["/dashboard/car-dealer", "/dashboard/car-dealer/car-listings/", "/dashboard/car-dealer/availability/", "/dashboard/car-dealer/bookings/"];


const CarBooking = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <BookingTable />
      </div>
    </div>
  );
};

export default CarBooking;
````

## File: src/app/dashboard/car-dealer/car-listings/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Listings",
  "Availability",
  "Bookings",
  "Profile",
];
const urls = [
  "/dashboard/car-dealer",
  "/dashboard/car-dealer/car-listings/",
  "/dashboard/car-dealer/availability/",
  "/dashboard/car-dealer/bookings/",
  "/dashboard/car-dealer/profile",
];

const CarsListing = () => {
  const [carListings, setCarListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);
  const [refresh, setRefresh] = useState(false);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const carResponse = await fetch(
          `${endpoint}api/protected/car-listing/by-id-car-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!carResponse.ok) throw new Error("Failed to fetch car listings");

        const carData = await carResponse.json();
        setCarListings(carData);
        setFilteredListings(carData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);
  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = carListings.filter((car) => {
      return (
        (!filters.make ||
          car.make?.toLowerCase().includes(filters.make.toLowerCase())) &&
        (!filters.model ||
          car.model?.toLowerCase().includes(filters.model.toLowerCase())) &&
        (!filters.price || car.price <= parseFloat(filters.price))
      );
    });

    setFilteredListings(filtered.slice());
  };

  // Debugging UI Update
  useEffect(() => {}, [filteredListings]);

  const carFiltersConfig = [
    { name: "make", type: "text", placeholder: "Make (e.g. Toyota)" },
    { name: "model", type: "text", placeholder: "Model (e.g. Corolla)" },
    { name: "price", type: "number", placeholder: "Max Price" },
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Links" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Cars Listing</h2>
          <ReusableFilter
            filtersConfig={carFiltersConfig}
            onFilterChange={handleFilterChange}
          />
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && filteredListings.length > 0 ? (
          <Listings key={refresh} listings={filteredListings} />
        ) : (
          <p>No cars found.</p>
        )}
      </div>
    </div>
  );
};

export default CarsListing;
````

## File: src/app/dashboard/car-dealer/page.tsx
````typescript
"use client";

import QuickLinks from "@/components/QuickLinks";
import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import { useEffect, useState } from "react";

export default function DashboardLayout() {
  const [listings, setListings] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  const services = ["Dashboard", "Listings","Availability", "Bookings"];
  const urls = ["/dashboard/car-dealer", "/dashboard/car-dealer/car-listings/", "/dashboard/car-dealer/availability/", "/dashboard/car-dealer/bookings/"];

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        // Fetch token
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });

        if (!tokenResponse.ok) {
          throw new Error("Failed to get authentication token");
        }

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;

        if (!token) {
          throw new Error("Invalid authentication token");
        }

        // Fetch car listings
        const response = await fetch(
          `${endpoint}api/protected/car-listing/by-id-car-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (response.status === 404) {
          throw new Error("No listing found");
        }
        

        const data = await response.json();
        setListings(data);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Links" urls={urls}/>
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Car Dealer Dashboard</h2>
          <QuickLinks links={[
            { label: "Add Listing", href: "car-dealer/add-listing" },
            { label: "View Listings", href: "car-dealer/car-listings" },
            { label: "Requests", href: "car-dealer/availability" },
          ]} />
          <h2 className="text-2xl font-bold mb-6 mt-5">View added listings</h2>
          {loading && <p>Loading...</p>}
          {error && <p>Error: {error}</p>}
          {!loading && !error && listings && <Listings listings={listings} />}
        </div>
      </div>
    </div>
  );
}
````

## File: src/app/dashboard/consultant/availability/page.tsx
````typescript
"use client";
import Availability from "@/components/availability/AvailabilityPage";
import SideCard from "@/components/Sidecard";



const services = ["Dashboard", "Availability", "Bookings"];
const urls = ["/dashboard/consultant", "/dashboard/consultant/availability", "/dashboard/consultant/bookings/"];



const ICAvailability = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <Availability />
      </div>
    </div>
  );
};

export default ICAvailability;
````

## File: src/app/dashboard/consultant/bookings/page.tsx
````typescript
"use client";
import BookingTable from "@/components/availability/BookingTable";
import SideCard from "@/components/Sidecard";


const services = ["Dashboard", "Availability", "Bookings"];
const urls = ["/dashboard/consultant", "/dashboard/consultant/availability", "/dashboard/consultant/bookings/"];



const ICBooking = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <BookingTable />
      </div>
    </div>
  );
};

export default ICBooking;
````

## File: src/app/dashboard/consultant/page.tsx
````typescript
"use client";

import QuickLinks from "@/components/QuickLinks";
import SideCard from "@/components/Sidecard";
import UpcomingConsultantMeetings from "@/components/consultant/UpcomingMeetings";
// import { useEffect, useState } from "react";

export default function DashboardLayout() {

  const services = ["Dashboard", "Availability", "Bookings"];
  const urls = ["/dashboard/consultant", "/dashboard/consultant/availability", "/dashboard/consultant/bookings/"];

 
  //   const fetchListings = async () => {
  //     try {
  //       const endpoint = process.env.NEXT_PUBLIC_API_URL;

  //       // Fetch token
  //       const tokenResponse = await fetch(`${endpoint}auth/token`, {
  //         credentials: "include",
  //       });

  //       if (!tokenResponse.ok) {
  //         throw new Error("Failed to get authentication token");
  //       }

  //       const tokenData = await tokenResponse.json();
  //       const token = tokenData?.token;

  //       if (!token) {
  //         throw new Error("Invalid authentication token");
  //       }

  //       // Fetch car listings
  //       const response = await fetch(
  //         `${endpoint}api/protected/`,
  //         {
  //           headers: { Authorization: `Bearer ${token}` },
  //         }
  //       );

  //       if (response.status === 404) {
  //         throw new Error("No listing found");
  //       }
        

  //       const data = await response.json();
  //       setListings(data);
  //     } catch (err) {
  //       setError(err.message);
  //     } finally {
  //       setLoading(false);
  //     }
  //   };

  //   fetchListings();
  // }, []);

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Links" urls={urls}/>
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Immigration Consultant Dashboard</h2>
          <QuickLinks links={[
            { label: "Add Availability", href: "/dashboard/consultant/availability" },
            { label: "View Bookings", href: "/dashboard/consultant/bookings" },
          ]} />
          <h2 className="text-2xl font-bold mb-6 mt-5">Upcoming Meetings</h2>
          {/* {loading && <p>Loading...</p>}
          {error && <p>Error: {error}</p>}
          {!loading && !error && listings && <Listings listings={listings} />} */}
          <UpcomingConsultantMeetings/>
        </div>
      </div>
    </div>
  );
}
````

## File: src/app/dashboard/layout.tsx
````typescript
import Header from "@/components/Header";
import { redirect } from "next/navigation";
import { getSession } from "@/lib/auth";
import React, { ReactNode } from "react";

async function Layout({ children }: { children: ReactNode }) {
  const session = await getSession();

  if (!session) {
    redirect("/");
  }

  return (
    <div className="flex flex-col h-screen min-w-full bg-background">
      <Header />
      <main className="w-full h-full">{children}</main>
    </div>
  );
}

export default Layout;
````

## File: src/app/dashboard/page.tsx
````typescript
import React from "react";

const Dashboard = () => {
  return <div>Dashboard</div>;
};

export default Dashboard;
````

## File: src/app/dashboard/realtor/availability/page.tsx
````typescript
"use client";
import Availability from "@/components/availability/AvailabilityPage";
import SideCard from "@/components/Sidecard";

const services = ["Dashboard", "Listings", "Availability","Bookings"];
const urls = ["/dashboard/realtor", "/dashboard/realtor/house-listings", "/dashboard/realtor/availability", "/dashboard/realtor/bookings"];


const RealtorAvailability = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <Availability />
      </div>
    </div>
  );
};

export default RealtorAvailability;
````

## File: src/app/dashboard/realtor/bookings/page.tsx
````typescript
"use client";
import BookingTable from "@/components/availability/BookingTable";
import SideCard from "@/components/Sidecard";

const services = ["Dashboard", "Listings", "Availability","Bookings"];
const urls = ["/dashboard/realtor", "/dashboard/realtor/house-listings", "/dashboard/realtor/availability", "/dashboard/realtor/bookings"];


const RealtorBooking = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <BookingTable />
      </div>
    </div>
  );
};

export default RealtorBooking;
````

## File: src/app/dashboard/realtor/house-listings/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Listings",
  "Availability",
  "Bookings",
  "Profile",
];
const urls = [
  "/dashboard/realtor",
  "/dashboard/realtor/house-listings",
  "/dashboard/realtor/availability",
  "/dashboard/realtor/bookings",
  "/dashboard/profile",
];

const HousesListing = () => {
  const [houseListings, setHouseListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const houseResponse = await fetch(
          `${endpoint}api/protected/house-listing/all-house-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!houseResponse.ok)
          throw new Error("Failed to fetch house listings");

        const houseData = await houseResponse.json();
        setHouseListings(houseData);
        setFilteredListings(houseData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = houseListings.filter((house) => {
      const openHouseValue = house.openhouse ? "Yes" : "No"; // Convert boolean to string

      return (
        (!filters.location ||
          house.location
            ?.toLowerCase()
            .includes(filters.location.toLowerCase())) &&
        (!filters.price || house.price <= parseFloat(filters.price)) &&
        (!filters.openHouse || openHouseValue === filters.openHouse)
      );
    });

    setFilteredListings(filtered.slice());
  };

  // Debugging UI Update
  useEffect(() => {}, [filteredListings]);

  const houseFiltersConfig = [
    { name: "location", type: "text", placeholder: "Location (e.g. Toronto)" },
    { name: "price", type: "number", placeholder: "Max Price" },
    {
      name: "openHouse",
      type: "select",
      placeholder: "Open-House",
      options: ["Yes", "No"],
    },
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Houses Listing</h2>
          <ReusableFilter
            filtersConfig={houseFiltersConfig}
            onFilterChange={handleFilterChange}
          />
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && filteredListings.length > 0 ? (
          <Listings listings={filteredListings} />
        ) : (
          <p>No houses found.</p>
        )}
      </div>
    </div>
  );
};

export default HousesListing;
````

## File: src/app/dashboard/realtor/page.tsx
````typescript
'use client';

import QuickLinks from "@/components/QuickLinks";
import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import { useEffect, useState } from 'react';

export default function DashboardLayout() {
  const [listings, setListings] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  const services = ["Dashboard", "Listings", "Availability","Bookings"];
const urls = ["/dashboard/realtor", "/dashboard/realtor/house-listings", "/dashboard/realtor/availability", "/dashboard/realtor/bookings"];

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        // Fetch token
        const tokenResponse = await fetch(`${endpoint}auth/token`, { credentials: 'include' });

        if (!tokenResponse.ok) {
          throw new Error('Failed to get authentication token');
        }

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;

        if (!token) {
          throw new Error('Invalid authentication token');
        }

        // Fetch house listings
        const response = await fetch(`${endpoint}api/protected/house-listing/by-id-house-listing`, {
          headers: { Authorization: `Bearer ${token}` },
        });

        if (!response.ok) {
          throw new Error('Failed to fetch house listings');
        }

        const data = await response.json();
        setListings(data);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  return (
    <div className="grid grid-cols-12 h-screen"> {/* h-screen for full viewport height */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3"> {/* Fixed SideCard */}
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Realtor Dashboard</h2>
          <QuickLinks links={[
            { label: "Add Listing", href: "realtor/add-listing" },
            { label: "View Listings", href: "realtor/house-listings" },
            { label: "Requests", href: "realtor/availability" },
          ]} />
          <h2 className="text-2xl font-bold mb-6 mt-5">View added listings</h2>
          {loading && <p>Loading...</p>}
          {error && <p>Error: {error}</p>}
          {!loading && !error && listings && <Listings listings={listings} />}
        </div>
      </div>
    </div>
  );
}
````

## File: src/app/dashboard/user/bookings/page.tsx
````typescript
"use client";

import SideCard from "@/components/Sidecard";
import BookingView from "@/components/availability/UserBooking";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings"
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings"
];
const UserBooking = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <BookingView />
      </div>
    </div>
  );
};

export default UserBooking;
````

## File: src/app/dashboard/user/cars/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];
const CarsListing = () => {
  const [carListings, setCarListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);
  const [refresh, setRefresh] = useState(false);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const carResponse = await fetch(
          `${endpoint}api/protected/car-listing/all-car-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!carResponse.ok) throw new Error("Failed to fetch car listings");

        const carData = await carResponse.json();
        setCarListings(carData);
        setFilteredListings(carData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);
  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = carListings.filter((car) => {
      return (
        (!filters.make ||
          car.make?.toLowerCase().includes(filters.make.toLowerCase())) &&
        (!filters.model ||
          car.model?.toLowerCase().includes(filters.model.toLowerCase())) &&
        (!filters.price || car.price <= parseFloat(filters.price))
      );
    });

    setFilteredListings(filtered.slice());
  };

  // Debugging UI Update
  useEffect(() => {}, [filteredListings]);

  const carFiltersConfig = [
    { name: "make", type: "text", placeholder: "Make (e.g. Toyota)" },
    { name: "model", type: "text", placeholder: "Model (e.g. Corolla)" },
    { name: "price", type: "number", placeholder: "Max Price" },
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Cars Listing</h2>
          <ReusableFilter
            filtersConfig={carFiltersConfig}
            onFilterChange={handleFilterChange}
          />
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && filteredListings.length > 0 ? (
          <Listings key={refresh} listings={filteredListings} />
        ) : (
          <p>No cars found.</p>
        )}
      </div>
    </div>
  );
};

export default CarsListing;
````

## File: src/app/dashboard/user/consultant/page.tsx
````typescript
"use client";

import ConsultantCarousel from "@/components/consultant/ConsultantCarousel";
import SideCard from "@/components/Sidecard";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];
const ConsultantPage = () => {
  const [consultanatListings, setConsultanatListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const consultantResponse = await fetch(
          `${endpoint}api/protected/consultants/view-consultant`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!consultantResponse.ok)
          throw new Error("Failed to fetch car listings");

        const consultantData = await consultantResponse.json();
        setConsultanatListings(consultantData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Consultants</h2>
          {/* <ReusableFilter filtersConfig={carFiltersConfig} onFilterChange={handleFilterChange} /> */}
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && consultanatListings && (
          <ConsultantCarousel
            consultants={consultanatListings.consultants || []}
          />
        )}
      </div>
    </div>
  );
};

export default ConsultantPage;
````

## File: src/app/dashboard/user/favourites-car/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];

const FavouriteCars = () => {
  const [carListings, setCarListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchFavourites = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenRes = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenRes.ok) throw new Error("Failed to get token");

        const { token } = await tokenRes.json();
        if (!token) throw new Error("Token missing");

        const carRes = await fetch(
          `${endpoint}api/protected/car-listing/favourites`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!carRes.ok) throw new Error("Failed to fetch favourite cars");

        const data = await carRes.json();
        setCarListings(data);
        setFilteredListings(data);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchFavourites();
  }, []);

  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = carListings.filter((car) => {
      return (
        (!filters.make ||
          car.make?.toLowerCase().includes(filters.make.toLowerCase())) &&
        (!filters.model ||
          car.model?.toLowerCase().includes(filters.model.toLowerCase())) &&
        (!filters.price || car.price <= parseFloat(filters.price))
      );
    });

    setFilteredListings(filtered.slice());
  };

  const carFiltersConfig = [
    { name: "make", type: "text" as const, placeholder: "Make (e.g. Toyota)" },
    {
      name: "model",
      type: "text" as const,
      placeholder: "Model (e.g. Corolla)",
    },
    { name: "price", type: "number" as const, placeholder: "Max Price" },
  ];

  return (
    <div>
      <div className="container mx-auto">
        <h2 className="text-2xl font-bold mb-6 mt-4">Favourite Cars</h2>
        <ReusableFilter
          filtersConfig={carFiltersConfig}
          onFilterChange={handleFilterChange}
        />
      </div>
      {loading && <p>Loading...</p>}
      {error && <p className="text-red-500">Error: {error}</p>}
      {!loading && !error && filteredListings.length > 0 ? (
        <Listings listings={filteredListings} />
      ) : (
        <p>No favourite cars found.</p>
      )}
    </div>
  );
};

export default FavouriteCars;
````

## File: src/app/dashboard/user/favourites-house/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];

const FavouriteHouse = () => {
  const [houseListings, setHouseListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchFavourites = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenRes = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenRes.ok) throw new Error("Failed to get authentication token");

        const { token } = await tokenRes.json();
        if (!token) throw new Error("Invalid token");

        const response = await fetch(
          `${endpoint}api/protected/house-listing/favourites`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!response.ok) throw new Error("Failed to fetch favourite houses");

        const data = await response.json();
        setHouseListings(data);
        setFilteredListings(data);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchFavourites();
  }, []);

  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = houseListings.filter((house) => {
      const openHouseValue = house.openhouse ? "Yes" : "No";

      return (
        (!filters.location ||
          house.location
            ?.toLowerCase()
            .includes(filters.location.toLowerCase())) &&
        (!filters.price || house.price <= parseFloat(filters.price)) &&
        (!filters.openHouse || openHouseValue === filters.openHouse)
      );
    });

    setFilteredListings(filtered);
  };

  const houseFiltersConfig = [
    { name: "location", type: "text", placeholder: "Location (e.g. Toronto)" },
    { name: "price", type: "number", placeholder: "Max Price" },
    {
      name: "openHouse",
      type: "select",
      placeholder: "Open-House",
      options: ["Yes", "No"],
    },
  ];

  return (
    <div>
      <div className="container mx-auto">
        <h2 className="text-2xl font-bold mb-6 mt-4">Favourite Houses</h2>
        <ReusableFilter
          filtersConfig={houseFiltersConfig}
          onFilterChange={handleFilterChange}
        />
      </div>
      {loading && <p>Loading...</p>}
      {error && <p className="text-red-500">Error: {error}</p>}
      {!loading && !error && filteredListings.length > 0 ? (
        <Listings listings={filteredListings} />
      ) : (
        <p>No favourite houses found.</p>
      )}
    </div>
  );
};

export default FavouriteHouse;
````

## File: src/app/dashboard/user/homes/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];
const HousesListing = () => {
  const [houseListings, setHouseListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const houseResponse = await fetch(
          `${endpoint}api/protected/house-listing/all-house-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!houseResponse.ok)
          throw new Error("Failed to fetch house listings");

        const houseData = await houseResponse.json();
        setHouseListings(houseData);
        setFilteredListings(houseData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = houseListings.filter((house) => {
      const openHouseValue = house.openhouse ? "Yes" : "No"; // Convert boolean to string

      return (
        (!filters.location ||
          house.location
            ?.toLowerCase()
            .includes(filters.location.toLowerCase())) &&
        (!filters.price || house.price <= parseFloat(filters.price)) &&
        (!filters.openHouse || openHouseValue === filters.openHouse)
      );
    });

    setFilteredListings(filtered.slice());
  };
  
  // Debugging UI Update
  useEffect(() => {
  }, [filteredListings]);

  


  const houseFiltersConfig = [
    { name: "location", type: "text", placeholder: "Location (e.g. Toronto)" },
    { name: "price", type: "number", placeholder: "Max Price" },
    {
      name: "openHouse",
      type: "select",
      placeholder: "Open-House",
      options: ["Yes", "No"],
    },
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Houses Listing</h2>
          <ReusableFilter
            filtersConfig={houseFiltersConfig}
            onFilterChange={handleFilterChange}
          />
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && filteredListings.length > 0 ? (
          <Listings listings={filteredListings} />
        ) : (
          <p>No houses found.</p>
        )}
      </div>
    </div>
  );
};

export default HousesListing;
````

## File: src/app/dashboard/user/profile/page.tsx
````typescript
// /app/profile/page.tsx
"use client";

import React, { useEffect, useState } from "react";
import SideCard from "@/components/Sidecard";
import UserProfile from "@/components/UserProfile";

interface UserData {
  fullName: string;
  DOB: string;
  phoneNo: string;
  email: string;
  alreadyInCanada?: boolean | null;
  statusInCanada?: string | null;
  countryOfOrigin?: string | null;
  currentLocation?: string | null;
}

const ProfilePage: React.FC = () => {
  const [userData, setUserData] = useState<UserData | null>(null);
  const [loading, setLoading] = useState<boolean>(true);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  useEffect(() => {
    const fetchUserData = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
    
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
    
          const tokenData = await tokenResponse.json();
          const token = tokenData.token;
          const response = await fetch(`${endpoint}api/protected/profile`, {
            method: "GET",
            headers: {
              Authorization: `Bearer ${token}`,
            },
          });
       
        if (!response.ok) {
          throw new Error("Failed to fetch user data");
        }
        const data = await response.json();
        setUserData(data);
      } catch (error) {
        console.error("Error fetching user data:", error);
      } finally {
        setLoading(false);
      }
    };

    fetchUserData();
  }, []);

  const services = [
    "Dashboard",
    "Explore Homes",
    "Explore Cars",
    "Book Consultation",
    "Bookings"
  ];
  const urls = [
    "/dashboard/user",
    "/dashboard/user/homes",
    "/dashboard/user/cars",
    "/dashboard/user/consultant",
    "/dashboard/user/bookings"
  ];

  if (loading) {
    return <p className="text-center mt-10">Loading...</p>;
  }

  if (!userData) {
    return <p className="text-center mt-10">No user data available</p>;
  }

  return(
    <div className="grid grid-cols-12 h-full">
          <div className="col-span-12 md:col-span-3 mt-3 p-3">
            <SideCard services={services} title="Services" urls={urls} />
          </div>
          <div className="col-span-12 md:col-span-9 p-5">
            
            
          <UserProfile userData={userData} />;
          </div>
        </div>
  ) 
};

export default ProfilePage;
````

## File: src/app/dashboard/user/saved/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";
import { Tabs, TabsContent, TabsList, TabsTrigger } from "@/components/ui/tabs";
import FavouriteCars from "../favourites-car/page";
import FavouriteHouse from "../favourites-house/page";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];

const Saved = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <Tabs defaultValue="account" className="">
          <TabsList className="grid w-full grid-cols-2">
            <TabsTrigger value="cars">Cars</TabsTrigger>
            <TabsTrigger value="houses">Houses</TabsTrigger>
          </TabsList>
          <TabsContent value="cars">
            <FavouriteCars />
          </TabsContent>
          <TabsContent value="houses">
            <FavouriteHouse />
          </TabsContent>
          <TabsContent value="consultants">No Saved Consultant</TabsContent>
        </Tabs>
      </div>
    </div>
  );
};

export default Saved;
````

## File: src/app/dashboard/user/slots/[listingId]/[type]/page.tsx
````typescript
"use client";

import { useParams } from "next/navigation";
import AppointmentBooking from "@/components/availability/AppointmentBooking";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";
import { Button } from "@/components/ui/button";

const AppointmentBookingPage = () => {
  const params = useParams();
  const listingId = params.listingId as string;
  const type = params.type as "car" | "house";

  if (!listingId || !type) {
    return (
      <div className="flex flex-col items-center justify-center h-screen text-gray-500">
        <p className="text-lg">Invalid request. Missing parameters.</p>
        <Link href="/dashboard/user">
          <Button variant="outline" className="mt-4">
            Back to Dashboard
          </Button>
        </Link>
      </div>
    );
  }
  const backLink =
  type === "car"
    ? `/dashboard/user/cars/car-listings/${listingId}`
    : `/dashboard/user/homes/house-listings/${listingId}`;

  return (
    <div className="max-w-4xl mx-auto p-6 mt-10 bg-white shadow-lg rounded-lg">
      {/* Back Button */}
      
      <Link href={backLink}>
        <Button variant="ghost" className="flex items-center gap-2 mb-4 text-gray-600 hover:text-gray-900">
          <FiArrowLeft size={20} />
          <span className="font-medium">Back to Listings</span>
        </Button>
      </Link>

      {/* Header Section */}
      <div className="text-center mb-6">
        <h1 className="text-3xl font-semibold text-gray-800">📅 Book an Appointment</h1>
        <p className="text-gray-600 mt-2">Select a time slot to schedule your appointment.</p>
      </div>

      {/* Appointment Booking Component */}
      <div className="bg-gray-100 p-5 rounded-lg shadow-sm">
        <AppointmentBooking listingId={listingId} type={type} />
      </div>
    </div>
  );
};

export default AppointmentBookingPage;
````

## File: src/app/dashboard/user/slots/consultant/[consultantId]/page.tsx
````typescript
"use client";

import { useParams } from "next/navigation";
import AppointmentBooking from "@/components/availability/AppointmentBooking";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";
import { Button } from "@/components/ui/button";

const AppointmentBookingCPage = () => {
  const params = useParams();
  const consultantId = params.consultantId as string;

  if (!consultantId) {
    return (
      <div className="flex flex-col items-center justify-center h-screen text-gray-500">
        <p className="text-lg">Invalid request. Missing parameters.</p>
        <Link href="/dashboard/user">
          <Button variant="outline" className="mt-4">
            Back to Dashboard
          </Button>
        </Link>
      </div>
    );
  }
  const backLink =
   `/dashboard/user/consultant`

  return (
    <div className="max-w-4xl mx-auto p-6 mt-10 bg-white shadow-lg rounded-lg">
      {/* Back Button */}
      
      <Link href={backLink}>
        <Button variant="ghost" className="flex items-center gap-2 mb-4 text-gray-600 hover:text-gray-900">
          <FiArrowLeft size={20} />
          <span className="font-medium">Back to Consultants</span>
        </Button>
      </Link>

      {/* Header Section */}
      <div className="text-center mb-6">
        <h1 className="text-3xl font-semibold text-gray-800">📅 Book an Appointment</h1>
        <p className="text-gray-600 mt-2">Select a time slot to schedule your appointment.</p>
      </div>

      {/* Appointment Booking Component */}
      <div className="bg-gray-100 p-5 rounded-lg shadow-sm">
        <AppointmentBooking listingId={consultantId} type={"consultant"} />
      </div>
    </div>
  );
};

export default AppointmentBookingCPage;
````

## File: src/app/globals.css
````css
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
````

## File: src/components/ai/EnhancedResumeUpload.tsx
````typescript
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

      const response = await fetch('/api/ai/resume/upload', {
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
````

## File: src/components/ai/JobSearchModal.tsx
````typescript
'use client';

import React, { useState } from 'react';
import { Dialog, DialogContent, DialogHeader, DialogTitle, DialogDescription } from '../ui/dialog';
import { Button } from '../ui/button';
import { Input } from '../ui/input';
import { Badge } from '../ui/badge';
import { Card, CardContent, CardHeader, CardTitle } from '../ui/card';
import { ScrollArea } from '../ui/scroll-area';
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
      // First try to get token from localStorage (Google login)
      let token = localStorage.getItem('token');
      console.log('🔐 Job Search - Token from localStorage:', token ? 'Present' : 'Missing');
      
      // If no token in localStorage, try to get from cookie-based auth
      if (!token) {
        console.log('🔐 Job Search - Fetching token from cookie-based auth...');
        const tokenResponse = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/auth/token`, {
          credentials: "include",
        });
        
        if (tokenResponse.ok) {
          const tokenData = await tokenResponse.json();
          token = tokenData?.token;
          console.log('🔐 Job Search - Token from cookie auth:', token ? 'Present' : 'Missing');
        }
      }
      
      if (!token) {
        setError('Please log in to search for jobs');
        console.error('❌ Job Search - No authentication token available');
        return;
      }

      const response = await fetch('/api/career/search-jobs', {
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
````

## File: src/components/ai/ResumeAnalysisList.tsx
````typescript
'use client';

import React, { useState, useEffect } from 'react';
import { Card, CardContent, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { FileText, Calendar, TrendingUp, Eye, Clock, AlertCircle } from 'lucide-react';

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
      
      // First try to get token from localStorage (Google login)
      let token = localStorage.getItem('token');
      console.log('🔐 Frontend - Token from localStorage:', token ? 'Yes' : 'No');
      
      // If no token in localStorage, try to get from cookie-based auth
      if (!token) {
        console.log('🔐 Frontend - Fetching token from cookie-based auth...');
        const tokenResponse = await fetch(`${process.env.NEXT_PUBLIC_API_URL}/auth/token`, {
          credentials: "include",
        });
        
        if (tokenResponse.ok) {
          const tokenData = await tokenResponse.json();
          token = tokenData?.token;
          console.log('🔐 Frontend - Token from cookie auth:', token ? 'Yes' : 'No');
        }
      }
      
      if (!token) {
        setError('Please log in to view your resume analyses');
        console.error('❌ Frontend - No authentication token available');
        return;
      }
      
      console.log('🔐 Frontend - Using token length:', token?.length || 0);
      
      const response = await fetch('/api/ai/resume/analyses', {
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
              onClick={() => window.location.href = '/login'}
              className="mt-4"
            >
              Go to Login
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
          <Button onClick={() => window.location.href = '/dashboard/user/ai/resume'}>
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
                onClick={() => window.location.href = '/dashboard/user/ai/resume'}
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
````

## File: src/components/AIFeatures.tsx
````typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { 
  FileText, 
  User, 
  Users, 
  MessageCircle, 
  Search, 
  TrendingUp, 
  Globe,
  Upload,
  Sparkles,
  CheckCircle,
  Clock,
  Star
} from 'lucide-react';

const AIFeatures = () => {
  const [activeFeature, setActiveFeature] = useState('resume');

  const features = [
    {
      id: 'resume',
      title: 'Resume Analysis',
      description: 'AI-powered resume analysis and auto-fill',
      icon: FileText,
      color: 'bg-blue-100 text-blue-600',
      status: 'available'
    },
    {
      id: 'profile',
      title: 'Career Profile',
      description: 'Generate comprehensive career profile',
      icon: User,
      color: 'bg-green-100 text-green-600',
      status: 'available'
    },
    {
      id: 'mentors',
      title: 'Find Mentors',
      description: 'AI-powered mentor matching',
      icon: Users,
      color: 'bg-purple-100 text-purple-600',
      status: 'available'
    },
    {
      id: 'coaching',
      title: 'AI Career Coach',
      description: 'Personalized career guidance',
      icon: MessageCircle,
      color: 'bg-orange-100 text-orange-600',
      status: 'available'
    },
    {
      id: 'jobs',
      title: 'Job Discovery',
      description: 'Find matching job opportunities',
      icon: Search,
      color: 'bg-cyan-100 text-cyan-600',
      status: 'available'
    },
    {
      id: 'skills',
      title: 'Skill Gap Analysis',
      description: 'Identify and bridge skill gaps',
      icon: TrendingUp,
      color: 'bg-yellow-100 text-yellow-600',
      status: 'available'
    },
    {
      id: 'cultural',
      title: 'Cultural Integration',
      description: 'Workplace culture guidance',
      icon: Globe,
      color: 'bg-pink-100 text-pink-600',
      status: 'available'
    }
  ];

  const getStatusBadge = (status: string) => {
    switch (status) {
      case 'available':
        return <Badge variant="default" className="text-green-700 bg-green-100">Available</Badge>;
      case 'coming-soon':
        return <Badge variant="secondary">Coming Soon</Badge>;
      default:
        return <Badge variant="outline">Available</Badge>;
    }
  };

  return (
    <div className="space-y-6">
      <div className="flex items-center gap-3">
        <Sparkles className="h-8 w-8 text-blue-600" />
        <h2 className="text-3xl font-bold text-gray-900">AI Career Assistant</h2>
      </div>
      
      <p className="text-gray-600">
        Leverage AI-powered tools to accelerate your career growth in Canada. 
        Get personalized insights, find mentors, and navigate your professional journey with confidence.
      </p>

      <Tabs value={activeFeature} onValueChange={setActiveFeature} className="space-y-6">
        <TabsList className="grid grid-cols-4 lg:grid-cols-7 gap-2">
          {features.map((feature) => (
            <TabsTrigger
              key={feature.id}
              value={feature.id}
              className="flex flex-col items-center gap-1 py-3 px-2 data-[state=active]:bg-blue-50"
            >
              <feature.icon className="h-4 w-4" />
              <span className="text-xs font-medium">{feature.title.split(' ')[0]}</span>
            </TabsTrigger>
          ))}
        </TabsList>

        {/* Resume Analysis Tab */}
        <TabsContent value="resume" className="space-y-4">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <FileText className="h-5 w-5 text-blue-600" />
                Resume Analysis & Auto-Fill
              </CardTitle>
              <CardDescription>
                Upload your resume for AI-powered analysis and automatic profile completion
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              <div className="border-2 border-dashed border-gray-300 rounded-lg p-8 text-center hover:border-blue-400 transition-colors">
                <Upload className="h-12 w-12 text-gray-400 mx-auto mb-4" />
                <p className="text-sm text-gray-600 mb-2">
                  Drag and drop your resume here, or click to browse
                </p>
                <p className="text-xs text-gray-500">
                  Supports PDF, DOCX, JPG, PNG (max 5MB)
                </p>
                <Button className="mt-4">Choose File</Button>
              </div>
              
              <div className="grid grid-cols-1 md:grid-cols-3 gap-4">
                <div className="flex items-center gap-2">
                  <CheckCircle className="h-5 w-5 text-green-500" />
                  <span className="text-sm">Extract work experience</span>
                </div>
                <div className="flex items-center gap-2">
                  <CheckCircle className="h-5 w-5 text-green-500" />
                  <span className="text-sm">Identify skills & qualifications</span>
                </div>
                <div className="flex items-center gap-2">
                  <CheckCircle className="h-5 w-5 text-green-500" />
                  <span className="text-sm">Canadian market analysis</span>
                </div>
              </div>
            </CardContent>
          </Card>
        </TabsContent>

        {/* Career Profile Tab */}
        <TabsContent value="profile" className="space-y-4">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <User className="h-5 w-5 text-green-600" />
                Career Profile Generation
              </CardTitle>
              <CardDescription>
                Create a comprehensive career profile tailored for the Canadian market
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              <div className="bg-green-50 p-4 rounded-lg">
                <h4 className="font-semibold mb-2">Your profile will include:</h4>
                <ul className="space-y-1 text-sm">
                  <li>• Professional summary optimized for Canadian employers</li>
                  <li>• Skills categorization and market alignment</li>
                  <li>• Career objectives and target industries</li>
                  <li>• Skill gap analysis and improvement roadmap</li>
                </ul>
              </div>
              <Button className="w-full">
                Generate Career Profile
              </Button>
            </CardContent>
          </Card>
        </TabsContent>

        {/* Mentor Matching Tab */}
        <TabsContent value="mentors" className="space-y-4">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <Users className="h-5 w-5 text-purple-600" />
                AI Mentor Matching
              </CardTitle>
              <CardDescription>
                Connect with experienced professionals who can guide your career journey
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                <div className="space-y-3">
                  <h4 className="font-semibold">Find Mentors</h4>
                  <p className="text-sm text-gray-600">
                    AI matches you with mentors based on your industry, experience level, 
                    and cultural background.
                  </p>
                  <Button>Browse Mentors</Button>
                </div>
                <div className="space-y-3">
                  <h4 className="font-semibold">Become a Mentor</h4>
                  <p className="text-sm text-gray-600">
                    Help newcomers by sharing your experience and knowledge.
                  </p>
                  <Button variant="outline">Register as Mentor</Button>
                </div>
              </div>
              
              <div className="border rounded-lg p-4">
                <h5 className="font-semibold mb-2">Matching Criteria:</h5>
                <div className="flex flex-wrap gap-2">
                  <Badge variant="secondary">Industry Experience</Badge>
                  <Badge variant="secondary">Cultural Background</Badge>
                  <Badge variant="secondary">Language Skills</Badge>
                  <Badge variant="secondary">Career Level</Badge>
                </div>
              </div>
            </CardContent>
          </Card>
        </TabsContent>

        {/* AI Coaching Tab */}
        <TabsContent value="coaching" className="space-y-4">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <MessageCircle className="h-5 w-5 text-orange-600" />
                AI Career Coaching
              </CardTitle>
              <CardDescription>
                Get personalized career advice and guidance powered by AI
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              <div className="bg-orange-50 p-4 rounded-lg">
                <h4 className="font-semibold mb-2">Ask your AI coach:</h4>
                <ul className="space-y-1 text-sm">
                  <li>• How to prepare for interviews in Canada?</li>
                  <li>• What skills should I develop for my target role?</li>
                  <li>• How to network effectively in my industry?</li>
                  <li>• What are the salary expectations for my role?</li>
                </ul>
              </div>
              <div className="border rounded-lg p-4">
                <textarea 
                  placeholder="Ask your career question here..."
                  className="w-full h-24 resize-none border-0 focus:outline-none"
                />
                <div className="flex justify-between items-center pt-2">
                  <span className="text-xs text-gray-500">Press Enter to send</span>
                  <Button size="sm">Send</Button>
                </div>
              </div>
            </CardContent>
          </Card>
        </TabsContent>

        {/* Job Discovery Tab */}
        <TabsContent value="jobs" className="space-y-4">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <Search className="h-5 w-5 text-cyan-600" />
                AI Job Discovery
              </CardTitle>
              <CardDescription>
                Find job opportunities that match your skills and career goals
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                <Card className="p-4">
                  <h4 className="font-semibold mb-2">Recent Matches</h4>
                  <div className="space-y-2">
                    <div className="flex justify-between items-center">
                      <span className="text-sm">Software Developer</span>
                      <div className="flex items-center gap-1">
                        <Star className="h-3 w-3 text-yellow-500" />
                        <span className="text-xs">92%</span>
                      </div>
                    </div>
                    <div className="flex justify-between items-center">
                      <span className="text-sm">Data Analyst</span>
                      <div className="flex items-center gap-1">
                        <Star className="h-3 w-3 text-yellow-500" />
                        <span className="text-xs">87%</span>
                      </div>
                    </div>
                  </div>
                  <Button variant="outline" size="sm" className="w-full mt-3">
                    View All Matches
                  </Button>
                </Card>
                
                <Card className="p-4">
                  <h4 className="font-semibold mb-2">Job Alerts</h4>
                  <p className="text-sm text-gray-600 mb-3">
                    Get notified when new opportunities match your profile
                  </p>
                  <Button size="sm" className="w-full">
                    Set Up Alerts
                  </Button>
                </Card>
              </div>
            </CardContent>
          </Card>
        </TabsContent>

        {/* Skills Gap Tab */}
        <TabsContent value="skills" className="space-y-4">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <TrendingUp className="h-5 w-5 text-yellow-600" />
                Skill Gap Analysis
              </CardTitle>
              <CardDescription>
                Identify skills gaps and get personalized learning recommendations
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              <div className="bg-yellow-50 p-4 rounded-lg">
                <h4 className="font-semibold mb-2">Analysis includes:</h4>
                <ul className="space-y-1 text-sm">
                  <li>• Current skills vs. market requirements</li>
                  <li>• Skill gap identification and prioritization</li>
                  <li>• Learning resources and certification recommendations</li>
                  <li>• Progress tracking and milestone setting</li>
                </ul>
              </div>
              <Button className="w-full">Start Skill Analysis</Button>
            </CardContent>
          </Card>
        </TabsContent>

        {/* Cultural Integration Tab */}
        <TabsContent value="cultural" className="space-y-4">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2">
                <Globe className="h-5 w-5 text-pink-600" />
                Cultural Integration Support
              </CardTitle>
              <CardDescription>
                Navigate Canadian workplace culture with confidence
              </CardDescription>
            </CardHeader>
            <CardContent className="space-y-4">
              <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                <div>
                  <h4 className="font-semibold mb-2">Workplace Culture</h4>
                  <ul className="space-y-1 text-sm text-gray-600">
                    <li>• Communication styles</li>
                    <li>• Meeting etiquette</li>
                    <li>• Professional relationships</li>
                    <li>• Work-life balance</li>
                  </ul>
                </div>
                <div>
                  <h4 className="font-semibold mb-2">Industry Insights</h4>
                  <ul className="space-y-1 text-sm text-gray-600">
                    <li>• Sector-specific norms</li>
                    <li>• Networking practices</li>
                    <li>• Career progression paths</li>
                    <li>• Professional development</li>
                  </ul>
                </div>
              </div>
              <Button className="w-full">Get Cultural Guidance</Button>
            </CardContent>
          </Card>
        </TabsContent>
      </Tabs>
    </div>
  );
};

export default AIFeatures;
````

## File: src/components/availability/UserBooking.tsx
````typescript
import React, { useEffect, useState } from "react";
import { Button } from "@/components/ui/button";
import { Dialog, DialogContent, DialogHeader, DialogTitle, DialogClose } from "@/components/ui/dialog";
import { Tabs, TabsList, TabsTrigger, TabsContent } from "@/components/ui/tabs";

interface Listing {
  id: number;
  title?: string;
  price?: string;
  location?: string;
  make?: string;
  model?: string;
  year?: number;
}

interface Booking {
  id: number;
  userId: number;
  listingId: number;
  startDate: string;
  endDate: string;
  status: string;
  meetLink?: string;
  createdAt: string;
  listing?: Listing;
  user?: {
    id: number;
    fullName: string;
    email: string;
    phoneNo: string;
  };
}

interface ConsultantBooking {
  id: number;
  consultantId: number;
  startDate: string;
  endDate: string;
  createdAt: string;
  status: string;
  meetLink: string;
  consultant: {
    fullName: string;
    email: string;
    phoneNo: string;
  };
}

interface User {
  id: number;
  fullName: string;
  email: string;
  phoneNo: string;
  role: string;
}

const BookingView = () => {
  const [houseBookings, setHouseBookings] = useState<Booking[]>([]);
  const [carBookings, setCarBookings] = useState<Booking[]>([]);
  const [consultantBookings, setConsultantBookings] = useState<ConsultantBooking[]>([]);
  const [user, setUser] = useState<User | null>(null);
  const [loading, setLoading] = useState(true);
  const [modalData, setModalData] = useState<{ type: "user" | "listing" | "consultant"; data: any } | null>(null);

  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  let id = 0;

  useEffect(() => {
    const fetchBookings = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, { credentials: "include" });
        if (!tokenResponse.ok) throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;

        // House & Car Bookings
        const response = await fetch(`${endpoint}api/protected/appointment/view-booking`, {
          method: "GET",
          headers: { Authorization: `Bearer ${token}` },
        });
        const data = await response.json();

        if (data.success) {
          setHouseBookings(data.houseBookings || []);
          setCarBookings(data.carBookings || []);
        }

        // Consultant Bookings
        const consultantRes = await fetch(`${endpoint}api/protected/appointment/view-Cbooking`, {
          method: "GET",
          headers: { Authorization: `Bearer ${token}` },
        });
        const consultantData = await consultantRes.json();
        if (Array.isArray(consultantData)) {
          setConsultantBookings(consultantData);
        }

      } catch (error) {
        console.error("Error fetching bookings:", error);
      } finally {
        setLoading(false);
      }
    };

    fetchBookings();
  }, []);

  if (loading) return <p>Loading...</p>;

  return (
    <div className="p-4">
      <h2 className="text-xl font-semibold mb-4">Booking Details</h2>

      <Tabs defaultValue="house">
        <TabsList className="grid w-full grid-cols-3">
          <TabsTrigger value="house">House Bookings</TabsTrigger>
          <TabsTrigger value="car">Car Bookings</TabsTrigger>
          <TabsTrigger value="consultant">Consultant Bookings</TabsTrigger>
        </TabsList>

        <TabsContent value="house">
          {houseBookings.length > 0 ? (
            <TableComponent data={houseBookings} id ={1} type="house" onViewDetails={setModalData} />
          ) : (
            <p>No house bookings found.</p>
          )}
        </TabsContent>

        <TabsContent value="car">
          {carBookings.length > 0 ? (
            <TableComponent data={carBookings}  id ={1}  type="car" onViewDetails={setModalData} />
          ) : (
            <p>No car bookings found.</p>
          )}
        </TabsContent>

        <TabsContent value="consultant">
          {consultantBookings.length > 0 ? (
            <TableComponent data={consultantBookings}  id ={1}  type="consultant" onViewDetails={setModalData} />
          ) : (
            <p>No consultant bookings found.</p>
          )}
        </TabsContent>
      </Tabs>

      {modalData && (
        <Dialog open={!!modalData} onOpenChange={() => setModalData(null)}>
          <DialogContent>
            <DialogHeader>
              <DialogTitle>
                {modalData.type === "user"
                  ? "User Details"
                  : modalData.type === "listing"
                  ? "Listing Details"
                  : "Consultant Details"}
              </DialogTitle>
            </DialogHeader>
            <div className="p-4 bg-gray-100 rounded">
              {modalData.type === "consultant" ? (
                <>
                  <p><strong>Full Name:</strong> {modalData.data.fullName}</p>
                  <p><strong>Email:</strong> {modalData.data.email}</p>
                  <p><strong>Phone:</strong> {modalData.data.phoneNo}</p>
                </>
              ) : modalData.type === "user" ? (
                modalData.data.listing?.landlord || modalData.data.listing?.dealership ? (
                  <>
                    <p><strong>Full Name:</strong> {modalData.data.listing.landlord?.fullName || modalData.data.listing.dealership?.fullName}</p>
                    <p><strong>Email:</strong> {modalData.data.listing.landlord?.email || modalData.data.listing.dealership?.email}</p>
                    <p><strong>Phone:</strong> {modalData.data.listing.landlord?.phoneNo || modalData.data.listing.dealership?.phoneNo}</p>
                  </>
                ) : (
                  <p>No landlord or dealership information available.</p>
                )
              ) : (
                <>
                  {modalData.data.title && <p><strong>Title:</strong> {modalData.data.title}</p>}
                  {modalData.data.price && <p><strong>Price:</strong> {modalData.data.price}</p>}
                  {modalData.data.location && <p><strong>Location:</strong> {modalData.data.location}</p>}
                  {modalData.data.make && <p><strong>Make:</strong> {modalData.data.make}</p>}
                  {modalData.data.model && <p><strong>Model:</strong> {modalData.data.model}</p>}
                  {modalData.data.year && <p><strong>Year:</strong> {modalData.data.year}</p>}
                </>
              )}
            </div>
            <DialogClose asChild>
              <Button className="mt-2">Close</Button>
            </DialogClose>
          </DialogContent>
        </Dialog>
      )}
    </div>
  );
};

const TableComponent = ({
  data,
  type,
  id,
  onViewDetails,
}: {
  data: any[];
  type: "house" | "car" | "consultant";
  id: number,
  onViewDetails: (data: { type: "user" | "listing" | "consultant"; data: any }) => void;
}) => {
  return (
    <table className="w-full border-collapse border border-gray-300">
      <thead>
        <tr className="bg-gray-100">
          <th className="border p-2">ID</th>
          {type === "consultant" ? <th className="border p-2">Consultant</th> : <>
            <th className="border p-2">User</th>
            <th className="border p-2">Listing</th>
          </>}
          <th className="border p-2">Start Date</th>
          <th className="border p-2">End Date</th>
          <th className="border p-2">Status</th>
        </tr>
      </thead>
      <tbody>
        {data.map((booking) => (
          <tr key={booking.id} className="border">
            <td className="border p-2 text-center">{id++}</td>
            {type === "consultant" ? (
              <td className="border p-2 text-center">
                <Button variant="link" onClick={() => onViewDetails({ type: "consultant", data: booking.consultant })}>
                  View Consultant
                </Button>
              </td>
            ) : (
              <>
                <td className="border p-2 text-center">
                  <Button variant="link" onClick={() => onViewDetails({ type: "user", data: booking })}>
                    View User
                  </Button>
                </td>
                <td className="border p-2 text-center">
                  <Button variant="link" onClick={() => onViewDetails({ type: "listing", data: booking.listing })}>
                    View Listing
                  </Button>
                </td>
              </>
            )}
            <td className="border p-2 text-center">{new Date(booking.startDate).toLocaleString()}</td>
            <td className="border p-2 text-center">{new Date(booking.endDate).toLocaleString()}</td>
            <td className="border p-2 text-center">{booking.status}</td>
          </tr>
        ))}
      </tbody>
    </table>
  );
};

export default BookingView;
````

## File: src/components/Filter.tsx
````typescript
import React, { useState } from "react";

interface FilterConfig {
  name: string;
  type: "text" | "number" | "select";
  placeholder: string;
  options?: string[]; // Only for select dropdowns
}

interface ReusableFilterProps {
  filtersConfig: FilterConfig[];
  onFilterChange: (filters: { [key: string]: string }) => void;
}

const Filter: React.FC<ReusableFilterProps> = ({ filtersConfig, onFilterChange }) => {
  const [filters, setFilters] = useState<{ [key: string]: string }>({});

  const handleApplyFilters = () => {
    onFilterChange(filters);
  };

  const handleResetFilters = () => {
    const resetFilters = filtersConfig.reduce((acc, filter) => {
      acc[filter.name] = "";
      return acc;
    }, {} as { [key: string]: string });
    
    setFilters(resetFilters);
    onFilterChange(resetFilters);
  };

  const handleFilterChange = (e: React.ChangeEvent<HTMLInputElement | HTMLSelectElement>) => {
    const { name, value } = e.target;
    setFilters({ ...filters, [name]: value });
  };

  return (
    <div className="p-4 shadow-md rounded-lg mb-4"> {/*removed bg-white*/}
      <h3 className="text-lg font-semibold mb-3">Filter Listings</h3>
      
      {/* Filter inputs in a grid layout */}
      <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
        {filtersConfig.map((filter) => (
          <div key={filter.name}>
            {filter.type === "select" ? (
              <select
                name={filter.name}
                value={filters[filter.name] || ""}
                onChange={handleFilterChange}
                className="border p-2 rounded w-full"
              >
                <option value="">{filter.placeholder}</option>
                {filter.options?.map((option) => (
                  <option key={option} value={option}>
                    {option}
                  </option>
                ))}
              </select>
            ) : (
              <input
                type={filter.type}
                name={filter.name}
                placeholder={filter.placeholder}
                value={filters[filter.name] || ""}
                onChange={handleFilterChange}
                className="border p-2 rounded w-full"
              />
            )}
          </div>
        ))}
      </div>

      {/* Buttons in a new row with spacing */}
      <div className="flex flex-wrap gap-4 mt-4 justify-center sm:justify-start">
        <button
          onClick={handleApplyFilters}
          className="bg-blue-500 hover:bg-blue-600 text-white font-semibold py-2 px-4 rounded transition duration-300"
        >
          Apply Filters
        </button>
        <button
          onClick={handleResetFilters}
          className="bg-red-500 hover:bg-red-600 text-white font-semibold py-2 px-4 rounded transition duration-300"
        >
          ✖ Reset Filters
        </button>
      </div>
    </div>
  );
};

export default Filter;
````

## File: src/components/Listings.tsx
````typescript
'use client';

import { useState, useEffect } from 'react';
import ListingCard from './ListingCard';
import { Swiper, SwiperSlide } from 'swiper/react';
import { Navigation } from 'swiper/modules';
import 'swiper/css';
import 'swiper/css/navigation'; // Import the navigation styles

interface Listing {
  id: number;
  title: string;
  location?: string;
  price: number;
  imageUrl: string;
  description?: string | null;
  houseImages?: string[];
  carImages?: string[];
  make?: string;
  model?: string;
}

interface ListingsProps {
  listings: Listing[];
}


export default function Listings({ listings: initialListings }: ListingsProps) {
  const [listings, setListings] = useState<Listing[]>(initialListings);
  const [savedListings, setSavedListings] = useState<Set<number>>(new Set());

  // ✅ Sync state with updated listings from parent
  useEffect(() => {
    setListings(initialListings);
  }, [initialListings]);

  const handleSave = (listingId: number) => {
    setSavedListings((prev) => {
      const newSavedListings = new Set(prev);
      if (newSavedListings.has(listingId)) {
        newSavedListings.delete(listingId); // Unsave the listing
      } else {
        newSavedListings.add(listingId); // Save the listing
      }
      return newSavedListings;
    });
  };

  return (
    <Swiper
      modules={[Navigation]} // Ensure Navigation module is added
      spaceBetween={10}
      slidesPerView={3}
      navigation
      breakpoints={{
        1200: { slidesPerView: 3},
        1024: { slidesPerView: 3},
        768: { slidesPerView: 2 },
        480: { slidesPerView: 1 },
        0: { slidesPerView: 1 },
      }}
      style={{ width: '100%', overflow: 'hidden' }}
    >
      {listings.map((listing) => (
        <SwiperSlide key={listing.id}>
          <ListingCard
            listing={listing}
            isSaved={savedListings.has(listing.id)}
            onSave={handleSave}
          />
        </SwiperSlide>
      ))}
    </Swiper>
  );
}
````

## File: src/components/onboarding/DocumentUpload.tsx
````typescript
import React from "react";
import { Label } from "@/components/ui/label";
import { Input } from "@/components/ui/input";

interface DocumentUploadProps<T> {
  formData: T;
  setFormData: React.Dispatch<React.SetStateAction<T>>;
  errors: { [key: string]: string };
}

const DocumentUpload = <T extends Record<string, any>>({
  formData,
  setFormData,
  errors
}: DocumentUploadProps<T>) => {
  const handleFileChange = (
    e: React.ChangeEvent<HTMLInputElement>,
    field: keyof T
  ) => {
    if (e.target.files) {
      setFormData({ ...formData, [field]: e.target.files[0] });
    }
  };

  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Document Upload</h2>
      <div className="flex justify-between items-center">
        <Label>Government ID:</Label>
        <Input
          className="w-1/2 mb-4"
          type="file"
          onChange={(e) => handleFileChange(e, "governmentId")}
        />
      </div>
      {errors.governmentId && <p className="text-red-500 text-sm mb-4">{errors.governmentId}</p>}
      <div className="flex justify-between items-center">
        <Label>Business Verification:</Label>
        <Input
          className="w-1/2 mb-4"
          type="file"
          onChange={(e) => handleFileChange(e, "businessVerification")}
        />
      </div>
      {errors.businessVerification && <p className="text-red-500 text-sm mb-4">{errors.businessVerification}</p>}
      <div className="flex justify-between items-center">
        <Label>License Document:</Label>
        <Input
          className="w-1/2 mb-4"
          type="file"
          onChange={(e) => handleFileChange(e, "licenseDocument")}
        />
      </div>
      {errors.licenseDocument && <p className="text-red-500 text-sm mb-4">{errors.licenseDocument}</p>}
    </div>
  );
};

export default DocumentUpload;
````

## File: src/components/onboarding/PersonalInformation.tsx
````typescript
"use client";

import React, { useState } from "react";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import {
  Popover,
  PopoverContent,
  PopoverTrigger,
} from "@/components/ui/popover";
import { CalendarIcon } from "lucide-react";
import { cn } from "@/lib/utils";
import { Button } from "@/components/ui/button";
import { Calendar } from "@/components/ui/calendar";
import { format } from "date-fns";

interface PersonalInformationProps<T> {
  formData: T;
  setFormData: React.Dispatch<React.SetStateAction<T>>;
  errors: { [key: string]: string };
}

const PersonalInformation = <T extends Record<string, any>>({
  formData,
  setFormData,
  errors,
}: PersonalInformationProps<T>) => {
  const [isOpen, setIsOpen] = useState(false);
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Personal Information</h2>
      <div className="flex justify-between items-center">
        <Label>Full Name:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.fullName || ""}
          onChange={(e) =>
            setFormData({ ...formData, fullName: e.target.value })
          }
        />
      </div>
      {errors.fullName && <p className="text-red-500 text-sm mb-4">{errors.fullName}</p>}
      <div className="flex justify-between items-center">
        <Label>Phone Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="tel"
          value={formData.phoneNumber || ""}
          onChange={(e) =>
            setFormData({ ...formData, phoneNumber: e.target.value })
          }
        />
      </div>
      {errors.phoneNumber && <p className="text-red-500 text-sm mb-4">{errors.phoneNumber}</p>}
      {errors.phoneLength && <p className="text-red-500 text-sm mb-4">{errors.phoneLength}</p>}
      <div className="flex justify-between items-center">
        <Label>Date of Birth:</Label>
        <Popover open={isOpen} onOpenChange={setIsOpen}>
          <PopoverTrigger asChild>
            <Button
              variant={"outline"}
              className={cn(
                "w-2/3 mb-4",
                !formData.dateOfBirth && "text-muted-foreground"
              )}
            >
              {formData.dateOfBirth ? (
                format(formData.dateOfBirth, "PPP")
              ) : (
                <span>Date of Birth</span>
              )}
              <CalendarIcon className="ml-auto h-4 w-4 opacity-50" />
            </Button>
          </PopoverTrigger>
          <PopoverContent className="w-auto p-0" align="start">
            <Calendar
              mode="single"
              captionLayout="dropdown"
              selected={
                formData.dateOfBirth
                  ? new Date(formData.dateOfBirth)
                  : undefined
              }
              onSelect={(date) =>
                setFormData({
                  ...formData,
                  dateOfBirth: date ? date.toISOString().split("T")[0] : "",
                })
              }
              onDayClick={() => setIsOpen(false)}
              fromYear={1960}
              toYear={new Date().getFullYear()}
            />
          </PopoverContent>
        </Popover>
      </div>
      {errors.dateOfBirth && <p className="text-red-500 text-sm mb-4">{errors.dateOfBirth}</p>}
    </div>
  );
};

export default PersonalInformation;
````

## File: src/components/onboarding/TermsAndConditions.tsx
````typescript
import React from "react";
import { Checkbox } from "@/components/ui/checkbox";
import { Label } from "@/components/ui/label";

interface TermsAndConditionsProps<T> {
  formData: T;
  setFormData: React.Dispatch<React.SetStateAction<T>>;
  errors: { [key: string]: string };
}

const TermsAndConditions = <T extends Record<string, any>>({
  formData,
  setFormData,
  errors,
}: TermsAndConditionsProps<T>) => {
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Terms and Conditions</h2>
      <div className="space-y-4">
        <div className="flex items-center space-x-2">
          <Checkbox
            checked={formData.backgroundCheckApproved || false} // Ensure it's a boolean
            onCheckedChange={(checked) => {
              setFormData({
                ...formData,
                backgroundCheckApproved: !!checked, // Convert to boolean
              });
            }}
          />
          <Label>I approve the background check.</Label>
        </div>
        {errors.backgroundCheckApproved && (
          <p className="text-red-500 text-sm mb-4">
            {errors.backgroundCheckApproved}
          </p>
        )}
        <div className="flex items-center space-x-2">
          <Checkbox
            checked={formData.termsAccepted || false} // Ensure it's a boolean
            onCheckedChange={(checked) =>
              setFormData({
                ...formData,
                termsAccepted: !!checked, // Convert to boolean
              })
            }
          />
          <Label>I agree to the terms and conditions.</Label>
        </div>
        {errors.termsAccepted && (
          <p className="text-red-500 text-sm mb-4">
            {errors.termsAccepted}
          </p>
        )}
      </div>
    </div>
  );
};

export default TermsAndConditions;
````

## File: src/components/providers/theme-provider.tsx
````typescript
"use client";

import * as React from "react";
import { ThemeProvider as NextThemesProvider } from "next-themes";

export function ThemeProvider({
  children,
  ...props
}: React.ComponentProps<typeof NextThemesProvider>) {
  return <NextThemesProvider {...props}>{children}</NextThemesProvider>;
}
````

## File: src/components/QuickLinks.tsx
````typescript
import { Card } from "@/components/ui/card";
import { buttonVariants } from "@/components/ui/button";

export default function QuickLinks({ links }: { links: { label: string; href: string }[] }) {
  return (
    <Card>
      <div className="p-4">
        <h2 className="text-lg font-semibold mb-2">Quick Links</h2>
        <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 2xl:grid-cols-6 gap-2">
          {links.map((link, index) => (
            <a
              key={index}
              href={link.href}
              className={buttonVariants({
                variant: "outline",
                size: "lg", 
                className: "w-full",
              })}
            >
              {link.label}
            </a>
          ))}
        </div>
      </div>
    </Card>
  );
}
````

## File: src/components/Sidecard.tsx
````typescript
import { Card } from "@/components/ui/card";
import { buttonVariants } from "@/components/ui/button";
import Link from "next/link";

interface SideCardProps {
  services: string[];
  title: string;
  urls: string[];
}

export default function SideCard({ services, title, urls }: SideCardProps) {
  return (
    <Card className="md:h-full">
      <div className="p-4">
        <h2 className="text-2xl font-bold mb-4 text-center">{title}</h2>
        <ul>
          {services.map((service, index) => (
            <li key={index} className="mb-2">
              <Link
                href={urls[index]}
                className={buttonVariants({
                  variant: "ghost",
                  size: "lg",
                  className: "w-full justify-start",
                })}
              >
                {service}
              </Link>
            </li>
          ))}
        </ul>
      </div>
    </Card>
  );
}
````

## File: src/components/ThemeSwitcher.tsx
````typescript
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
````

## File: src/components/ui/alert.tsx
````typescript
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
````

## File: src/components/ui/badge.tsx
````typescript
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
````

## File: src/components/ui/button.tsx
````typescript
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
````

## File: src/components/ui/calendar.tsx
````typescript
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
````

## File: src/components/ui/card.tsx
````typescript
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
````

## File: src/components/ui/chart.tsx
````typescript
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
````

## File: src/components/ui/checkbox.tsx
````typescript
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
````

## File: src/components/ui/dialog.tsx
````typescript
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
````

## File: src/components/ui/dropdown-menu.tsx
````typescript
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
````

## File: src/components/ui/form.tsx
````typescript
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
````

## File: src/components/ui/input.tsx
````typescript
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
````

## File: src/components/ui/label.tsx
````typescript
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
````

## File: src/components/ui/popover.tsx
````typescript
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
````

## File: src/components/ui/progress.tsx
````typescript
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
````

## File: src/components/ui/radio-group.tsx
````typescript
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
````

## File: src/components/ui/scroll-area.tsx
````typescript
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
````

## File: src/components/ui/select.tsx
````typescript
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
````

## File: src/components/ui/table.tsx
````typescript
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
````

## File: src/components/ui/tabs.tsx
````typescript
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
````

## File: src/components/ui/textarea.tsx
````typescript
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
````

## File: src/components/ui/toast.tsx
````typescript
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
````

## File: src/components/ui/toaster.tsx
````typescript
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
````

## File: src/hooks/use-toast.ts
````typescript
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
````

## File: src/lib/auth.ts
````typescript
import { cookies } from 'next/headers'

export async function getSession() {
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  
  try {
    const cookieHeader = await cookies()
    const tokenResponse = await fetch(`${endpoint}auth/token`, {
      credentials: 'include',
      headers: {
        Cookie: cookieHeader.toString()
      }
    })
    
    if (!tokenResponse.ok) {
      return null
    }

    const tokenData = await tokenResponse.json()
    return tokenData.token ? { token: tokenData.token } : null
  } catch {
    return null
  }
}
````

## File: src/lib/utils.ts
````typescript
import { clsx, type ClassValue } from "clsx"
import { twMerge } from "tailwind-merge"

export function cn(...inputs: ClassValue[]) {
  return twMerge(clsx(inputs))
}
````

## File: src/middleware.ts
````typescript
import { NextResponse } from 'next/server'
import type { NextRequest } from 'next/server'

 
const publicRoutes = ['/', '/login', '/signup']
 
// Define role-based access control
const roleBasedAccess = {
  Admin: ['/dashboard/admin'],
  Immigrant: ['/dashboard/user'],
  Realtor: ['/dashboard/realtor'],
  CarDealership: ['/dashboard/car-dealer'],
  ImmigrationConsultant: ['/dashboard/consultant'],
  Onboarding: ['/onboarding'],
  NotVerified: ['/dashboard/not-verified']
}
 
export async function middleware(request: NextRequest) {
  const pathname = request.nextUrl.pathname
 
  // Skip public routes
  if (publicRoutes.includes(pathname)) {
    return NextResponse.next()
  }
 
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
 
  try {
    const cookies = request.cookies
    const tokenResponse = await fetch(`${endpoint}auth/token`, {
      credentials: 'include',
      headers: {
        Cookie: cookies.toString(),
      },
    })
 
    if (!tokenResponse.ok) {
      return NextResponse.redirect(new URL('/login', request.url))
    }
 
    const tokenData = await tokenResponse.json()
    const token = tokenData.token
 
    if (!token) {
      return NextResponse.redirect(new URL('/login', request.url))
    }
    const roleName = tokenData.roleName.split(" ").join("");
    const allowedRoutes = roleBasedAccess[roleName] || []
 
    // Check if user is allowed to access this route
    const isAllowed = allowedRoutes.some(route => pathname.startsWith(route))
 
    if (!isAllowed) {
      return NextResponse.redirect(new URL('/unauthorized', request.url)) // or any fallback route
    }
 
    // Add token to request headers
    const requestHeaders = new Headers(request.headers)
    requestHeaders.set('Authorization', `Bearer ${token}`)
 
    return NextResponse.next({
      request: {
        headers: requestHeaders,
      },
    })
  } catch {
    return NextResponse.redirect(new URL('/', request.url))
  }
}
 
export const config = {
  matcher: [
    '/dashboard/:path*',
    '/onboarding/:path*',
  ],
}
````

## File: tailwind.config.ts
````typescript
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
````

## File: README.md
````markdown
# Frontend for ImmiGrow.ai

Welcome to the frontend repository of **ImmiGrow.ai**! This project aims to provide a seamless user experience for individuals navigating the immigration process to Canada, the U.S., and the U.K. through AI-driven solutions.

## Table of Contents

1. [About ImmiGrow.ai](#about-immigratexai)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Getting Started](#getting-started)
5. [Folder Structure](#folder-structure)

---

## About ImmiGrow.ai

**ImmiGrow.ai** is a platform that:

- Assists individuals from countries such as India, the Philippines, Sri Lanka, Bangladesh, Pakistan, Nigeria, Cameroon, and Eritrea.
- Provides services to apply for work permits, study permits, and permanent residency without traditional immigration agents.
- Offers innovative solutions like building Canadian credit history before arrival.

Our mission is to make immigration processes accessible, cost-effective, and efficient for everyone.

---

## Features

### For Immigrants

- Budgeting assistance for pre- and post-arrival stages.
- Checklists covering essential tasks like obtaining SIN, health cards, and PR confirmation.
- Search functionality for houses, cars, and other essential services.
- Video calling for virtual tours and consultations.

### For Service Providers

- Account creation and onboarding for Realtors and Car Dealerships.
- Listing management (houses, cars).
- Tenant and buyer document verification.
- Open house announcements and booking requests.
- Insurance and financing calculators.

---

## Tech Stack

### Framework

- **Next.js**: React-based framework for server-side rendering and static site generation.

### Libraries and Tools

- **Tailwind CSS**: Utility-first CSS framework for styling.
- **shadcn/ui**: Component library for design consistency.
- **Framer Motion**: Animations and transitions.
- **lucide-react**: Icon library.

---

## Getting Started

### Prerequisites

- Node.js (>= 16.x)
- npm or yarn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/ImmigrateXai/ImmigrateXai-Frontend.git
   ```

2. Navigate to the project directory:

   ```bash
   cd ImmigrateXai-Frontend
   ```

3. Install dependencies:

   ```bash
   npm install
   # or
   yarn install
   ```

4. Start the development server:

   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. Open your browser and visit:
   ```
   http://localhost:3000
   ```

---

## Folder Structure

```
frontend-ImmiGrow/
├── public/         # Static files and assets
├── src/
   ├── app/         # Application files
   ├── components/  # Reusable components
   └── utils/       # Helper functions and utilities
└── package.json    # Project metadata and dependencies
```

---

### Contact

For questions, feedback, or support, please contact us at [support@ImmiGrow.ai](mailto:admin@ImmiGrow.ai).
````

## File: src/app/(auth)/forgot-password/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import Link from "next/link";
import { useState } from "react";
import { FaSpinner } from "react-icons/fa";

const ForgotPassword = () => {
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const [email, setEmail] = useState("");
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);

  const handleForgotPassword = async (
    e: React.MouseEvent<HTMLButtonElement>
  ) => {
    e.preventDefault();
    setLoading(true);
    if (!email) {
      setError("Please fill in all fields");
      setLoading(false);
      return;
    }
    const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    if (!emailPattern.test(email)) {
      setError("Please enter a valid email address");
      setLoading(false);
      return;
    }

    try {
      const response = await fetch(`${endpoint}api/users/forgot-password`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        body: JSON.stringify({ email }),
      });

      const data = await response.json();

      if (!response.ok) {
        setError(data.error);
        return;
      }

      if (data.message) {
        setError(data.message);
      }
    } catch (error) {
      console.error(error);
      setError("Failed to reset password");
    } finally {
      setLoading(false);
    }
  };
  return (
    <div className="h-full md:flex">
      <div className="w-full p-12 h-full flex flex-col justify-center items-center">
        <div className="max-w-md lg:max-w-lg">
          <div className=" py-8 px-6 shadow shadow-muted-foreground rounded-lg sm:px-10 text-center">
            <h2 className="text-3xl font-bold mb-4">Forgot Password?</h2>
            <p className=" mb-8">Enter your email and password below</p>
            <Input
              placeholder="email"
              className="mb-4"
              type="email"
              value={email}
              onChange={(e) => setEmail(e.target.value)}
            />
            <Button
              className={
                "bg-blue-600 hover:bg-blue-500 w-full mb-4" +
                (loading
                  ? " cursor-not-allowed bg-blue-300 hover:bg-blue-300"
                  : "")
              }
              onClick={(e) => handleForgotPassword(e)}
            >
              {loading ? <FaSpinner className="animate-spin" /> : "Verify"}
            </Button>
            {error && <p className="text-red-500 text-sm">{error}</p>}
            <p className="text-md mt-6 pt-6 border-t">
              Remember Password?{" "}
              <Link
                className="text-blue-600 hover:text-blue-500 font-semibold"
                href="/login"
              >
                Login
              </Link>
            </p>
          </div>
        </div>
      </div>
    </div>
  );
};

export default ForgotPassword;
````

## File: src/app/(auth)/login/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import Link from "next/link";
import { useRouter } from "next/navigation";
import { useState } from "react";
import { FaSpinner } from "react-icons/fa";
import { FcGoogle } from "react-icons/fc";
import CryptoJS from "crypto-js";
import { getAuth, GoogleAuthProvider, signInWithPopup } from "firebase/auth";
import { initializeApp } from "firebase/app";
import { Checkbox } from "@/components/ui/checkbox";
import { Label } from "@/components/ui/label";
import {
  Dialog,
  DialogContent,
  DialogHeader,
  DialogTitle,
  DialogFooter,
} from "@/components/ui/dialog";
import { useToast } from "@/hooks/use-toast";
import Cookies from "js-cookie";
import Image from "next/image";

// Define the UserData interface for checking user verification
interface UserData {
  emailVerified: boolean;
  userVerified: boolean;
  onboarded: boolean;
  userRole?: string;
}

const endpoint = process.env.NEXT_PUBLIC_API_URL;

const Login = () => {
  const [email, setEmail] = useState("");
  const [password, setPassword] = useState("");
  const [rememberMe, setRememberMe] = useState(false);
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);
  const [showDialog, setShowDialog] = useState(false);
  // const [token, setToken] = useState("");
  const { toast } = useToast();

  const router = useRouter();
  const secret = process.env.NEXT_PUBLIC_SECRET_KEY;

  function encryptPassword(password: string) {
    if (!secret) {
      throw new Error("Secret key is not defined");
    }
    const iv = CryptoJS.lib.WordArray.random(16).toString(); // Random IV
    const encrypted = CryptoJS.AES.encrypt(
      password,
      CryptoJS.enc.Utf8.parse(secret),
      {
        iv: CryptoJS.enc.Hex.parse(iv),
        mode: CryptoJS.mode.CBC,
        padding: CryptoJS.pad.Pkcs7,
      }
    );
    return {
      encryptedData: encrypted.ciphertext.toString(CryptoJS.enc.Base64),
      iv: iv,
    };
  }

  const checkUserVerification = (data: UserData) => {
    if (data.onboarded === false) {
      router.push("/onboarding");
      return false;
    } else if (!data.userVerified) {
      router.push("/dashboard/not-verified?reason=user");
      return false;
    } else {
      if (data.userRole === "Car Dealership") {
        router.push("/dashboard/car-dealer");
        return false;
      } else if (data.userRole === "Immigrant") {
        router.push("/dashboard/user");
        return false;
      } else if (data.userRole === "Realtor") {
        router.push("/dashboard/realtor");
        return false;
      } else if (data.userRole === "Immigration Consultant") {
        router.push("/dashboard/consultant");
        return false;
      } else if (data.userRole === "Admin") {
        router.push("/dashboard/admin");
        return false;
      }

      return true;
    }
  };

  const handleLogin = async (e: React.MouseEvent<HTMLButtonElement>) => {
    e.preventDefault();
    setLoading(true);
    setError(""); // Clear any previous errors

    if (!email || !password) {
      setError("Please fill in all fields");
      setLoading(false);
      return;
    }

    const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;

    if (!emailPattern.test(email)) {
      setError("Please enter a valid email address");
      setLoading(false);
      return;
    }

    if (password.length < 6) {
      setError("Password must be at least 6 characters long");
      setLoading(false);
      return;
    }

    const { encryptedData, iv } = encryptPassword(password);

    try {
      const response = await fetch(`${endpoint}api/users/login`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        credentials: "include",
        body: JSON.stringify({ email, password: encryptedData, iv }),
      });

      const data = await response.json();

      if (!response.ok) {
        if (data.emailVerified == false) {
          setError("Please verify your email first");
          // setToken(data.token);
          setShowDialog(true);
          return;
        }
        setError(data.error || "Failed to login");
        return;
      }

      if (data.emailVerified == true) {
        if (rememberMe) {
          localStorage.setItem("email", data.email);
        }
        if (!checkUserVerification(data)) return;
        router.push("/dashboard");
      } else {
        setError(data.message || "Failed to login");
      }
    } catch (error) {
      console.error("Login error:", error);
      setError("Failed to login");
    } finally {
      setLoading(false);
    }
  };

  const handleResendEmail = async () => {
    try {
      await fetch(`${endpoint}api/users/refresh-token`, {
        method: "POST",
        credentials: "include",
      });
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");

      const tokenData = await tokenResponse.json();
      const token = tokenData?.token;
      if (!token) throw new Error("Invalid authentication token");

      await fetch(`${endpoint}api/users/resend-verification`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
      });
      toast({
        title: "Verification email sent",
        description: "Please check your email to verify your account",
      });
      setShowDialog(false);
    } catch (error) {
      console.error("Failed to resend email:", error);
    }
  };

  const firebaseConfig = {
    apiKey: process.env.NEXT_PUBLIC_API_KEY,
    authDomain: process.env.NEXT_PUBLIC_AUTH_DOMAIN,
    projectId: process.env.NEXT_PUBLIC_PROJECT_ID,
  };

  const app = initializeApp(firebaseConfig);

  const handleGoogleLogin = async () => {
    const auth = getAuth(app);
    const provider = new GoogleAuthProvider();
    const rememberMe = false;

    setLoading(true);
    try {
      const result = await signInWithPopup(auth, provider);
      const refreshToken = await result.user.refreshToken;
      const idToken = await result.user.getIdToken();

      const response = await fetch(`${endpoint}api/users/google-signin`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        credentials: "include",
        body: JSON.stringify({ idToken, refreshToken, rememberMe }),
      });

      const data = await response.json();

      if (data) {
        localStorage.setItem("token", idToken);
        if (!checkUserVerification(data)) return;
        router.push("/dashboard");
      } else {
        setError(data.message || "Google Sign-In failed");
      }
    } catch (error) {
      console.error(
        "Error during Google Sign-In or backend communication:",
        error
      );
      setError("Failed to sign up with Google");
    } finally {
      setLoading(false);
    }
  };

  return (
    <>
      <div className="h-full md:flex">
        <div className="md:w-1/2 p-12 h-full flex flex-col justify-center items-center">
          <div className="max-w-md lg:max-w-lg">
            <div className=" py-8 px-6 shadow shadow-muted-foreground rounded-lg sm:px-10 text-center">
              <h2 className="text-3xl font-bold mb-4">Login to your account</h2>
              <p className=" mb-8">Enter your email and password below</p>
              <Input
                placeholder="email"
                className="mb-4"
                type="email"
                value={email}
                onChange={(e) => setEmail(e.target.value)}
              />
              <Input
                placeholder="password"
                className="mb-4"
                type="password"
                value={password}
                onChange={(e) => setPassword(e.target.value)}
              />
              {/* <div className="flex items-center space-x-2 my-4 px-1">
                <Checkbox
                  id="remember"
                  checked={rememberMe}
                  onCheckedChange={(checked) =>
                    setRememberMe(checked ? true : false)
                  }
                />
                <Label
                  htmlFor="remember"
                  className="text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
                >
                  Remember Me
                </Label>
              </div>
              {error && <p className="text-red-500 text-sm">{error}</p>} */}
              <Button
                className={
                  "bg-blue-600 hover:bg-blue-500 w-full mb-4" +
                  (loading
                    ? " cursor-not-allowed bg-blue-300 hover:bg-blue-300"
                    : "")
                }
                onClick={(e) => handleLogin(e)}
              >
                {loading ? <FaSpinner className="animate-spin" /> : "Login"}
              </Button>
              <p className="text-sm mb-4">
                Forgot Password?{" "}
                <Link
                  href={"/forgot-password"}
                  className="font-bold text-blue-600 hover:text-blue-500"
                >
                  Reset
                </Link>
              </p>
              <div className="flex items-center mb-4">
                <div className="flex-grow h-px" />
                <span className="mx-4 text-sm">OR</span>
                <div className="flex-grow h-px" />
              </div>
              <Button
                variant="outline"
                className={
                  "flex items-center justify-center w-full mb-4" +
                  (loading
                    ? " cursor-not-allowed bg-neutral-300 hover:bg-neutral-300"
                    : "")
                }
                onClick={() => handleGoogleLogin()}
              >
                {loading ? (
                  <FaSpinner className="animate-spin" />
                ) : (
                  <>
                    <FcGoogle size={6} /> Continue with Google
                  </>
                )}
              </Button>
              <p className="text-xs mt-4">
                By clicking login, you agree to our Terms of Service and Privacy
                Policy.
              </p>
              <p className="text-md mt-6 pt-6 border-t">
                Don&apos;t have an account?{" "}
                <Link
                  className="text-blue-600 hover:text-blue-500 font-semibold"
                  href="/signup"
                >
                  Sign up
                </Link>
              </p>
            </div>
          </div>
        </div>
        <div className="relative w-1/2 p-12 bg-blue-600 md:flex flex-col justify-between hidden">
          <Image
            src={"/login.jpg"}
            alt="signup"
            layout="fill"
            objectFit="cover"
            className="absolute inset-0 opacity-50"
          />
        </div>
      </div>

      <Dialog open={showDialog} onOpenChange={setShowDialog}>
        <DialogContent>
          <DialogHeader>
            <DialogTitle>Email Verification Required</DialogTitle>
          </DialogHeader>
          <p>Please verify your email to continue.</p>
          <DialogFooter>
            <Button variant="secondary" onClick={() => setShowDialog(false)}>
              Cancel
            </Button>
            <Button onClick={handleResendEmail}>
              Resend Verification Email
            </Button>
          </DialogFooter>
        </DialogContent>
      </Dialog>
    </>
  );
};

export default Login;
````

## File: src/app/(auth)/onboarding/immigrant/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import { Checkbox } from "@/components/ui/checkbox";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";
import React, { useState } from "react";
import {
  Popover,
  PopoverContent,
  PopoverTrigger,
} from "@/components/ui/popover";
import { CalendarIcon } from "lucide-react";
import { cn } from "@/lib/utils";
import { Calendar } from "@/components/ui/calendar";
import { format } from "date-fns";
import TermsAndConditions from "@/components/onboarding/TermsAndConditions";
import { useRouter } from "next/navigation";

interface FormData {
  fullName: string;
  phoneNumber: string;
  dateOfBirth: string;
  alreadyInCanada: boolean;
  countryOfOrigin: string;
  workSchoolLocation: string;
  statusInCanada: string;
  governmentId: File | null;
  backgroundCheckApproved: boolean;
  termsAccepted: boolean;
}

const Immigrant = () => {
  const [isOpen, setIsOpen] = useState(false);
  const router = useRouter();
  const [currentStep, setCurrentStep] = useState(1);

  const [formData, setFormData] = useState<FormData>({
    fullName: "",
    phoneNumber: "",
    dateOfBirth: "",
    alreadyInCanada: false,
    countryOfOrigin: "",
    workSchoolLocation: "",
    statusInCanada: "",
    governmentId: null,
    backgroundCheckApproved: false,
    termsAccepted: false,
  });

  const [isLoading, setIsLoading] = useState(false);
  const [error, setError] = useState("");
  const [success, setSuccess] = useState(false);

  // const [token, setToken] = useState("");
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const handleNextStep = () => {
    setCurrentStep((prevStep) => prevStep + 1);
  };

  const handlePreviousStep = () => {
    setCurrentStep((prevStep) => prevStep - 1);
  };

  const handleFileChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    if (e.target.files && e.target.files[0]) {
      setFormData({ ...formData, governmentId: e.target.files[0] });
    }
  };

  const validateForm = () => {
    if (!formData.fullName.trim()) {
      setError("Full name is required");
      return false;
    }
    if (!formData.phoneNumber.trim()) {
      setError("Phone number is required");
      return false;
    }
    if (!formData.dateOfBirth) {
      setError("Date of birth is required");
      return false;
    }

    if (!formData.statusInCanada && formData.alreadyInCanada) {
      setError("Status in Canada is required");
      return false;
    }
    if (!formData.countryOfOrigin) {
      setError("Country of Origin is required");
      return false;
    }
    if (!formData.workSchoolLocation && formData.alreadyInCanada) {
      setError("Location is required");
      return false;
    }
    if (!formData.governmentId) {
      setError("Government ID is required");
      return false;
    }
    if (!formData.termsAccepted) {
      setError("You must accept the terms and conditions");
      return false;
    }
    if (!formData.backgroundCheckApproved) {
      setError("You must approve background check");
      return false;
    }
    setError("");
    return true;
  };

  const handleSubmit = async () => {
    if (!validateForm()) return;

    setIsLoading(true);
    setError("");
    setSuccess(false);

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataToSend = new FormData();
      formDataToSend.append("fullName", formData.fullName);
      formDataToSend.append("DOB", formData.dateOfBirth);
      formDataToSend.append("phoneNo", formData.phoneNumber);
      formDataToSend.append(
        "alreadyInCanada",
        formData.alreadyInCanada ? "true" : "false"
      );
      formDataToSend.append("workSchoolLocation", formData.workSchoolLocation);
      formDataToSend.append("countryOfOrigin", formData.countryOfOrigin);
      formDataToSend.append("statusInCanada", formData.statusInCanada);
      formDataToSend.append("rolename", "Immigrant");
      formDataToSend.append(
        "backgroundVerification",
        String(formData.backgroundCheckApproved)
      );

      formDataToSend.append(
        "termsConditionCheck",
        String(formData.termsAccepted)
      );
      if (formData.governmentId) {
        formDataToSend.append("govId", formData.governmentId);
      }

      const response = await fetch(`${endpoint}api/onboarding/information`, {
        method: "POST",
        headers: {
          Authorization: `Bearer ${token}`,
        },
        body: formDataToSend,
      });

      if (!response.ok) {
        const errorData = await response.json();
        throw new Error(errorData.error || "Failed to submit form");
      }

      setSuccess(true);
      router.push("/dashboard/not-verified?reason=user");
    } catch (error) {
      setError(
        error instanceof Error ? error.message : "An unexpected error occurred"
      );
    } finally {
      setIsLoading(false);
    }
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl w-full min-h-[600px] h-full">
        <div className="py-8 px-6 shadow text-center w-full h-full flex flex-col justify-between">
          {currentStep === 1 && (
            <div className="text-left">
              <h2 className="text-xl font-semibold mb-4">
                Personal Information
              </h2>
              <div className="flex justify-between items-center">
                <Label>Full Name:</Label>
                <Input
                  className="w-2/3 mb-4"
                  type="text"
                  value={formData.fullName}
                  onChange={(e) =>
                    setFormData({ ...formData, fullName: e.target.value })
                  }
                />
              </div>
              <div className="flex justify-between items-center">
                <Label>Phone Number:</Label>
                <Input
                  className="w-2/3 mb-4"
                  type="tel"
                  value={formData.phoneNumber}
                  onChange={(e) =>
                    setFormData({ ...formData, phoneNumber: e.target.value })
                  }
                />
              </div>
              <div className="flex justify-between items-center">
                <Label>Date of Birth:</Label>
                <Popover open={isOpen} onOpenChange={setIsOpen}>
                  <PopoverTrigger asChild>
                    <Button
                      variant={"outline"}
                      className={cn(
                        "w-2/3 mb-4",
                        !formData.dateOfBirth && "text-muted-foreground"
                      )}
                    >
                      {formData.dateOfBirth ? (
                        format(new Date(formData.dateOfBirth), "PPP")
                      ) : (
                        <span>Date of Birth</span>
                      )}
                      <CalendarIcon className="ml-auto h-4 w-4 opacity-50" />
                    </Button>
                  </PopoverTrigger>
                  <PopoverContent className="w-auto p-0" align="start">
                    <Calendar
                      mode="single"
                      captionLayout="dropdown"
                      selected={
                        formData.dateOfBirth
                          ? new Date(formData.dateOfBirth)
                          : undefined
                      }
                      onSelect={(date) =>
                        setFormData({
                          ...formData,
                          dateOfBirth: date
                            ? date.toISOString().split("T")[0]
                            : "",
                        })
                      }
                      onDayClick={() => setIsOpen(false)}
                      fromYear={1960}
                      toYear={new Date().getFullYear()}
                    />
                  </PopoverContent>
                </Popover>
              </div>

              <div className="flex justify-between items-center">
                <Label>Country Of Origin:</Label>
                <Input
                  className="w-2/3 mb-4"
                  type="text"
                  value={formData.countryOfOrigin}
                  onChange={(e) =>
                    setFormData({
                      ...formData,
                      countryOfOrigin: e.target.value,
                    })
                  }
                />
              </div>

              <div className="flex mt-2 items-center mb-4">
                <Label htmlFor="alreadyInCanada">Already In Canada:</Label>
                <Checkbox
                  id="alreadyInCanada"
                  className="ml-14"
                  checked={formData.alreadyInCanada}
                  onCheckedChange={(checked) =>
                    setFormData({ ...formData, alreadyInCanada: !!checked })
                  }
                />
              </div>

              {formData.alreadyInCanada === true && (
                <div className="flex justify-between items-center">
                  <Label>Status in Canada:</Label>
                  <Select
                    value={formData.statusInCanada}
                    onValueChange={(value) =>
                      setFormData({ ...formData, statusInCanada: value })
                    }
                  >
                    <SelectTrigger className="w-2/3 mb-4">
                      <SelectValue placeholder="Select Status" />
                    </SelectTrigger>
                    <SelectContent>
                      <SelectItem value="Study Permit">Study Permit</SelectItem>
                      <SelectItem value="Work Permit">Work Permit</SelectItem>
                      <SelectItem value="Permanent Resident">
                        Permanent Resident
                      </SelectItem>
                      <SelectItem value="Citizen">Citizen</SelectItem>
                    </SelectContent>
                  </Select>
                </div>
              )}
              {formData.alreadyInCanada === true && (
                <div className="flex justify-between items-center">
                  <Label>School/Work Location:</Label>
                  <Input
                    className="w-2/3 mb-4"
                    type="text"
                    value={formData.workSchoolLocation}
                    onChange={(e) =>
                      setFormData({
                        ...formData,
                        workSchoolLocation: e.target.value,
                      })
                    }
                  />
                </div>
              )}

              <div className="flex justify-between items-center">
                <Label>Government ID:</Label>
                <Input
                  className="w-2/3 mb-4"
                  type="file"
                  onChange={handleFileChange}
                />
              </div>
            </div>
          )}
          {currentStep === 2 && (
            <TermsAndConditions
              formData={formData}
              setFormData={setFormData}
              errors={{}}
            />
          )}
          {currentStep === 3 && (
            <div>
              <h2 className="text-xl font-semibold mb-2">Review Details</h2>
              <p className="mb-4">
                Please review the details you have provided below.
              </p>
              {error && (
                <div className="mb-4 p-2 bg-red-100 text-red-600 rounded">
                  {error}
                </div>
              )}
              {success && (
                <div className="mb-4 p-2 bg-blue-100 text-blue-600 rounded">
                  Form submitted successfully!
                </div>
              )}
              <span className="flex justify-between mb-1">
                <strong>Full Name:</strong> {formData.fullName}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Phone Number:</strong> {formData.phoneNumber}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Date of Birth:</strong> {formData.dateOfBirth}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Country Of Origin:</strong> {formData.countryOfOrigin}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Already In Canada</strong>{" "}
                {formData.alreadyInCanada ? "Yes" : "No"}
              </span>
              {formData.alreadyInCanada && (
                <span className="flex justify-between mb-1">
                  <strong>Status in Canada:</strong> {formData.statusInCanada}
                </span>
              )}
              {formData.alreadyInCanada && (
                <span className="flex justify-between mb-1">
                  <strong>School/Work Location:</strong>{" "}
                  {formData.workSchoolLocation}
                </span>
              )}
              <span className="flex justify-between mb-1">
                <strong>Status in Canada:</strong> {formData.statusInCanada}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Government ID:</strong>{" "}
                {formData.governmentId ? "Provided" : "Not Provided"}
              </span>
            </div>
          )}

          <div className="flex gap-4 justify-center">
            {currentStep > 1 && (
              <Button onClick={handlePreviousStep}>Back</Button>
            )}
            {currentStep == 1 && (
              <Button onClick={() => router.push("/onboarding")}>Back</Button>
            )}
            {currentStep < 3 && <Button onClick={handleNextStep}>Next</Button>}
            {currentStep === 3 && (
              <Button onClick={handleSubmit} disabled={isLoading}>
                {isLoading ? "Submitting..." : "Submit"}
              </Button>
            )}
          </div>
        </div>
      </div>
    </div>
  );
};

export default Immigrant;
````

## File: src/app/(auth)/onboarding/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";
import { useRouter } from "next/navigation";
import { useState } from "react";
import { FaSpinner } from "react-icons/fa";

const Onboarding = () => {
  const router = useRouter();
  const [loading, setLoading] = useState(false);
  const [error, setError] = useState("");
  const [userType, setUserType] = useState("");

  const handleUserTypeChange = (value: string) => {
    setUserType(value);
  };

  const handleSubmit = () => {
    setLoading(true);
    setError("");

    if (!userType) {
      setError("Please select a user type.");
      setLoading(false);
      return;
    }

    const routeMap: { [key: string]: string } = {
      Realtors: "/onboarding/realtor",
      "Car Dealers": "/onboarding/car-dealer",
      "Immigration Consultants": "/onboarding/consultant",
      Immigrant: "/onboarding/immigrant",
    };

    // Redirect based on user type
    router.push(routeMap[userType]);
    setLoading(false);
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl">
        <div className="py-8 px-6 shadow rounded-lg text-center">
          <h2 className="text-3xl font-bold mb-6">Onboarding Form</h2>
          <div className="flex gap-2"></div>
          <Select onValueChange={handleUserTypeChange}>
            <SelectTrigger className="w-full mb-4">
              <SelectValue placeholder="Select User Type" />
            </SelectTrigger>
            <SelectContent>
              <SelectItem value="Realtors">Realtors</SelectItem>
              <SelectItem value="Car Dealers">Car Dealers</SelectItem>
              <SelectItem value="Immigration Consultants">
                Immigration Consultants
              </SelectItem>
              <SelectItem value="Immigrant">Immigrant</SelectItem>
            </SelectContent>
          </Select>
          <Button
            className={
              "bg-blue-600 hover:bg-blue-500 w-full mb-4" +
              (loading ? " cursor-not-allowed bg-blue-300" : "")
            }
            onClick={handleSubmit}
            disabled={loading}
          >
            {loading ? <FaSpinner className="animate-spin" /> : "Next"}
          </Button>
          {error && <p className="text-red-500 text-sm">{error}</p>}
        </div>
      </div>
    </div>
  );
};

export default Onboarding;
````

## File: src/app/(auth)/signup/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import Link from "next/link";
import { useState } from "react";
import { FaSpinner } from "react-icons/fa";
import { FcGoogle } from "react-icons/fc";
import { useRouter } from "next/navigation";
import { useToast } from "@/hooks/use-toast";
import CryptoJS from "crypto-js";
import { getAuth, GoogleAuthProvider, signInWithPopup } from "firebase/auth";
import { initializeApp } from "firebase/app";
import Image from "next/image";

const endpoint = process.env.NEXT_PUBLIC_API_URL;

const Signup = () => {
  const [email, setEmail] = useState("");
  const [password, setPassword] = useState("");
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);

  const router = useRouter();
  const { toast } = useToast();
  const secret = process.env.NEXT_PUBLIC_SECRET_KEY;

  function encryptPassword(password: string) {
    if (!secret) {
      throw new Error("Secret key is not defined");
    }
    // Generate a random IV and convert it to a hexadecimal string
    const iv = CryptoJS.lib.WordArray.random(16).toString(CryptoJS.enc.Hex);

    // Encrypt the password using AES-256-CBC
    const encrypted = CryptoJS.AES.encrypt(
      password,
      CryptoJS.enc.Utf8.parse(secret), // Parse the secret key as UTF-8
      {
        iv: CryptoJS.enc.Hex.parse(iv), // Parse the IV as hexadecimal
        mode: CryptoJS.mode.CBC, // Use CBC mode
        padding: CryptoJS.pad.Pkcs7, // Use PKCS7 padding
      }
    );

    // Return the encrypted password and IV
    return {
      encryptedData: encrypted.ciphertext.toString(CryptoJS.enc.Base64),
      iv: iv,
    };
  }

  const handleSignup = async (e: React.MouseEvent<HTMLButtonElement>) => {
    e.preventDefault();
    setLoading(true);
    setError(""); // Clear any previous errors

    if (!email || !password) {
      setError("Please fill in all fields");
      setLoading(false);
      return;
    }

    const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    if (!emailPattern.test(email)) {
      setError("Please enter a valid email address");
      setLoading(false);
      return;
    }

    if (password.length < 6) {
      setError("Password must be at least 6 characters long");
      setLoading(false);
      return;
    }

    // Encrypt the password
    const { encryptedData, iv } = encryptPassword(password);

    try {
      // Send encrypted password and IV to the backend
      const response = await fetch(`${endpoint}api/users/signup`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        body: JSON.stringify({ email, password: encryptedData, iv }),
        credentials: "include",
      });

      const data = await response.json();

      if (!response.ok) {
        if (data.error === "EMAIL_EXISTS") {
          setError("Email already exists");
        } else {
          setError(data.error || "Failed to signup");
        }
        return;
      }

      if (data.userId) {
        localStorage.setItem("user", JSON.stringify(data.userId));
        toast({
          title: "Signup success",
          description: "Please verify your email before logging in",
        });
        router.push("/login");
      } else {
        setError(data.error || "Failed to signup");
      }
    } catch (error) {
      console.error("Signup error:", error);
      setError("Failed to signup");
    } finally {
      setLoading(false);
    }
  };

  const firebaseConfig = {
    apiKey: process.env.NEXT_PUBLIC_API_KEY,
    authDomain: process.env.NEXT_PUBLIC_AUTH_DOMAIN,
    projectId: process.env.NEXT_PUBLIC_PROJECT_ID,
  };

  const app = initializeApp(firebaseConfig);

  const handleGoogleSignup = async () => {
    const auth = getAuth(app);
    const provider = new GoogleAuthProvider();

    setLoading(true);
    try {
      const result = await signInWithPopup(auth, provider);

      const idToken = await result.user.getIdToken();
      const response = await fetch(`${endpoint}api/users/google-signin`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        body: JSON.stringify({ idToken }),
      });

      const data = await response.json();

      if (data.user) {
        localStorage.setItem("token", idToken);
        // localStorage.setItem("user", JSON.stringify(data.user));
        router.push("/onboarding");
      } else {
        setError(data.message || "Google Sign-In failed");
      }
    } catch (error) {
      console.error(
        "Error during Google Sign-In or backend communication:",
        error
      );
      setError("Failed to sign up with Google");
    } finally {
      setLoading(false);
    }
  };

  return (
    <div className="h-full md:flex">
      <div className="w-1/2  bg-blue-600 md:flex flex-col justify-between hidden">
        <div className="relative h-full flex flex-col items-center justify-center">
          {/* ✅ Background Image with Overlay */}
          <div className="absolute inset-0 opacity-50">
            <Image
              src={"/signup.jpg"} // 🔹 Ensure the correct image path
              alt="signup"
              layout="fill"
              objectFit="cover"
            />
          </div>
        </div>
      </div>
      <div className="md:w-1/2 p-12 h-full flex flex-col justify-center items-center">
        <div className="max-w-md lg:max-w-lg">
          <div className=" py-8 px-6 shadow shadow-muted-foreground rounded-lg sm:px-10 text-center">
            <h2 className="text-3xl font-bold mb-4">Create an account</h2>
            <p className=" mb-8">
              Enter your email below to create your account
            </p>
            <Input
              placeholder="email"
              className="mb-4"
              type="email"
              value={email}
              onChange={(e) => setEmail(e.target.value)}
            />
            <Input
              placeholder="password"
              className="mb-4"
              type="password"
              value={password}
              onChange={(e) => setPassword(e.target.value)}
            />
            <Button
              className={
                "bg-blue-600 hover:bg-blue-500 w-full mb-4" +
                (loading
                  ? " cursor-not-allowed bg-blue-300 hover:bg-blue-300"
                  : "")
              }
              onClick={(e) => handleSignup(e)}
            >
              {loading ? (
                <FaSpinner className="animate-spin" />
              ) : (
                "Sign up with Email"
              )}
            </Button>
            {error && <p className="text-red-500 text-sm">{error}</p>}
            <div className="flex items-center mb-4">
              <div className="flex-grow h-px" />
              <span className="mx-4 text-sm">OR</span>
              <div className="flex-grow h-px" />
            </div>
            <Button
              variant="outline"
              className={
                "flex items-center justify-center w-full mb-4" +
                (loading
                  ? " cursor-not-allowed bg-neutral-300 hover:bg-neutral-300"
                  : "")
              }
              onClick={() => handleGoogleSignup()}
            >
              {loading ? (
                <FaSpinner className="animate-spin" />
              ) : (
                <>
                  <FcGoogle size={6} /> Continue with Google
                </>
              )}
            </Button>
            <p className="text-xs mt-4">
              By clicking signup, you agree to our Terms of Service and Privacy
              Policy.
            </p>
            <p className="text-md mt-6 pt-6 border-t">
              Already have an account?{" "}
              <Link
                className="text-blue-600 hover:text-blue-500 font-semibold"
                href="/login"
              >
                Login
              </Link>
            </p>
          </div>
        </div>
      </div>
    </div>
  );
};

export default Signup;
````

## File: src/app/dashboard/admin/page.tsx
````typescript
"use client";

import { useEffect, useState } from "react";
import { useRouter } from "next/navigation";
import SideCard from "@/components/Sidecard";
import {
  Pie,
  PieChart,
  Cell,
  LineChart,
  Line,
  XAxis,
  CartesianGrid,
  BarChart,
  YAxis,
  Bar,
} from "recharts";
import { TrendingUp } from "lucide-react";

import { Card, CardContent, CardHeader, CardTitle } from "@/components/ui/card";
import {
  ChartConfig,
  ChartContainer,
  ChartLegend,
  ChartLegendContent,
  ChartTooltip,
  ChartTooltipContent,
} from "@/components/ui/chart";

interface AdminStats {
  totalUsers: number;
  verifiedUsers: number;
  unverifiedUsers: number;
  houseListings: number;
  carListings: number;
  noOfImmigrant: number;
  formattedData: { month: string; count: number }[];
  userTypeGraph: { userType: string; count: number }[];
  verificationPieChart: { label: string; value: number }[];
}

export default function AdminDashboard() {
  const [stats, setStats] = useState<AdminStats | null>(null);
  const [error, setError] = useState<string>("");
  const [loading, setLoading] = useState<boolean>(true);
  const router = useRouter();
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const services = ["Dashboard", "User List", "Verify Users"];
  const urls = [
    "/dashboard/admin",
    "/dashboard/admin/user-list",
    "/dashboard/admin/verify-users",
  ];

  useEffect(() => {
    const fetchStats = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;
        if (!token) throw new Error("Invalid token");

        const response = await fetch(`${endpoint}api/admin/dashboard/stats`, {
          headers: { Authorization: `Bearer ${token}` },
        });
        if (!response.ok) throw new Error("Failed to fetch admin stats");

        const data = await response.json();

        setStats(data);
      } catch (err: any) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchStats();
  }, [endpoint]);

  if (loading) return <p className="p-6">Loading admin dashboard...</p>;
  if (error) return <p className="p-6 text-red-500">Error: {error}</p>;

  // Prepare User Type data for Pie Chart
  const userTypeChartData =
    stats?.userTypeGraph?.length > 0
      ? stats.userTypeGraph.map((item, index) => ({
          name: item.userType || "Unknown",
          value: item.count || 0,
          fill: ["#0088FE", "#00C49F", "#FFBB28", "#FF8042", "#AA336A"][
            index % 5
          ],
        }))
      : [];

  // Prepare Verified vs. Non-Verified Users data
  const registrationChartData =
    stats?.verificationPieChart?.length > 0
      ? stats.verificationPieChart.map((item, index) => ({
          name: item.label,
          value: item.value,
          fill: ["#34D399", "#ff5733"][index % 2], // blue for Verified, Red for Unverified
        }))
      : [];

  // Prepare Formatted Data for Line Chart (Monthly User Counts)
  const barChartData =
    stats?.formattedData?.length > 0 ? stats.formattedData : [];

  // Chart Configurations
  const userTypeChartConfig: ChartConfig = userTypeChartData.reduce(
    (acc, item) => {
      acc[item.name] = {
        label: item.name,
        color: item.fill,
      };
      return acc;
    },
    {} as ChartConfig
  );

  const registrationChartConfig: ChartConfig = registrationChartData.reduce(
    (acc, item) => {
      acc[item.name] = {
        label: item.name,
        color: item.fill,
      };
      return acc;
    },
    {} as ChartConfig
  );

  const barChartConfig: ChartConfig = {
    count: {
      label: "Users",
      color: "#3498db", // Blue color
    },
  };

  return (
    <div className="grid grid-cols-12 min-h-screen">
      {/* Sidebar */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Quick Links" urls={urls} />
      </div>

      {/* Main Content */}
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Admin Dashboard</h2>

          {/* Stats & Line Chart Side-by-Side */}
          <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
            {/* Stats */}
            <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
              {[
                { title: "Total Users", value: stats?.totalUsers },
                { title: "Verified Users", value: stats?.verifiedUsers },
                { title: "Unverified Users", value: stats?.unverifiedUsers },
                { title: "Total Immigrants", value: stats?.noOfImmigrant },
                { title: "House Listings", value: stats?.houseListings },
                { title: "Car Listings", value: stats?.carListings },
              ].map((stat, index) => (
                <Card key={index} className="p-4 border rounded shadow">
                  <CardHeader>
                    <CardTitle>{stat.title}</CardTitle>
                  </CardHeader>
                  <CardContent>
                    <p className="text-2xl">{stat.value}</p>
                  </CardContent>
                </Card>
              ))}
            </div>

            {/* Line Chart */}
            <Card>
              <CardHeader>
                <CardTitle>Monthly Users Added</CardTitle>
              </CardHeader>
              <CardContent>
                <ChartContainer config={barChartConfig}>
                  <BarChart data={barChartData} width={500} height={300}>
                    <CartesianGrid strokeDasharray="3 3" stroke="#ddd" />
                    <XAxis
                      dataKey="month"
                      tickLine={false}
                      axisLine={false}
                      tickMargin={8}
                      interval={0} // Ensures all months are shown
                    />
                    <YAxis />
                    <ChartTooltip content={<ChartTooltipContent />} />
                    <Bar dataKey="count" fill="#3498db" barSize={40} />
                  </BarChart>
                </ChartContainer>
              </CardContent>
            </Card>
          </div>

          {/* Pie Charts */}
          <div className="mt-8 grid grid-cols-1 md:grid-cols-2 gap-6">
            <Card>
              <CardHeader>
                <CardTitle>User Type Distribution</CardTitle>
              </CardHeader>
              <CardContent>
                <ChartContainer config={userTypeChartConfig}>
                  <PieChart>
                    <ChartTooltip
                      content={<ChartTooltipContent nameKey="name" />}
                    />
                    <Pie data={userTypeChartData} dataKey="value">
                      {userTypeChartData.map((entry, index) => (
                        <Cell key={`cell-${index}`} fill={entry.fill} />
                      ))}
                    </Pie>
                    <ChartLegend
                      content={<ChartLegendContent nameKey="name" />}
                    />
                  </PieChart>
                </ChartContainer>
              </CardContent>
            </Card>

            <Card>
              <CardHeader>
                <CardTitle>Verified vs. Non-Verified Users</CardTitle>
              </CardHeader>
              <CardContent>
                <ChartContainer config={registrationChartConfig}>
                  <PieChart>
                    <ChartTooltip
                      content={<ChartTooltipContent nameKey="name" />}
                    />
                    <Pie data={registrationChartData} dataKey="value">
                      {registrationChartData.map((entry, index) => (
                        <Cell key={`cell-${index}`} fill={entry.fill} />
                      ))}
                    </Pie>
                    <ChartLegend
                      content={<ChartLegendContent nameKey="name" />}
                    />
                  </PieChart>
                </ChartContainer>
              </CardContent>
            </Card>
          </div>
        </div>
      </div>
    </div>
  );
}
````

## File: src/app/dashboard/admin/user-list/page.tsx
````typescript
"use client";

import { useEffect, useState } from "react";
import { useRouter } from "next/navigation";
import SideCard from "@/components/Sidecard";
import {
  ColumnDef,
  ColumnFiltersState,
  VisibilityState,
  flexRender,
  getCoreRowModel,
  getFilteredRowModel,
  getPaginationRowModel,
  useReactTable,
} from "@tanstack/react-table";
import { MoreHorizontal } from "lucide-react";
import { Button } from "@/components/ui/button";
import { Checkbox } from "@/components/ui/checkbox";
import {
  DropdownMenu,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuLabel,
  DropdownMenuTrigger,
} from "@/components/ui/dropdown-menu";
import { Input } from "@/components/ui/input";
import {
  Table,
  TableBody,
  TableCell,
  TableHead,
  TableHeader,
  TableRow,
} from "@/components/ui/table";

export type User = {
  id: string;
  fullName: string;
  email: string;
  phoneNo: string;
  DOB: string;
  firebaseUid: string;
  userVerified: boolean;
  statusInCanada: string | null;
  role: { name: string };
};

export default function UserListPage() {
  const [users, setUsers] = useState<User[]>([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState("");
  const [columnFilters, setColumnFilters] = useState<ColumnFiltersState>([]);
  const [columnVisibility, setColumnVisibility] = useState<VisibilityState>({});
  const [rowSelection, setRowSelection] = useState({});
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  const router = useRouter();

  const services = ["Dashboard", "User List", "Verify Users"];
  const urls = [
    "/dashboard/admin",
    "/dashboard/admin/user-list",
    "/dashboard/admin/verify-users",
  ];

  useEffect(() => {
    const fetchUsers = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });

        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;

        if (!token) throw new Error("Invalid token");

        const response = await fetch(
          `${endpoint}api/admin/user-list/user-details`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!response.ok) throw new Error("Failed to fetch user details");

        const data = await response.json();

        // Extract users array correctly
        const extractedUsers = data?.user ?? [];
        if (!Array.isArray(extractedUsers)) {
          throw new Error(
            `Unexpected API response format: ${JSON.stringify(data, null, 2)}`
          );
        }

        setUsers(extractedUsers);
      } catch (err: any) {
        console.error("Error fetching users:", err.message);
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchUsers();
  }, [endpoint]);

  const columns: ColumnDef<User>[] = [
    {
      id: "select",
      header: ({ table }) => (
        <Checkbox
          checked={
            table.getIsAllPageRowsSelected() ||
            (table.getIsSomePageRowsSelected() && "indeterminate")
          }
          onCheckedChange={(value) => table.toggleAllPageRowsSelected(!!value)}
          aria-label="Select all"
        />
      ),
      cell: ({ row }) => (
        <Checkbox
          checked={row.getIsSelected()}
          onCheckedChange={(value) => row.toggleSelected(!!value)}
          aria-label="Select row"
        />
      ),
      enableSorting: false,
      enableHiding: false,
    },
    {
      accessorKey: "fullName",
      header: "Full Name",
      cell: ({ row }) => <div>{row.getValue("fullName")}</div>,
    },
    {
      accessorKey: "email",
      header: "Email",
      cell: ({ row }) => (
        <div className="lowercase">{row.getValue("email")}</div>
      ),
    },
    {
      accessorKey: "phoneNo",
      header: "Phone Number",
      cell: ({ row }) => <div>{row.getValue("phoneNo")}</div>,
    },
    {
      accessorKey: "DOB",
      header: "Date of Birth",
      cell: ({ row }) => (
        <div>{new Date(row.getValue("DOB")).toLocaleDateString()}</div>
      ),
    },
    {
      accessorKey: "statusInCanada",
      header: "Status in Canada",
      cell: ({ row }) => <div>{row.getValue("statusInCanada") || "N/A"}</div>,
    },
    {
      accessorKey: "userVerified",
      header: "Verified",
      cell: ({ row }) => (
        <div
          className={`font-bold ${
            row.getValue("userVerified") ? "text-blue-600" : "text-red-600"
          }`}
        >
          {row.getValue("userVerified") ? "Yes" : "No"}
        </div>
      ),
    },
    {
      accessorFn: (row) => row.role?.name ?? "Unknown",
      header: "Role",
      cell: ({ row }) => (
        <div className="capitalize">{row.original.role?.name ?? "Unknown"}</div>
      ),
    },
    {
      id: "actions",
      header: "Actions",
      enableHiding: false,
      cell: ({ row }) => {
        const user = row.original;

        return (
          <DropdownMenu>
            <DropdownMenuTrigger asChild>
              <Button variant="ghost" className="h-8 w-8 p-0">
                <span className="sr-only">Open menu</span>
                <MoreHorizontal />
              </Button>
            </DropdownMenuTrigger>
            <DropdownMenuContent align="end">
              <DropdownMenuItem
                onClick={() =>
                  router.push(`/dashboard/admin/view-user/${user.id}`)
                }
              >
                View Details
              </DropdownMenuItem>
            </DropdownMenuContent>
          </DropdownMenu>
        );
      },
    },
  ];

  const table = useReactTable({
    data: users,
    columns,
    getCoreRowModel: getCoreRowModel(),
    getPaginationRowModel: getPaginationRowModel(),
    getFilteredRowModel: getFilteredRowModel(),
    state: {
      columnFilters,
      columnVisibility,
      rowSelection,
    },
    onColumnFiltersChange: setColumnFilters,
    onColumnVisibilityChange: setColumnVisibility,
    onRowSelectionChange: setRowSelection,
  });

  return (
    <div className="grid grid-cols-12 min-h-screen">
      {/* Sidebar */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Admin Links" urls={urls} />
      </div>

      {/* Main Content */}
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">User List</h2>

          {loading && <p className="text-gray-500">Loading users...</p>}
          {error && <p className="text-red-500">{error}</p>}

          {!loading && !error && (
            <>
              {/* Search by Name */}
              <div className="flex items-center py-4">
                <Input
                  placeholder="Search by Name..."
                  value={
                    (table.getColumn("fullName")?.getFilterValue() as string) ??
                    ""
                  }
                  onChange={(event) =>
                    table
                      .getColumn("fullName")
                      ?.setFilterValue(event.target.value)
                  }
                  className="max-w-sm"
                />
              </div>

              {/* User Table */}
              <div className="rounded-md border">
                <Table>
                  <TableHeader>
                    {table.getHeaderGroups().map((headerGroup) => (
                      <TableRow key={headerGroup.id}>
                        {headerGroup.headers.map((header) => (
                          <TableHead key={header.id}>
                            {flexRender(
                              header.column.columnDef.header,
                              header.getContext()
                            )}
                          </TableHead>
                        ))}
                      </TableRow>
                    ))}
                  </TableHeader>
                  <TableBody>
                    {table.getRowModel().rows.length > 0 ? (
                      table.getRowModel().rows.map((row) => (
                        <TableRow key={row.id}>
                          {row.getVisibleCells().map((cell) => (
                            <TableCell key={cell.id}>
                              {flexRender(
                                cell.column.columnDef.cell,
                                cell.getContext()
                              )}
                            </TableCell>
                          ))}
                        </TableRow>
                      ))
                    ) : (
                      <TableRow>
                        <TableCell
                          colSpan={columns.length}
                          className="text-center py-6"
                        >
                          No users found.
                        </TableCell>
                      </TableRow>
                    )}
                  </TableBody>
                </Table>
              </div>
            </>
          )}
        </div>
      </div>
    </div>
  );
}
````

## File: src/app/dashboard/admin/verify-users/page.tsx
````typescript
"use client";

import { useEffect, useState } from "react";
import { useRouter } from "next/navigation";
import SideCard from "@/components/Sidecard";
import {
  ColumnDef,
  ColumnFiltersState,
  VisibilityState,
  flexRender,
  getCoreRowModel,
  getFilteredRowModel,
  getPaginationRowModel,
  useReactTable,
} from "@tanstack/react-table";
import { MoreHorizontal } from "lucide-react";
import { Button } from "@/components/ui/button";
import { Checkbox } from "@/components/ui/checkbox";
import {
  DropdownMenu,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuLabel,
  DropdownMenuTrigger,
} from "@/components/ui/dropdown-menu";
import { Input } from "@/components/ui/input";
import {
  Table,
  TableBody,
  TableCell,
  TableHead,
  TableHeader,
  TableRow,
} from "@/components/ui/table";

export type UnverifiedUser = {
  id: string;
  fullName: string;
  email: string;
  phoneNo: string;
  DOB: string;
  firebaseUid: string;
  userVerified: boolean;
  statusInCanada: string | null;
  roleId: number;
  userDocuments: { id: string }[];
};

export default function VerifyUsersPage() {
  const [users, setUsers] = useState<UnverifiedUser[]>([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState("");
  const [columnFilters, setColumnFilters] = useState<ColumnFiltersState>([]);
  const [columnVisibility, setColumnVisibility] = useState<VisibilityState>({});
  const [rowSelection, setRowSelection] = useState({});
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  const router = useRouter();

  const services = ["Dashboard", "User List", "Verify Users"];
  const urls = [
    "/dashboard/admin",
    "/dashboard/admin/user-list",
    "/dashboard/admin/verify-users",
  ];

  useEffect(() => {
    const fetchUnverifiedUsers = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });

        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;

        if (!token) throw new Error("Invalid token");

        const response = await fetch(
          `${endpoint}api/admin/verify/unverified-user`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        const data = await response.json();

        if (response.status === 404) {
          setError("No unverified users found");
        }

        const extractedUsers = data?.user ?? [];
        if (!Array.isArray(extractedUsers)) {
          throw new Error(
            `Unexpected API response format: ${JSON.stringify(data, null, 2)}`
          );
        }

        setUsers(extractedUsers);
      } catch (err: any) {
        console.error("Error fetching unverified users:", err.message);
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchUnverifiedUsers();
  }, [endpoint]);

  const columns: ColumnDef<UnverifiedUser>[] = [
    {
      id: "select",
      header: ({ table }) => (
        <Checkbox
          checked={
            table.getIsAllPageRowsSelected() ||
            (table.getIsSomePageRowsSelected() && "indeterminate")
          }
          onCheckedChange={(value) => table.toggleAllPageRowsSelected(!!value)}
          aria-label="Select all"
        />
      ),
      cell: ({ row }) => (
        <Checkbox
          checked={row.getIsSelected()}
          onCheckedChange={(value) => row.toggleSelected(!!value)}
          aria-label="Select row"
        />
      ),
      enableSorting: false,
      enableHiding: false,
    },
    {
      accessorKey: "fullName",
      header: "Full Name",
      cell: ({ row }) => <div>{row.getValue("fullName")}</div>,
    },
    {
      accessorKey: "email",
      header: "Email",
      cell: ({ row }) => (
        <div className="lowercase">{row.getValue("email")}</div>
      ),
    },
    {
      accessorKey: "phoneNo",
      header: "Phone Number",
      cell: ({ row }) => <div>{row.getValue("phoneNo")}</div>,
    },
    {
      accessorKey: "DOB",
      header: "Date of Birth",
      cell: ({ row }) => (
        <div>{new Date(row.getValue("DOB")).toLocaleDateString()}</div>
      ),
    },
    {
      accessorKey: "statusInCanada",
      header: "Status in Canada",
      cell: ({ row }) => <div>{row.getValue("statusInCanada") || "N/A"}</div>,
    },
    {
      accessorKey: "userVerified",
      header: "Verified",
      cell: ({ row }) => (
        <div
          className={`font-bold ${
            row.getValue("userVerified") ? "text-blue-600" : "text-red-600"
          }`}
        >
          {row.getValue("userVerified") ? "Yes" : "No"}
        </div>
      ),
    },
    {
      id: "actions",
      header: "Actions",
      enableHiding: false,
      cell: ({ row }) => {
        const user = row.original;

        return (
          <DropdownMenu>
            <DropdownMenuTrigger asChild>
              <Button variant="ghost" className="h-8 w-8 p-0">
                <span className="sr-only">Open menu</span>
                <MoreHorizontal />
              </Button>
            </DropdownMenuTrigger>
            <DropdownMenuContent align="end">
              <DropdownMenuLabel>Actions</DropdownMenuLabel>
              <DropdownMenuItem
                onClick={() =>
                  router.push(`/dashboard/admin/view-user/${user.id}`)
                }
              >
                View User
              </DropdownMenuItem>
            </DropdownMenuContent>
          </DropdownMenu>
        );
      },
    },
  ];

  const table = useReactTable({
    data: users,
    columns,
    getCoreRowModel: getCoreRowModel(),
    getPaginationRowModel: getPaginationRowModel(),
    getFilteredRowModel: getFilteredRowModel(),
    state: {
      columnFilters,
      columnVisibility,
      rowSelection,
    },
    onColumnFiltersChange: setColumnFilters,
    onColumnVisibilityChange: setColumnVisibility,
    onRowSelectionChange: setRowSelection,
  });

  return (
    <div className="grid grid-cols-12 min-h-screen">
      {/* Sidebar */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Admin Links" urls={urls} />
      </div>

      {/* Main Content */}
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Non-Verified Users</h2>

          {loading && <p className="text-gray-500">Loading users...</p>}
          {error && <p className="text-red-500">{error}</p>}

          {!loading && !error && (
            <>
              {/* Search by Name */}
              <div className="flex items-center py-4">
                <Input
                  placeholder="Search by Name..."
                  value={
                    (table.getColumn("fullName")?.getFilterValue() as string) ??
                    ""
                  }
                  onChange={(event) =>
                    table
                      .getColumn("fullName")
                      ?.setFilterValue(event.target.value)
                  }
                  className="max-w-sm"
                />
              </div>

              {/* User Table */}
              <div className="rounded-md border">
                <Table>
                  <TableHeader>
                    {table.getHeaderGroups().map((headerGroup) => (
                      <TableRow key={headerGroup.id}>
                        {headerGroup.headers.map((header) => (
                          <TableHead key={header.id}>
                            {flexRender(
                              header.column.columnDef.header,
                              header.getContext()
                            )}
                          </TableHead>
                        ))}
                      </TableRow>
                    ))}
                  </TableHeader>
                  <TableBody>
                    {table.getRowModel().rows.length > 0 ? (
                      table.getRowModel().rows.map((row) => (
                        <TableRow key={row.id}>
                          {row.getVisibleCells().map((cell) => (
                            <TableCell key={cell.id}>
                              {flexRender(
                                cell.column.columnDef.cell,
                                cell.getContext()
                              )}
                            </TableCell>
                          ))}
                        </TableRow>
                      ))
                    ) : (
                      <TableRow>
                        <TableCell
                          colSpan={columns.length}
                          className="text-center py-6"
                        >
                          No users found.
                        </TableCell>
                      </TableRow>
                    )}
                  </TableBody>
                </Table>
              </div>
            </>
          )}
        </div>
      </div>
    </div>
  );
}
````

## File: src/app/dashboard/admin/view-user/[id]/page.tsx
````typescript
"use client";

import { useEffect, useState } from "react";
import { useParams, useRouter } from "next/navigation";
import { Document, Page, pdfjs } from "react-pdf";
import "react-pdf/dist/esm/Page/AnnotationLayer.css";
import "react-pdf/dist/esm/Page/TextLayer.css";

// Load PDF.js worker locally
pdfjs.GlobalWorkerOptions.workerSrc = `//unpkg.com/pdfjs-dist@${pdfjs.version}/build/pdf.worker.min.mjs`;

type UserDetail = {
  id: number;
  fullName: string;
  email: string;
  phoneNo: string;
  DOB: string;
  firebaseUid: string;
  userVerified: boolean;
  statusInCanada: string | null;
  roleId: number;
  userDocuments: { id: number }[];
  userType: string;
  // Realtor details from Prisma model
  realtor?: {
    businessName: string;
    businessAddress?: string;
    realEstateLicenseNumber: string;
    affiliatedAssociations?: string;
    areasCovered: string;
    specialties: string;
    portfolioWebsite?: string;
    businessRegistration: string;
    workType: string;
    brokerageName?: string;
    officeLocationAvailable: boolean;
    teamMembers: number;
    virtualPropertyTour: boolean;
    yearsOfExperience: string;
  };
  // Car Dealership details from Prisma model
  carDealership?: {
    showroomLocations: string;
    testDrivePolicy: string;
    financingOptions: string;
    tradeInAvailable: boolean;
    serviceWarrantyInfo: string;
    businessRegistration: string;
    businessName: string;
    yearsInBusiness: string;
    dealershipLicenseNumber: string;
    carBrandsSold: string;
    newOrUsedCars: string;
  };
  // Immigration Consultant details from Prisma model
  immigrationConsultant?: {
    countriesServed: string;
    consultationFee: number | null;
    businessRegistration: string;
    partneredLegalFirms?: string;
    websiteOrSocialMedia?: string;
    businessName: string;
    businessAddress: string;
    licenseNumber: string;
    servicesOffered: string;
    languagesSpoken: string;
    yearsOfExperience: string;
  };
};

export default function ViewUserPage() {
  const { id: userId } = useParams();
  const router = useRouter();
  const [user, setUser] = useState<UserDetail | null>(null);
  const [step, setStep] = useState(1);
  const [selectedDocId, setSelectedDocId] = useState<number | null>(null);
  const [documentUrl, setDocumentUrl] = useState<string | null>(null);
  const [numPages, setNumPages] = useState<number | null>(null);
  const [currentPage, setCurrentPage] = useState(1);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState("");
  const [showModal, setShowModal] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const handleBack = () => router.push("/dashboard/admin/user-list");

  // Reset current page when step changes
  useEffect(() => {
    setCurrentPage(1);
  }, [step]);

  // Fetch user details on mount
  useEffect(() => {
    if (!userId || !endpoint) {
      setError("Missing userId or API endpoint.");
      setLoading(false);
      return;
    }
    async function fetchUserDetails() {
      try {
        const token = await fetchAuthToken();
        if (!token) throw new Error("Invalid token received");
        const response = await fetch(
          `${endpoint}api/admin/user-list/user-details/${userId}`,
          { headers: { Authorization: `Bearer ${token}` } }
        );
        if (!response.ok) throw new Error("Failed to fetch user details");
        const data = await response.json();
        setUser(data.user);
        // For step 1, if a document exists, select the first one
        if (data.user.userDocuments.length > 0) {
          setSelectedDocId(data.user.userDocuments[0].id);
        }
      } catch (err: any) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    }
    fetchUserDetails();
  }, [userId, endpoint]);

  // Update selected document when step changes
  useEffect(() => {
    if (!user) {
      setSelectedDocId(null);
      return;
    }
    // If fewer documents than the step number exist, clear the selection
    if (user.userDocuments.length < step) {
      setSelectedDocId(null);
    } else {
      if (step === 1) setSelectedDocId(user.userDocuments[0].id);
      else if (step === 2) setSelectedDocId(user.userDocuments[1].id);
      else if (step === 3) setSelectedDocId(user.userDocuments[2].id);
    }
  }, [step, user]);

  // Fetch PDF when selectedDocId changes
  useEffect(() => {
    if (selectedDocId) {
      fetchUserDocument(selectedDocId);
    } else {
      setDocumentUrl(null);
    }
  }, [selectedDocId]);

  async function fetchAuthToken(): Promise<string | null> {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");
      const tokenData = await tokenResponse.json();
      return tokenData.token;
    } catch (err: any) {
      return null;
    }
  }

  async function fetchUserDocument(documentId: number): Promise<void> {
    try {
      const token = await fetchAuthToken();
      if (!token) throw new Error("Invalid token received");
      // Revoke previous URL if exists
      if (documentUrl) URL.revokeObjectURL(documentUrl);
      const docUrl = `${endpoint}api/admin/user-list/user-document/${documentId}`;
      const response = await fetch(docUrl, {
        method: "GET",
        headers: {
          Authorization: `Bearer ${token}`,
          Accept: "application/pdf",
        },
      });
      if (!response.ok) throw new Error("Failed to fetch document");
      const blob = await response.blob();
      setDocumentUrl(URL.createObjectURL(blob));
    } catch (err: any) {
      setDocumentUrl(null);
    }
  }

  const handleVerifyUser = async (userId: string) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const response = await fetch(`${endpoint}api/admin/verify/verify-user`, {
        method: "PUT",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
        body: JSON.stringify({ id: userId }),
      });

      if (!response.ok) throw new Error("Failed to verify user");

      alert("User has been successfully verified!");

      router.push("/dashboard/admin/user-list");
    } catch (err: any) {
      console.error("Error verifying user:", err.message);
      alert("Failed to verify user. Please try again.");
    }
  };

  if (loading) return <div className="p-5">Loading user details...</div>;
  if (error) return <div className="p-5 text-red-600">Error: {error}</div>;

  // Helper: PDF Viewer with navigation buttons and a key to force re-mounting
  const renderPDFViewer = (title: string) => (
    <div className="p-5 border rounded shadow-sm">
      <h2 className="text-2xl font-bold mb-4">{title}</h2>
      {documentUrl ? (
        <div onContextMenu={(e) => e.preventDefault()} className="border p-3">
          <Document
            key={`doc-${step}-${selectedDocId}`}
            file={documentUrl}
            onLoadSuccess={({ numPages }) => setNumPages(numPages)}
          >
            <Page
              pageNumber={currentPage}
              renderTextLayer={false}
              renderAnnotationLayer={false}
            />
          </Document>
          <div className="flex justify-center space-x-2 mt-2">
            <button
              onClick={() => setCurrentPage((prev) => Math.max(prev - 1, 1))}
              disabled={currentPage <= 1}
              className="px-3 py-1 bg-gray-200 rounded disabled:opacity-50"
            >
              Previous
            </button>
            <span>
              {currentPage} of {numPages}
            </span>
            <button
              onClick={() =>
                setCurrentPage((prev) => Math.min(prev + 1, numPages || 1))
              }
              disabled={numPages === null || currentPage >= (numPages || 1)}
              className="px-3 py-1 bg-gray-200 rounded disabled:opacity-50"
            >
              Next
            </button>
          </div>
        </div>
      ) : (
        <p>No document available.</p>
      )}
    </div>
  );

  // Render step content in a 50/50 layout
  const renderStepContent = () => {
    if (step === 1) {
      return (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {/* Left: User Details */}
          <div className="p-5 border rounded shadow-sm">
            <h2 className="text-2xl font-bold mb-4">User Details</h2>
            <p>
              <strong>Name:</strong> {user?.fullName}
            </p>
            <p>
              <strong>Email:</strong> {user?.email}
            </p>
            <p>
              <strong>Phone:</strong> {user?.phoneNo}
            </p>
            <p>
              <strong>Date of Birth:</strong>{" "}
              {new Date(user?.DOB || "").toLocaleDateString()}
            </p>
            <p>
              <strong>Status in Canada:</strong> {user?.statusInCanada || "N/A"}
            </p>
            <p>
              <strong>Verified:</strong> {user?.userVerified ? "Yes" : "No"}
            </p>
          </div>
          {/* Right: Government ID PDF */}
          {renderPDFViewer("Government ID")}
        </div>
      );
    } else if (step === 2) {
      return (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {/* Left: Business Details */}
          <div className="p-5 border rounded shadow-sm">
            <h2 className="text-2xl font-bold mb-4">Business Details</h2>
            {user.realtor ? (
              <>
                <p>
                  <strong>Business Name:</strong> {user.realtor.businessName}
                </p>
                <p>
                  <strong>Business Address:</strong>{" "}
                  {user.realtor.businessAddress || "N/A"}
                </p>
                <p>
                  <strong>Real Estate License Number:</strong>{" "}
                  {user.realtor.realEstateLicenseNumber}
                </p>
                <p>
                  <strong>Affiliated Associations:</strong>{" "}
                  {user.realtor.affiliatedAssociations || "N/A"}
                </p>
                <p>
                  <strong>Areas Covered:</strong> {user.realtor.areasCovered}
                </p>
                <p>
                  <strong>Specialties:</strong> {user.realtor.specialties}
                </p>
                <p>
                  <strong>Portfolio Website:</strong>{" "}
                  {user.realtor.portfolioWebsite ? (
                    <a
                      href={user.realtor.portfolioWebsite}
                      target="_blank"
                      rel="noopener noreferrer"
                      className="text-blue-600 underline"
                    >
                      {user.realtor.portfolioWebsite}
                    </a>
                  ) : (
                    "N/A"
                  )}
                </p>
                <p>
                  <strong>Business Registration:</strong>{" "}
                  {user.realtor.businessRegistration}
                </p>
                <p>
                  <strong>Work Type:</strong> {user.realtor.workType}
                </p>
                <p>
                  <strong>Brokerage Name:</strong>{" "}
                  {user.realtor.brokerageName || "N/A"}
                </p>
                <p>
                  <strong>Office Location Available:</strong>{" "}
                  {user.realtor.officeLocationAvailable ? "Yes" : "No"}
                </p>
                <p>
                  <strong>Team Members:</strong> {user.realtor.teamMembers}
                </p>
                <p>
                  <strong>Virtual Property Tour:</strong>{" "}
                  {user.realtor.virtualPropertyTour ? "Yes" : "No"}
                </p>
                <p>
                  <strong>Years of Experience:</strong>{" "}
                  {user.realtor.yearsOfExperience}
                </p>
              </>
            ) : user.carDealership ? (
              <>
                <p>
                  <strong>Business Name:</strong>{" "}
                  {user.carDealership.businessName}
                </p>
                <p>
                  <strong>Showroom Locations:</strong>{" "}
                  {user.carDealership.showroomLocations}
                </p>
                <p>
                  <strong>Test Drive Policy:</strong>{" "}
                  {user.carDealership.testDrivePolicy}
                </p>
                <p>
                  <strong>Financing Options:</strong>{" "}
                  {(() => {
                    try {
                      const options = JSON.parse(
                        user.carDealership.financingOptions
                      );
                      return `In House Financing: ${
                        options.inHouseFinancing ? "Yes" : "No"
                      }, Third Party Banks: ${
                        options.thirdPartyBanks ? "Yes" : "No"
                      }, Lease Options: ${options.leaseOptions ? "Yes" : "No"}`;
                    } catch (error) {
                      return user.carDealership.financingOptions;
                    }
                  })()}
                </p>
                <p>
                  <strong>Trade In Available:</strong>{" "}
                  {user.carDealership.tradeInAvailable ? "Yes" : "No"}
                </p>
                <p>
                  <strong>Service Warranty Info:</strong>{" "}
                  {user.carDealership.serviceWarrantyInfo}
                </p>
                <p>
                  <strong>Business Registration:</strong>{" "}
                  {user.carDealership.businessRegistration}
                </p>
                <p>
                  <strong>Years in Business:</strong>{" "}
                  {user.carDealership.yearsInBusiness}
                </p>
              </>
            ) : user.immigrationConsultant ? (
              <>
                <p>
                  <strong>Business Name:</strong>{" "}
                  {user.immigrationConsultant.businessName}
                </p>
                <p>
                  <strong>Business Address:</strong>{" "}
                  {user.immigrationConsultant.businessAddress}
                </p>
                <p>
                  <strong>License Number:</strong>{" "}
                  {user.immigrationConsultant.licenseNumber}
                </p>
                <p>
                  <strong>Countries Served:</strong>{" "}
                  {user.immigrationConsultant.countriesServed}
                </p>
                <p>
                  <strong>Consultation Fee:</strong>{" "}
                  {user.immigrationConsultant.consultationFee}
                </p>
                <p>
                  <strong>Business Registration:</strong>{" "}
                  {user.immigrationConsultant.businessRegistration}
                </p>
                <p>
                  <strong>Partnered Legal Firms:</strong>{" "}
                  {user.immigrationConsultant.partneredLegalFirms || "N/A"}
                </p>
                <p>
                  <strong>Website/Social Media:</strong>{" "}
                  {user.immigrationConsultant.websiteOrSocialMedia ? (
                    <a
                      href={user.immigrationConsultant.websiteOrSocialMedia}
                      target="_blank"
                      rel="noopener noreferrer"
                      className="text-blue-600 underline"
                    >
                      {user.immigrationConsultant.websiteOrSocialMedia}
                    </a>
                  ) : (
                    "N/A"
                  )}
                </p>
                <p>
                  <strong>Years of Experience:</strong>{" "}
                  {user.immigrationConsultant.yearsOfExperience}
                </p>
                <p>
                  <strong>Services Offered:</strong>{" "}
                  {user.immigrationConsultant.servicesOffered}
                </p>
                <p>
                  <strong>Languages Spoken:</strong>{" "}
                  {user.immigrationConsultant.languagesSpoken}
                </p>
              </>
            ) : (
              <p>No business details available.</p>
            )}
          </div>
          {/* Right: Business Info PDF */}
          {renderPDFViewer("Business Info Document")}
        </div>
      );
    } else if (step === 3) {
      return (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {/* Left: License Details */}
          <div className="p-5 border rounded shadow-sm">
            <h2 className="text-2xl font-bold mb-4">License Details</h2>
            {user.realtor ? (
              <p>
                <strong>License Number:</strong>{" "}
                {user.realtor.realEstateLicenseNumber}
              </p>
            ) : user.carDealership ? (
              <p>
                <strong>Dealership License Number:</strong>{" "}
                {user.carDealership.dealershipLicenseNumber}
              </p>
            ) : user.immigrationConsultant ? (
              <p>
                <strong>License Number:</strong>{" "}
                {user.immigrationConsultant.licenseNumber}
              </p>
            ) : (
              <p>No license details available.</p>
            )}
          </div>
          {/* Right: License Document PDF */}
          {renderPDFViewer("License Document")}
        </div>
      );
    }
  };

  return (
    <div className="min-h-screen p-5">
      {/* Back to Users Button */}
      <button
        onClick={handleBack}
        className="px-4 py-2 rounded hover:bg-gray-200 transition mb-5"
      >
        ← Back to Users
      </button>

      {/* Step Navigation */}
      <div className="flex justify-between mb-4">
        <button
          onClick={() => setStep((prev) => Math.max(prev - 1, 1))}
          disabled={step === 1}
          className={`px-4 py-2 rounded ${
            step === 1
              ? "bg-gray-300"
              : "bg-blue-600 text-white hover:bg-blue-700"
          }`}
        >
          ← Previous
        </button>
        <span className="text-lg font-semibold">
          {step === 1
            ? "User Details"
            : step === 2
            ? "Business Details"
            : "License Details"}
        </span>
        <button
          disabled={step === 3 && user?.userVerified === true}
          onClick={() =>
            step === 3 ? setShowModal(true) : setStep((prev) => prev + 1)
          }
          className={`px-4 py-2 rounded ${
            step === 3 && user?.userVerified === true
              ? "bg-gray-400 cursor-not-allowed"
              : "bg-blue-600 text-white hover:bg-blue-700"
          }`}
        >
          {step === 3 ? "Verify User" : "Next →"}
        </button>
      </div>

      {/* Step Content */}
      {renderStepContent()}

      {/* Modal Confirmation */}
      {showModal && (
        <div className="fixed inset-0 bg-gray-700 bg-opacity-50 flex justify-center items-center">
          <div className="bg-white p-6 rounded">
            <h2 className="text-xl font-bold mb-4">Confirm Verification</h2>
            <p>Are you sure you want to verify this user?</p>
            <div className="mt-4 flex justify-end space-x-2">
              <button
                onClick={() => setShowModal(false)}
                className="px-4 py-2 bg-gray-300 rounded"
              >
                Cancel
              </button>
              <button
                onClick={() => handleVerifyUser(user.id)}
                className="px-4 py-2 bg-blue-600 text-white rounded"
              >
                Verify
              </button>
            </div>
          </div>
        </div>
      )}
    </div>
  );
}
````

## File: src/app/dashboard/car-dealer/add-listing/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { useState } from "react";
import { useRouter } from "next/navigation";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";

const AddCarListing = () => {
  const [formData, setFormData] = useState({
    model: "",
    make: "",
    price: "",
    year: "",
    mileage: "",
    exteriorColor: "",
    interiorColor: "",
    transmission: "",
    fuelType: "",
    vin: "",
    vehicleType: "",
    noOfSeats: "",
    status: "",
  });

  const [images, setImages] = useState<File[]>([]);
  const [errorMessage, setErrorMessage] = useState("");
  const [successMessage, setSuccessMessage] = useState("");
  const router = useRouter();
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Handle input changes for text/number fields
  const handleChange = (
    e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>
  ) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  // Handle image uploads
  const handleFileChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    if (e.target.files) {
      setImages(Array.from(e.target.files));
    }
  };

  // Basic validation for required fields and image count
  const validateForm = () => {
    // Check that every field is provided (adjust as needed)
    for (const [key, value] of Object.entries(formData)) {
      if (!value) {
        setErrorMessage(`Field "${key}" is required.`);
        return false;
      }
    }

    if (isNaN(Number(formData.price)) || Number(formData.price) <= 0) {
      setErrorMessage("Please enter a valid price.");
      return false;
    }

    if (images.length === 0 || images.length > 3) {
      setErrorMessage("You must upload between 1 and 3 images.");
      return false;
    }

    setErrorMessage(""); // Clear any previous error
    return true;
  };

  // Submit form data
  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();

    if (!validateForm()) {
      return;
    }

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataObj = new FormData();
      // Append every field from the formData state
      Object.entries(formData).forEach(([key, value]) => {
        formDataObj.append(key, value);
      });
      // Append images
      images.forEach((image) => formDataObj.append("images", image));

      const response = await fetch(
        `${endpoint}api/protected/car-listing/add-car-listing`,
        {
          method: "POST",
          headers: {
            Authorization: `Bearer ${token}`,
          },
          body: formDataObj,
        }
      );

      if (response.ok) {
        setSuccessMessage("Car listing created successfully!");
        setErrorMessage("");
        router.push("/dashboard/car-dealer/car-listings");
      } else {
        setErrorMessage("Failed to create car listing. Please try again.");
        setSuccessMessage("");
      }
    } catch (error) {
      setErrorMessage("An error occurred. Please try again.");
      setSuccessMessage("");
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 ">
      {/* Back Button */}
      <Link href="/dashboard/car-dealer">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>
      <div className="max-w-4xl mx-auto p-6 shadow-lg rounded-lg mt-8">
        <h1 className="text-2xl font-bold mb-6">Add Car Listing</h1>
        <form onSubmit={handleSubmit}>
          {/* Model */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Model</label>
            <input
              type="text"
              name="model"
              value={formData.model}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Make */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Make</label>
            <input
              type="text"
              name="make"
              value={formData.make}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Price */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Price</label>
            <input
              type="number"
              name="price"
              value={formData.price}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Year */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Year</label>
            <input
              type="number"
              name="year"
              value={formData.year}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Mileage */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Mileage</label>
            <input
              type="number"
              name="mileage"
              value={formData.mileage}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Exterior Color */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Exterior Color</label>
            <input
              type="text"
              name="exteriorColor"
              value={formData.exteriorColor}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Interior Color */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Interior Color</label>
            <input
              type="text"
              name="interiorColor"
              value={formData.interiorColor}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Transmission */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Transmission</label>
            <input
              type="text"
              name="transmission"
              value={formData.transmission}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Fuel Type */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Fuel Type</label>
            <input
              type="text"
              name="fuelType"
              value={formData.fuelType}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* VIN */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">VIN</label>
            <input
              type="text"
              name="vin"
              value={formData.vin}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Vehicle Type */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Vehicle Type</label>
            <input
              type="text"
              name="vehicleType"
              value={formData.vehicleType}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Number of Seats */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Number of Seats</label>
            <input
              type="number"
              name="noOfSeats"
              value={formData.noOfSeats}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Status */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Status</label>
            <input
              type="text"
              name="status"
              value={formData.status}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Image Upload */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">
              Upload Images (Max: 3)
            </label>
            <input
              type="file"
              multiple
              accept="image/*"
              onChange={handleFileChange}
              className="w-full border rounded p-2"
            />
          </div>

          {errorMessage && <p className="text-red-500">{errorMessage}</p>}
          {successMessage && <p className="text-blue-500">{successMessage}</p>}

          {/* Submit Button */}
          <Button
            type="submit"
            className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-500 mt-3"
          >
            Submit Car Listing
          </Button>
        </form>
      </div>
    </div>
  );
};

export default AddCarListing;
````

## File: src/app/dashboard/car-dealer/car-listings/[id]/page.tsx
````typescript
"use client";

import { useParams, useRouter } from "next/navigation";
import { useEffect, useState } from "react";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import {
  FiEdit,
  FiTrash2,
  FiArrowLeft,
  FiCalendar,
  FiDroplet,
  FiSettings,
  FiUsers,
  FiPhoneCall,
  FiMail,
  FiMapPin,
  FiDollarSign,
} from "react-icons/fi";
import { MdSpeed, MdCarRental, MdFormatPaint } from "react-icons/md";
import { Swiper, SwiperSlide } from "swiper/react";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";
import { Card, CardContent } from "@/components/ui/card";

const ViewCarListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [listing, setListing] = useState<any>(null);
  const [userRole, setUserRole] = useState<string | null>(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);

  useEffect(() => {
    if (id) {
      const fetchListing = async () => {
        try {
          const endpoint = process.env.NEXT_PUBLIC_API_URL;
          // Fetch token
          const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
          const tokenData = await tokenResponse.json();
          const token = tokenData?.token;
          const role = tokenData?.role;
          if (!token) {
            throw new Error("Invalid authentication token");
          }
          setUserRole(role);

          // Fetch car listing
          const response = await fetch(
            `${endpoint}api/protected/car-listing/carlisting/${id}`,
            {
              headers: { Authorization: `Bearer ${token}` },
            }
          );
          if (!response.ok) {
            throw new Error("Failed to fetch car listing");
          }
          const data = await response.json();
          setListing(data);
        } catch (err: any) {
          setError(err.message);
        } finally {
          setLoading(false);
        }
      };
      fetchListing();
    }
  }, [id]);

  const handleDelete = async () => {
    if (confirm("Are you sure you want to delete this car listing?")) {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) {
          throw new Error("Invalid authentication token");
        }
        const response = await fetch(
          `${endpoint}api/protected/car-listing/delete-car-listing/${id}`,
          {
            method: "DELETE",
            headers: { Authorization: `Bearer ${token}` },
          }
        );
        if (!response.ok) {
          throw new Error("Failed to delete car listing");
        }
        alert("Car listing deleted successfully");
        router.push("/dashboard/car-dealer/car-listings");
      } catch (err: any) {
        alert(`Error deleting car listing: ${err.message}`);
      }
    }
  };

  // Helper functions to format dealership info
  const formatFinancingOptions = (optionsStr: string) => {
    return optionsStr
      .replace(/[{}"]/g, "")
      .split(",")
      .map((o) => o.trim());
  };

  const formatShowroomLocations = (locationsStr: string) => {
    return locationsStr.replace(/[{}"]/g, "");
  };

  if (loading) {
    return <p className="text-center text-lg text-gray-500">Loading...</p>;
  }
  if (error) {
    return <p className="text-center text-red-500 text-lg">Error: {error}</p>;
  }
  if (!listing) {
    return (
      <p className="text-center text-gray-500 text-lg">No car listing found</p>
    );
  }

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      <Link href="/dashboard/car-dealer/car-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>

      <div className="flex flex-col md:flex-row gap-6">
        {/* Main Listing Card */}
        <div className="md:w-2/3">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              {/* Image Carousel */}
              {listing.carImages && listing.carImages.length > 0 && (
                <Swiper
                  navigation={true}
                  modules={[Navigation]}
                  className="w-full h-96 rounded-lg shadow-lg mb-6"
                >
                  {listing.carImages.map((image, index) => (
                    <SwiperSlide key={index}>
                      <img
                        src={image.base64}
                        alt={`Car Image ${index + 1}`}
                        className="w-full h-96 object-cover rounded-lg"
                      />
                    </SwiperSlide>
                  ))}
                </Swiper>
              )}
              {/* Car Details */}
              <div className="mb-4">
                <h1 className="text-3xl font-semibold">
                  {listing.model} - {listing.make}
                </h1>
                {listing.createdAt && (
                  <p className="mt-2 text-sm text-gray-500">
                    Created At:{" "}
                    {new Date(listing.createdAt).toLocaleDateString()}
                  </p>
                )}
                <p className="text-2xl mt-2 text-blue-600 font-bold flex items-center gap-1">
                  <FiDollarSign size={24} />
                  {listing.price ?? "N/A"}
                </p>
              </div>
              {/* Specifications */}
              <div className="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-3 gap-4">
                <div className="flex items-center gap-1">
                  <FiCalendar size={20} />
                  <p className="text-lg font-semibold">
                    {listing.year ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <MdSpeed size={20} />
                  <p className="text-lg font-semibold">
                    {listing.mileage ? `${listing.mileage} km` : "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiSettings size={20} />
                  <p className="text-lg font-semibold">
                    {listing.transmission ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiDroplet size={20} />
                  <p className="text-lg font-semibold">
                    {listing.fuelType ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiUsers size={20} />
                  <p className="text-lg font-semibold">
                    {listing.noOfSeats ? `${listing.noOfSeats} Seats` : "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <MdFormatPaint size={20} />
                  <p className="text-lg font-semibold">
                    {listing.exteriorColor ?? "N/A"}
                  </p>
                </div>
              </div>

              {/* Action Buttons */}
              <div className="mt-6 flex flex-wrap gap-4">
                <Link href={`/dashboard/car-dealer/edit-listing/${id}`}>
                  <Button variant="default" className="flex items-center gap-2">
                    <FiEdit size={18} />
                    Edit Listing
                  </Button>
                </Link>
                <Button
                  onClick={handleDelete}
                  variant="destructive"
                  className="flex items-center gap-2"
                >
                  <FiTrash2 size={18} />
                  Delete Listing
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>

        {/* Separate Dealership Info Container */}
        {listing.dealership && (
          <div className="md:w-1/3">
            <Card className="shadow-lg">
              <CardContent className="p-6">
                <h2 className="text-xl font-bold mb-4">Contact Details: </h2>
                <div className="mb-3">
                  <p className="font-semibold">{listing.dealership.fullName}</p>
                </div>
                <div className="flex items-center mb-3">
                  <FiPhoneCall size={18} className="text-blue-500 mr-2" />
                  <p>{listing.dealership.phoneNo}</p>
                </div>
                <div className="flex items-center mb-3">
                  <FiMail size={18} className="text-blue-500 mr-2" />
                  <p>{listing.dealership.email}</p>
                </div>
                {listing.dealership.carDealership && (
                  <>
                    <div className="flex items-center mb-3">
                      <FiMapPin size={18} className="text-red-500 mr-2" />
                      <div>
                        <p className="text-lg">
                          {listing.dealership.carDealership.businessName}
                        </p>
                        <p className="text-lg">
                          {formatShowroomLocations(
                            listing.dealership.carDealership.showroomLocations
                          )}
                        </p>
                      </div>
                    </div>
                    <div className="mb-3">
                      <ul className="list-disc list-inside list-none">
                        {formatFinancingOptions(
                          listing.dealership.carDealership.financingOptions
                        ).map((option, idx) => (
                          <li key={idx} className="text-lg">
                            {option === "inHouseFinancing:true" &&
                              "🏠 In-House Financing"}
                            {option === "thirdPartyBanks:true" &&
                              "🏦 Third-Party Banks"}
                            {option === "leaseOptions:true" &&
                              "📄 Lease Options"}
                            {option === "inHouseFinancing:false" &&
                              "❌ No In-House Financing"}
                            {option === "thirdPartyBanks:false" &&
                              "❌ No Third-Party Banks"}
                            {option === "leaseOptions:false" &&
                              "❌ No Lease Options"}
                          </li>
                        ))}
                      </ul>
                    </div>
                  </>
                )}
              </CardContent>
            </Card>
          </div>
        )}
      </div>
    </div>
  );
};

export default ViewCarListing;
````

## File: src/app/dashboard/car-dealer/edit-listing/[id]/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { useEffect, useState } from "react";
import { useRouter, useParams } from "next/navigation";
import { Card } from "@/components/ui/card";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";

const EditCarListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [formData, setFormData] = useState({
    model: "",
    make: "",
    price: "",
    year: "",
    mileage: "",
    exteriorColor: "",
    interiorColor: "",
    transmission: "",
    fuelType: "",
    vin: "",
    vehicleType: "",
    noOfSeats: "",
    status: "",
  });

  // existingImages will contain both server images (as base64) and previews for newly added images.
  const [existingImages, setExistingImages] = useState([]);
  // newImages holds only new File objects
  const [newImages, setNewImages] = useState([]);
  const [errorMessage, setErrorMessage] = useState("");
  const [successMessage, setSuccessMessage] = useState("");

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Helper function to convert a base64 data URL to a File object.
  const dataURLtoFile = (dataurl, filename) => {
    const arr = dataurl.split(",");
    const mimeMatch = arr[0].match(/:(.*?);/);
    if (!mimeMatch) return null;
    const mime = mimeMatch[1];
    const bstr = atob(arr[1]);
    let n = bstr.length;
    const u8arr = new Uint8Array(n);
    while (n--) {
      u8arr[n] = bstr.charCodeAt(n);
    }
    return new File([u8arr], filename, { type: mime });
  };

  useEffect(() => {
    const fetchData = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const response = await fetch(
          `${endpoint}api/protected/car-listing/carlisting/${id}`,
          { headers: { Authorization: `Bearer ${token}` } }
        );

        if (!response.ok) throw new Error("Failed to fetch listing data");

        const data = await response.json();
        setFormData({
          model: data.model ?? "",
          make: data.make ?? "",
          price: data.price?.toString() ?? "",
          year: data.year?.toString() ?? "",
          mileage: data.mileage?.toString() ?? "",
          exteriorColor: data.exteriorColor ?? "",
          interiorColor: data.interiorColor ?? "",
          transmission: data.transmission ?? "",
          fuelType: data.fuelType ?? "",
          vin: data.vin ?? "",
          vehicleType: data.vehicleType ?? "",
          noOfSeats: data.noOfSeats?.toString() ?? "",
          status: data.status ?? "",
        });
        // Set existing images from the server as base64 strings.
        setExistingImages(data.carImages.map((img) => img.base64));
      } catch (error) {
        setErrorMessage("Failed to fetch listing data: " + error.message);
      }
    };
    fetchData();
  }, [id, endpoint]);

  const handleChange = (e) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  const handleFileChange = (e) => {
    if (e.target.files) {
      const filesArray = Array.from(e.target.files);
      const newPreviews = filesArray.map((file) => URL.createObjectURL(file));
      setNewImages((prev) => [...prev, ...filesArray]);
      setExistingImages((prev) => [...prev, ...newPreviews]);
    }
  };

  const removeImage = (index) => {
    const newExisting = [...existingImages];
    newExisting.splice(index, 1);
    setExistingImages(newExisting);
    // Determine if the removed image is from newImages.
    if (index >= existingImages.length - newImages.length) {
      const newIndex = index - (existingImages.length - newImages.length);
      const newFiles = [...newImages];
      newFiles.splice(newIndex, 1);
      setNewImages(newFiles);
    }
  };

  const handleSubmit = async (e) => {
    e.preventDefault();
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;
      const formDataObj = new FormData();

      Object.keys(formData).forEach((key) => {
        formDataObj.append(key, formData[key]);
      });

      // Calculate how many images came from the server.
      const serverImagesCount = existingImages.length - newImages.length;
      const serverImages = existingImages.slice(0, serverImagesCount);

      // Convert each server image (base64 string) to a File and append.
      serverImages.forEach((dataURL, index) => {
        const file = dataURLtoFile(dataURL, `server-image-${index}.png`);
        if (file) {
          formDataObj.append("images", file);
        }
      });

      // Append new images (already File objects).
      newImages.forEach((image) => {
        formDataObj.append("images", image);
      });

      const response = await fetch(
        `${endpoint}api/protected/car-listing/update-car-listing/${id}`,
        {
          method: "PUT",
          headers: { Authorization: `Bearer ${token}` },
          body: formDataObj,
        }
      );

      if (!response.ok)
        throw new Error(`Failed to update listing: ${response.statusText}`);

      setSuccessMessage("Car listing updated successfully!");
      router.push(`/dashboard/car-dealer/car-listings/${id}`);
    } catch (error) {
      setErrorMessage("Error updating listing: " + error.message);
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      {/* Back Button */}
      <Link href="/dashboard/car-dealer/car-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>
      <Card className="shadow-lg p-6">
        <h1 className="text-2xl font-bold mb-6">Edit Car Listing</h1>
        <form onSubmit={handleSubmit}>
          {Object.keys(formData).map(
            (key) =>
              // Exclude fields not intended for editing
              !["id", "dealership", "createdAt", "carImages"].includes(key) && (
                <div key={key} className="mb-4">
                  <label className="block font-semibold mb-2 capitalize">
                    {key.replace(/([A-Z])/g, " $1")}
                  </label>
                  <input
                    type="text"
                    name={key}
                    value={formData[key as keyof typeof formData]}
                    onChange={handleChange}
                    className="w-full border rounded p-2"
                  />
                </div>
              )
          )}

          <div className="mb-4">
            <label className="block font-semibold mb-2">Add Images</label>
            <input
              type="file"
              multiple
              accept="image/*"
              onChange={handleFileChange}
              className="w-full border rounded p-2"
            />
            <div className="flex flex-wrap gap-4 mt-4">
              {existingImages.map((image, index) => (
                <div key={index} className="relative">
                  <img
                    src={image}
                    alt={`Car Image ${index}`}
                    className="w-24 h-24 object-cover rounded"
                  />
                  <button
                    type="button"
                    className="absolute top-0 right-0 bg-red-500 text-white p-1 rounded"
                    onClick={() => removeImage(index)}
                  >
                    &times;
                  </button>
                </div>
              ))}
            </div>
          </div>

          <Button
            type="submit"
            className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-500 mt-3"
          >
            Update Listing
          </Button>
        </form>
        {errorMessage && <p className="text-red-500">{errorMessage}</p>}
        {successMessage && <p className="text-blue-500">{successMessage}</p>}
      </Card>
    </div>
  );
};

export default EditCarListing;
````

## File: src/app/dashboard/not-verified/page.tsx
````typescript
"use client";
import { useSearchParams, useRouter } from "next/navigation";
import { FaCheckCircle } from "react-icons/fa";

export default function NotVerified() {
  const searchParams = useSearchParams();
  const reason = searchParams.get("reason");
  let message = "";
  if (reason === "user") {
    message = "Your account verification is pending.";
  }
  return (
    <div className="flex flex-col items-center justify-center p-6">
      <div className="shadow-lg rounded-2xl p-8 text-center max-w-md w-full">
        <FaCheckCircle className="text-blue-500 w-16 h-16 mx-auto" />
        <h1 className="text-2xl font-semibold mt-4">
          Form Submitted Successfully!
        </h1>
        <p className="text-gray-600 mt-2">{`${message} We will notify you once the process is complete.`}</p>
      </div>
    </div>
  );
}
````

## File: src/app/dashboard/realtor/add-listing/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { useState } from "react";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";

const AddListing = () => {
  const [formData, setFormData] = useState({
    title: "",
    description: "",
    price: "",
    location: "",
    bedrooms: "",
    bathrooms: "",
    squareFeet: "",
    openhouse: false,
    startDate: "",
    endDate: "",
    startTime: "",
    endTime: "",
  });

  const [images, setImages] = useState<File[]>([]);
  const [errorMessage, setErrorMessage] = useState("");
  const [successMessage, setSuccessMessage] = useState("");

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Handle input changes
  const handleChange = (
    e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>
  ) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  // Toggle open house checkbox
  const handleToggleOpenHouse = () => {
    setFormData((prev) => ({ ...prev, openhouse: !prev.openhouse }));
  };

  // Handle image uploads
  const handleFileChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    if (e.target.files) {
      setImages(Array.from(e.target.files));
    }
  };

  // Validation function
  const validateForm = () => {
    if (!formData.title || !formData.price || !formData.location) {
      setErrorMessage("Title, price, and location are required.");
      return false;
    }

    if (isNaN(Number(formData.price)) || Number(formData.price) <= 0) {
      setErrorMessage("Please enter a valid price.");
      return false;
    }

    if (formData.openhouse) {
      if (
        !formData.startDate ||
        !formData.endDate ||
        !formData.startTime ||
        !formData.endTime
      ) {
        setErrorMessage(
          "Start and end date, and time are required for open house."
        );
        return false;
      }
      if (new Date(formData.startDate) > new Date(formData.endDate)) {
        setErrorMessage("Start date must be earlier than end date.");
        return false;
      }
    }

    if (images.length === 0 || images.length > 3) {
      setErrorMessage("You must upload between 1 and 3 images.");
      return false;
    }

    setErrorMessage(""); // Clear any previous error message
    return true;
  };

  // Submit form
  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();

    if (!validateForm()) {
      return;
    }

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataObj = new FormData();
      Object.entries(formData).forEach(([key, value]) => {
        formDataObj.append(key, value);
      });

      images.forEach((image) => formDataObj.append("images", image));

      const response = await fetch(
        `${endpoint}api/protected/house-listing/add-house-listing`,
        {
          method: "POST",
          headers: {
            Authorization: `Bearer ${token}`,
          },
          body: formDataObj,
        }
      );

      if (response.ok) {
        setSuccessMessage("Listing created successfully!");
        setErrorMessage("");
      } else {
        setErrorMessage("Failed to create listing. Please try again.");
        setSuccessMessage("");
      }
    } catch (error) {
      setErrorMessage("An error occurred. Please try again.");
      setSuccessMessage("");
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-2">
      {/* Back Button */}
      <Link href="/dashboard/realtor/house-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>
      <div className="max-w-4xl mx-auto p-6 bg-white shadow-lg rounded-lg mt-8">
        <h1 className="text-2xl font-bold mb-6">Add House Listing</h1>
        <form onSubmit={handleSubmit}>
          {/* Title */}
          <input
            type="text"
            name="title"
            value={formData.title}
            onChange={handleChange}
            className="w-full border rounded p-2 mb-4"
            placeholder="Title"
            required
          />

          {/* Description */}
          <textarea
            name="description"
            value={formData.description}
            onChange={handleChange}
            className="w-full border rounded p-2 mb-4"
            placeholder="Description"
          />

          {/* Price & Location */}
          <div className="grid grid-cols-2 gap-4 mb-4">
            <input
              type="number"
              name="price"
              value={formData.price}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Price"
              required
            />
            <input
              type="text"
              name="location"
              value={formData.location}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Location"
              required
            />
          </div>

          {/* Bedrooms, Bathrooms, Square Feet */}
          <div className="grid grid-cols-3 gap-4 mb-4">
            <input
              type="number"
              name="bedrooms"
              value={formData.bedrooms}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Bedrooms"
            />
            <input
              type="number"
              name="bathrooms"
              value={formData.bathrooms}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Bathrooms"
            />
            <input
              type="number"
              name="squareFeet"
              value={formData.squareFeet}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Square Feet"
            />
          </div>

          {/* Open House Checkbox */}
          <label className="flex items-center space-x-2 mb-4">
            <input
              type="checkbox"
              checked={formData.openhouse}
              onChange={handleToggleOpenHouse}
            />
            <span>Open House</span>
          </label>

          {/* Open House Details */}
          {formData.openhouse && (
            <div className="grid grid-cols-2 gap-4">
              <input
                type="date"
                name="startDate"
                value={formData.startDate}
                onChange={handleChange}
                className="w-full border rounded p-2"
              />
              <input
                type="date"
                name="endDate"
                value={formData.endDate}
                onChange={handleChange}
                className="w-full border rounded p-2"
              />
              <input
                type="time"
                name="startTime"
                value={formData.startTime}
                onChange={handleChange}
                className="w-full border rounded p-2"
              />
              <input
                type="time"
                name="endTime"
                value={formData.endTime}
                onChange={handleChange}
                className="w-full border rounded p-2"
              />
            </div>
          )}

          {/* Image Upload */}
          <input
            type="file"
            multiple
            accept="image/*"
            onChange={handleFileChange}
            className="w-full border rounded p-2 mb-4"
          />

          {errorMessage && <p className="text-red-500">{errorMessage}</p>}
          {successMessage && <p className="text-blue-500">{successMessage}</p>}

          {/* Submit Button */}
          <Button
            type="submit"
            className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-500"
          >
            Submit Listing
          </Button>
        </form>
      </div>
    </div>
  );
};

export default AddListing;
````

## File: src/app/dashboard/realtor/edit-listing/[id]/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { useEffect, useState } from "react";
import { useRouter, useParams } from "next/navigation";
import { Card } from "@/components/ui/card";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";

// Helper function to convert a base64 data URL to a File object.
const dataURLtoFile = (dataurl: string, filename: string) => {
  const arr = dataurl.split(",");
  const mimeMatch = arr[0].match(/:(.*?);/);
  if (!mimeMatch) return null;
  const mime = mimeMatch[1];
  const bstr = atob(arr[1]);
  let n = bstr.length;
  const u8arr = new Uint8Array(n);
  while (n--) {
    u8arr[n] = bstr.charCodeAt(n);
  }
  return new File([u8arr], filename, { type: mime });
};

const EditHouseListing = () => {
  const { id } = useParams();
  const router = useRouter();

  const [formData, setFormData] = useState({
    title: "",
    description: "",
    price: "",
    location: "",
    bedrooms: "",
    bathrooms: "",
    squareFeet: "",
    openhouse: false,
    startDate: "",
    endDate: "",
    startTime: "",
    endTime: "",
  });

  // existingImages holds base64 strings from the server and previews for new images.
  const [existingImages, setExistingImages] = useState<string[]>([]);
  // newImages holds File objects from new uploads.
  const [newImages, setNewImages] = useState<File[]>([]);
  const [errorMessage, setErrorMessage] = useState("");
  const [successMessage, setSuccessMessage] = useState("");

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Fetch listing data
  useEffect(() => {
    const fetchData = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok) {
          throw new Error("Failed to get authentication token");
        }
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const response = await fetch(
          `${endpoint}api/protected/house-listing/houselisting/${id}`,
          { headers: { Authorization: `Bearer ${token}` } }
        );
        if (!response.ok) {
          throw new Error("Failed to fetch listing data");
        }
        const data = await response.json();
        setFormData({
          title: data.title || "",
          description: data.description || "",
          price: data.price?.toString() || "",
          location: data.location || "",
          bedrooms: data.bedrooms?.toString() || "",
          bathrooms: data.bathrooms?.toString() || "",
          squareFeet: data.squareFeet?.toString() || "",
          openhouse: data.openhouse || false,
          startDate: data.startdate ? data.startdate.split("T")[0] : "",
          endDate: data.endDate ? data.endDate.split("T")[0] : "",
          startTime: data.startTime || "",
          endTime: data.endTime || "",
        });
        // Assume the API returns houseImages as an array of { base64: string } objects.
        setExistingImages(data.houseImages.map((img: any) => img.base64));
      } catch (error: any) {
        setErrorMessage("Failed to fetch listing data: " + error.message);
      }
    };

    fetchData();
  }, [id, endpoint]);

  // Update form values
  const handleChange = (
    e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>
  ) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  // Toggle open house checkbox
  const handleToggleOpenHouse = () => {
    setFormData((prev) => ({ ...prev, openhouse: !prev.openhouse }));
  };

  // Handle new file selection
  const handleFileChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    if (e.target.files) {
      const filesArray = Array.from(e.target.files);
      const newPreviews = filesArray.map((file) => URL.createObjectURL(file));
      setNewImages((prev) => [...prev, ...filesArray]);
      setExistingImages((prev) => [...prev, ...newPreviews]);
    }
  };

  // Remove an image from the preview and newImages if applicable.
  const removeExistingImage = (index: number) => {
    setExistingImages((prev) => prev.filter((_, i) => i !== index));
    if (index >= existingImages.length - newImages.length) {
      const newIndex = index - (existingImages.length - newImages.length);
      setNewImages((prev) => prev.filter((_, i) => i !== newIndex));
    }
  };

  const validateForm = () => {
    if (!formData.title || !formData.price || !formData.location) {
      setErrorMessage("Title, price, and location are required.");
      return false;
    }
    if (isNaN(Number(formData.price)) || Number(formData.price) <= 0) {
      setErrorMessage("Please enter a valid price.");
      return false;
    }
    if (formData.openhouse) {
      if (
        !formData.startDate ||
        !formData.endDate ||
        !formData.startTime ||
        !formData.endTime
      ) {
        setErrorMessage(
          "Start and end date, and time are required for open house."
        );
        return false;
      }
      if (new Date(formData.startDate) > new Date(formData.endDate)) {
        setErrorMessage("Start date must be earlier than end date.");
        return false;
      }
    }
    if (newImages.length > 3) {
      setErrorMessage("You can upload a maximum of 3 new images.");
      return false;
    }
    setErrorMessage("");
    return true;
  };

  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();
    if (!validateForm()) return;

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");
      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      // Convert numeric fields to numbers.
      const numericFields = {
        price: Number(formData.price),
        bedrooms: Number(formData.bedrooms),
        bathrooms: Number(formData.bathrooms),
        // Backend expects key "sqft" for square footage.
        sqft: Number(formData.squareFeet),
      };

      const formDataObj = new FormData();
      formDataObj.append("title", formData.title);
      formDataObj.append("description", formData.description);
      formDataObj.append("location", formData.location);
      formDataObj.append("openhouse", JSON.stringify(formData.openhouse));
      if (formData.openhouse) {
        formDataObj.append("startDate", formData.startDate);
        formDataObj.append("endDate", formData.endDate);
        formDataObj.append("startTime", formData.startTime);
        formDataObj.append("endTime", formData.endTime);
      }
      // Append numeric fields with correct keys.
      formDataObj.append("price", numericFields.price.toString());
      formDataObj.append("bedrooms", numericFields.bedrooms.toString());
      formDataObj.append("bathrooms", numericFields.bathrooms.toString());
      formDataObj.append("sqft", numericFields.sqft.toString());

      // Append existing images from the server.
      const serverImagesCount = existingImages.length - newImages.length;
      const serverImages = existingImages.slice(0, serverImagesCount);
      serverImages.forEach((dataURL, index) => {
        const file = dataURLtoFile(dataURL, `server-image-${index}.png`);
        if (file) formDataObj.append("images", file);
      });

      // Append newly selected images.
      newImages.forEach((image) => {
        formDataObj.append("images", image);
      });

      const response = await fetch(
        `${endpoint}api/protected/house-listing/update-house-listing/${id}`,
        {
          method: "PUT",
          headers: { Authorization: `Bearer ${token}` },
          body: formDataObj,
        }
      );
      if (!response.ok) {
        throw new Error(`Failed to update listing: ${response.statusText}`);
      }
      setSuccessMessage("House listing updated successfully!");
      router.push(`/dashboard/realtor/house-listings/${id}`);
    } catch (error: any) {
      console.error("Error updating listing:", error);
      setErrorMessage("Error updating listing: " + error.message);
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      {/* Back Button */}
      <Link href="/dashboard/realtor/house-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>
      <Card className="shadow-lg">
        <div className="p-6">
          <h1 className="text-2xl font-bold mb-6">Edit House Listing</h1>
          <form onSubmit={handleSubmit}>
            <div className="grid grid-cols-2 gap-4">
              <input
                type="text"
                name="title"
                value={formData.title}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Title"
                required
              />
              <input
                type="text"
                name="price"
                value={formData.price}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Price"
                required
              />
              <input
                type="text"
                name="location"
                value={formData.location}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Location"
                required
              />
              <input
                type="number"
                name="bedrooms"
                value={formData.bedrooms}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Bedrooms"
              />
              <input
                type="number"
                name="bathrooms"
                value={formData.bathrooms}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Bathrooms"
              />
              <input
                type="number"
                name="squareFeet"
                value={formData.squareFeet}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Square Feet"
              />
            </div>

            <textarea
              name="description"
              value={formData.description}
              onChange={handleChange}
              className="border p-2 rounded w-full mt-4"
              placeholder="Description"
            ></textarea>

            <div className="mt-4">
              <label className="flex items-center space-x-2">
                <input
                  type="checkbox"
                  checked={formData.openhouse}
                  onChange={handleToggleOpenHouse}
                />
                <span>Open House</span>
              </label>
            </div>

            {formData.openhouse && (
              <div className="grid grid-cols-2 gap-4 mt-4">
                <input
                  type="date"
                  name="startDate"
                  value={formData.startDate}
                  onChange={handleChange}
                  className="border p-2 rounded"
                  placeholder="Start Date"
                />
                <input
                  type="date"
                  name="endDate"
                  value={formData.endDate}
                  onChange={handleChange}
                  className="border p-2 rounded"
                  placeholder="End Date"
                />
                <input
                  type="time"
                  name="startTime"
                  value={formData.startTime}
                  onChange={handleChange}
                  className="border p-2 rounded"
                  placeholder="Start Time"
                />
                <input
                  type="time"
                  name="endTime"
                  value={formData.endTime}
                  onChange={handleChange}
                  className="border p-2 rounded"
                  placeholder="End Time"
                />
              </div>
            )}

            <div className="mt-4">
              <label className="block font-semibold mb-2">Upload Images</label>
              <input
                type="file"
                multiple
                accept="image/*"
                onChange={handleFileChange}
                className="border p-2 rounded w-full"
              />
              <div className="flex flex-wrap gap-4 mt-4">
                {existingImages.map((image, index) => (
                  <div key={index} className="relative">
                    <img
                      src={image}
                      alt={`House Image ${index}`}
                      className="w-24 h-24 object-cover rounded"
                    />
                    <button
                      type="button"
                      className="absolute top-0 right-0 bg-red-500 text-white p-1 rounded"
                      onClick={() => removeExistingImage(index)}
                    >
                      &times;
                    </button>
                  </div>
                ))}
              </div>
            </div>

            {errorMessage && (
              <p className="text-red-500 mt-4">{errorMessage}</p>
            )}
            {successMessage && (
              <p className="text-blue-500 mt-4">{successMessage}</p>
            )}

            <Button
              type="submit"
              className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-500 mt-4"
            >
              Update Listing
            </Button>
          </form>
        </div>
      </Card>
    </div>
  );
};

export default EditHouseListing;
````

## File: src/app/dashboard/realtor/house-listings/[id]/page.tsx
````typescript
"use client";

import { useParams, useRouter } from "next/navigation";
import { useEffect, useState } from "react";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

// Swiper (Carousel)
import { Swiper, SwiperSlide } from "swiper/react";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";

// Icons
import {
  FiArrowLeft,
  FiEdit,
  FiTrash2,
  FiPhoneCall,
  FiMail,
  FiMapPin,
  FiCalendar,
  FiClock,
  FiHome,
  FiGlobe,
  FiDollarSign,
} from "react-icons/fi";
import { FaBed, FaBath } from "react-icons/fa";

const ViewListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [listing, setListing] = useState<any>(null);
  const [userRole, setUserRole] = useState<string | null>(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);

  // Helper: Format dates.
  const formatDate = (dateStr: string) => {
    if (!dateStr) return "N/A";
    return new Date(dateStr).toLocaleDateString();
  };

  useEffect(() => {
    if (id) {
      const fetchListing = async () => {
        try {
          const endpoint = process.env.NEXT_PUBLIC_API_URL;
          const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
          const tokenData = await tokenResponse.json();
          const token = tokenData?.token;
          const role = tokenData?.role;
          if (!token) {
            throw new Error("Invalid authentication token");
          }
          setUserRole(role);
          const response = await fetch(
            `${endpoint}api/protected/house-listing/houselisting/${id}`,
            {
              headers: { Authorization: `Bearer ${token}` },
            }
          );
          if (!response.ok) {
            throw new Error("Failed to fetch listing");
          }
          const data = await response.json();
          setListing(data);
        } catch (err: any) {
          setError(err.message);
        } finally {
          setLoading(false);
        }
      };

      fetchListing();
    }
  }, [id]);

  const handleDelete = async () => {
    if (confirm("Are you sure you want to delete this listing?")) {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) {
          throw new Error("Invalid authentication token");
        }
        const response = await fetch(
          `${endpoint}api/protected/house-listing/delete-house-listing/${id}`,
          {
            method: "DELETE",
            headers: { Authorization: `Bearer ${token}` },
          }
        );
        if (!response.ok) {
          throw new Error("Failed to delete listing");
        }
        alert("Listing deleted successfully");
        router.push("/dashboard/realtor/house-listings");
      } catch (err: any) {
        alert(`Error deleting listing: ${err.message}`);
      }
    }
  };

  if (loading) {
    return <p className="text-center text-lg text-gray-500">Loading...</p>;
  }

  if (error) {
    return <p className="text-center text-red-500 text-lg">Error: {error}</p>;
  }

  if (!listing) {
    return (
      <p className="text-center text-gray-500 text-lg">No listing found</p>
    );
  }

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      {/* Back Button */}
      <Link href="/dashboard/realtor/house-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>

      <div className="flex flex-col md:flex-row gap-6">
        {/* Left: Main Listing Card */}
        <div className="md:w-2/3">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              {/* Image Carousel */}
              {listing.houseImages && listing.houseImages.length > 0 && (
                <Swiper
                  navigation={true}
                  modules={[Navigation]}
                  className="w-full h-96 rounded-lg shadow-lg mb-6"
                >
                  {listing.houseImages.map((image: any, index: number) => (
                    <SwiperSlide key={index}>
                      <img
                        src={image.base64}
                        alt={`House Image ${index + 1}`}
                        className="w-full h-96 object-cover rounded-lg"
                      />
                    </SwiperSlide>
                  ))}
                </Swiper>
              )}

              {/* Title, Price, and Created At */}
              <div className="mb-4">
                <h1 className="text-3xl font-semibold flex items-center gap-2">
                  {listing.title ?? "Untitled"}
                </h1>
                <p className="text-2xl mt-2 text-blue-600 font-bold flex items-center gap-2">
                  <FiDollarSign size={24} />
                  {listing.price ?? "N/A"}
                </p>
                {listing.createdAt && (
                  <p className="mt-2 text-sm text-gray-500">
                    Created At:{" "}
                    {new Date(listing.createdAt).toLocaleDateString()}
                  </p>
                )}
              </div>

              {/* Description */}
              {listing.description && (
                <p className="mb-4">{listing.description}</p>
              )}

              {/* House Attributes */}
              <div className="grid grid-cols-2 md:grid-cols-4 gap-4 mb-4">
                {listing.bedrooms !== null && (
                  <div className="flex items-center gap-2">
                    <FaBed size={20} />
                    <p className="text-lg font-semibold">
                      {listing.bedrooms} Beds
                    </p>
                  </div>
                )}
                {listing.bathrooms !== null && (
                  <div className="flex items-center gap-2">
                    <FaBath size={20} />
                    <p className="text-lg font-semibold">
                      {listing.bathrooms} Baths
                    </p>
                  </div>
                )}
                {listing.squareFeet && (
                  <div className="flex items-center gap-2">
                    <FiHome size={20} />
                    <p className="text-lg font-semibold">
                      {listing.squareFeet} sq ft
                    </p>
                  </div>
                )}
                {listing.location && (
                  <div className="flex items-center gap-2">
                    <FiMapPin size={40} />
                    <p className="text-sm font-semibold">{listing.location}</p>
                  </div>
                )}
              </div>

              {/* Action Buttons */}
              <div className="mt-6 flex flex-wrap gap-4">
                <Link href={`/dashboard/realtor/edit-listing/${id}`}>
                  <Button variant="default" className="flex items-center gap-2">
                    <FiEdit size={18} />
                    Edit Listing
                  </Button>
                </Link>
                <Button
                  variant="destructive"
                  className="flex items-center gap-2"
                  onClick={handleDelete}
                >
                  <FiTrash2 size={18} />
                  Delete Listing
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>

        {/* Right: Landlord / Realtor Info Card */}
        {listing.landlord && (
          <div className="md:w-1/3">
            <Card className="shadow-lg">
              <CardContent className="p-6">
                <h2 className="text-xl font-bold mb-4">Contact</h2>
                {listing.landlord.fullName && (
                  <p className="font-semibold mb-4">
                    {listing.landlord.fullName}
                  </p>
                )}
                {listing.landlord.phoneNo && (
                  <div className="flex items-center gap-2 mb-3">
                    <FiPhoneCall size={18} className="text-blue-500" />
                    <p>{listing.landlord.phoneNo}</p>
                  </div>
                )}
                {listing.landlord.email && (
                  <div className="flex items-center gap-2 mb-3">
                    <FiMail size={18} className="text-blue-500" />
                    <p>{listing.landlord.email}</p>
                  </div>
                )}
                {listing.landlord.realtor && (
                  <>
                    <div className="flex items-center mb-3">
                      <FiMapPin size={18} className="text-red-500 mr-2" />
                      <p>
                        {listing.landlord.realtor.businessName},{" "}
                        {listing.landlord.realtor.businessAddress}
                      </p>
                    </div>
                    <div className="flex items-center mb-3">
                      <FiGlobe size={25} className="mr-2" />
                      <p>{listing.landlord.realtor.portfolioWebsite}</p>
                    </div>
                  </>
                )}
              </CardContent>
            </Card>

            {listing.openhouse && (
              <Card className="shadow-lg mt-2">
                <CardContent className="p-6">
                  <h3 className="text-xl font-semibold mb-2">Open House</h3>
                  <div className="flex items-center gap-2 mb-1">
                    <FiCalendar size={18} />
                    <p className="text-">
                      Start Date: {formatDate(listing.startdate)}
                    </p>
                  </div>
                  <div className="flex items-center gap-2 mb-1">
                    <FiCalendar size={18} />
                    <p>End Date: {formatDate(listing.endDate)}</p>
                  </div>
                  <div className="flex items-center gap-2 mb-1">
                    <FiClock size={18} />
                    <p>Start Time: {listing.startTime ?? "N/A"}</p>
                  </div>
                  <div className="flex items-center gap-2">
                    <FiClock size={18} />
                    <p>End Time: {listing.endTime ?? "N/A"}</p>
                  </div>
                </CardContent>
              </Card>
            )}
          </div>
        )}
      </div>
    </div>
  );
};

export default ViewListing;
````

## File: src/app/dashboard/user/ai/career-profile/page.tsx
````typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs';
import { Progress } from '@/components/ui/progress';
import { Alert, AlertDescription } from '@/components/ui/alert';
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
  Download,
  Eye,
  Search
} from 'lucide-react';
import { useToast } from '@/hooks/use-toast';
import { Dialog, DialogContent, DialogDescription, DialogHeader, DialogTitle } from '@/components/ui/dialog';
import JobSearchModal from '@/components/ai/JobSearchModal';

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
  const [generatedResume, setGeneratedResume] = useState<any>(null);
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

      const token = document.cookie.split('; ').find(row => row.startsWith('token='))?.split('=')[1];
      
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
      const token = document.cookie.split('; ').find(row => row.startsWith('token='))?.split('=')[1];
      
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
      const token = document.cookie.split('; ').find(row => row.startsWith('token='))?.split('=')[1];
      
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
````

## File: src/app/dashboard/user/ai/page.tsx
````typescript
"use client";

import React, { useState } from 'react';
import AIFeaturesPanel from '@/components/ai/AIFeaturesPanel';
import ResumeAnalysisList from '@/components/ai/ResumeAnalysisList';
import ResumeAnalysisDetail from '@/components/ai/ResumeAnalysisDetail';
import { Button } from '@/components/ui/button';
import { FileText, Grid3x3 } from 'lucide-react';

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

export default function AIPage() {
  const [currentView, setCurrentView] = useState<'features' | 'analyses' | 'detail'>('analyses');
  const [selectedAnalysis, setSelectedAnalysis] = useState<ResumeAnalysis | null>(null);

  const handleAnalysisSelect = (analysis: ResumeAnalysis) => {
    setSelectedAnalysis(analysis);
    setCurrentView('detail');
  };

  const handleBackToList = () => {
    setSelectedAnalysis(null);
    setCurrentView('analyses');
  };

  const handleBackToFeatures = () => {
    setCurrentView('features');
  };

  return (
    <div className="min-h-screen bg-gray-50">
      <div className="container mx-auto px-4 py-8">
        <div className="mb-8">
          <div className="flex items-center justify-between">
            <div>
              <h1 className="text-4xl font-bold text-gray-900 mb-4">
                AI Career Assistant
              </h1>
              <p className="text-xl text-gray-600">
                {currentView === 'analyses' && 'Your resume analysis history'}
                {currentView === 'detail' && 'Detailed resume analysis'}
                {currentView === 'features' && 'Accelerate your career journey in Canada with our AI-powered tools'}
              </p>
            </div>
            
            {/* View Toggle Buttons */}
            <div className="flex space-x-2">
              <Button
                onClick={() => setCurrentView('analyses')}
                variant={currentView === 'analyses' || currentView === 'detail' ? 'default' : 'outline'}
                className="flex items-center space-x-2"
              >
                <FileText className="w-4 h-4" />
                <span>Resume Analyses</span>
              </Button>
              <Button
                onClick={handleBackToFeatures}
                variant={currentView === 'features' ? 'default' : 'outline'}
                className="flex items-center space-x-2"
              >
                <Grid3x3 className="w-4 h-4" />
                <span>All Features</span>
              </Button>
            </div>
          </div>
        </div>
        
        {/* Content based on current view */}
        {currentView === 'features' && <AIFeaturesPanel />}
        
        {currentView === 'analyses' && (
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
````

## File: src/app/dashboard/user/ai/resume/page.tsx
````typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Alert } from '@/components/ui/alert';
import { Upload, FileText, CheckCircle, XCircle, Loader2, User, Briefcase, GraduationCap, Award, Globe, Zap, Target, TrendingUp, ArrowRight } from 'lucide-react';

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
      
      const token = localStorage.getItem('token');
      console.log('Uploading to:', `${process.env.NEXT_PUBLIC_API_URL}api/protected/ai-local/resume/upload`);
      console.log('Token available:', !!token);
      
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}api/protected/ai-local/resume/upload`, {
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
      const token = localStorage.getItem('token');
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}api/protected/ai-local/career-profile/position-recommendations`, {
        method: 'POST',
        headers: {
          'Authorization': `Bearer ${token}`,
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
      const token = localStorage.getItem('token');
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}api/protected/ai-local/career-profile/enhanced-profile`, {
        method: 'POST',
        headers: {
          'Authorization': `Bearer ${token}`,
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
        window.location.href = '/dashboard/user/ai/career-profile';
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
````

## File: src/app/dashboard/user/cars/car-listings/[id]/page.tsx
````typescript
"use client";

import { useParams, useRouter } from "next/navigation";
import { useEffect, useState } from "react";
import Link from "next/link";

import { Button } from "@/components/ui/button";
import {
  FiArrowLeft,
  FiCalendar,
  FiDroplet,
  FiSettings,
  FiUsers,
  FiPhoneCall,
  FiMail,
  FiMapPin,
  FiDollarSign,
  FiHeart,
} from "react-icons/fi";
import { MdSpeed, MdFormatPaint } from "react-icons/md";
import { Swiper, SwiperSlide } from "swiper/react";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";
import { Card, CardContent } from "@/components/ui/card";

const ViewCarListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [listing, setListing] = useState<any>(null);
  const [userRole, setUserRole] = useState<string | null>(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const checkIfAnyDateIsFuture = (data) => {
    // Get current UTC time
    const currentTime = new Date();

    // Use Array.some() to stop as soon as a future date is found
    const isFuture = data.some((item) => {
      // Validate if endDate exists and is a valid date
      if (!item.endDate) return false;

      // Convert endDate to a Date object
      const endDateUTC = new Date(item.endDate);

      // Check if endDate is valid and greater than currentTime
      return !isNaN(endDateUTC.getTime()) && endDateUTC > currentTime;
    });

    return isFuture;
  };

  useEffect(() => {
    if (id) {
      const fetchListing = async () => {
        try {
          // Fetch token
          const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
          const tokenData = await tokenResponse.json();
          const token = tokenData?.token;
          const role = tokenData?.role;
          if (!token) {
            throw new Error("Invalid authentication token");
          }
          setUserRole(role);

          // Fetch car listing
          const response = await fetch(
            `${endpoint}api/protected/car-listing/carlisting/${id}`,
            {
              headers: { Authorization: `Bearer ${token}` },
            }
          );
          if (!response.ok) {
            throw new Error("Failed to fetch car listing");
          }
          const data = await response.json();
          setListing(data);
        } catch (err: any) {
          setError(err.message);
        } finally {
          setLoading(false);
        }
      };
      fetchListing();
    }
  });

  // Helper functions to format dealership info
  const formatFinancingOptions = (optionsStr: string) => {
    return optionsStr
      .replace(/[{}"]/g, "")
      .split(",")
      .map((o) => o.trim());
  };

  const formatShowroomLocations = (locationsStr: string) => {
    return locationsStr.replace(/[{}"]/g, "");
  };

  if (loading) {
    return <p className="text-center text-lg text-gray-500">Loading...</p>;
  }
  if (error) {
    return <p className="text-center text-red-500 text-lg">Error: {error}</p>;
  }
  if (!listing) {
    return (
      <p className="text-center text-gray-500 text-lg">No car listing found</p>
    );
  }

  const handleContactSeller = async (listingId: number, type: string) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData?.token;

      const response = await fetch(
        `${endpoint}api/protected/appointment/booking-status?listingId=${listingId}&type=${type}`,
        {
          method: "GET",
          headers: {
            "Content-Type": "application/json",
            Authorization: `Bearer ${token}`,
          },
        }
      );

      if (response.status === 200) {
        const data = await response.json();
        if (checkIfAnyDateIsFuture(data.booking)) {
          alert("You have already booked an appointment with this seller");
        } else {
          alert("Action Pending from Consultant");
        }
      } else {
        router.push(`/dashboard/user/slots/${listingId}/${type}`);
      }
    } catch (error) {
      console.error("Error contacting seller:", error);
      alert("An error occurred while processing your request.");
    }
  };

  const handleSaveListing = async (listingId: number) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData?.token;
      const response = await fetch(
        `${endpoint}api/protected/car-listing/add-to-favourites`,
        {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            Authorization: `Bearer ${token}`,
          },
          body: JSON.stringify({
            listingId: listingId,
          }),
        }
      );

      if (response.status === 200) {
        const data = await response.json();
      }
    } catch (error) {
      console.error("Error saving listing:", error);
      alert("An error occurred while processing your request.");
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      <Link href="/dashboard/user">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>

      <div className="flex flex-col md:flex-row gap-6">
        {/* Main Listing Card */}
        <div className="md:w-2/3">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              {/* Image Carousel */}
              {listing.carImages && listing.carImages.length > 0 && (
                <Swiper
                  navigation={true}
                  modules={[Navigation]}
                  className="w-full h-96 rounded-lg shadow-lg mb-6"
                >
                  {listing.carImages.map((image, index) => (
                    <SwiperSlide key={index}>
                      <img
                        src={image.base64}
                        alt={`Car Image ${index + 1}`}
                        className="w-full h-96 object-cover rounded-lg"
                      />
                    </SwiperSlide>
                  ))}
                </Swiper>
              )}
              {/* Car Details */}
              <div className="mb-4">
                <h1 className="text-3xl font-semibold">
                  {listing.model} - {listing.make}
                </h1>
                {listing.createdAt && (
                  <p className="mt-2 text-sm text-gray-500">
                    Created At:{" "}
                    {new Date(listing.createdAt).toLocaleDateString()}
                  </p>
                )}
                <p className="text-2xl mt-2 text-blue-600 font-bold flex items-center gap-1">
                  <FiDollarSign size={24} />
                  {listing.price ?? "N/A"}
                </p>
              </div>
              {/* Specifications */}
              <div className="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-3 gap-4">
                <div className="flex items-center gap-1">
                  <FiCalendar size={20} />
                  <p className="text-lg font-semibold">
                    {listing.year ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <MdSpeed size={20} />
                  <p className="text-lg font-semibold">
                    {listing.mileage ? `${listing.mileage} km` : "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiSettings size={20} />
                  <p className="text-lg font-semibold">
                    {listing.transmission ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiDroplet size={20} />
                  <p className="text-lg font-semibold">
                    {listing.fuelType ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiUsers size={20} />
                  <p className="text-lg font-semibold">
                    {listing.noOfSeats ? `${listing.noOfSeats} Seats` : "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <MdFormatPaint size={20} />
                  <p className="text-lg font-semibold">
                    {listing.exteriorColor ?? "N/A"}
                  </p>
                </div>
              </div>

              {/* Action Buttons */}
              <div className="mt-6 flex flex-wrap gap-4">
                {/* Public buttons */}
                <Button
                  variant="outline"
                  className="flex items-center gap-2"
                  onClick={() => handleContactSeller(listing.id, "car")}
                >
                  <FiPhoneCall size={18} />
                  Contact Seller
                </Button>

                <Button
                  variant="secondary"
                  className="flex items-center gap-2"
                  onClick={() => handleSaveListing(listing.id)}
                >
                  <FiHeart size={18} />
                  Save Listing
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>

        {/* Separate Dealership Info Container */}
        {listing.dealership && (
          <div className="md:w-1/3">
            <Card className="shadow-lg">
              <CardContent className="p-6">
                <h2 className="text-xl font-bold mb-4">Contact Details: </h2>
                <div className="mb-3">
                  <p className="font-semibold">{listing.dealership.fullName}</p>
                </div>
                <div className="flex items-center mb-3">
                  <FiPhoneCall size={18} className="text-blue-500 mr-2" />
                  <p>{listing.dealership.phoneNo}</p>
                </div>
                <div className="flex items-center mb-3">
                  <FiMail size={18} className="text-blue-500 mr-2" />
                  <p>{listing.dealership.email}</p>
                </div>
                {listing.dealership.carDealership && (
                  <>
                    <div className="flex items-center mb-3">
                      <FiMapPin size={18} className="text-red-500 mr-2" />
                      <div>
                        <p className="text-lg">
                          {listing.dealership.carDealership.businessName}
                        </p>
                        <p className="text-lg">
                          {formatShowroomLocations(
                            listing.dealership.carDealership.showroomLocations
                          )}
                        </p>
                      </div>
                    </div>
                    <div className="mb-3">
                      <ul className="list-disc list-inside">
                        {formatFinancingOptions(
                          listing.dealership.carDealership.financingOptions
                        ).map((option, idx) => (
                          <li key={idx} className="text-lg">
                            {option}
                          </li>
                        ))}
                      </ul>
                    </div>
                  </>
                )}
              </CardContent>
            </Card>
          </div>
        )}
      </div>
    </div>
  );
};

export default ViewCarListing;
````

## File: src/app/dashboard/user/homes/house-listings/[id]/page.tsx
````typescript
"use client";

import { useParams, useRouter } from "next/navigation";
import { useEffect, useState } from "react";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

// Swiper (Carousel)
import { Swiper, SwiperSlide } from "swiper/react";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";

// Icons
import {
  FiArrowLeft,
  FiEdit,
  FiTrash2,
  FiPhoneCall,
  FiMail,
  FiMapPin,
  FiCalendar,
  FiClock,
  FiHome,
  FiGlobe,
  FiDollarSign,
  FiHeart,
} from "react-icons/fi";
import { FaBed, FaBath } from "react-icons/fa";

const ViewListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [listing, setListing] = useState<any>(null);
  const [userRole, setUserRole] = useState<string | null>(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Helper: Format dates.
  const formatDate = (dateStr: string) => {
    if (!dateStr) return "N/A";
    return new Date(dateStr).toLocaleDateString();
  };

  const checkIfAnyDateIsFuture = (data) => {
    // Get current UTC time
    const currentTime = new Date();

    // Use Array.some() to stop as soon as a future date is found
    const isFuture = data.some((item) => {
      // Validate if endDate exists and is a valid date
      if (!item.endDate) return false;

      // Convert endDate to a Date object
      const endDateUTC = new Date(item.endDate);

      // Check if endDate is valid and greater than currentTime
      return !isNaN(endDateUTC.getTime()) && endDateUTC > currentTime;
    });

    return isFuture;
  };

  useEffect(() => {
    if (id) {
      const fetchListing = async () => {
        try {
          const endpoint = process.env.NEXT_PUBLIC_API_URL;
          const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
          const tokenData = await tokenResponse.json();
          const token = tokenData?.token;
          const role = tokenData?.role;
          if (!token) {
            throw new Error("Invalid authentication token");
          }
          setUserRole(role);
          const response = await fetch(
            `${endpoint}api/protected/house-listing/houselisting/${id}`,
            {
              headers: { Authorization: `Bearer ${token}` },
            }
          );
          if (!response.ok) {
            throw new Error("Failed to fetch listing");
          }
          const data = await response.json();
          setListing(data);
        } catch (err: any) {
          setError(err.message);
        } finally {
          setLoading(false);
        }
      };

      fetchListing();
    }
  }, [id]);

  const handleDelete = async () => {
    if (confirm("Are you sure you want to delete this listing?")) {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) {
          throw new Error("Invalid authentication token");
        }
        const response = await fetch(
          `${endpoint}api/protected/house-listing/delete-house-listing/${id}`,
          {
            method: "DELETE",
            headers: { Authorization: `Bearer ${token}` },
          }
        );
        if (!response.ok) {
          throw new Error("Failed to delete listing");
        }
        alert("Listing deleted successfully");
        router.push("/dashboard/realtor/house-listings");
      } catch (err: any) {
        alert(`Error deleting listing: ${err.message}`);
      }
    }
  };

  if (loading) {
    return <p className="text-center text-lg text-gray-500">Loading...</p>;
  }

  if (error) {
    return <p className="text-center text-red-500 text-lg">Error: {error}</p>;
  }

  if (!listing) {
    return (
      <p className="text-center text-gray-500 text-lg">No listing found</p>
    );
  }

  const handleContactSeller = async (listingId: number, type: string) => {
    const tokenResponse = await fetch(`${endpoint}auth/token`, {
      credentials: "include",
    });
    if (!tokenResponse.ok) {
      throw new Error("Failed to get authentication token");
    }
    const tokenData = await tokenResponse.json();
    const token = tokenData?.token;
    const response = await fetch(
      `${endpoint}api/protected/appointment/booking-status?listingId=${listingId}&type=${type}`,
      {
        method: "GET",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
      }
    );

    if (response.status === 200) {
      const data = await response.json();
      if (checkIfAnyDateIsFuture(data.booking)) {
        alert("You have already booked an appointment with this seller");
      } else {
        alert("Action Pending from Realtor");
      }
    } else {
      router.push(`/dashboard/user/slots/${listingId}/${type}`);
    }
  };

  const handleSaveListing = async (listingId: number) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData?.token;
      const response = await fetch(
        `${endpoint}api/protected/house-listing/add-to-favourites`,
        {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            Authorization: `Bearer ${token}`,
          },
          body: JSON.stringify({
            listingId: listingId,
          }),
        }
      );

      if (response.status === 200) {
        const data = await response.json();
      }
    } catch (error) {
      console.error("Error saving listing:", error);
      alert("An error occurred while processing your request.");
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      {/* Back Button */}
      <Link href="/dashboard/user/">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>

      <div className="flex flex-col md:flex-row gap-6">
        {/* Left: Main Listing Card */}
        <div className="md:w-2/3">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              {/* Image Carousel */}
              {listing.houseImages && listing.houseImages.length > 0 && (
                <Swiper
                  navigation={true}
                  modules={[Navigation]}
                  className="w-full h-96 rounded-lg shadow-lg mb-6"
                >
                  {listing.houseImages.map((image: any, index: number) => (
                    <SwiperSlide key={index}>
                      <img
                        src={image.base64}
                        alt={`House Image ${index + 1}`}
                        className="w-full h-96 object-cover rounded-lg"
                      />
                    </SwiperSlide>
                  ))}
                </Swiper>
              )}

              {/* Title, Price, and Created At */}
              <div className="mb-4">
                <h1 className="text-3xl font-semibold flex items-center gap-2">
                  {listing.title ?? "Untitled"}
                </h1>
                <p className="text-2xl mt-2 text-blue-600 font-bold flex items-center gap-2">
                  <FiDollarSign size={24} />
                  {listing.price ?? "N/A"}
                </p>
                {listing.createdAt && (
                  <p className="mt-2 text-sm text-gray-500">
                    Created At:{" "}
                    {new Date(listing.createdAt).toLocaleDateString()}
                  </p>
                )}
              </div>

              {/* Description */}
              {listing.description && (
                <p className="mb-4">{listing.description}</p>
              )}

              {/* House Attributes */}
              <div className="grid grid-cols-2 md:grid-cols-4 gap-4 mb-4">
                {listing.bedrooms !== null && (
                  <div className="flex items-center gap-2">
                    <FaBed size={20} />
                    <p className="text-lg font-semibold">
                      {listing.bedrooms} Beds
                    </p>
                  </div>
                )}
                {listing.bathrooms !== null && (
                  <div className="flex items-center gap-2">
                    <FaBath size={20} />
                    <p className="text-lg font-semibold">
                      {listing.bathrooms} Baths
                    </p>
                  </div>
                )}
                {listing.squareFeet && (
                  <div className="flex items-center gap-2">
                    <FiHome size={20} />
                    <p className="text-lg font-semibold">
                      {listing.squareFeet} sq ft
                    </p>
                  </div>
                )}
                {listing.location && (
                  <div className="flex items-center gap-2">
                    <FiMapPin size={40} />
                    <p className="text-sm font-semibold">{listing.location}</p>
                  </div>
                )}
              </div>

              {/* Action Buttons */}
              <div className="mt-6 flex flex-wrap gap-4">
                {/* Public buttons */}
                <Button
                  variant="outline"
                  className="flex items-center gap-2"
                  onClick={() => handleContactSeller(listing.id, "house")}
                >
                  <FiPhoneCall size={18} />
                  Contact Seller
                </Button>

                <Button
                  variant="secondary"
                  className="flex items-center gap-2"
                  onClick={() => handleSaveListing(listing.id)}
                >
                  <FiHeart size={18} />
                  Save Listing
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>

        {/* Right: Landlord / Realtor Info Card */}
        {listing.landlord && (
          <div className="md:w-1/3">
            <Card className="shadow-lg">
              <CardContent className="p-6">
                <h2 className="text-xl font-bold mb-4">Contact</h2>
                {listing.landlord.fullName && (
                  <p className="font-semibold mb-4">
                    {listing.landlord.fullName}
                  </p>
                )}
                {listing.landlord.phoneNo && (
                  <div className="flex items-center gap-2 mb-3">
                    <FiPhoneCall size={18} className="text-blue-500" />
                    <p>{listing.landlord.phoneNo}</p>
                  </div>
                )}
                {listing.landlord.email && (
                  <div className="flex items-center gap-2 mb-3">
                    <FiMail size={18} className="text-blue-500" />
                    <p>{listing.landlord.email}</p>
                  </div>
                )}
                {listing.landlord.realtor && (
                  <>
                    <div className="flex items-center mb-3">
                      <FiMapPin size={18} className="text-red-500 mr-2" />
                      <p>
                        {listing.landlord.realtor.businessName},{" "}
                        {listing.landlord.realtor.businessAddress}
                      </p>
                    </div>
                    <div className="flex items-center mb-3">
                      <FiGlobe size={25} className="mr-2" />
                      <p>{listing.landlord.realtor.portfolioWebsite}</p>
                    </div>
                  </>
                )}
              </CardContent>
            </Card>

            {listing.openhouse && (
              <Card className="shadow-lg mt-2">
                <CardContent className="p-6">
                  <h3 className="text-xl font-semibold mb-2">Open House</h3>
                  <div className="flex items-center gap-2 mb-1">
                    <FiCalendar size={18} />
                    <p className="text-">
                      Start Date: {formatDate(listing.startdate)}
                    </p>
                  </div>
                  <div className="flex items-center gap-2 mb-1">
                    <FiCalendar size={18} />
                    <p>End Date: {formatDate(listing.endDate)}</p>
                  </div>
                  <div className="flex items-center gap-2 mb-1">
                    <FiClock size={18} />
                    <p>Start Time: {listing.startTime ?? "N/A"}</p>
                  </div>
                  <div className="flex items-center gap-2">
                    <FiClock size={18} />
                    <p>End Time: {listing.endTime ?? "N/A"}</p>
                  </div>
                </CardContent>
              </Card>
            )}
          </div>
        )}
      </div>
    </div>
  );
};

export default ViewListing;
````

## File: src/app/dashboard/user/page.tsx
````typescript
"use client";

import QuickLinks from "@/components/QuickLinks";
import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import AIFeaturesPanel from "@/components/ai/AIFeaturesPanel";
import { useEffect, useState } from "react";

export default function DashboardLayout() {
  const [carListings, setCarListings] = useState(null);
  const [houseListings, setHouseListings] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        // Fetch token
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });

        if (!tokenResponse.ok) {
          throw new Error("Failed to get authentication token");
        }

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;

        if (!token) {
          throw new Error("Invalid authentication token");
        }

        // Fetch house listings
        const houseResponse = await fetch(
          `${endpoint}api/protected/house-listing/all-house-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!houseResponse.ok) {
          throw new Error("Failed to fetch house listings");
        }

        const houseData = await houseResponse.json();
        setHouseListings(houseData);

        // Fetch car listings
        const carResponse = await fetch(
          `${endpoint}api/protected/car-listing/all-car-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!carResponse.ok) {
          throw new Error("Failed to fetch car listings");
        }

        const carData = await carResponse.json();
        setCarListings(carData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  const services = [
    "Dashboard",
    "AI Assistant",
    "Explore Homes",
    "Explore Cars",
    "Book Consultation",
    "Bookings",
  ];
  const urls = [
    "/dashboard/user",
    "/dashboard/user/ai",
    "/dashboard/user/homes",
    "/dashboard/user/cars",
    "/dashboard/user/consultant",
    "/dashboard/user/bookings",
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      {" "}
      {/* h-screen for full viewport height */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        {" "}
        {/* Fixed SideCard */}
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">User Dashboard</h2>
          <QuickLinks
            links={[
              { label: "AI Assistant", href: "/dashboard/user/ai" },
              { label: "Profile Settings", href: "/dashboard/user/profile" },
              { label: "Saved Listings", href: "/dashboard/user/saved" },
              { label: "Booking History", href: "/dashboard/user/bookings" },
            ]}
          />
          
          {/* AI Features Section */}
          <div className="mb-8">
            <AIFeaturesPanel />
          </div>
          <h2 className="text-2xl font-bold mb-6 mt-4">
            Explore recent home listings
          </h2>
          {loading && <p>Loading...</p>}
          {error && <p>Error: {error}</p>}
          {!loading && !error && houseListings && (
            <Listings listings={houseListings} />
          )}
          <h2 className="text-2xl font-bold mb-6 mt-4">
            Explore recent car listings
          </h2>
          {!loading && !error && carListings && (
            <Listings listings={carListings} />
          )}
        </div>
      </div>
    </div>
  );
}
````

## File: src/app/layout.tsx
````typescript
import type { Metadata } from "next";
import { Poppins } from "next/font/google";
import "./globals.css";
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
  title: "ImmiGrow",
  description: "ImmiGrow",
  icons: {
    icon: "/logo.png",
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
````

## File: src/app/page.tsx
````typescript
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import { Button } from "@/components/ui/button";
import {
  Card,
  CardContent,
  CardDescription,
  CardHeader,
  CardTitle,
} from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import {
  ArrowRight,
  Building,
  Car,
  CheckCircle,
  ChevronRight,
  Globe,
  GraduationCap,
  Home,
  MessageSquare,
  Star,
  Users,
} from "lucide-react";
import Image from "next/image";
import Link from "next/link";

export default function LandingPage() {
  return (
    <div className="flex flex-col min-h-screen min-w-full  bg-background">
      {/* Header */}
      <Header />
      <main className="flex-1">
        {/* Hero Section */}
        <section className="relative overflow-hidden bg-white py-20 md:py-12">
          <div className="absolute inset-0 bg-gradient-to-br from-blue-50 to-white z-0"></div>
          <div className="container relative z-10 mx-auto">
            <div className="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
              <div className="flex m-3 flex-col gap-6">
                <h1 className="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight">
                  Your New Life{" "}
                  <span className="text-blue-500">Starts Here</span>
                </h1>
                <p className="text-xl text-gray-600">
                  AI-powered help for housing, cars, and immigration support —
                  all in one place.
                </p>
                <div className="flex flex-col sm:flex-row gap-4 mt-4">
                  <Link href={"/signup"}>
                    <Button size="lg" className="bg-blue-500 hover:bg-blue-600">
                      Start Planning
                      <ArrowRight className="ml-2 h-4 w-4" />
                    </Button>
                  </Link>
                  <Link href="#how-it-works">
                    <Button size="lg" variant="outline">
                      How It Works
                    </Button>
                  </Link>
                </div>
              </div>
              <div className="relative h-[600px] w-full ">
                <Image
                  src="/landing-1.png"
                  alt="ImmiGrow Hero Image"
                  fill
                  // className="object-cover"
                  priority
                />
                {/* <div className="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent"></div> */}
              </div>
            </div>
          </div>
        </section>

        {/* Platform Overview */}
        <section id="about" className="py-20 bg-white">
          <div className="container mx-auto">
            <div className="text-center mb-16">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                All-in-One Platform for New Immigrants
              </h2>
              <p className="text-xl text-gray-600 max-w-3xl mx-auto">
                Everything you need to start your new life in one place, powered
                by AI.
              </p>
            </div>

            <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
              <Card className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full">
                <CardHeader className="pb-2">
                  <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mb-4">
                    <Home className="h-6 w-6 text-blue-500" />
                  </div>
                  <CardTitle>Housing</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-base">
                    Verified rentals across top cities with virtual tours and
                    trusted landlords.
                  </CardDescription>
                </CardContent>
              </Card>

              <Card className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full">
                <CardHeader className="pb-2">
                  <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mb-4">
                    <Car className="h-6 w-6 text-blue-500" />
                  </div>
                  <CardTitle>Cars</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-base">
                    New & used cars with insurance options tailored for
                    newcomers.
                  </CardDescription>
                </CardContent>
              </Card>

              <Card className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full">
                <CardHeader className="pb-2">
                  <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mb-4">
                    <MessageSquare className="h-6 w-6 text-blue-500" />
                  </div>
                  <CardTitle>Consultants</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-base">
                    Trusted immigration consultants with verified credentials
                    and reviews.
                  </CardDescription>
                </CardContent>
              </Card>

              <Card className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full">
                <CardHeader className="pb-2">
                  <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mb-4">
                    <Globe className="h-6 w-6 text-blue-500" />
                  </div>
                  <CardTitle>Smart Planner</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-base">
                    AI-powered immigration guidance customized to your unique
                    situation.
                  </CardDescription>
                </CardContent>
              </Card>
            </div>
          </div>
        </section>

        {/* How It Works */}
        <section id="how-it-works" className="py-20 bg-gray-50">
          <div className="container mx-auto">
            <div className="text-center mb-16">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                How ImmiGrow Works
              </h2>
              <p className="text-xl text-gray-600 max-w-3xl mx-auto">
                Our AI-powered platform simplifies your immigration journey in
                three easy steps.
              </p>
            </div>

            <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
              {[
                {
                  number: "01",
                  title: "Tell Us About Your Move",
                  description:
                    "Where, when, and why you're immigrating. We'll customize everything to your needs.",
                  icon: Globe,
                },
                {
                  number: "02",
                  title: "Get Smart Matches Instantly",
                  description:
                    "AI finds you the right homes, cars, and consultants based on your preferences.",
                  icon: CheckCircle,
                },
                {
                  number: "03",
                  title: "Connect, Book, and Arrive Ready",
                  description:
                    "No stress. No scams. Just a smooth transition to your new home.",
                  icon: Home,
                },
              ].map((step, index) => (
                <div
                  key={index}
                  className="relative flex flex-col items-center text-center p-6"
                >
                  <div className="w-16 h-16 rounded-full bg-blue-500 text-white flex items-center justify-center text-2xl font-bold mb-6">
                    {step.number}
                  </div>
                  <h3 className="text-xl font-bold mb-3">{step.title}</h3>
                  <p className="text-gray-600">{step.description}</p>

                  {index < 2 && (
                    <div className="hidden md:block absolute top-1/4 right-0 transform translate-x-1/2">
                      <ChevronRight className="h-8 w-8 text-blue-300" />
                    </div>
                  )}
                </div>
              ))}
            </div>
          </div>
        </section>

        {/* Who It's For */}
        <section id="who-its-for" className="py-20 bg-white">
          <div className="container mx-auto">
            <div className="text-center mb-16">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                Built for Every Immigrant Journey
              </h2>
              <p className="text-xl text-gray-600 max-w-3xl mx-auto">
                No matter your situation, ImmiGrow has the tools and resources
                you need.
              </p>
            </div>

            <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
              {[
                {
                  title: "International Students",
                  description:
                    "Find student housing, affordable cars, and visa support.",
                  icon: GraduationCap,
                  color: "bg-blue-100",
                },
                {
                  title: "Skilled Workers",
                  description:
                    "Professional relocation support for you and your family.",
                  icon: Building,
                  color: "bg-purple-100",
                },
                {
                  title: "Families",
                  description:
                    "Family-friendly homes, safe vehicles, and community connections.",
                  icon: Users,
                  color: "bg-orange-100",
                },
                {
                  title: "Realtors & Car Dealers",
                  description:
                    "Connect with newcomers looking for your services.",
                  icon: Home,
                  color: "bg-blue-100",
                },
              ].map((segment, index) => (
                <Card
                  key={index}
                  className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full"
                >
                  <CardHeader className="pb-2">
                    <div
                      className={`w-12 h-12 rounded-full ${segment.color} flex items-center justify-center mb-4`}
                    >
                      <segment.icon className="h-6 w-6 text-blue-500" />
                    </div>
                    <CardTitle>{segment.title}</CardTitle>
                  </CardHeader>
                  <CardContent className="space-y-4">
                    <CardDescription className="text-base">
                      {segment.description}
                    </CardDescription>
                    <Button
                      variant="outline"
                      size="sm"
                      className="text-blue-500 border-blue-500 hover:bg-blue-50"
                    >
                      Get Started
                    </Button>
                  </CardContent>
                </Card>
              ))}
            </div>
          </div>
        </section>

        {/* Testimonials */}
        <section id="testimonials" className="py-20 bg-gray-50">
          <div className="container mx-auto">
            <div className="text-center mb-16">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                Trusted by Thousands Worldwide
              </h2>
              <p className="text-xl text-gray-600 max-w-3xl mx-auto">
                Hear from people who&apos;ve successfully started their new
                lives with ImmiGrow.
              </p>
            </div>

            <div className="grid grid-cols-1 md:grid-cols-3 gap-8 mb-12">
              {[
                {
                  name: "Sarah Chen",
                  location: "From China to Canada",
                  quote:
                    "ImmiGrow helped me find a perfect apartment and a reliable car within days of arriving. The consultant they matched me with made my visa process so much easier.",
                  rating: 5,
                },
                {
                  name: "Miguel Rodriguez",
                  location: "From Mexico to USA",
                  quote:
                    "As a student, I was worried about finding affordable housing. ImmiGrow not only found me a great place but also connected me with other students from my country.",
                  rating: 5,
                },
                {
                  name: "Priya Sharma",
                  location: "From India to Australia",
                  quote:
                    "Moving with my family was stressful until we found ImmiGrow. Their AI recommendations were spot-on for our needs, and we felt at home right away.",
                  rating: 4,
                },
              ].map((testimonial, index) => (
                <Card key={index} className="border-none shadow-lg h-full">
                  <CardContent className="pt-6">
                    <div className="flex items-center mb-4">
                      {Array(testimonial.rating)
                        .fill(0)
                        .map((_, i) => (
                          <Star
                            key={i}
                            className="h-5 w-5 fill-yellow-400 text-yellow-400"
                          />
                        ))}
                    </div>
                    <p className="text-gray-700 mb-6 italic">
                      {testimonial.quote}
                    </p>
                    <div className="flex items-center gap-4">
                      <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center">
                        <span className="text-blue-500 font-bold">
                          {testimonial.name
                            .split(" ")
                            .map((n) => n[0])
                            .join("")}
                        </span>
                      </div>
                      <div>
                        <p className="font-medium">{testimonial.name}</p>
                        <p className="text-sm text-gray-500">
                          {testimonial.location}
                        </p>
                      </div>
                    </div>
                  </CardContent>
                </Card>
              ))}
            </div>

            <div className="flex justify-center gap-12 flex-wrap">
              <div className="text-center">
                <p className="text-4xl font-bold text-blue-500">5,000+</p>
                <p className="text-gray-600">Users Onboarded</p>
              </div>
              <div className="text-center">
                <p className="text-4xl font-bold text-blue-500">12+</p>
                <p className="text-gray-600">Countries Served</p>
              </div>
              <div className="text-center">
                <p className="text-4xl font-bold text-blue-500">4.9/5</p>
                <p className="text-gray-600">Average Rating</p>
              </div>
            </div>
          </div>
        </section>

        {/* CTA Banner */}
        <section className="py-16 bg-blue-500 text-white">
          <div className="container mx-auto">
            <div className="max-w-4xl mx-auto text-center">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                Let&apos;s Plan Your Move - Together
              </h2>
              <p className="text-xl mb-8">
                Takes less than 2 minutes to get matched with the perfect
                housing, transportation, and support.
              </p>
              <Link href={"/signup"}>
                <Button
                  size="lg"
                  className="bg-white text-blue-500 hover:bg-gray-100"
                >
                  Start Now — It&apos;s Free
                  <ArrowRight className="ml-2 h-4 w-4" />
                </Button>
              </Link>
            </div>
          </div>
        </section>

        {/* Contact Form */}
        <section id="contact" className="py-20 m-4 bg-white">
          <div className="container mx-auto">
            <div className="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
              <div>
                <h2 className="text-3xl md:text-4xl font-bold mb-4">
                  Have Questions? Reach Out!
                </h2>
                <p className="text-xl text-gray-600 mb-8">
                  Our team is here to help you with any questions about your
                  immigration journey.
                </p>

                <form className="space-y-6">
                  <div className="space-y-2">
                    <label htmlFor="name" className="text-sm font-medium">
                      Name
                    </label>
                    <Input id="name" placeholder="Your name" />
                  </div>

                  <div className="space-y-2">
                    <label htmlFor="email" className="text-sm font-medium">
                      Email
                    </label>
                    <Input
                      id="email"
                      type="email"
                      placeholder="your.email@example.com"
                    />
                  </div>

                  <div className="space-y-2">
                    <label htmlFor="message" className="text-sm font-medium">
                      Message
                    </label>
                    <Textarea
                      id="message"
                      placeholder="How can we help you?"
                      rows={4}
                    />
                  </div>

                  <Button className="w-full bg-blue-500 hover:bg-blue-600">
                    Send Message
                  </Button>
                </form>
              </div>

              <div className="relative h-[500px] w-full ">
                <Image
                  src="/landing-2.jpg"
                  alt="Contact ImmiGrow"
                  fill
                  className="object-cover"
                />
                {/* <div className="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent"></div> */}
              </div>
            </div>
          </div>
        </section>
      </main>
      {/* Footer */}
      <Footer />
    </div>
  );
}
````

## File: src/components/ai/AIFeaturesPanel.tsx
````typescript
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
      route: '/dashboard/user/ai/resume'
    },
    {
      id: 'profile',
      title: 'Career Profile Generator',
      description: 'Generate tailored career profiles with position recommendations',
      icon: '🎯',
      color: 'border-green-200 bg-green-50',
      benefits: ['Position recommendations', 'Success probability analysis', 'Enhanced profile generation'],
      route: '/dashboard/user/ai/career-profile'
    },
    {
      id: 'mentors',
      title: 'Find Mentors',
      description: 'AI-powered mentor matching',
      icon: '👥',
      color: 'border-purple-200 bg-purple-50',
      benefits: ['Industry experts', 'Cultural guidance', 'Career advice'],
      route: '/dashboard/user/ai/mentors'
    },
    {
      id: 'coaching',
      title: 'AI Career Coach',
      description: 'Personalized career guidance',
      icon: '💬',
      color: 'border-orange-200 bg-orange-50',
      benefits: ['Interview prep', 'Skill development', 'Networking tips'],
      route: '/dashboard/user/ai/coaching'
    },
    {
      id: 'jobs',
      title: 'Job Discovery',
      description: 'Find matching job opportunities',
      icon: '🔍',
      color: 'border-cyan-200 bg-cyan-50',
      benefits: ['Smart matching', 'Compatibility scores', 'Job alerts'],
      route: '/dashboard/user/ai/jobs'
    },
    {
      id: 'skills',
      title: 'Skill Gap Analysis',
      description: 'Identify and bridge skill gaps',
      icon: '📈',
      color: 'border-yellow-200 bg-yellow-50',
      benefits: ['Gap identification', 'Learning path', 'Progress tracking'],
      route: '/dashboard/user/ai/skills'
    }
  ];

  const toggleCard = (id) => {
    setExpandedCard(expandedCard === id ? null : id);
  };

  return (
    <div className="space-y-6">
      <div className="text-center space-y-3">
        <h2 className="text-3xl font-bold text-gray-900 flex items-center justify-center gap-2">
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
                      {feature.id === 'profile' || feature.id === 'resume' ? 'Available' : 'Coming Soon'}
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
                    disabled={feature.id !== 'profile' && feature.id !== 'resume'}
                    onClick={(e) => {
                      e.stopPropagation();
                      if (feature.id === 'profile' || feature.id === 'resume') {
                        window.location.href = feature.route;
                      }
                    }}
                  >
                    {feature.id === 'profile' || feature.id === 'resume' ? 'Get Started' : 'Coming Soon'}
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
            onClick={() => window.location.href = '/dashboard/user/ai/resume'}
            className="bg-blue-600 hover:bg-blue-700"
          >
            Upload Resume
          </Button>
          <Button 
            onClick={() => window.location.href = '/dashboard/user/ai/career-profile'}
            className="bg-green-600 hover:bg-green-700"
          >
            Career Profile
          </Button>
          <Button 
            variant="outline" 
            disabled
            className="border-blue-600 text-blue-600"
          >
            More Features Coming Soon
          </Button>
        </div>
      </div>
    </div>
  );
};

export default AIFeaturesPanel;
````

## File: src/components/availability/AppointmentBooking.tsx
````typescript
import { useState, useEffect } from "react";
import { Button } from "@/components/ui/button";
import { CalendarClock, Clock, CheckCircle } from "lucide-react";

interface Availability {
  id: string;
  startTime: string;
  endTime: string;
  status: string;
}

interface AppointmentBookingProps {
  listingId: string;
  type: "car" | "house" | "consultant";
}

const AppointmentBooking: React.FC<AppointmentBookingProps> = ({
  listingId,
  type,
}) => {
  const [availability, setAvailability] = useState<Availability[]>([]);
  const [loading, setLoading] = useState(false);
  const [selectedSlot, setSelectedSlot] = useState<string | null>(null);
  const [error, setError] = useState("");
  const [authToken, setAuthToken] = useState<string | null>(null);
  const [isAppointmentBooked, setIsAppointmentBooked] = useState<string | null>(
    null
  );

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // ✅ Convert UTC to User's Timezone for Display
  const formatToUserTimezone = (utcDate: string) => {
    return new Intl.DateTimeFormat("en-US", {
      year: "numeric",
      month: "2-digit",
      day: "2-digit",
      hour: "2-digit",
      minute: "2-digit",
      hour12: true,
    }).format(new Date(utcDate));
  };

  // ✅ Fetch Authentication Token Once
  useEffect(() => {
    const fetchToken = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        setAuthToken(tokenData.token);
      } catch (error) {
        setError("Authentication error. Please try again.");
      }
    };

    fetchToken();
  }, []);

  // ✅ Fetch Availability Slots
  const fetchAvailability = async () => {
    if (!authToken) return;

    setLoading(true);
    setError("");

    if (type === "consultant") {
      try {
        const response = await fetch(
          `${endpoint}api/protected/availability/consultant-availability/${listingId}`,
          {
            method: "GET",
            headers: { Authorization: `Bearer ${authToken}` },
          }
        );

        if (!response.ok) throw new Error("Failed to fetch availability");

        const data: Availability[] = await response.json();
        setAvailability(data);
      } catch (error) {
        setError("Error fetching availability. Please try again.");
      } finally {
        setLoading(false);
      }
    } else {
      try {
        const response = await fetch(
          `${endpoint}api/protected/availability/express-interest?type=${type}&listingId=${listingId}`,
          {
            method: "GET",
            headers: { Authorization: `Bearer ${authToken}` },
          }
        );

        if (!response.ok) throw new Error("Failed to fetch availability");

        const data: Availability[] = await response.json();
        setAvailability(data);
      } catch (error) {
        setError("Error fetching availability. Please try again.");
      } finally {
        setLoading(false);
      }
    }
  };

  useEffect(() => {
    if (authToken) fetchAvailability();
  }, [authToken, listingId, type]);

  // ✅ Handle Booking Appointment
  const handleBookAppointment = async (
    availabilityId: string,
    listingId: string
  ) => {
    if (!authToken) return;

    try {
      setSelectedSlot(availabilityId);

      const response = await fetch(
        `${endpoint}api/protected/appointment/schedule`,
        {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            Authorization: `Bearer ${authToken}`,
          },
          body: JSON.stringify({
            listingId: parseInt(listingId),
            availabilityId: parseInt(availabilityId),
          }),
        }
      );

      const data = await response.json();

      if (
        data.error ===
        "Google Calendar access required. Please connect your Google account."
      ) {
        alert("Google Calendar access required. Redirecting...");
        window.open(data.connectUrl, "_blank"); // Open Google OAuth link
      } else if (data.appointment) {
        alert("✅ Appointment Scheduled! Check your Google Calendar.");
        setIsAppointmentBooked(availabilityId);
      } else {
        alert("Failed to schedule appointment.");
      }
    } catch (error) {
      console.error("Error scheduling appointment:", error);
      alert("Error scheduling event.");
    }
  };

  return (
    <div className="mx-auto p-6">
      {loading ? (
        <p className="text-center text-gray-600">Loading...</p>
      ) : error ? (
        <p className="text-red-500 text-center">{error}</p>
      ) : availability.length === 0 ? (
        <p className="text-gray-500 text-center">
          No available slots at the moment.
        </p>
      ) : (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {availability.map((slot) => (
            <div
              key={slot.id}
              className={`p-5 border rounded-lg shadow-md flex flex-col ${
                selectedSlot === slot.id ? "bg-blue-100" : "bg-white"
              } transition-transform hover:scale-105`}
            >
              <div className="flex items-center space-x-3 mb-3">
                <CalendarClock className="w-6 h-6 text-gray-600" />
                <h3 className="text-lg font-semibold text-gray-800">
                  Time Slot
                </h3>
              </div>

              <div className="bg-gray-100 p-4 rounded-lg mb-3">
                <div className="flex items-center space-x-2">
                  <Clock className="w-5 h-5 text-blue-600" />
                  <p className="text-gray-900 font-semibold">Start:</p>
                  <p className="text-gray-700">
                    {formatToUserTimezone(slot.startTime)}
                  </p>
                </div>
                <div className="flex items-center space-x-2 mt-2">
                  <Clock className="w-5 h-5 text-red-600" />
                  <p className="text-gray-900 font-semibold">End:</p>
                  <p className="text-gray-700">
                    {formatToUserTimezone(slot.endTime)}
                  </p>
                </div>
              </div>

              <Button
                className="bg-blue-600 hover:bg-blue-500 text-white px-4 py-2 rounded-lg flex items-center justify-center"
                onClick={() => handleBookAppointment(slot.id, listingId)}
                disabled={isAppointmentBooked === slot.id}
              >
                {isAppointmentBooked === slot.id ? (
                  <>
                    <CheckCircle className="w-5 h-5 mr-2" />
                    Appointment Booked
                  </>
                ) : (
                  "Book Appointment"
                )}
              </Button>
            </div>
          ))}
        </div>
      )}
    </div>
  );
};

export default AppointmentBooking;
````

## File: src/components/availability/AvailabilityForm.tsx
````typescript
import { useState, useEffect } from "react";
import { Button } from "@/components/ui/button";

interface AvailabilityFormProps {
  initialData?: { id: string; startTime: string; endTime: string };
  refreshSlots: () => void;
  onClose: () => void;
}

const AvailabilityForm: React.FC<AvailabilityFormProps> = ({
  initialData,
  refreshSlots,
  onClose,
}) => {
  const [formData, setFormData] = useState({
    startTime: "",
    endTime: "",
  });

  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // **UseEffect to load initial data properly when editing**
  useEffect(() => {
    if (initialData) {
      setFormData({
        startTime: initialData.startTime || "",
        endTime: initialData.endTime || "",
      });
    }
  }, [initialData]); // ✅ Triggers when initialData changes

  const handleChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    setFormData((prev) => ({
      ...prev,
      [e.target.name]: e.target.value,
    }));
  };

  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();

    if (!formData.startTime || !formData.endTime) {
      setError("Both start time and end time are required.");
      return;
    }

    const start = new Date(formData.startTime);
    const end = new Date(formData.endTime);

    if (start >= end) {
      setError("Start time must be before end time.");
      return;
    }

    const duration = (end.getTime() - start.getTime()) / (1000 * 60); // Duration in minutes

    if (duration > 60) {
      setError("Slots cannot be longer than 1 hour.");
      return;
    }

    setError("");
    setLoading(true);

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const url = initialData
        ? `${endpoint}api/protected/availability/update/${initialData.id}`
        : `${endpoint}api/protected/availability/add`;
      const method = initialData ? "PUT" : "POST";

      const response = await fetch(url, {
        method,
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
        body: JSON.stringify({
          startTime: formData.startTime,
          endTime: formData.endTime,
          status: "Available",
        }),
      });

      if (!response.ok) throw new Error("Failed to save availability");

      refreshSlots(); // Refresh the slots list
      onClose(); // Close form
    } catch (error) {
      setError("Error saving availability. Please try again." + error);
    } finally {
      setLoading(false);
    }
  };

  return (
    <div className="max-w-md mx-auto p-6 border rounded-lg shadow-lg mb-4 ">
      <h2 className="text-2xl font-semibold text-gray-800 mb-4">
        {initialData ? "Edit Availability" : "Add Availability"}
      </h2>

      {error && <p className="text-red-500  p-2 rounded mb-2">{error}</p>}

      <form onSubmit={handleSubmit} className="space-y-4">
        <div>
          <label className="block text-sm font-medium text-gray-700">
            Start Time
          </label>
          <input
            type="datetime-local"
            name="startTime"
            value={formData.startTime}
            onChange={handleChange}
            className="w-full p-2 border rounded-md focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
            required
          />
        </div>

        <div>
          <label className="block text-sm font-medium text-gray-700">
            End Time
          </label>
          <input
            type="datetime-local"
            name="endTime"
            value={formData.endTime}
            onChange={handleChange}
            className="w-full p-2 border rounded-md focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
            required
          />
        </div>

        <div className="flex justify-between">
          <Button
            type="submit"
            className="bg-blue-600 hover:bg-blue-500"
            disabled={loading}
          >
            {loading ? "Saving..." : initialData ? "Update" : "Submit"}
          </Button>
          <Button
            className="bg-gray-400 hover:bg-gray-300"
            onClick={onClose}
            disabled={loading}
          >
            Cancel
          </Button>
        </div>
      </form>
    </div>
  );
};

export default AvailabilityForm;
````

## File: src/components/availability/AvailabilityPage.tsx
````typescript
import { useState, useEffect } from "react";
import { Button } from "@/components/ui/button";
import { Pencil, Trash, Plus, CalendarClock, Clock } from "lucide-react";
import AvailabilityForm from "./AvailabilityForm";

interface Availability {
  id: string;
  startTime: string;
  endTime: string;
}

const AvailabilityPage: React.FC = () => {
  const [slots, setSlots] = useState<Availability[]>([]);
  const [showForm, setShowForm] = useState(false);
  const [editSlot, setEditSlot] = useState<Availability | null>(null);
  const [loading, setLoading] = useState(false);

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const fetchSlots = async () => {
    setLoading(true);
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;
      const response = await fetch(
        `${endpoint}api/protected/availability/byId`,
        {
          method: "GET",
          headers: { Authorization: `Bearer ${token}` },
        }
      );

      if (!response.ok) throw new Error("Failed to fetch slots");

      const data: Availability[] = await response.json();

      if (data.length == 0) {
        setSlots([]);
      } else {
        setSlots(data);
      }
    } catch (error) {
      console.error(error);
    } finally {
      setLoading(false);
    }
  };

  useEffect(() => {
    fetchSlots();
  }, []);

  const handleDelete = async (id: string) => {
    if (!confirm("Are you sure you want to delete this slot?")) return;

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;
      const response = await fetch(
        `${endpoint}api/protected/availability/delete/${id}`,
        {
          method: "DELETE",
          headers: {
            Authorization: `Bearer ${token}`,
          },
        }
      );
      if (!response.ok) throw new Error("Failed to delete");

      setSlots(slots.filter((slot) => slot.id !== id));
    } catch (error) {
      console.error(error);
    }
  };
  const formatToDateTimeLocal = (utcDate: string) => {
    if (!utcDate) return "";

    const date = new Date(utcDate);

    // Get user's local time components
    const year = date.getFullYear();
    const month = String(date.getMonth() + 1).padStart(2, "0"); // Months are 0-based
    const day = String(date.getDate()).padStart(2, "0");
    const hours = String(date.getHours()).padStart(2, "0");
    const minutes = String(date.getMinutes()).padStart(2, "0");

    return `${year}-${month}-${day}T${hours}:${minutes}`; // Format: "YYYY-MM-DDTHH:MM"
  };

  const handleEdit = (slot: Availability) => {
    const slotLocal = { ...slot };
    slotLocal.startTime = formatToDateTimeLocal(slot.startTime);
    slotLocal.endTime = formatToDateTimeLocal(slot.endTime);

    setEditSlot(slotLocal);
    setShowForm(true);
  };

  return (
    <div className=" mx-auto p-6">
      <div className="flex justify-between items-center mb-6">
        <h2 className="text-2xl font-bold mb-6 mt-4">Availability Slots</h2>
        <Button
          className="bg-blue-600 hover:bg-blue-500 flex items-center px-4 py-2 text-white font-medium rounded-lg shadow-md"
          onClick={() => {
            setShowForm(true);
            setEditSlot(null);
          }}
        >
          <Plus className="w-5 h-5 mr-2" /> Add Slots
        </Button>
      </div>

      {showForm && (
        <AvailabilityForm
          initialData={editSlot}
          refreshSlots={fetchSlots}
          onClose={() => setShowForm(false)}
        />
      )}

      {loading ? (
        <p className="text-center text-gray-600">Loading...</p>
      ) : slots.length === 0 ? (
        <p className="text-gray-500 text-center">No slots added yet.</p>
      ) : (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {slots.map((slot) => (
            <div
              key={slot.id}
              className="p-5 border border-gray-200 rounded-xl shadow-md bg-white flex flex-col transition-transform hover:scale-105 hover:shadow-lg"
            >
              <div className="flex items-center space-x-3 mb-2">
                <CalendarClock className="w-6 h-6 text-gray-600" />
                <h3 className="text-lg font-semibold text-gray-800">
                  Availability Slot
                </h3>
              </div>

              <div className="bg-gray-100 p-4 rounded-lg mb-3 flex flex-col">
                <div className="flex items-center space-x-2">
                  <Clock className="w-5 h-5 text-blue-600" />
                  <p className="text-gray-900 font-semibold">Start:</p>
                  <p className="text-gray-700">
                    {slot.startTime
                      ? new Date(slot.startTime).toLocaleString()
                      : "Invalid Date"}
                  </p>
                </div>
                <div className="flex items-center space-x-2 mt-2">
                  <Clock className="w-5 h-5 text-red-600" />
                  <p className="text-gray-900 font-semibold">End:</p>
                  <p className="text-gray-700">
                    {" "}
                    {slot.endTime
                      ? new Date(slot.endTime).toLocaleString()
                      : "Invalid Date"}
                  </p>
                </div>
              </div>

              <div className="flex justify-between items-center">
                <span className="text-blue-600 font-semibold bg-blue-100 px-3 py-1 rounded-full text-sm">
                  ✅ Available
                </span>
                <div className="flex gap-2">
                  <Button
                    className="bg-blue-500 hover:bg-blue-400 p-2 rounded-lg"
                    size="icon"
                    onClick={() => handleEdit(slot)}
                  >
                    <Pencil className="w-5 h-5 text-white" />
                  </Button>
                  <Button
                    className="bg-red-500 hover:bg-red-400 p-2 rounded-lg"
                    size="icon"
                    onClick={() => handleDelete(slot.id)}
                  >
                    <Trash className="w-5 h-5 text-white" />
                  </Button>
                </div>
              </div>
            </div>
          ))}
        </div>
      )}
    </div>
  );
};

export default AvailabilityPage;
````

## File: src/components/availability/BookingTable.tsx
````typescript
import React, { useEffect, useState } from "react";
import { Button } from "@/components/ui/button";
import {
  Dialog,
  DialogContent,
  DialogHeader,
  DialogTitle,
  DialogClose,
} from "@/components/ui/dialog";

interface Booking {
  id: number;
  userId: number;
  listingId: number;
  startDate: string;
  endDate: string;
  status: string;
  meetLink?: string;
  createdAt: string;
  listing?: {
    id: number;
    title?: string;
    price?: string;
    location?: string;
    make?: string;
    model?: string;
    year?: number;
  };
}

interface User {
  id: number;
  fullName: string;
  email: string;
  phoneNo: string;
  role: string;
}

const BookingTable = () => {
  const [houseBookings, setHouseBookings] = useState<Booking[]>([]);
  const [carBookings, setCarBookings] = useState<Booking[]>([]);
  const [icBookings, setIcBookings] = useState<Booking[]>([]);
  const [loading, setLoading] = useState(true);
  const [modalData, setModalData] = useState<{
    type: "user" | "listing";
    data: any;
  } | null>(null);
  let id = 1;

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  useEffect(() => {
    const fetchBookings = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;

        const response = await fetch(
          `${endpoint}api/protected/appointment/user-info`,
          {
            method: "GET",
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        const data = await response.json();
        if (data.success) {
          setHouseBookings(data.houseBookings || []);
          setCarBookings(data.carBookings || []);
          setIcBookings(data.icBookings || []);
          id = 1;
        }
      } catch (error) {
        console.error("Error fetching bookings:", error);
      } finally {
        setLoading(false);
      }
    };

    fetchBookings();
  }, []);

  const markAsComplete = async (
    id: number,
    type: "house" | "car" | "consultant"
  ) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;
      const res = await fetch(`${endpoint}api/protected/appointment/complete`, {
        method: "PUT",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
        body: JSON.stringify({ id, type }),
      });

      if (res.ok) {
        id = 1;
        window.location.reload();
      }
    } catch (error) {
      console.error("Error updating booking status:", error);
    }
  };

  if (loading) return <p>Loading...</p>;

  return (
    <div className="p-4">
      <h2 className="text-xl font-semibold mb-4">Booking Details</h2>

      {/* House Bookings */}

      {houseBookings.length > 0 && (
        <div>
          <table className="w-full border-collapse border border-gray-300">
            <thead>
              <tr className="bg-gray-100">
                <th className="border p-2">ID</th>
                <th className="border p-2">User</th>
                <th className="border p-2">Listing</th>
                <th className="border p-2">Start Date</th>
                <th className="border p-2">End Date</th>
                <th className="border p-2">Status</th>
                <th className="border p-2">Actions</th>
              </tr>
            </thead>
            <tbody>
              {houseBookings.map((booking) => (
                <tr key={booking.id} className="border">
                  <td className="border p-2 text-center">{id++}</td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "user", data: booking.user })
                      }
                    >
                      View User
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "listing", data: booking.listing })
                      }
                    >
                      View Listing
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.startDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.endDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">{booking.status}</td>
                  <td className="border p-2 text-center">
                    {booking.status !== "completed" && (
                      <Button
                        onClick={() => markAsComplete(booking.id, "house")}
                        className="bg-blue-600 hover:bg-blue-500"
                      >
                        Mark as Complete
                      </Button>
                    )}
                  </td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      )}
      {carBookings.length > 0 && (
        <div>
          <table className="w-full border-collapse border border-gray-300">
            <thead>
              <tr className="bg-gray-100">
                <th className="border p-2">ID</th>
                <th className="border p-2">User</th>
                <th className="border p-2">Listing</th>
                <th className="border p-2">Start Date</th>
                <th className="border p-2">End Date</th>
                <th className="border p-2">Status</th>
                <th className="border p-2">Actions</th>
              </tr>
            </thead>
            <tbody>
              {carBookings.map((booking) => (
                <tr key={booking.id} className="border">
                  <td className="border p-2 text-center">{id++}</td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "user", data: booking.user })
                      }
                    >
                      View User
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "listing", data: booking.listing })
                      }
                    >
                      View Listing
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.startDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.endDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">{booking.status}</td>
                  <td className="border p-2 text-center">
                    {booking.status !== "completed" && (
                      <Button
                        onClick={() => markAsComplete(booking.id, "car")}
                        className="bg-blue-600 hover:bg-blue-500"
                      >
                        Mark as Complete
                      </Button>
                    )}
                  </td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      )}

      {icBookings.length > 0 && (
        <div>
          <table className="w-full border-collapse border border-gray-300">
            <thead>
              <tr className="bg-gray-100">
                <th className="border p-2">ID</th>
                <th className="border p-2">User</th>
                <th className="border p-2">Start Date</th>
                <th className="border p-2">End Date</th>
                <th className="border p-2">Status</th>
                <th className="border p-2">Actions</th>
              </tr>
            </thead>
            <tbody>
              {icBookings.map((booking) => (
                <tr key={booking.id} className="border">
                  <td className="border p-2 text-center">{id++}</td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "user", data: booking.user })
                      }
                    >
                      View User
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.startDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.endDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">{booking.status}</td>
                  <td className="border p-2 text-center">
                    {booking.status !== "completed" && (
                      <Button
                        onClick={() => markAsComplete(booking.id, "consultant")}
                        className="bg-blue-600 hover:bg-blue-500"
                      >
                        Mark as Complete
                      </Button>
                    )}
                  </td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      )}
      {houseBookings.length === 0 &&
        carBookings.length === 0 &&
        icBookings.length === 0 && (
          <div className="text-center p-4">No bookings found</div>
        )}
      {/* Modal for viewing details */}
      {modalData && (
        <Dialog open={!!modalData} onOpenChange={() => setModalData(null)}>
          <DialogContent>
            <DialogHeader>
              <DialogTitle>
                {modalData.type === "user" ? "User Details" : "Listing Details"}
              </DialogTitle>
            </DialogHeader>
            <div className="p-4 bg-gray-100 rounded">
              {modalData.type === "user" ? (
                <>
                  <p>
                    <strong>Full Name:</strong> {modalData.data.fullName}
                  </p>
                  <p>
                    <strong>Email:</strong> {modalData.data.email}
                  </p>
                  <p>
                    <strong>Phone:</strong> {modalData.data.phoneNo}
                  </p>
                </>
              ) : (
                <>
                  {modalData.data.title && (
                    <p>
                      <strong>Title:</strong> {modalData.data.title}
                    </p>
                  )}
                  {modalData.data.price && (
                    <p>
                      <strong>Price:</strong> {modalData.data.price}
                    </p>
                  )}
                  {modalData.data.location && (
                    <p>
                      <strong>Location:</strong> {modalData.data.location}
                    </p>
                  )}
                  {modalData.data.make && (
                    <p>
                      <strong>Make:</strong> {modalData.data.make}
                    </p>
                  )}
                  {modalData.data.model && (
                    <p>
                      <strong>Model:</strong> {modalData.data.model}
                    </p>
                  )}
                  {modalData.data.year && (
                    <p>
                      <strong>Year:</strong> {modalData.data.year}
                    </p>
                  )}
                </>
              )}
            </div>
            <DialogClose asChild>
              <Button className="mt-2">Close</Button>
            </DialogClose>
          </DialogContent>
        </Dialog>
      )}
    </div>
  );
};

export default BookingTable;
````

## File: src/components/consultant/ConsultantCarousel.tsx
````typescript
"use client";

import React, { useState } from "react";
import { useRouter } from "next/navigation";
import {
  Dialog,
  DialogContent,
  DialogHeader,
  DialogTitle,
} from "@/components/ui/dialog";
import { Button } from "@/components/ui/button";
import { User } from "lucide-react";

const ConsultantCarousel = ({ consultants }) => {
  const [selectedConsultant, setSelectedConsultant] = useState(null);
  const [modalOpen, setModalOpen] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  const router = useRouter();

  const checkIfAnyDateIsFuture = (data) => {
    // Get current UTC time
    const currentTime = new Date();

    // Use Array.some() to stop as soon as a future date is found
    const isFuture = data.some((item) => {
      // Validate if endDate exists and is a valid date
      if (!item.endDate) return false;

      // Convert endDate to a Date object
      const endDateUTC = new Date(item.endDate);

      // Check if endDate is valid and greater than currentTime
      return !isNaN(endDateUTC.getTime()) && endDateUTC > currentTime;
    });

    return isFuture;
  };

  const openModal = (consultant) => {
    setSelectedConsultant(consultant);
    setModalOpen(true);
  };

  const closeModal = () => {
    setSelectedConsultant(null);
    setModalOpen(false);
  };

  if (!consultants || consultants.length === 0) {
    return <p className="text-gray-500">No consultants available.</p>;
  }

  const handleAvailability = async (consultantId: number, type: string) => {
    const tokenResponse = await fetch(`${endpoint}auth/token`, {
      credentials: "include",
    });
    if (!tokenResponse.ok) {
      throw new Error("Failed to get authentication token");
    }
    const tokenData = await tokenResponse.json();
    const token = tokenData?.token;
    const listingId = consultantId;
    const response = await fetch(
      `${endpoint}api/protected/appointment/booking-status?listingId=${listingId}&type=${type}`,
      {
        method: "GET",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
      }
    );
    if (response.status === 200) {
      const data = await response.json();
      if (checkIfAnyDateIsFuture(data.booking)) {
        alert("You have already booked an appointment with this seller");
      } else {
        alert("Action Pending from Consultant");
      }
    } else {
      router.push(`/dashboard/user/slots/consultant/${consultantId}`);
    }
  };

  return (
    <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
      {consultants.map((consultant) => (
        <div key={consultant.id} className="p-2">
          <div className="rounded-2xl overflow-hidden shadow-md bg-white text-center">
            {/* Top bar with gradient */}
            <div className="relative bg-gradient-to-r from-blue-600 to-blue-400 h-20 flex justify-center items-end rounded-t-2xl">
              {/* User Icon inside circle */}
              <div className="w-16 h-16 rounded-full bg-white flex items-center justify-center shadow-lg -mb-8">
                <User className="w-8 h-8 text-blue-600" />
              </div>
            </div>

            {/* Info below icon */}
            <div className="pt-10 px-4 pb-6">
              <p className="text-sm font-semibold text-blue-600 uppercase tracking-wide">
                {consultant.user?.fullName || "Unknown Consultant"}
              </p>
              <p className="text-sm text-gray-600">
                {consultant.user?.email || "No email provided"}
              </p>
              <p className="text-xs text-gray-500 mt-1 italic">
                {(consultant.servicesOffered || "")
                  .split(",")
                  .map((s) => s.trim())
                  .join(" | ")}
              </p>

              <div className="mt-4 space-y-2">
                <Button
                  className="w-full bg-blue-600 hover:bg-blue-500"
                  onClick={() => openModal(consultant)}
                >
                  View Details
                </Button>

                <Button
                  className="w-full bg-blue-600 hover:bg-blue-500"
                  onClick={() =>
                    handleAvailability(consultant.user.id, "consultant")
                  }
                >
                  View Availability
                </Button>
              </div>
            </div>
          </div>
        </div>
      ))}

      {/* Consultant Details Modal */}
      <Dialog open={modalOpen} onOpenChange={setModalOpen}>
        <DialogContent>
          <DialogHeader>
            <DialogTitle>Consultant Info</DialogTitle>
          </DialogHeader>
          {selectedConsultant && (
            <div className="space-y-2">
              <p>
                <strong>Business Name:</strong>{" "}
                {selectedConsultant.businessName || "N/A"}
              </p>
              <p>
                <strong>Address:</strong>{" "}
                {selectedConsultant.businessAddress || "N/A"}
              </p>
              <p>
                <strong>Experience:</strong>{" "}
                {selectedConsultant.yearsOfExperience || "N/A"} years
              </p>

              <p>
                <strong>Languages:</strong>{" "}
                {selectedConsultant.languagesSpoken || "N/A"}
              </p>
              <p>
                <strong>Website/Social:</strong>{" "}
                {selectedConsultant.websiteOrSocialMedia || "N/A"}
              </p>
              <p>
                <strong>Consultation Fee:</strong>{" "}
                {selectedConsultant.consultationFee
                  ? `$${selectedConsultant.consultationFee}`
                  : "N/A"}
              </p>
            </div>
          )}
        </DialogContent>
      </Dialog>
    </div>
  );
};

export default ConsultantCarousel;
````

## File: src/components/consultant/UpcomingMeetings.tsx
````typescript
"use client";

import React, { useEffect, useState } from "react";
import { VideoIcon } from "lucide-react";
import { Button } from "@/components/ui/button";

interface Meeting {
  id: number;
  startDate: string; // already timezone-adjusted by backend
  endDate: string;
  meetLink: string;
  user: {
    fullName: string;
    email: string;
    phoneNo: string;
  };
}

const UpcomingConsultantMeetings = () => {
  const [meetings, setMeetings] = useState<Meeting[]>([]);
  const [loading, setLoading] = useState(true);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  useEffect(() => {
    const fetchMeetings = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok) {
          throw new Error("Failed to get authentication token");
        }
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        const res = await fetch(
          `${endpoint}api/protected/consultants/upcoming`,
          {
            credentials: "include",
            headers: {
              Authorization: `Bearer ${token}`,
            },
          }
        );
        const data = await res.json();

        if (data.success) {
          setMeetings(data.meetings);
        }
      } catch (err) {
        console.error("Failed to fetch upcoming meetings:", err);
      } finally {
        setLoading(false);
      }
    };

    fetchMeetings();
  }, []);

  if (loading) return <p>Loading meetings...</p>;
  if (meetings.length === 0) return <p>No upcoming meetings.</p>;

  return (
    <div className="flex flex-col gap-4">
      {meetings.map((meeting) => (
        <div
          key={meeting.id}
          className="flex flex-row items-center bg-white shadow-sm border border-gray-200 rounded-xl p-4 max-w-xs"
        >
          {/* Blue circular icon */}
          <a href={meeting.meetLink} target="_blank" rel="noopener noreferrer">
            <div className="flex items-center justify-center w-20 h-24 mr-2 bg-blue-500 hover:bg-blue-600 text-white border">
              <VideoIcon className="w-8 h-8" />
            </div>
          </a>

          {/* Info section */}
          <div className="flex-1 ml-2">
            <p className="text-sm font-semibold text-gray-800">
              {meeting.user.fullName}
            </p>
            <p className="text-sm text-gray-600">
              {new Date(meeting.startDate).toDateString()}
            </p>
            <p className="text-sm text-gray-600">
              {new Date(meeting.startDate).toLocaleTimeString()} –{" "}
              {new Date(meeting.endDate).toLocaleTimeString()}
            </p>
            {/* <Button
              asChild
              size="sm"
              className="mt-2 bg-blue-600 hover:bg-blue-500"
            >
              <a href={meeting.meetLink} target="_blank" rel="noopener noreferrer">
                Join Meeting
              </a>
            </Button> */}
          </div>
        </div>
      ))}
    </div>
  );
};

export default UpcomingConsultantMeetings;
````

## File: src/components/Footer.tsx
````typescript
import React from "react";
import Logo from "@/components/Logo";
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
          <p className="text-sm mt-2">&copy; 2025 ImmiGrow.A.I</p>
          <p className="text-sm">Edmonton, Alberta, Canada</p>
        </div>
        <div>
          <div className="flex justify-center mt-4 space-x-4">
            <Link
              href="https://www.linkedin.com/showcase/ImmiGrow-a-i/"
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
          At ImmiGrow.ai, we acknowledge that we operate on the traditional
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
````

## File: src/components/Header.tsx
````typescript
"use client";
import { useState } from "react";
import { FiMenu, FiX } from "react-icons/fi";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import { usePathname } from "next/navigation";
import Logo from "./Logo";
import ThemeSwitcher from "./ThemeSwitcher";

export default function Header() {
  const [isMenuOpen, setIsMenuOpen] = useState(false);
  const pathname = usePathname();
  const isProtectedPath =
    pathname?.startsWith("/dashboard") || pathname?.startsWith("/onboarding");

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

        {/* Desktop Navigation */}

        {pathname.endsWith("/") && (
          <div className="hidden md:flex items-center gap-12">
            <Link href="#about">About</Link>
            <Link href="#testimonials">Testimonials</Link>
            <Link href="#contact">Contact</Link>
          </div>
        )}

        {/* Right Actions */}
        <div className="hidden md:flex items-center gap-4">
          {/* <ThemeSwitcher /> */}
          <Button className="bg-blue-600 hover:bg-blue-500">
            <Link href={isProtectedPath ? "/login" : "/login"}>
              {isProtectedPath ? "Logout" : "Login"}
            </Link>
          </Button>
        </div>
      </nav>

      {/* Mobile Navigation Menu */}
      {isMenuOpen && (
        <div className="md:hidden flex flex-col items-center gap-4 px-4 py-4">
          {pathname.endsWith("/") && (
            <>
              <Link href="/" onClick={() => setIsMenuOpen(false)}>
                About
              </Link>
              <Link href="/" onClick={() => setIsMenuOpen(false)}>
                Services
              </Link>
              <Link href="/" onClick={() => setIsMenuOpen(false)}>
                Contact
              </Link>
            </>
          )}
          <div className="flex flex-col items-center gap-4 mt-4">
            <ThemeSwitcher />
            <Button className="bg-blue-600 hover:bg-blue-500">
              <Link href={isProtectedPath ? "/logout" : "/login"}>
                {isProtectedPath ? "Logout" : "Login"}
              </Link>
            </Button>
          </div>
        </div>
      )}
    </header>
  );
}
````

## File: src/components/ListingCard.tsx
````typescript
"use client";

import { useRouter, usePathname } from "next/navigation";
import { Card, CardContent, CardHeader } from "@/components/ui/card";
import { Bed, Bath, Clock, MapPin, DollarSign, Calendar } from "lucide-react";
import { TbBrandSpeedtest } from "react-icons/tb";

export default function ListingCard({ listing }) {
  const {
    id,
    title,
    location,
    price,
    houseImages,
    carImages,
    bedrooms,
    bathrooms,
    createdAt,
    make, // Used to determine car listing
    model,
    mileage,
    year,
  } = listing;

  const router = useRouter();
  const pathname = usePathname();

  const isCarListing = Boolean(make); // Check if the listing is a car
  const isHouseListing = Boolean(houseImages && houseImages.length > 0);

  const getSlicedPathname = (pathname: string) => {
    const pathArray = pathname.split("/");

    if (pathArray[1] === "dashboard" && pathArray[2] === "user") {
      return isCarListing
        ? `/${pathArray[1]}/${pathArray[2]}/cars`
        : `/${pathArray[1]}/${pathArray[2]}/homes`;
    }

    if (
      pathArray[1] === "dashboard" &&
      (pathArray[2] === "realtor" || pathArray[2] === "car-dealer")
    ) {
      return `/${pathArray[1]}/${pathArray[2]}`;
    }

    return pathArray.slice(0, pathArray.length - 1).join("/");
  };

  const handleCardClick = () => {
    if (isHouseListing) {
      router.push(`${getSlicedPathname(pathname)}/house-listings/${id}`);
    }
    if (isCarListing) {
      router.push(`${getSlicedPathname(pathname)}/car-listings/${id}`);
    }
  };

  return (
    <Card
      className="sm:w-full h-full border rounded-lg p-2 shadow-sm cursor-pointer hover:shadow-md transition flex"
      onClick={handleCardClick}
    >
      {/* Image Section */}
      <div className="w-1/3">
        {isHouseListing && (
          <img
            src={houseImages[0].base64}
            alt="House"
            className="w-full h-full object-cover rounded-l-lg"
          />
        )}
        {isCarListing && carImages?.length > 0 && (
          <img
            src={carImages[0].base64}
            alt="Car"
            className="w-full h-full object-cover rounded-l-lg"
          />
        )}
      </div>

      {/* Content Section */}
      <div className="w-2/3 p-2 flex flex-col justify-between">
        <CardHeader className="p-0">
          <div className="flex items-center justify-between">
            {title && (
              <p className="text-xl font-bold truncate w-30">{title}</p>
            )}
            {make && model && (
              <p className="text-xl font-bold">
                {model} {make}
              </p>
            )}
          </div>

          {/* Price */}
          <p className="text-xl font-bold text-blue-600 flex items-center">
            <DollarSign className="h-5 w-5 text-blue-600 mr-1" />
            {price.toLocaleString()}
          </p>

          {/* Location (Visible Only for Houses) */}
          {isHouseListing && (
            <p className="text-sm font-medium text-gray-700 flex items-start  gap-2">
              <MapPin size={20} />
              <span className="truncate w-50">{location}</span>
            </p>
          )}
          {isCarListing && (
            <p className="text-sm font-medium text-gray-700 flex items-start  gap-2">
              <Calendar size={20} />
              {year}
            </p>
          )}
        </CardHeader>

        {/* Features (House: Bedrooms & Bathrooms | Car: Just an Icon) */}
        <CardContent className="p-0 flex items-center space-x-4 text-gray-600 text-sm mt-2">
          {isHouseListing && bedrooms !== undefined && (
            <span className="flex items-center">
              <Bed className="h-4 w-4 mr-1" />
              {bedrooms}
            </span>
          )}
          {isHouseListing && bathrooms !== undefined && (
            <span className="flex items-center">
              <Bath className="h-4 w-4 mr-1" />
              {bathrooms}
            </span>
          )}
          {isCarListing && (
            <span className="flex items-center">
              <TbBrandSpeedtest className="h-4 w-4 mr-1" /> {mileage}
            </span>
          )}
          <span className="flex items-center">
            <Clock className="h-4 w-4 mr-1" />
            {createdAt ? new Date(createdAt).toDateString() : "Just now"}
          </span>
        </CardContent>
      </div>
    </Card>
  );
}
````

## File: src/components/Logo.tsx
````typescript
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
      <Image src={"/logo.png"} width={40} height={40} alt="ImmiGrow" />
      <p className="text-3xl font-bold tracking-tighter">ImmiGrow</p>
    </Link>
  );
};

export default Logo;
````

## File: src/components/UserProfile.tsx
````typescript
// /app/profile/UserProfile.tsx
import React from "react";
import { UserCircleIcon } from "@heroicons/react/24/solid";

interface UserProfileProps {
  userData: {
    fullName: string;
    DOB: string;
    phoneNo: string;
    email: string;
    roleId: number;
    role: string;
    alreadyInCanada?: boolean | null;
    statusInCanada?: string | null;
    countryOfOrigin?: string | null;
    currentLocation?: string | null;
  };
}

const UserProfile: React.FC<UserProfileProps> = ({ userData }) => {
  return (
    <div className="max-w-5xl  mx-auto grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-20">
      {/* Card 1 - Profile Section */}
      <div className="bg-white shadow-md rounded-lg overflow-hidden">
        <div className="bg-gradient-to-r from-blue-600 to-blue-400 p-6 flex flex-col justify-center items-center text-white">
          <UserCircleIcon className="w-24 h-24 mb-4" />
          <h2 className="text-xl font-bold">{userData.fullName}</h2>
          <p className="text-sm">{userData.role.name}</p>
        </div>
        <div className="p-6 text-center">
          <p className="text-gray-600 font-semibold">Date of Birth</p>
          <p className="text-gray-600 text-center">
            {new Date(userData.DOB).toLocaleDateString()}
          </p>
          <p className="text-gray-600 font-semibold mt-4">Phone Number</p>
          <p className="text-gray-600 text-center">{userData.phoneNo}</p>
        </div>
      </div>

      {/* Card 2 - Email and Status */}
      <div className="bg-white shadow-md rounded-lg p-6">
        <div className="mt-12">
          <h3 className="text-lg text-center font-bold mb-4">
            Additional Information
          </h3>
          {userData.roleId === 1 && (
            <>
              <div className="mb-4">
                <p className="text-gray-600 text-center font-semibold">Email</p>
                <p className="text-gray-600 text-center">{userData.email}</p>
              </div>
              <div className="mb-4">
                <p className="text-gray-600 text-center font-semibold">
                  Already In Canada
                </p>
                <p className="text-gray-600 text-center">
                  {userData.alreadyInCanada ? "Yes" : "No"}
                </p>
              </div>
              {userData.alreadyInCanada && (
                <div className="mb-4">
                  <p className="text-gray-600 text-center font-semibold">
                    Status In Canada
                  </p>
                  <p className="text-gray-600 text-center">
                    {userData.statusInCanada || "N/A"}
                  </p>
                </div>
              )}
            </>
          )}
        </div>
      </div>

      {/* Card 3 - Country and Location */}
      <div className="bg-white shadow-md rounded-lg p-6">
        <div className="mt-14">
          <h3 className="text-lg text-center font-bold mb-4">
            Location Information
          </h3>
          {userData.roleId === 1 && (
            <>
              <div className="mb-4">
                <p className="text-gray-600 text-center font-semibold">
                  Country of Origin
                </p>
                <p className="text-gray-600 text-center">
                  {userData.countryOfOrigin || "N/A"}
                </p>
              </div>
              {userData.alreadyInCanada && (
                <div className="mb-4">
                  <p className="text-gray-600 text-center font-semibold">
                    School/Work Location
                  </p>
                  <p className="text-gray-600 text-center">
                    {userData.currentLocation || "N/A"}
                  </p>
                </div>
              )}
            </>
          )}
        </div>
      </div>
    </div>
  );
};

export default UserProfile;
````

## File: src/components/ai/ResumeAnalysisDetail.tsx
````typescript
"use client";

import React, { useState } from 'react';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Badge } from '@/components/ui/badge';
import { Progress } from '@/components/ui/progress';
import { ArrowLeft, FileText, User, Mail, Phone, MapPin, Calendar, TrendingUp, Star, AlertCircle, CheckCircle, Briefcase, GraduationCap, Code, Languages, Target, ArrowRight, X, Loader2, Globe, Award, DollarSign, Search } from 'lucide-react';
import JobSearchModal from './JobSearchModal';

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

      const token = localStorage.getItem('token');
      const response = await fetch(`${process.env.NEXT_PUBLIC_API_URL}api/protected/ai-local/career-profile/enhanced-profile`, {
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
              onClick={() => window.location.href = '/dashboard/user/ai/resume'}
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
````
