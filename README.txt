# Inventory & Sales (PWA)
This folder contains a GitHub Pages–ready version of your app.

## Files
- `index.html` — the app
- `manifest.json` — PWA manifest
- `service-worker.js` — offline caching
- `icons/` — app icons (192px, 512px)
- `.nojekyll` — ensures GitHub Pages serves files as-is

## Deploy on GitHub Pages
1. Create a new repo (or use an existing one).
2. Upload all files in this folder to the repo root (drag & drop on github.com or push via git).
3. In **Settings → Pages**, set **Source** to **Deploy from a branch**, choose **main** branch and folder **/** (root). Save.
4. Wait ~1–2 minutes, then open: `https://<YOUR-USERNAME>.github.io/<REPO>/`
5. On Android/Chrome you'll see `Install App`. On iOS: Share → Add to Home Screen.

## Update the app later
- Edit files and push again.
- Bump the cache name in `service-worker.js` (e.g., `inv-app-v3`) when you change core files so clients fetch the new version.
- If you see an old version, refresh twice or clear site data to evict old caches.

## Data & backups
- Your data is stored **locally on each device** (browser storage).
- To move data: **Settings → Data Backup → Export All (JSON)** on device A, then **Restore (Replace)** on device B.
