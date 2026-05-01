# Project Orion Map Demo

**Applied Concepts Inc / Stalker Street Dynamics**  
Created by DJ

Interactive traffic and crash data visualization platform built on the Google Maps JavaScript API.

[View Live Demo →](https://projectorionaci.github.io/ProjectOrionMapDemo/)

---

## Features

### Map Styles & Themes
- **4 Map Styles** — Orion, Google, Terrain, Monochromatic — each with Dark / Light themes
- **Map Types** — Roadmap, Hybrid, Satellite

### Data Layers
- **Live Traffic** — real-time traffic flow overlay
- **Transit** — public transit route network
- **Crash Data** — Texas ZIP-level incident markers, pulsing and color-scaled by intensity, with statistics popup on click
- **Weather** — combined NOAA severe weather alerts + Google Weather current conditions
- **Air Quality** — live AQI readings across Dallas metro

### Infrastructure Layers
- **Hospitals** — hospital locations across Dallas metro (OpenStreetMap)
- **Fire Stations** — fire station locations
- **Police** — police stations and precincts
- **Schools** — all schools in the metro area
- **EMS** — ambulance stations
- **Rail Crossings** — railroad level crossings
- **Earthquakes** — last 30 days of seismic activity in Texas (USGS)

### Location Intelligence
- **Street View** — windowed panorama viewer with title bar, address, expand and close controls
- **Elevation** — meters and feet for any selected location
- **Reverse Geocoding** — address lookup on marker click
- **Solar Potential** — annual sunshine hours from Solar API on marker click
- **Crash Statistics** — collision types, fatal/injury rates, contributing factors per ZIP zone

### Map Interaction
- **Right-click context menu** — Street View, Measure Distance, Print
- **Measure tool** — fixed-pixel dots and dashed line, live waypoint panel showing start, end, intermediate points and running distance
- **Print** — sidebar hidden, map fills page
- **Places Search** — autocomplete address/location search with fly-to
- **Marker clustering** — grouped location markers with per-group toggles

### UI & Access
- **Passphrase-gated splash screen** — terminal lockout sequence on 3 failed attempts
- **Version number** — displayed on login screen and top-right header
- **Cinematic intro** — US overview on load, snaps to Dallas cluster
- **Popup card** — street view thumbnail, address, elevation, group, status per marker
- **Activity log** — real-time event log in sidebar
- **Global API call limit** — 50 calls per session across all external APIs

## Tech Stack

- Vanilla HTML/CSS/JS — single file, no build step required
- Google Maps JavaScript API (vector tiles, Advanced Markers, Geometry library)
- Google Air Quality API
- Google Solar API
- Google Weather API
- Google Places Autocomplete (PlaceAutocompleteElement)
- Google Street View Service and Geocoding API
- Google Elevation API
- NOAA Weather Alerts API (free, no key required)
- OpenStreetMap Overpass API (free, no key required)
- USGS Earthquake Feed (free, no key required)
- IBM Plex Sans / IBM Plex Mono / Orbitron (Google Fonts)

## Required Google Cloud APIs

Enable the following in Google Cloud Console → APIs and Services → Library:

- Maps JavaScript API
- Places API
- Geocoding API
- Elevation API
- Air Quality API
- Solar API
- Weather API
- Street View Static API
- Street View Publish API

## Setup

1. Clone this repository under `ProjectOrionACI/ProjectOrionMapDemo`
2. Add your Google Maps API key to `index.html`
3. Restrict your API key to `projectorionaci.github.io/*` in Google Cloud Console
4. Enable all required APIs listed above
5. Enable GitHub Pages: Settings → Pages → Deploy from `main` branch root

## Security

The API key in this repository is restricted to the authorized deployment domain only.  
See [SECURITY.md](./SECURITY.md) for vulnerability reporting and security policy.

---

*Map data © 2026 Google. Crash data: ZIP-level incident aggregation, Texas focus.*
