# Lithuanian Vocabulary Practice App (PWA Version)

## What is this?

This is a Progressive Web App (PWA) version of the Lithuanian vocabulary practice app. It can be installed on your phone like a native app!

## Files Included

1. **index.html** - The main app file
2. **manifest.json** - Tells phones how to install the app
3. **service-worker.js** - Enables offline functionality
4. **icon-192.png** - App icon (small)
5. **icon-512.png** - App icon (large)

## How to Install on Your Phone

### Android (Chrome):
1. Open the app URL in Chrome
2. Look for the "Add to Home screen" prompt at the bottom
3. Tap "Add" or "Install"
4. The app icon will appear on your home screen
5. Tap it to open - it will look like a real app!

### iPhone (Safari):
1. Open the app URL in Safari
2. Tap the Share button (square with arrow pointing up)
3. Scroll down and tap "Add to Home Screen"
4. Tap "Add" in the top right
5. The app icon will appear on your home screen
6. Tap it to open!

### Desktop (Chrome/Edge):
1. Open the app URL
2. Look for the install icon in the address bar (⊕ or computer icon)
3. Click it and click "Install"
4. The app will open in its own window

## Features

✅ Works offline after first load
✅ Installs like a native app
✅ No app store needed
✅ Free forever
✅ Works on all devices

## For Testing

After deploying to GitHub Pages, your students can access it at:
`https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

## Updating the App

When you update the files on GitHub:
1. Students just need to refresh the app
2. Or close and reopen it
3. The service worker will automatically update

## Troubleshooting

**App won't install?**
- Make sure you're using HTTPS (GitHub Pages does this automatically)
- Try refreshing the page first
- Some browsers require you to visit the page multiple times before showing install prompt

**App not updating?**
- Close the app completely
- Clear browser cache
- Reopen the app

## Technical Notes

- Cache version: v1 (update CACHE_NAME in service-worker.js to force updates)
- Icons: Simple "LT" design in indigo (#4F46E5)
- Works offline: Yes (after first visit)
