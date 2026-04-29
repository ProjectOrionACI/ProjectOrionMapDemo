# Project Orion — Map Platform

**Applied Concepts Inc / Stalker Street Dynamics**

Interactive traffic and crash data visualization platform built on the Google Maps JavaScript API.

**[View Live Demo →](https://ProjectOrionACI.github.io/ProjectOrionMapDemo/)**

---

## Features

- **4 Map Styles** — Orion, Google, Terrain, Monochromatic — each with Dark / Light themes
- **Crash Data Layer** — Real Texas ZIP-level incident counts, color-scaled by intensity
- **Layers** — Live Traffic, Weather Radar, Transit Routes, Bike Lanes
- **Marker Clustering** — Grouped location markers with per-group toggles
- **Location Detail** — Street View panorama, elevation, reverse geocoding, popup card
- **Places Search** — Autocomplete address search with map fly-to
- **Cinematic Fly-in** — Smooth animated zoom on load
- **Access Control** — Passphrase-gated splash screen

## Map IDs

| Style | Map ID |
|-------|--------|
| Orion | `fd49d1035c87f47ce253f8de` |
| Google | `dcac3fd0ea6fb9c7` |
| Mono | `fd49d1035c87f47c13020651` |

## Setup

1. Import or push this repository under `ProjectOrionACI/ProjectOrionMapDemo`
2. Enable GitHub Pages: Settings → Pages → Deploy from `main` branch root
3. Add `ProjectOrionACI.github.io/*` to your API key's authorized referrers in Google Cloud Console
4. Site will be live at `https://ProjectOrionACI.github.io/ProjectOrionMapDemo/`

## Changing the Access Passphrase

Default passphrase is `orion2025`. To change it:

1. Open `index.html`
2. Find: `if (hashPass(val) === hashPass('orion2025'))`
3. Replace `orion2025` with your new passphrase
4. Push the change

## Security

See [SECURITY.md](./SECURITY.md) for vulnerability reporting.

---
*Map data © 2026 Google. Crash data: ZIP-level incident aggregation, Texas focus.*
