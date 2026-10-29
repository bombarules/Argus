# Argus

Photo-real ball hub app: a large realistic soccer ball whose panels open
the apps (PoolTrack Live aquatics, Field Reports, parks map), with settings,
recents and live screens.

Build it with:

    ./gradlew assembleDebug

The APK lands at `app/build/outputs/apk/debug/app-debug.apk`.

Notes:
- Package `com.argus.hub`, version 1.0. Debug builds are signed with the
  committed `app/debug.keystore` (standard Android debug key) so every
  build, local or CI, installs and updates cleanly.
- This is a WebView wrapper around the photo-real web hub in
  `app/src/main/assets/`. The original Bomba's native phone features
  (app drawer, wallpaper, home settings, screen sharing) are not in this
  build; the ball hub, app pages and live viewing work as before.
