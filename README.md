# Focus Rest Timer (APK build kit)

60 min focus -> alarm + vibration -> 20 min rest -> alarm + vibration -> repeat.

## Get the APK (about 10 minutes, no coding)
1. Create a free account at github.com and make a **new repository** (any name, Public or Private).
2. Click **"uploading an existing file"** on the new repo page, drag in ALL files from this folder
   (including the hidden `.github` folder, `www`, `package.json`, `capacitor.config.json`, `.gitignore`), then **Commit changes**.
   Tip: if the hidden `.github` folder is hard to drag, use the repo's Add file > Create new file, name it
   `.github/workflows/build-apk.yml` and paste the file contents.
3. Open the **Actions** tab. The "Build APK" run starts by itself (or click it > **Run workflow**). Wait ~5 minutes for the green tick.
4. Click the finished run, scroll to **Artifacts**, download `focus-rest-timer-apk` (a zip), unzip it, and you get `app-debug.apk`.
5. Send the APK to your phone, tap it, allow "Install unknown apps" if asked.

## First run on the phone
- Tap Start and **allow notifications**.
- For reliable alarms with the screen locked: Settings > Apps > Focus Rest Timer > Battery > **Unrestricted**, and make sure Do Not Disturb is off.
- Alerts are scheduled as phone alarms, so they fire even if the app is closed.
