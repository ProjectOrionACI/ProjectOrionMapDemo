# Project Orion — Map Platform

**Applied Concepts Inc / Stalker Street Dynamics**

Interactive traffic and crash data visualization platform built on the Google Maps JavaScript API.

**[View Live Demo →](https://ProjectOrionACI.github.io/ProjectOrionMapDemo/)**

---

## Features

- **4 Map Styles** — Orion, Google, Terrain, Monochromatic — each with Dark / Light themes
- **Crash Data Layer** — Texas ZIP-level incident visualization, color-scaled by intensity
- **Layers** — Live Traffic, Weather Radar, Transit Routes
- **Marker Clustering** — Grouped location markers with per-group toggles
- **Location Detail** — Street View, elevation, reverse geocoding, popup card
- **Places Search** — Autocomplete address search with map fly-to
- **Cinematic Fly-in** — Smooth animated zoom on load
- **Access Control** — Passphrase-gated splash screen

## Tech Stack

- Vanilla HTML/CSS/JS — single file, no build step required
- Google Maps JavaScript API (vector tiles)
- Google Maps Advanced Markers
- Google Maps Places Autocomplete
- Google Maps Street View Service
- [@googlemaps/markerclusterer](https://github.com/googlemaps/js-markerclusterer)
- RainViewer API (live radar tiles)
- IBM Plex Sans / IBM Plex Mono / Orbitron (Google Fonts)

## Setup

1. Clone this repository
2. Add your Google Maps API key to `index.html`
3. Restrict your API key to your deployment domain in Google Cloud Console
4. Enable GitHub Pages: Settings → Pages → Deploy from `main` branch root

## Security

See [SECURITY.md](./SECURITY.md) for vulnerability reporting and security policy.

## Organization

Maintained by **Applied Concepts Inc** under the [ProjectOrionACI](https://github.com/ProjectOrionACI) GitHub organization.

---

*Map data © 2026 Google.*
