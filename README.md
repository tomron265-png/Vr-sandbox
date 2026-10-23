# PocketVR Sandbox (Android APK starter)

This is a buildable Android Studio project intended for a Samsung Galaxy S10 (Android 11).
It opens a bundled web app inside an Android WebView, requests camera permission for hand tracking,
and provides a simple stereoscopic sandbox prototype with gyro look controls.

## Build an APK with GitHub Actions (beginner-friendly)

1. Create a GitHub account and a new repository named `PocketVRSandbox`.
2. Upload the contents of this folder to the repository (not the ZIP itself).
3. Open the repository's **Actions** tab and enable Actions if prompted.
4. The workflow **Build PocketVR Sandbox APK** should run automatically.
5. Open the completed workflow run, scroll to **Artifacts**, and download `PocketVRSandbox-debug-apk`.
6. Extract the ZIP and install `app-debug.apk` on your phone. You may need to allow installs from your browser/files app.

## Notes
- This is a starter prototype, not a finished PC game streamer.
- The included demo uses a bundled HTML page and remote CDN libraries for Three.js and MediaPipe Hands,
  so internet is required for those libraries on first launch.
- Camera access should work in the native WebView after permission is granted. Hand landmark detection depends
  on the MediaPipe CDN/model being reachable.
- The app does not yet stream Windows games or inject controls into third-party games.
