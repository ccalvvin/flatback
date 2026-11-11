# Gym Planner

A static workout-plan generator and exercise explorer built on [hasaneyldrm/exercises-dataset](https://github.com/hasaneyldrm/exercises-dataset).
Both pages fetch `data/exercises.json` and the GIFs directly from that repo at runtime — there is no local data file to upload or keep in sync.
Media © [Gym visual](https://gymvisual.com/), so keep the attribution in the footer.

- `index.html` — weekly plan generator + searchable library
- `tracker.html` — **SG Parcel Tracker**: paste a tracking number (SingPost, Ninja Van, J&T, SPX, Lazada LEX, Qxpress, DHL/FedEx/UPS, Cainiao, Pinduoduo `YJD…`, China couriers), it guesses the carrier, shows live results via the free 17TRACK widget, links to the official carrier sites, and keeps a saved parcel list in your browser. Shareable links: `tracker.html#YJD5701039652016`
- `explorer.html` — cascading filters (category → body part → equipment → target → exercise) showing one exercise + GIF + instructions at a time

## Deploy on GitHub Pages
1. Create a new repo (e.g. `gym-planner`) and upload just `index.html`, `explorer.html`, `tracker.html` and `README.md` — no `data/` folder needed.
2. Repo **Settings → Pages → Deploy from a branch → `main` / root → Save**.
3. Your site will be live at `https://<your-username>.github.io/gym-planner/` in about a minute.

## Run locally
    python3 -m http.server   # then open http://localhost:8000

## Troubleshooting
If exercises don't show up, open the browser console (F12) on the page — the error message there (e.g. a fetch/network error) will say exactly what failed. Both pages need internet access to `raw.githubusercontent.com`; they won't work fully offline.
