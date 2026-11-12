# Local Event Creator (GitHub Pages)

This is a simple, single-page event creator. Event records and photos are stored in the browser's local storage on the device that created them. There is no event database, login, cloud upload, Bluetooth feature, or server-side event publishing.

## Put it on GitHub Pages (step by step)

1. Sign in at https://github.com/.
2. Click the **+** button near the top-right, then choose **New repository**.
3. Give the repository a name, for example `my-event-creator`.
4. Choose **Public** (or use a plan/settings combination that supports Pages for a private repository).
5. Click **Create repository**.
6. On the repository page, click **Add file** → **Upload files**.
7. Unzip this downloaded ZIP on your computer.
8. Drag the file named **index.html** from the unzipped folder into the GitHub upload area. You can also upload `README.md`.
9. Scroll down and click **Commit changes**.
10. In the repository, click **Settings** → **Pages**.
11. Under **Build and deployment**, choose **Deploy from a branch**.
12. Set the branch to **main** and the folder to **/(root)**, then click **Save**.
13. Wait a minute or two. Refresh the Pages settings screen; GitHub will show your website address. It will look like `https://YOUR-USERNAME.github.io/my-event-creator/`.
14. Open that address on your phone or computer.

## Important notes

- Use the website over HTTPS (GitHub Pages does this). Browser GPS and the native share sheet generally require HTTPS and a supported browser.
- The map preview uses Google Maps' embed page and needs internet access. The app itself does not send your event record to Google; the map frame requests map content for the coordinates/place you entered.
- GPS accuracy is supplied by the device/browser and is only an estimate. The nudge buttons move the pin by the chosen distance; they do not make the GPS reading more accurate. Longitude step size is adjusted for latitude.
- The default nudge is **3.3 feet (about 1 meter)**. You can change it before pressing North, South, East, or West.
- The native share sheet may share the photo and event text together on supported devices/browsers. If image sharing is unsupported, it shares the text instead. Availability varies by browser and operating system.
- Local storage is tied to the browser and device. It is not automatically synced between devices and may be cleared by browser settings. Sharing is the way to send an event to someone else.
- Photos are resized before being saved to help reduce browser storage use.
