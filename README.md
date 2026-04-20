# Time Tracker PWA

Personal time tracking app with client management, projects, reports, and AI-powered invoice generation.

## Features

- **Log time** in hours and minutes (no decimal gymnastics)
- **Projects** with archive/complete workflow
- **Clients** with editable rates, parent client tracking
- **Reports** — weekly, bi-weekly, monthly, custom range
- **Invoice generation** via Claude AI — upload your template, it matches the style
- Works offline as a PWA
- All data stored locally in your browser

## Deploy to GitHub Pages

1. Create a new repo (e.g. `time-tracker`)
2. Push all these files to the `main` branch:
   ```
   index.html
   manifest.json
   sw.js
   icons/icon-192.png
   icons/icon-512.png
   ```
3. Go to **Settings → Pages → Source → main branch / root**
4. Your app will be live at `https://yourusername.github.io/time-tracker/`

## Install as PWA

- **iOS Safari**: tap Share → Add to Home Screen
- **Chrome/Android**: tap the install prompt or Menu → Add to Home Screen
- **Desktop Chrome**: click the install icon in the address bar

## Notes

- Data is stored in `localStorage` — it lives in the browser. If you clear site data, you lose it.
- For multi-device sync, the next step would be adding a backend (Supabase, Firebase, etc.)
- Invoice generation calls the Anthropic API — make sure you're on a network that allows it.
