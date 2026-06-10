# Terminal Emulator for Android

> **Note:** This project is a modernized refactoring of the original "Terminal Emulator for Android" by jackpal. It has been updated to use modern build tools (Gradle, CMake) and target newer Android SDKs while preserving the core functionality.

Terminal Emulator for Android is a terminal emulator for communicating with the built-in Android shell. It emulates a reasonably large subset of Digital Equipment Corporation VT-100 terminal codes, so that programs like "vi", "Emacs" and "NetHack" will display properly.

## Features

- Full Linux terminal emulation.
- Multiple windows support.
- Launcher shortcuts.
- UTF-8 text support (Arabic, Chinese, Greek, Hebrew, Japanese, Korean, Russian, Thai, etc.).
- Completely free. No ads, no in-app-purchases, no nag screens.
- Modernized build system using Gradle and CMake.

## Build Instructions

You can build the project from the command line using the Gradle wrapper included in the repository.

### Prerequisites

- [Android Studio](https://developer.android.com/studio) or Android SDK Command-line Tools.
- Android NDK (installed via Android SDK Manager).
- Ensure your `local.properties` file in the project root has the correct paths to your SDK and NDK, or simply open the project in Android Studio to have it generated automatically.

### Build Debug APK

To build a debug version of the app, run:

```bash
./gradlew assembleDebug
```
The resulting APK will be located at `term/build/outputs/apk/debug/term-debug.apk`.

### Build Release APK

To build a release version of the app, run:

```bash
./gradlew assembleRelease
```
The resulting APK will be located at `term/build/outputs/apk/release/term-release-unsigned.apk` (or `term-release.apk` if signing is configured).

## Historical Information

This application was previously named "Android Terminal Emulator". The code is based on the "Term" application which is included in the Android Open Source Project.

- Got questions? Please check out the [FAQ](http://github.com/jackpal/Android-Terminal-Emulator/wiki/Frequently-Asked-Questions).
- Please see the [Recent Updates](http://github.com/jackpal/Android-Terminal-Emulator/wiki/Recent-Updates) page for recent updates.
