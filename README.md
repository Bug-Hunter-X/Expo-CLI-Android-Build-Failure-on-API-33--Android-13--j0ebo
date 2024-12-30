# Expo CLI Android Build Failure on API 33 (Android 13)

This repository demonstrates a bug and its solution related to building Expo projects targeting Android API level 33 (Android 13).  The issue stems from incompatibilities between the Android Gradle Plugin version and the target SDK version used in the Expo project.  The bug results in a build failure when attempting to run the project on an Android device or emulator.

## Bug
The `bug.js` file contains a minimal Expo project setup that, when built for Android API 33, fails with a Gradle build error.

## Solution
The `bugSolution.js` file shows the corrected project setup. The solution addresses the incompatibility by adjusting relevant configuration settings within the Expo project's Android build configuration to ensure compatibility with Android API level 33.

## Steps to Reproduce the Bug
1. Clone this repository.
2. Navigate to the project directory.
3. Install the project dependencies using `npm install`.
4. Attempt to build the project for Android using `expo prebuild` or `expo run:android` targeting API level 33.

## Solution Implementation
The solution involves modifying the `android/gradle.properties` file, as shown in `bugSolution.js`. This ensures the Android Gradle Plugin version and other Android configurations are suitable for API level 33.