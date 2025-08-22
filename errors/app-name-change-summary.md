# App Name Change Summary: Athena → System Info

## Overview
This document summarizes all the changes made to rename the app from "Athena" to "System Info" throughout the project.

## Changes Made

### 1. App Name String
**File**: `app/src/main/res/values/strings.xml`
**Change**: Updated `app_name` string from "Athena" to "System Info"

### 2. Project Name
**File**: `settings.gradle.kts`
**Change**: Updated `rootProject.name` from "Athena" to "device-info"

### 3. README.md
**File**: `README.md`
**Change**: Updated main title from "# Athena" to "# System Info"

### 4. REUSE.toml
**File**: `REUSE.toml`
**Change**: Updated `SPDX-PackageName` from "Athena" to "System Info"

### 5. Native Code
**File**: `app/src/main/cpp/vulkan/VkUtils.cpp`
**Change**: Updated `appInfo.pApplicationName` from "Athena" to "System Info"

### 6. Theme Names
**File**: `app/src/main/res/values/themes.xml`
**Changes**:
- `Theme.Athena` → `Theme.SystemInfo`
- `Theme.Athena.SectionLayout` → `Theme.SystemInfo.SectionLayout`
- `Theme.Athena.SectionTitle` → `Theme.SystemInfo.SectionTitle`
- `Theme.Athena.SectionEntry` → `Theme.SystemInfo.SectionEntry`
- `Theme.Athena.CustomDialog` → `Theme.SystemInfo.CustomDialog`

### 7. AndroidManifest.xml
**File**: `app/src/main/AndroidManifest.xml`
**Changes**: Updated both theme references from `@style/Theme.Athena` to `@style/Theme.SystemInfo`

### 8. Layout Files
**Files**: Multiple layout files (fragment_treble.xml, fragment_gpu.xml, fragment_audio.xml, etc.)
**Changes**: Updated all style references from `Theme.Athena.*` to `Theme.SystemInfo.*`

## Files Modified
1. `app/src/main/res/values/strings.xml`
2. `settings.gradle.kts`
3. `README.md`
4. `REUSE.toml`
5. `app/src/main/cpp/vulkan/VkUtils.cpp`
6. `app/src/main/res/values/themes.xml`
7. `app/src/main/AndroidManifest.xml`
8. Multiple layout files with theme style references

## Impact
- **App Display Name**: Now shows as "System Info" in the system
- **Project Identity**: Project is now named "device-info" 
- **Theme Consistency**: All UI elements now use the new theme names
- **Native Integration**: Vulkan application name updated for consistency

## Notes
- The package name (`dev.sebaubuntu.athena`) remains unchanged to avoid breaking existing code
- All theme references have been updated to maintain UI consistency
- The app will now display as "System Info" to users
- Build and functionality remain unchanged

## Verification
After these changes:
1. The app should display as "System Info" in the system
2. All UI elements should maintain their styling
3. The project should build successfully
4. No functionality should be affected
