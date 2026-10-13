BIKE TRACKER SPORT PRO — PWA PACKAGE

FILES
- index.html: your original Bike Tracker app with PWA metadata and service-worker registration added.
- manifest.webmanifest: standalone app display and sporty icons.
- sw.js: caches the app shell for repeat/offline opening where supported.
- icon-192.png / icon-512.png: custom sporty red/graphite speedometer icons.

DEPLOY TO GITHUB PAGES
1. Create a GitHub repository.
2. Upload all five files in this folder to the repository root (not the ZIP itself).
3. Open Settings > Pages, choose deployment from the main branch and root folder, then Save.
4. Open the published HTTPS URL in Chrome on Android, then use the browser menu > Install app / Add to Home screen.

NOTES
- Installability/service workers require HTTPS (GitHub Pages provides HTTPS) or localhost.
- Existing app features and localStorage data model were preserved; browser data is stored on that device/browser and does not automatically sync to another device.
- The app loads XLSX and web fonts from external CDNs, so those particular resources may need internet access. Service-worker caching does not guarantee offline GPS/background tracking.
- GPS/trip recording while the screen is off is not guaranteed by a browser PWA; Android may suspend background browser activity.
