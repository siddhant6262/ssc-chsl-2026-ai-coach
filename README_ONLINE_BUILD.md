# SSC CHSL 2026 AI Coach — Phone/Online Build

This version is intentionally a FLAT Android Gradle project because files
uploaded from the phone were flattened in the GitHub repository.

IMPORTANT:
- Keep `.github/workflows/build-apk.yml` inside `.github/workflows/`.
- All other project files can stay at the repository root.
- Do NOT create an `app/` folder for this version.

GitHub:
1. Replace the root files with the files from this ZIP.
2. Open Actions.
3. Select "Build SSC CHSL 2026 APK".
4. Tap "Run workflow".
5. When the run finishes, open the run and download the artifact
   "SSC-CHSL-2026-AI-Coach-debug".
6. Extract it and install `app-debug.apk`.

The workflow builds a debug APK using Android SDK 35 and Gradle 8.7.
