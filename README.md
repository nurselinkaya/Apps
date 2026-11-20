# December Challenge — PWA package

This package converts the standalone December Challenge v2.0 into a Progressive Web App (PWA) while preserving its original app design and content.

## Files
- `index.html` — the app (images and code remain embedded)
- `manifest.json` — app identity and install settings
- `service-worker.js` — offline app-shell caching
- `icons/` — home-screen icons

## Publish using GitHub Pages
1. Create a **public** GitHub repository (for example `december-challenge`).
2. Upload all files and folders in this package to the repository root. Ensure the main file is named `index.html`.
3. In the repository, open **Settings → Pages**. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
4. Wait for the deployment and open the published URL.
5. Test on iPhone using **Safari**: open the URL → Share → **Add to Home Screen**.

## Offline behavior
The service worker caches the app shell after the first successful online visit. Open the website once while online before relying on offline use.

## Progress storage
Challenge progress is stored in the browser's local storage. It is not synced across devices and can be lost if browser website data is cleared.

## Note
GitHub Pages serves this repository publicly. The app source files are viewable by visitors. This is intended for personal, non-commercial sharing.
