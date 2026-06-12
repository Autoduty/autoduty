# AutoDuty — Deployment Guide

## What's in this folder
- `index.html` — the complete AutoDuty app (everything in one file)
- `manifest.json` — makes it installable as a PWA on iOS/Android
- `netlify.toml` — Netlify configuration
- `icon-192.png` / `icon-512.png` — add your own app icons (optional)

---

## Deploy to Netlify (free, ~2 minutes)

1. Go to **netlify.com** and sign up / log in (free account)
2. From the dashboard click **"Add new site" → "Deploy manually"**
3. Drag this entire folder onto the upload area
4. Netlify gives you a URL like `https://autoduty-abc123.netlify.app`
5. Optionally rename it under Site Settings → change site name to `autoduty`

That's it — your app is live.

---

## Install on pilots' phones

### iPhone / iPad (Safari)
1. Open the app URL in Safari
2. Tap the **Share** button (box with arrow)
3. Scroll down → tap **"Add to Home Screen"**
4. Tap **Add** — AutoDuty appears on the home screen like a native app

### Android (Chrome)
1. Open the app URL in Chrome
2. Tap the three-dot menu → **"Add to Home Screen"**
3. Tap **Add**

---

## First-time setup (done once, on one device)

1. Open AutoDuty and tap the **Settings** gear icon
2. Paste your **Anthropic API key** (from console.anthropic.com)
3. Paste the full contents of your **Google Service Account JSON key file**
4. Tap **Save & Continue**

The app is ready. Keys are stored locally on the device only.

---

## Google Sheet setup reminder
- Sheet ID already configured: `1yRzA5gfDKpjMPuvtEA-m74ZJGfDMLcgiTgzokKBI2rM`
- Make sure the sheet is shared with your service account email (Editor access)
- Each pilot must have a tab named exactly: Colin, Jack, Zach, Liam, Jim

---

## Updating the app
To update (new features, bug fixes):
1. Get the new `index.html` from your developer
2. Go to netlify.com → your site → **Deploys** tab
3. Drag the new file onto the deploy area — live in seconds
