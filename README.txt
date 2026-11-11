# GreyWater — free personal habit tracker

## What it does
- Custom habits and daily check-ins
- Streak counts
- XP and levels
- Daily quest progress and milestone badges
- 91-day activity heatmap and 7-day chart
- Local manual leaderboard
- Local browser storage, JSON export/import
- PWA manifest and service worker for home-screen/offline use

## Important limitations
- Data is stored in this browser on this device. Clearing site/browser data may erase it. Export a backup from Settings.
- The leaderboard is manual and local; it does not sync with friends.
- Notification permission does not guarantee scheduled notifications while the app is closed. Reliable closed-app reminders generally need platform/browser support beyond this simple version.
- This is a starter project; test it with non-critical data first.

## Easiest free way to put it on your Android home screen
1. Download and unzip `greywater.zip`.
2. On a computer, create a free GitHub account if you do not already have one.
3. Create a new public repository named `greywater`.
4. Upload `index.html`, `manifest.json`, `sw.js`, and `icon.svg` to the repository root.
5. In repository Settings → Pages, choose deploy from the `main` branch and root folder. Save.
6. Wait for GitHub Pages to publish the site. Open the URL GitHub gives you on your Android phone in Chrome.
7. In Chrome, open the three-dot menu and choose **Add to Home screen** or **Install app** if available.
8. Open the new home-screen icon. Add a habit and test it. Export a backup occasionally.

GitHub Pages is a free static hosting option. Your app's code is public in this setup, but personal habit data stays in your browser storage and is not sent to GitHub by this app. Do not put private information in the habit names if that concerns you.

## If you only have your phone
You can create the GitHub repository and upload files through the GitHub website in your browser, though uploading several files is more fiddly on mobile. Keep the four files together in the repository root. GitHub Pages must be enabled for the home-screen install flow to work reliably; opening `index.html` directly from Downloads may not support the PWA/offline features.

## How to use it
- Tap **Add habit** to make a custom habit.
- Tap the square on a habit to check it off or undo it.
- Visit **Progress** for heatmap and weekly stats.
- Visit **Quests & rewards** for milestones.
- Visit **Leaderboard** to manually add a friend's nickname and score.
- **Settings** lets you set your display name and export/import a JSON backup.

## XP rules
Each completed habit gives its chosen XP for that date. XP is derived from saved daily check-ins, so undoing a check-in removes that XP. The quest cards show progress and rewards conceptually; bonus quest XP is not added to total XP in this starter version.
