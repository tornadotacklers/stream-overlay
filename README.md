# Tornado Tacklers — Stream Overlay

A live OBS browser source overlay built for storm chasers. Displays a branded top bar with live clock, current temperature, your real-time location, and an automatic NWS Tornado Warning alert system.

---

## Features

- **Live clock** — 12-hour format with AM/PM, updates every second
- **Live location** — auto-detects your GPS position and displays City, County, State
- **Live temperature** — current °F pulled from Open-Meteo (free, no API key needed)
- **NWS Tornado Warning** — automatically checks for active tornado warnings at your location every time your position updates. If a warning is active, the top bar border turns red and pulses, and a 🌪 TORNADO WARNING badge appears
- **Transparent background** — your chase footage shows through behind the overlay
- **Fully responsive** — scales to any resolution, optimized for 1920×1080

---

## Setup Instructions

### Step 1 — Fork or Clone This Repo

1. Click **Fork** at the top right of this GitHub page
2. Name it whatever you like (e.g. `stream-overlay`)

### Step 2 — Enable GitHub Pages

1. Go to your repo **Settings**
2. Click **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Set branch to `main` and folder to `/ (root)`
5. Click **Save**
6. Wait 1–2 minutes, then your overlay will be live at:
   `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/stream_layout.html`

### Step 3 — Add to OBS

See `OBS_SETUP.md` for step-by-step OBS instructions.

---

## Customization

To change your stream name, open `stream_layout.html` in any text editor and find:

```html
<div class="logo-box">TORNADO TACKLERS</div>
```

Replace `TORNADO TACKLERS` with your stream name.

---

## APIs Used (all free, no keys required)

- [Open-Meteo](https://open-meteo.com/) — temperature
- [Nominatim / OpenStreetMap](https://nominatim.org/) — reverse geocoding
- [NWS Weather.gov](https://www.weather.gov/documentation/services-web-api) — tornado warnings
- [Google Fonts](https://fonts.google.com/) — Orbitron & Rajdhani fonts

---

*Built by Ginger Murray — [gingermurray.github.io](https://gingermurray.github.io)*
