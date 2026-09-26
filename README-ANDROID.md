# ULTINO TOOL TECH — Android APK package

This package is the **actual AI Studio ULTINO TOOL TECH job-card source** wrapped for Android with Capacitor. It is mobile-first and does not require a PC interface at runtime.

## Easiest APK build without Android Studio

1. Create a GitHub repository.
2. Upload this entire project.
3. Open **Actions**.
4. Run **Build ULTINO TOOL TECH Android APK**.
5. Open the completed workflow run.
6. Download the artifact named `ultino-tool-tech-jobcard-debug-apk`.
7. Extract the artifact and install `app-debug.apk` on the Android phone.

## Local build if desired

```bash
npm install
npm run android:build
```

The APK will be at:
`android/app/build/outputs/apk/debug/app-debug.apk`

## App data

The existing IndexedDB storage layer from the AI Studio project is retained. Jobs, customers, items and drawings remain local to the installed app. The project also retains its existing backup/restore workflow.
