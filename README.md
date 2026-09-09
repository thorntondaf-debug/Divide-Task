# Slatted Fence Spacing Calculator (Full-Screen App)

## What's in this zip
- `index.html` — the calculator (renamed so it loads at your repo's root URL)
- `manifest.json` — makes the page installable as a full-screen app
- `sw.js` — service worker, lets it work offline once installed
- `icon-192.png` / `icon-512.png` — app icons

## Setup
1. Upload **all files** in this zip to your GitHub repo `Divide-Task`, replacing the old `Division_Calculator.html`.
2. In the repo: **Settings → Pages → Source: Deploy from a branch → main / root → Save**.
3. Wait 1–2 minutes, then visit:
   `https://thorntondaf-debug.github.io/Divide-Task/`

## Installing as a full-screen app
- **iPhone (Safari):** open the link → Share icon → **Add to Home Screen**
- **Android (Chrome):** open the link → ⋮ menu → **Install app** (or **Add to Home Screen**)

Once installed, tapping the icon opens it full-screen — no browser bar — and it'll keep working even offline.

## Improvements made to the code
- Added a warning message when the entered slat width/gap/setbacks don't physically fit (previously it would silently show a negative or wrong gap).
- Guarded against divide-by-zero if slat width and gap are both 0.
- Made the layout stack vertically on very small phone screens.
- Added safe-area padding so content isn't hidden behind the iPhone notch/home bar in full-screen mode.
- Added the PWA files above so it can run as a real app instead of just a webpage.
