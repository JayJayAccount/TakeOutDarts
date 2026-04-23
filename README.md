# Take-Out Darts - Progressive Web App

A fullscreen Progressive Web App optimized for Samsung Galaxy S25 that runs without borders and address bar.

## Installation on Samsung Galaxy S25

### Method 1: Chrome/Samsung Internet Browser
1. Open this website in **Chrome** or **Samsung Internet**
2. You should see an "Install" or "Add to Home screen" prompt
3. Tap the prompt to install
4. The app will launch in fullscreen mode without the address bar

### Method 2: Manual Installation
1. Open the website in Chrome or Samsung Internet
2. Tap the **three-dot menu** (⋮)
3. Select **"Install app"** or **"Add to Home screen"**
4. Confirm installation

## Features

✅ **Fullscreen Mode** - No address bar or borders on Samsung Galaxy S25  
✅ **Offline Support** - Works without internet connection via Service Worker  
✅ **Immersive Experience** - Notch/safe area aware  
✅ **Portrait Lock** - Prevents accidental rotation  
✅ **Fast Loading** - Cached assets load instantly  
✅ **App-like Feel** - Standalone display mode  
✅ **Touch Optimized** - Full Samsung Galaxy S25 gesture support

## Technical Details

### PWA Components
- **manifest.json** - Defines app metadata and fullscreen display
- **sw.js** - Service Worker for offline caching
- **index.html** - Progressive enhancement with responsive design
- **.htaccess** - Apache server configuration for proper MIME types
- **web.config** - IIS server configuration

### Display Modes
- **Fullscreen**: No address bar or system UI (supported on Android)
- **Standalone**: App-like experience with minimal system UI
- **Portrait Primary**: Locked to portrait orientation

### Caching Strategy
- Service Worker caches all resources
- Offline fallback for network errors
- Auto-updates when manifest.json changes

## Browser Support

✅ Chrome 67+  
✅ Samsung Internet 6+  
✅ Firefox 58+ (Android)  
✅ Edge 79+ (Android)  
❌ Safari (iOS - uses Apple's PWA implementation)

## Deployment

1. Upload all files to your web server
2. Ensure HTTPS is enabled (required for PWA)
3. Visit the site from Samsung Galaxy S25
4. Install using the browser prompt or manual method above

## Troubleshooting

**App not installing?**
- Make sure you're using HTTPS
- Check browser is Chrome or Samsung Internet
- Clear browser cache and try again

**Fullscreen not working?**
- Grant all permissions when prompted
- Make sure manifest.json has `"display": "fullscreen"`
- Try tapping the screen to trigger fullscreen request

**Offline not working?**
- Ensure service worker is registered (check DevTools)
- Clear app cache and reinstall
- Check server MIME types are configured correctly

## Support

For issues or suggestions, please check:
- Browser Console (DevTools)
- Application tab (Service Worker status)
- Manifest tab (PWA configuration)

---

**Built for Samsung Galaxy S25** - Works with Chrome, Samsung Internet, and other Chromium-based browsers on Android.
