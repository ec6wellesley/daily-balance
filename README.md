# Daily Balance — web app

A mobile-friendly sage-and-cream calorie, activity, and weight tracker.

## Included
- Quick food list and free-text meal estimates (simple heuristics, not AI or a full nutrition database)
- Manual step and exercise entries
- Editable placeholder baseline energy estimate
- Optional weight log and basic change summary
- Local-device storage, JSON export, delete-all-data option
- PWA manifest, service worker, and app icons

## Important limitations
- This is a prototype, not a medical device or nutrition advice.
- Calories burned and consumed are estimates; the baseline defaults to 1,800 kcal and should not be treated as personalized.
- Step burn uses a rough 0.04 kcal/step approximation. Exercise and steps can overlap, so avoid double counting.
- It does not integrate with Apple Health. Automatic HealthKit access requires a native iOS app and explicit permissions.
- Data is stored in the browser's local storage on that device/browser. It is not synced to another device and can be lost if browser data is cleared. Export backups from Insights.

## Quick test on a computer
Open `index.html` in a modern browser. Some install/offline features require HTTPS or localhost.

## Host it free using GitHub Pages
1. Create or sign into a GitHub account.
2. Create a new public repository, e.g. `daily-balance`.
3. Upload all files in this folder to the repository root (`index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`).
4. In the repository, open **Settings → Pages**.
5. Under build/deployment, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
6. Wait for GitHub to publish the site. The URL will look like `https://YOUR-USERNAME.github.io/daily-balance/`.
7. Open that HTTPS URL in Safari on your iPhone.

## Add to iPhone Home Screen
1. Open the published website in **Safari** (not an in-app browser).
2. Tap **Share** (the square with an upward arrow).
3. Scroll and tap **Add to Home Screen**. If shown, enable **Open as Web App**.
4. Tap **Add**. The Daily Balance icon will appear on your Home Screen.

## Data and privacy
Entries stay in local browser storage on the device unless you export them. Do not use a shared device if you want the entries private. This project does not send entries to a server.
