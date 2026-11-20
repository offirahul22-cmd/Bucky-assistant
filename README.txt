BUCKY 0.2 — PHONE-FIRST PROTOTYPE

Files:
- index.html: assistant interface and offline commands
- sw.js: offline cache for a hosted HTTPS install
- manifest.webmanifest: installable web-app metadata

Quick test on Android:
1. Open index.html in Chrome or another compatible browser.
2. Try Speak, Time, Date, 'remember buy milk', and 'show my notes'.
3. Notes are saved in this browser's local storage.

For full offline/PWA installation, these files must be hosted on an HTTPS site; service workers do not run from a file:// URL. You can still test the basic page locally, but speech recognition depends on browser support and may need internet.

NOT YET IMPLEMENTED:
- online AI backend
- always-on wake word
- reliable background reminders
- native Android app controls

Security: never put an API key, password, or OTP in index.html. Online AI must be connected through a secure backend.
