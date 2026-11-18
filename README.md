# Hari Smruti Path – Android App

A native Android application built in Java with zero third-party runtime dependencies.

## Features
- One large button: each tap increments today's Hari Smruti Path count by 1.
- Today's count, lifetime total, and a day-by-day summary sorted newest first.
- Undo the latest tap made today.
- Reset today's count with a confirmation dialog; previous dates are untouched.
- Saves counts locally through Android SharedPreferences as date-keyed JSON.
- On a new local calendar day, a new count starts automatically at zero.
- Works offline, with no sign-in or ads.

## Build an installable APK
1. Install Android Studio (with Android SDK 35 and JDK 17).
2. Open the **HariSmrutiPath** directory as a project.
3. Allow Android Studio to sync Gradle. The Android Gradle Plugin version is 8.7.3.
4. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. Android Studio shows the APK location, typically `app/build/outputs/apk/debug/app-debug.apk`.
6. Transfer the APK to the phone and install it. Android may ask for permission to install apps from that source.

## Important
The ZIP is the Android Studio **source project**, not an APK. This environment does not have the Android SDK needed to compile an APK.
Counts remain on the device; clearing app storage or uninstalling can remove data. Dates depend on the phone's local date/time. Day totals are nonnegative integers.
