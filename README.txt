KHARCHA 4.0 — CLEAN START (GITHUB PAGES)

PACKAGE CONTENTS
- index.html
- manifest.json
- sw.js
- icon-192.png
- icon-512.png
- icon-maskable-512.png

WHAT CHANGED
- Starts with zero transactions and zero preloaded categories.
- Does not read, migrate, or display data from the older Kharcha v2/v3 localStorage key.
- Uses a separate browser storage key: kharcha-v4-clean-start.
- Simple insights: category spending bars and a six-month spending trend.
- Keeps quick expense entry, editing/deleting, search, monthly filter, optional budget, themes, JSON backup/restore and Excel export/import.
- Updated service-worker cache name for the new release.

IMPORTANT ABOUT YOUR OLD DATA
The previous data is not deleted. Kharcha 4.0 simply uses a separate storage key, so your older expenses and categories will not appear in this clean version. This avoids accidentally destroying your earlier data. You can still access the old data by restoring the previous app files and storage setup, or importing a backup manually if needed.

DEPLOY
1. Download and extract the ZIP.
2. Open the GitHub repository that publishes https://badcolonel4333.github.io/Kharcha/.
3. Back up the current repository files.
4. Upload and replace all six app files in the same folder used by GitHub Pages.
5. Commit the changes to the published branch.
6. Open the site in Chrome on your phone while online. Allow the new service worker to update; close and reopen the installed app if the previous shell remains visible.

INSTALL ON ANDROID
Open the website in Chrome → three-dot menu → Install app (or Add to Home screen).

DATA & PRIVACY
Expenses are stored locally in this browser under the new Kharcha 4 storage key. No account or cloud sync is included. Export a JSON backup regularly, especially before changing phones or clearing browser data.

CHARTS
The Insights tab shows a category breakdown for the selected month and a compact six-month trend. Empty charts display a prompt instead of filling the screen with zero-value bars.

NOTES
- GitHub Pages hosts the PWA; this package is not an APK or Play Store release.
- Excel import/export uses the SheetJS CDN and requires internet access for that library. JSON backup/restore is built in.
- Browser notifications are best-effort and may only work while the app is open, depending on browser/OS restrictions.
