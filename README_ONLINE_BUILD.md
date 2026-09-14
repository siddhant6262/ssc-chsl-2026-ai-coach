# SSC CHSL 2026 AI Coach — Online APK Build

This project is configured to build an installable Android debug APK using **GitHub Actions**, so you do not need Android Studio, Gradle, Java, or the Android SDK on your phone.

## Phone-only steps

1. Create/sign in to a GitHub account.
2. Create a new repository, e.g. `ssc-chsl-2026-ai-coach`.
3. Upload **all files inside this project folder** to the repository root (do not upload the outer ZIP folder itself).
4. Open the repository's **Actions** tab.
5. Select **Build SSC CHSL 2026 APK**.
6. Tap **Run workflow**.
7. Wait for the green check to appear.
8. Open that workflow run and scroll to **Artifacts**.
9. Download `SSC-CHSL-2026-AI-Coach-debug`.
10. Extract the downloaded ZIP; inside is `app-debug.apk`.
11. Tap `app-debug.apk` and install it on your Android phone.

## Automatic builds

The workflow also runs automatically whenever you push to `main` or `master`.

## What the workflow does

- Uses GitHub's hosted Ubuntu runner.
- Installs JDK 17.
- Installs the Android SDK and Android 35 platform/build tools.
- Installs Gradle 8.7.
- Runs `assembleDebug`.
- Uploads the resulting APK as a downloadable Actions artifact.

The debug APK is already signed with the standard Android debug key and is suitable for direct testing/installing on a phone. For Google Play publishing, a separate release-signing setup is required.
