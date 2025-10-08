# StudyBuddy - AI Accountability Study Partner (Skeleton)

This is a minimal Android app skeleton (Kotlin, Jetpack Compose) implementing:
- On-device Room entities for tasks/sessions
- WorkManager scheduled jobs for session end / mid-check
- Basic notification helpers and FCM-ready intent hooks
- Simple Compose UI: onboarding, task list, start session flow

**What I provide here**
- Complete Android project skeleton ready to open in Android Studio.
- GitHub Actions workflow to build APK (requires secrets for signing if releasing).
- Instructions to build the APK locally.

**Important**
I cannot produce a signed, working APK from this environment. Use the instructions below to build locally or set up CI using the included `/.github/workflows/android-build.yml`.

## Build locally
1. Install Android Studio + Android SDK (recommend SDK 33+).
2. Open this folder as a project in Android Studio.
3. Let Gradle sync and download dependencies.
4. Build -> Build Bundle(s) / APK(s) -> Build APK(s).
5. To install: `adb install -r app/build/outputs/apk/debug/app-debug.apk`

## CI (GitHub Actions)
A sample workflow is included at `.github/workflows/android-build.yml`. Follow comments in the file.

## Notes
- This is a skeleton for fast iteration. Integrate your own backend, Firebase, and AI models as needed.
- See `app/src/main/java/com/example/studybuddy/` for Kotlin sources.

