Elevor360D Image Editor & Resizer V1
===================================
GitHub Pages installation:
1. Create a public repository, e.g. Elevor360D-Image-Editor-Resizer.
2. Upload the CONTENTS of this ZIP (index.html, app.js, sw.js, icon.svg, manifest.webmanifest, advert.json and adverts folder) into the repository root.
3. Settings > Pages > Deploy from a branch > main / (root) > Save.
4. Open https://YOUR-USERNAME.github.io/REPOSITORY-NAME/ in Chrome or Edge.
5. Use Install App when offered, or browser menu > Install app / Add to Home Screen.

Advertising:
Edit advert.json to enable/disable, change title/text/url, and set image filename.
Place the image in adverts/ and set e.g. "image":"my-ad.jpg".
After changes, update the service-worker CACHE version to ensure returning offline users get updates.

This is an original, browser-only implementation. No proprietary Slim plugin files are bundled.
All editing occurs locally on the user's device. There are no server uploads or user accounts.

Notes:
- The crop frame ratio and output width/height are independently adjustable if the aspect lock is disabled; non-matching values can stretch the output. Keep lock enabled for normal use.
- Browser image format support varies. JPG, PNG and WebP exports rely on browser canvas support.
- Some mobile browsers may limit very large output images.

V1.3 INSTALL UPDATE
- Android Chrome opens its native installation prompt when Chrome provides beforeinstallprompt.
- If Chrome does not provide the event, the app cannot force the native popup. Open the direct GitHub Pages URL in Chrome, then use Chrome menu > Install app.
- The service worker uses network-first navigation so updates are less likely to be stuck behind a previous cached page.
- Upload ALL files from this ZIP, replacing the older versions.
