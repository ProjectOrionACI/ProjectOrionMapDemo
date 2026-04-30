# Project Orion — Map Platform

**Applied Concepts Inc / Stalker Street Dynamics**

Interactive traffic and crash data visualization platform built on the Google Maps JavaScript API.

**[View Live Demo →](https://ProjectOrionACI.github.io/ProjectOrionMapDemo/)**

---

## Features

### Map Styles & Themes
- **4 Map Styles** — Orion, Google, Terrain, Monochromatic
- **Dark / Light themes** per style
- **Map Types** — Roadmap, Hybrid (Google style only)

### Data Layers
- **Live Traffic** — real-time traffic flow overlay
- **Transit** — public transit route network
- **Crash Data** — Texas ZIP-level incident markers, pulsing and color-scaled by intensity
- **Air Quality** — live AQI readings across Dallas metro (Google Air Quality API)
- **Weather Alerts** — active NOAA severe weather polygons for Texas, click for details

### Location Intelligence
- **Street View** — thumbnail in popup, full-screen launch from marker or right-click
- **Elevation** — meters and feet for any selected location
- **Reverse Geocoding** — address lookup on marker click
- **Speed Limit** — Roads API lookup shown in Map Status on marker click
- **Solar Potential** — annual sunshine hours from Solar API on marker click

### Map Interaction
- **Right-click context menu** — Street View, Measure Distance, Print
- **Measure tool** — click to place points, running total in miles and kilometers
- **Print** — sidebar hidden, map fills page
- **Places Search** — autocomplete address/location search with fly-to
- **Long description** — marker clustering with group toggles

### UI
- **Access control** — passphrase-gated splash screen with terminal lockout on 3 failed attempts
- **Cinematic intro** — US overview on load, snaps to Dallas cluster
- **Popup card** — street view, address, elevation, group, status per marker
- **Activity log** — real-time event log in sidebar
- **API call limits** — layers auto-disable after 10 calls per session

## Tech Stack

- Vanilla HTML/CSS/JS — single file, no build step required
- Google Maps JavaScript API (vector tiles, Advanced Markers, Geometry)
- Google Air Quality API
- Google Roads API
- Google Solar API
- Google Places Autocomplete & Street View
- NOAA Weather API (free, no key required)
- IBM Plex Sans / IBM Plex Mono / Orbitron (Google Fonts)

## Setup

1. Clone this repository
2. Add your Google Maps API key to `index.html`
3. Restrict your API key to your deployment domain in Google Cloud Console
4. Enable required APIs: Maps JS, Places, Air Quality, Roads, Solar, Geocoding, Elevation
5. Enable GitHub Pages: Settings → Pages → Deploy from `main` branch root

## Security

See [SECURITY.md](./SECURITY.md) for vulnerability reporting and security policy.

---

*Map data © 2026 Google. Crash data: ZIP-level incident aggregation, Texas focus.*
