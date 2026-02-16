# PLN ↔ RFS ↔ KML Converter (Offline)

A tiny **browser-only** tool to convert **MSFS/Flight Simulator .PLN** routes, **KML Geoplan File** and **RFS .RFS (JSON)** flight plans — with editable fields like weather, time, load, and runways.

**Try it online:** (GitHub Pages link here)  
**No install. No backend. Works offline.**

## Why
Flight plans are fragmented across simulators:
- MSFS exports `.pln`
- RFS uses `.rfs` JSON with its own schema
- Geoplan Software exports `.kml`

This tool bridges the gap so you can move routes between platforms quickly.

## Features
- Convert between **PLN** **RFS** and **KML**
- Drag & drop `.pln` / `.rfs` / `.kml`/`.txt`  into the page
- Offline by design (pure HTML + JS)
- Edit common RFS fields:
  - Weather / METAR mode
  - UTC date/time (custom or real)
  - Fuel / pax / cargo
  - Assigned takeoff/landing runway

## Quick Start (30 seconds)
1. Open the website (or download and open `index.html`)
2. Paste or drop your `.pln` / `.rfs`/ `.kml`
3. Click **Load Input**
4. Adjust settings
5. Click **Generate**
6. Download the output

## Limitations (important)
- **No navdata lookup**: if a PLN waypoint has no coordinates, it may be dropped.
- **No terminal procedure synthesis**: STAR/APP alignment is not automatically generated.
  Use your simulator's procedure selection tools when needed.

## Screenshot
![UI Screenshot](/screenshot.png)

## License
MIT
