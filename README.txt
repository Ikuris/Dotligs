DOTLINGS - Android app project
================================

This folder is a complete Android app. The game runs fully offline inside the app.

EASIEST WAY (no installs, free GitHub account):
1. Make a free account at github.com and create a new repository (any name).
2. Click "uploading an existing file" and drag in EVERYTHING inside this folder
   (including the hidden ".github" folder - on a computer, drag the folder contents;
   if .github doesn't upload, create the file .github/workflows/build-apk.yml by hand
   and paste in its contents).
3. Click "Commit changes". GitHub starts building automatically.
4. Open the "Actions" tab, wait ~5 minutes for the green check, open the run,
   and download "Dotlings-APK" at the bottom. Unzip it to get app-debug.apk.
5. Send the APK to your Android phone, tap it, and allow "Install unknown apps".

ANDROID STUDIO WAY:
1. Install Android Studio, choose File > Open, pick this folder.
2. Let it sync (it may offer to add a Gradle wrapper - say yes).
3. Build > Build Bundle(s)/APK(s) > Build APK(s).

UPDATING THE GAME:
Replace app/src/main/assets/index.html with the newer game file and build again.
Raise versionCode in app/build.gradle.kts (1 -> 2) so phones accept the update.

NOTES:
- Saves are kept inside the app. Use Settings > Save Code to back them up.
- The Android back button works like the game's BACK button.
- Read-aloud depends on the phone's built-in voice support and may not work in the app.
- This is a "debug" APK for your own devices. Publishing on Google Play needs a signed release build.
