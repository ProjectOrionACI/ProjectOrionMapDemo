# Project Orion — Map Platform

**Applied Concepts Inc / Stalker Street Dynamics**

Interactive traffic and crash data visualization platform built on the Google Maps JavaScript API.

**[View Live Demo →](https://ProjectOrionACI.github.io/ProjectOrionMapDemo/)**

---

## Features

### Map Styles & Themes
- **4 Map Styles** — Orion, Google, Terrain, Monochromatic
- **Dark / Light themes** per style
- **Map Types** — Roadmap, Hybrid, Satellite

### Data Layers
- **Live Traffic** — real-time traffic flow overlay
- **Transit** — public transit route network with purple tint
- **Crash Data** — Texas ZIP-level incident markers, pulsing and color-scaled by intensity
- **Air Quality** — live AQI readings across Dallas metro (Google Air Quality API)
- **Weather Alerts** — active NOAA severe weather polygons for Texas, click for details

### Location Intelligence
- **Street View** — thumbnail in popup, full-screen launch from marker or right-click
- **Elevation** — meters and feet for any selected location
- **Reverse Geocoding** — address lookup on marker click
- **Solar Potential** — annual sunshine hours from Solar API on marker click
- **Crash Statistics** — popup with collision type breakdown, fatal/injury rates, and contributing factors on crash dot click

### Map Interaction
- **Right-click context menu** — Street View, Measure Distance, Print
- **Measure tool** — click to place points, running total in miles and kilometers
- **Print** — sidebar hidden, map fills page
- **Places Search** — autocomplete address/location search with fly-to
- **Marker clustering** — grouped location markers with per-group toggles

### UI & Access
- **Passphrase-gated splash screen** — with terminal lockout sequence on 3 failed attempts
- **Version number** — displayed on login screen and top-right header
- **Cinematic intro** — US overview on load, snaps to Dallas cluster
- **Popup card** — street view thumbnail, address, elevation, group, status per marker
- **Activity log** — real-time event log in sidebar
- **API call limits** — Air Quality and Weather layers auto-disable after 10 calls per session

## Tech Stack

- Vanilla HTML/CSS/JS — single file, no build step required
- Google Maps JavaScript API (vector tiles, Advanced Markers, Geometry library)
- Google Air Quality API
- Google Solar API
- Google Places Autocomplete (PlaceAutocompleteElement)
- Google Street View Service
- NOAA Weather Alerts API (free, no key required)
- IBM Plex Sans / IBM Plex Mono / Orbitron (Google Fonts)

## Required Google Cloud APIs

Enable all of the following in Google Cloud Console → APIs & Services → Library:

- Maps JavaScript API
- Places API
- Geocoding API
- Elevation API
- Air Quality API
- Solar API
- Street View Publish API

## Setup

1. Clone this repository
2. Add your Google Maps API key to `index.html`
3. Restrict your API key to your deployment domain in Google Cloud Console
4. Enable all required APIs listed above
5. Enable GitHub Pages: Settings → Pages → Deploy from `main` branch root

## Security

The API key in this repository is restricted to the authorized deployment domain only. See [SECURITY.md](./SECURITY.md) for vulnerability reporting and security policy.

---

*Map data © 2026 Google. Crash data: ZIP-level incident aggregation, Texas focus.*
