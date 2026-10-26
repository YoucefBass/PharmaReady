# PharmaReady Android project

This project wraps the PharmaReady HTML app in an Android WebView and keeps the app's files bundled locally.

## Build an APK
1. Install Android Studio on a computer.
2. Open this folder (`PharmaReadyAndroid`) in Android Studio.
3. Allow Gradle sync and install Android SDK Platform 35 if prompted.
4. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. Android Studio will show the generated APK location, typically `app/build/outputs/apk/debug/app-debug.apk`.
6. Transfer that APK to your Android phone and install it. If prompted, allow installing apps from that source.

Package ID: `com.pharmaready.app`
Minimum Android version: Android 6.0 (API 23)

Note: This is the Android Studio project source, not a precompiled APK. A compiled APK requires Android SDK/Gradle build tools, which are not installed in this environment.

Cloud build note:
The GitHub Actions workflow is included as a starting point, but this project currently has no Gradle wrapper files. A wrapper must be added (or Gradle installed on a build runner) before the cloud workflow can produce an APK. The simplest reliable method remains opening the project in Android Studio and building an APK.
