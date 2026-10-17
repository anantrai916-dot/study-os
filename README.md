# STUDY_OS — JEE Focus Planner

A mobile-first, Japanese night-themed gamified study planner built as a Progressive Web App (PWA). Designed around a Class 12 JEE workflow: Aakash Class 12 work is primary, Vedantu Eklavya Class 11 backlog is secondary, with a 30-minute focus / 7-minute break cycle.

## Features implemented
- Responsive dark UI with Japanese-inspired night palette and sakura accents.
- Home, Quests, Planner and Stats views.
- Add/check custom quests; XP and level calculation.
- Editable daily routine.
- 30-minute focus / 7-minute break timer with pause, reset and skip.
- Progress, quests and routine saved in browser `localStorage`.
- Export a plain-text session summary.
- PWA manifest, app icon and service worker for installability/offline shell.
- Optional generated ambient tone; external link for lofi radio.

## Honest limitations
- No account, cloud sync, push notifications, real historical analytics or verified daily streak tracking.
- Ambient tone is not a lofi music track; the lofi link opens YouTube search.
- Timer reliability depends on browser/app lifecycle; background throttling may pause or delay it.
- The hero background image loads from Unsplash and therefore may not appear offline.
- This repository is a PWA, not a native APK.

## Run locally
Because service workers require localhost or HTTPS, use a local static server instead of opening `index.html` directly.

For example, if Python is installed:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000` in your browser.

## Install on Android
1. Deploy the project to an HTTPS static host (for example GitHub Pages).
2. Open the deployed URL in Chrome on Android.
3. Use the browser menu and choose **Install app** or **Add to Home screen** (wording varies).
4. For best offline behavior, open the app once while online.

## Deploy with GitHub Pages
1. Create a public repository named `study-os`.
2. Upload all files from this folder to the repository root.
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**, choose `main` and `/(root)`, then save.
5. Wait for the deployment URL to appear and open it on your phone.

## Portfolio improvements to build next
- Unit tests and accessibility checks.
- Subject/chapter backlog import and due dates.
- Actual day-by-day analytics with a local date model.
- Optional backend sync and authentication.
- Custom original illustration/music assets and a clear privacy policy.

## Tech
HTML · CSS · Vanilla JavaScript · Web App Manifest · Service Worker · localStorage
