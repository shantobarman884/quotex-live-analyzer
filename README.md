# Quotex Live Analyzer — Android prototype

This is a starter Android Studio project with a GitHub Actions workflow to build a debug APK in the cloud.

## What it does
- Requests explicit Android MediaProjection consent.
- Shows a local screen preview.
- Displays `WAIT` because this prototype does not reliably recognize candles or validate BUY/SELL signals.
- Does not log into Quotex, click controls, place trades, upload screenshots, or store screen captures permanently.

## Build an APK using GitHub from an Android phone
1. Sign in to GitHub and create a **new public or private repository**.
2. Upload the contents of this ZIP (not the ZIP file itself) to the repository's root. Make sure `.github/workflows/android-apk.yml` is included.
3. Open the repository's **Actions** tab and enable Actions if GitHub asks.
4. Choose **Build Android APK** and tap **Run workflow**. If the workflow does not appear, verify the YAML is in `.github/workflows/android-apk.yml` on the default branch.
5. Wait for the run to finish successfully.
6. Open the completed run, scroll to **Artifacts**, and download `quotex-live-analyzer-debug-apk`.
7. Extract the downloaded artifact ZIP on your phone. Tap `app-debug.apk` to install it. Android may ask you to allow installs from your browser or file manager. Only enable this for the app you trust, and disable it afterward.

## Important
- This is a debug APK, not a Play Store release.
- It has not been device-tested in this environment.
- The app currently previews the screen and displays WAIT; it does not generate validated trading signals.
- Screen capture may expose private notifications. Close sensitive apps first and stop capture when done.
- Use only in accordance with local law and the platform's terms.
