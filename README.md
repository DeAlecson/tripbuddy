# TripBuddy · Boracay Jun 2026

Mobile-first travel companion web app for a group trip to Boracay, Philippines (22–26 June 2026).

A single self-contained `index.html` — no build step, no dependencies to install, no server. Open it in a browser or deploy it anywhere static.

## Features

- 🗺 **Map** — Leaflet + OpenStreetMap, colour-coded markers (Food / POI / Watersports zones), GPS locate-me, layer toggles
- 🍴 **Food** — 35 restaurants with search, meal-type filters, sort by Station / Price / Nearest
- 📍 **POI** — 26 spots with "Your Picks" pinned at top, category filters
- 🌊 **Watersports** — 18 activities, walk-up beach rates
- ⚙️ **Settings** — currency toggle (PHP · SGD · USD · CAD), location toggle, persisted in localStorage
- 📲 Bottom sheet with swipe-to-dismiss, Navigate (Google Maps deeplink), Copy Address

## Run locally

GPS only works on `https://` or `localhost`, not `file://`. Use any static server:

```bash
python -m http.server 8000
# or
npx serve
```

Then open `http://localhost:8000`.

## Deploy

- **Vercel** — `vercel` then `vercel --prod` from this folder
- **GitHub Pages** — Settings → Pages → Source: main branch / root
- **Anywhere static** — drop `index.html` on any host

## Stack

Vanilla HTML/CSS/JS · Leaflet 1.9.4 (CDN) · OpenStreetMap tiles · Google Fonts (Syne + DM Sans)
