# Nova — PWA App Shell

A minimal, installability-focused vanilla HTML/CSS/JS mobile app shell. It includes a Web App Manifest, generated PNG/ICO artwork, iOS Home Screen metadata and guidance, an offline cache for core files, install prompt handling, and a native-feeling bottom tab bar.

## Run / deploy
Serve this directory over **HTTPS** (or `localhost` for development). A static host such as GitHub Pages is suitable. Keep `index.html`, `manifest.webmanifest`, `sw.js`, and the `icons/` directory together at the same deployment root/path. The service worker and relative manifest URLs support deployment under a subdirectory.

On Android/desktop Chrome, the custom install prompt appears when the browser fires `beforeinstallprompt` (eligibility is controlled by the browser). On iOS Safari, use **Share → Add to Home Screen**; browsers do not expose a programmatic iOS install prompt.

The external Google Fonts import is optional; the system font stack remains the fallback. Browser support and install criteria are ultimately determined by the target browser and hosting context.
