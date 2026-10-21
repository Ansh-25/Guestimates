# Guesstimate Cheat Sheet

An interactive single-page cheat sheet for Indian market-sizing and estimation interviews.

## Run locally
Open `index.html` in a browser. The Chart.js visualisations load from a CDN, so an internet connection is needed for charts when the browser has not cached that library.

## Publish with GitHub Pages
1. Create a GitHub repository (for example, `guesstimate-cheat-sheet`).
2. Upload the **contents** of this folder to the repository root. `index.html` must be at the root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`, then save.
6. After deployment, open the URL shown in the Pages settings.

## Install as an app
- **Android (Chrome):** open the published site and choose **Install app** or **Add to Home screen** from the browser menu.
- **Windows (Chrome/Edge):** use the install icon in the address bar or the browser menu.
- **iPhone/iPad (Safari):** Share → Add to Home Screen.

The manifest supplies the app name and icon. The service worker caches the app shell for basic offline reopening; the Chart.js library is external, so charts may not render offline until that library is available in the browser cache.

## Included files
- `index.html` — the original cheat sheet, configured as the site homepage
- `manifest.json` — install metadata
- `service-worker.js` — app-shell caching
- `icons/` — install and browser icons
- `LICENSE` — MIT license

## Note on figures
The estimation benchmarks and statistics are included as supplied in the original cheat sheet. Treat them as interview assumptions and verify time-sensitive figures before relying on them in a real-world analysis.
