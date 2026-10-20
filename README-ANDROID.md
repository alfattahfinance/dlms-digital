# DLMD Digital DSP Android APK

This Android wrapper loads the existing DSP console from
`app/src/main/assets/index.html`.

## Build and download on Android
1. Open the repository's Actions tab.
2. Select **Build DLMD Digital DSP APK** and tap **Run workflow** on branch `main`.
3. Open the completed run and download artifact **DLMD-Digital-DSP-debug-APK**.
4. Extract the ZIP and install `app-debug.apk`.

## Important
This APK packages the existing HTML interface in a WebView. It does not itself add
DSP audio processing or an ESP32 network service. Existing requests such as `/update`,
`/mute`, and `/power` need a reachable device/server endpoint and may need the
ESP32's actual IP address configured. This is a debug APK, not a Play Store release.
