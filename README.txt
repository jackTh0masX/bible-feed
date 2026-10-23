THE BIBLE FEED — PWA PACKAGE

FILES
- index.html: app, install prompt, and service-worker registration
- manifest.webmanifest: install name, icons, and standalone display settings
- sw.js: offline app-shell caching and cached Bible API responses
- icons/: install icons

INSTALL ON ANDROID
1. Upload the contents of this folder to an HTTPS host. Keep the folder structure intact.
2. Open the hosted URL in Chrome on Android.
3. Tap Install app if shown, or Chrome menu (⋮) → Install app / Add to Home screen.
4. Launch it from the new home-screen icon.

HOSTING
GitHub Pages, Netlify, and Cloudflare Pages can host this static folder. No build step or database is required.

OFFLINE
The app shell is cached after the first successful visit. Previously fetched Bible API responses can be served offline; uncached passages still need a connection. Likes, saved verses, comments, and settings remain in that browser's local storage.

IMPORTANT
The app is local-first. Simulated live updates and character replies are not synchronized across users. For installability and service workers, use HTTPS (localhost is the development exception).
