# EHS Report – Android APK (build with GitHub, no Android Studio needed)

1. Create a free account at github.com and a new **private** repository (e.g. `ehs-report`).
2. Upload everything in this folder to the repository root. Use a PC browser: "Add file → Upload files".
   The hidden folder `.github/workflows/build-apk.yml` must be included. If it is not, choose
   "Add file → Create new file", type `.github/workflows/build-apk.yml` as the name and paste its contents.
3. Open the **Actions** tab → **Build APK** → **Run workflow**. Wait about 5–10 minutes.
4. Open the finished run → under **Artifacts** download **EHS-Report-APK** (a zip) → unzip → `app-debug.apk`.
5. Copy the APK to your Android phone and open it. Allow "Install unknown apps" when asked.
6. In the app tap **⚙ AI key** and paste your Anthropic API key (console.anthropic.com → API keys).
   Use a dedicated key with a low spending limit; it is stored only on the phone.

## Saving to Google Drive / printing
Every download (Excel, memo, register, photos) opens the Android share sheet. Choose **Drive** (Save to Drive),
Gmail, WhatsApp, or a print/PDF app. Memo and register files are HTML: open the shared file in Chrome and tap Print.

## Notes
- Data is stored on the phone. Export Excel regularly. Uninstalling the app erases its data.
- This is a debug-signed APK for your own factory use (not for the Play Store).
