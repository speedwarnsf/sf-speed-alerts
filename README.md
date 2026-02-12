# SpeedWarn SF 🚗📸

Real-time speed camera alerts for San Francisco drivers.

**Live:** [speedwarn.com](https://speedwarn.com)

## What It Does

- **33 speed camera locations** mapped across SF
- **GPS-powered alerts** with audio warnings as you approach cameras
- **Speed limit signs** pop up showing the limit for each camera zone
- **Works offline** as an installable PWA
- **100% on-device** — no location data ever leaves your phone

## How It Works

1. Open [speedwarn.com](https://speedwarn.com) on your phone
2. Accept the safety terms and enable GPS + Sound
3. Drive around SF — audio alerts play when you approach a camera zone
4. Install to your home screen for quicker access

## Tech

- Single-page PWA (vanilla JS, no framework)
- Leaflet.js for the interactive map
- Turf.js + KDBush for spatial indexing and geofencing
- Web Audio API for reliable alert playback
- Service Worker for offline support
- Hosted on GitHub Pages with custom domain

## Data

Camera locations and corridors are in `/data/`:
- `poles.json` — GeoJSON FeatureCollection of camera pole positions
- `corridors.json` — GeoJSON approach corridors
- `camera_speed_limits.json` — speed limits per camera

## Audio

Custom TTS audio files in `/images/audio/`:
- Location announcements for each camera
- Randomized "speed camera ahead" stems
- Fun reminder tags ("slow is the new fast", etc.)

## License

© 2025–2026 SF Speed Cameras. All rights reserved.
