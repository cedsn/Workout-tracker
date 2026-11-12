# Workout Tracker PWA

A minimal, English-language, offline-first workout tracker for iPhone.

## Features
- Create, rename, edit and delete workout templates
- Add, rename, remove and reorder exercises (drag and drop)
- Log one current weight per exercise (no sets or reps)
- Previous completed weight displayed inline as a read-only value
- Separate workout history screen
- JSON backup import/export and CSV history export
- Local device storage; no account, analytics, or network calls by the app
- kg/lbs display setting

## Deploy
A Progressive Web App must be opened from a secure HTTPS address at least once to install and cache its files. GitHub Pages is a free option:

1. Create a GitHub account and a new public repository (for example `workout-tracker`).
2. Upload all files in this folder to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Wait for the Pages URL, usually `https://YOUR-USERNAME.github.io/workout-tracker/`.
6. On iPhone, open that URL in **Safari**, tap **Share → Add to Home Screen → Add**.
7. Launch the new home-screen icon once while online. The service worker caches the app shell; after that, the app works offline.

## Data
Workout data is stored in the browser's local storage on the iPhone. Use Settings → Export backup regularly. Import replaces the current local workouts and history, so export first if you want to keep both.

## Notes
- Use Safari for installation on iPhone.
- The app does not sync between devices.
- Removing website data or uninstalling the web app may remove locally stored workouts. Keep backups.
- This is a PWA package, not an App Store-signed native app.
