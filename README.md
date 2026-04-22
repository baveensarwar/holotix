# HoloTix

Interactive 3D holographic concert tickets — a Progressive Web App.

Built for the **Yousuke Yukimatsu** show at Celebrities Nightclub, Vancouver. April 15, 2026.

## Features

- Three floating tickets in **Spanish**, **English**, and **French**
- Holographic foil surface with cursor/gyroscope-reactive shine and glow
- Tap to flip with smooth 1s 3D animation
- Tilt your phone to shift the 3D perspective (uses DeviceOrientation API)
- Installable on iPhone as a standalone app (PWA)
- Offline support via service worker
- Safe area support for Dynamic Island / notch

## Install on iPhone

1. Deploy to [Netlify Drop](https://app.netlify.com/drop) or GitHub Pages
2. Open the URL in **Safari** on your iPhone
3. Tap **Share → Add to Home Screen**
4. Launch from your home screen — runs full-screen like a native app

## Deploy to GitHub Pages

```bash
# in repo settings → Pages → Source: Deploy from branch → main → / (root)
```

Or use Netlify: drag the project folder into [app.netlify.com/drop](https://app.netlify.com/drop).

## Tech

Single `index.html` with inline CSS/JS. No build step, no dependencies.

- CSS `conic-gradient` + `mix-blend-mode` for holographic foil
- CSS `perspective` + `transform-style: preserve-3d` for 3D tilt
- `DeviceOrientationEvent` for iPhone gyroscope
- Service Worker for offline caching
- Web App Manifest for PWA install

## Credits

Design by **Bavin Abdulrahman**
