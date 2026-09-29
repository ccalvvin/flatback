# Gym Planner

A static workout-plan generator and exercise explorer built on [hasaneyldrm/exercises-dataset](https://github.com/hasaneyldrm/exercises-dataset).
Exercise GIFs load directly from that repo. Media © [Gym visual](https://gymvisual.com/), so keep the attribution in the footer.

- `index.html` — weekly plan generator + searchable library
- `explorer.html` — cascading filters (category → body part → equipment → target → exercise) showing one exercise + GIF + instructions at a time

## Deploy on GitHub Pages
1. Create a new repo (e.g. `gym-planner`) and upload `index.html`, `explorer.html`, `README.md` and the `data/` folder.
2. Repo **Settings → Pages → Deploy from a branch → `main` / root → Save**.
3. Your site will be live at `https://<your-username>.github.io/gym-planner/` in about a minute.

## Run locally
    python3 -m http.server   # then open http://localhost:8000

## Regenerate the data
`data/exercises.min.json` is an English-only slim copy of the dataset's `data/exercises.json`.
