MOBILE-FRIENDLY FREE APK BUILD
==============================
This project was adjusted so a debug APK does NOT require debug.keystore or a release keystore.
A GitHub Actions workflow is included at:
.github/workflows/build-apk.yml

Important:
- Java 17 is required by Android Gradle Plugin 9.1.1.
- Gradle 9.3.1 is used by the included cloud workflow.
- google-services.json is still optional for compilation because the project is configured to WARN if missing. Firebase/Google sign-in features need a real Firebase configuration to work correctly.
- .env.example contains a placeholder Gemini API key. AI features need your own valid API key/configuration.
- YouTube-related features may require a YouTube API key entered/configured by the app.

The included workflow builds a DEBUG APK, suitable for installing/testing on Android. It is not a Play Store release signing setup.
