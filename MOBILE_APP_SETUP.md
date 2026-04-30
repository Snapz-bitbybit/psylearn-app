# PSYLEARN Mobile App Setup

This version has been prepared as a Progressive Web App (PWA). It can be opened on Android and iPhone and installed to the Home Screen like an app.

## Option A: Use as a phone app through browser

1. Host the project online using Vercel, Netlify, Firebase Hosting, GitHub Pages, or any web hosting service.
2. Open the hosted link on the phone.
3. Android: open Chrome > menu > Add to Home Screen / Install App.
4. iPhone: open Safari > Share button > Add to Home Screen.

After installation, PSYLEARN will open in a standalone app-like window.

## Option B: Turn into Android/iOS native wrapper using Capacitor

Run these commands after installing the project dependencies:

```bash
npm install
npm run build
npm install @capacitor/core @capacitor/cli @capacitor/android @capacitor/ios
npx cap init PSYLEARN com.psylearn.quizapp --web-dir=dist
npx cap add android
npx cap add ios
npx cap sync
```

Android:
```bash
npx cap open android
```
Then build APK/AAB in Android Studio.

IOS:
```bash
npx cap open ios
```
Then build using Xcode on macOS.

## Notes

- The app is portrait-first and mobile-ready.
- PWA manifest and icons have been added.
- Service worker has been added for basic offline caching.
- For iOS App Store, you need Apple Developer account and Xcode.
- For Google Play Store, you need Google Play Console and Android Studio.
