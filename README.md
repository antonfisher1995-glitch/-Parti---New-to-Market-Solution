# Local Event Creator — upgraded

A standalone, static-hosted event creator. It can run on GitHub Pages without Node.js, a database, or server code.

## What's upgraded
- Event information remains saved locally in this browser.
- Event photos are stored separately as image Blobs in IndexedDB, rather than embedded in event records in localStorage.
- Existing photos embedded in the older version are automatically migrated when the upgraded site first opens (if browser storage permits).
- Export a complete JSON backup containing events and photos; import that backup on another browser/device.
- Export individual event photo files to your device.
- Offline app shell cache and installable PWA manifest.
- Storage clearing controls and event/photo deletion.
- Existing GPS, Google Maps preview, location pin nudging, event fields, payment links and share flow are retained.

## Important storage note
IndexedDB is device/browser-managed storage, not an unrestricted filesystem folder. Browsers control access and storage limits. Use **Export backup** to create a file you can move elsewhere, and **Export event photos** to save image files individually. Clearing browser/site data may erase the app's local data. The backup is the portable copy.

## Run locally
Open `index.html` for basic testing. Service-worker offline features and installation require a secure origin (HTTPS or localhost), so use GitHub Pages for those features.

## Deploy with GitHub Pages
1. Create or open a GitHub repository.
2. Upload all files in this folder (not just `index.html`): `index.html`, `manifest.json`, `icon.svg`, and `sw.js`.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose your branch (usually `main`) and folder `/ (root)`, then Save.
6. Wait for the Pages URL to appear. Open it over HTTPS.
7. On mobile or desktop browsers, use the browser's install/add-to-home-screen option if available.

No npm install, build command, or GitHub Actions workflow is required for this static version.
