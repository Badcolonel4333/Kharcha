KHARCHA 3.0 — GITHUB PAGES DEPLOYMENT

FILES TO UPLOAD
- index.html
- manifest.json
- sw.js
- icon-192.png
- icon-512.png
- icon-maskable-512.png

DEPLOY / UPDATE
1. Open the GitHub repository that publishes https://badcolonel4333.github.io/Kharcha/.
2. Back up your current files (especially index.html, manifest.json and sw.js).
3. Upload/replace all six files above in the same repository folder (the repository root if the current app is published from root).
4. Commit the changes to the branch/folder configured in GitHub Pages.
5. Open the site in Chrome on your phone. If an old version appears, close the installed app/browser tab, reopen the site, and refresh once. The new service-worker cache is kharcha-v3-shell.
6. If you already installed Kharcha, open the website once while online so the updated app shell can install, then launch the installed app again.

DATA PRESERVATION
The upgraded app reads the existing localStorage key "kharcha" and migrates the old v2 fields (e / cats / rt / lastSum) to the new format. Deploying to the same GitHub Pages origin should preserve browser-local data. Do not clear site data or uninstall the old app before opening the upgraded version. As a precaution, export your existing expenses to Excel from the old app before updating. For moving data to another phone/browser, use Settings > Backup JSON on the new app and import that JSON on the new device.

WHAT'S NEW
- Updated responsive mobile-first interface.
- Monthly budget and remaining-budget overview.
- Today, month, daily average, 7-day and top-category summaries.
- Add descriptions/notes; edit and delete transactions.
- Search transactions and filter by month.
- Monthly category and daily spending insights with month navigation.
- Manage categories and choose system/light/dark theme.
- JSON backup/restore and Excel export; CSV fallback if the spreadsheet library is unavailable.
- Legacy v2 data migration and updated offline app-shell cache.

NOTES / LIMITATIONS
- Expenses remain in browser localStorage on this device; there is no account, cloud sync or multi-device sync.
- Scheduled reminders are best-effort and only run while the app is open; browser/OS notification restrictions apply.
- Excel import/export uses the SheetJS CDN library and therefore requires internet access for that library. JSON backup/restore works without it.
- GitHub Pages serves a web app/PWA. It can be installed on Android from Chrome; it is not a Play Store APK.
