=====================================================
 MY HEALTH — BUILD YOUR ANDROID APP (APK) FOR FREE
 Notifications work even when the screen is OFF.
=====================================================

You do NOT need a computer with special software. A free GitHub account
builds the app for you in the cloud. It takes about 15 minutes the first time.

WHAT THIS FOLDER IS:
  A ready-made Android app project. You upload it to GitHub once, and GitHub
  automatically turns it into an installable APK file you download to your phone.

-----------------------------------------------------
 PART 1 — PUT THE PROJECT ON GITHUB
-----------------------------------------------------
1. Go to github.com and make a free account (or log in).
2. Click the "+" at the top right -> "New repository".
3. Name it:  my-health-app
   - Choose "Public".
   - Do NOT tick "Add a README".
   - Click "Create repository".
4. On the next page click the link: "uploading an existing file".
5. Unzip this project on your computer. Then drag EVERYTHING inside the
   MyHealthApp-Android folder into the upload box. This must include:
      package.json, capacitor.config.json, README-BUILD.txt,
      the "www" folder, the "assets" folder, and the ".github" folder.
   IMPORTANT: the ".github" folder is required (it builds the app). If your
   computer hides it, turn on "show hidden files", or see PART 4 below.
6. Click "Commit changes" at the bottom.

-----------------------------------------------------
 PART 2 — LET GITHUB BUILD THE APK
-----------------------------------------------------
7. At the top of your repository click the "Actions" tab.
8. You will see a run called "Build Android APK" (it starts by itself).
   Wait until it finishes and shows a green tick (about 5-10 minutes).
   - If it asks you to enable Actions, click the green "I understand / Enable".
9. Click on the finished run. Scroll to the bottom to the "Artifacts" box.
10. Click "MyHealthApp-APK" to download it. It downloads a .zip.
11. Open that .zip -> inside is the file "app-debug.apk". That is your app!

-----------------------------------------------------
 PART 3 — INSTALL ON YOUR ANDROID PHONE
-----------------------------------------------------
12. Send app-debug.apk to your phone (WhatsApp to yourself, email, or USB).
13. Tap the file on your phone. Android may say "install unknown apps" is off:
    tap Settings -> allow for your browser/Files app -> go back -> Install.
14. Open "My Health". When it asks, ALLOW notifications.

VERY IMPORTANT for screen-off alarms to be reliable:
15. Phone Settings -> Apps -> My Health -> Battery -> set to "Unrestricted"
    (or turn OFF battery optimization for this app).
16. On Android 12 and newer: Settings -> Apps -> My Health -> "Alarms & reminders"
    -> allow. This lets it ring at the exact time even when locked.

Done! Set your reminders in the app; they will now ring with the screen off.

-----------------------------------------------------
 PART 4 — IF THE ".github" FOLDER IS HARD TO UPLOAD
-----------------------------------------------------
You can create it by hand on GitHub:
  a. In your repo click "Add file" -> "Create new file".
  b. In the name box type exactly:  .github/workflows/build-apk.yml
     (typing the slashes makes the folders automatically)
  c. Open the file .github/workflows/build-apk.yml from this project in Notepad,
     copy ALL of it, paste into the GitHub box.
  d. Click "Commit changes". The build will start.

-----------------------------------------------------
 NOTES
-----------------------------------------------------
- This is a "debug" APK: perfect for personal use. It is not on the Play Store.
- Your data stays on your phone only.
- To change the app later, edit files in "www" and re-upload; a new APK builds.
- Stuck on any step? Tell me the step number and what you see, and I'll help.
