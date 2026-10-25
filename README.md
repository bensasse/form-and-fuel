# Form & Fuel — 12-week fitness tracker

A mobile-friendly, static fitness web app built from your 12-week Excel workout and nutrition tracker. No build tools, paid services, or login required.

## Deploy with GitHub Pages

1. Create a new **public** GitHub repository, e.g. `form-and-fuel`.
2. Upload **all files in this folder** to the repository root (`index.html`, `app.js`, `data.js`, `style.css`, `sw.js`, `manifest.webmanifest`, `icon.svg`).
3. In GitHub, open **Settings → Pages → Build and deployment**.
4. Select **Deploy from a branch**, branch **main**, folder **/(root)**, and save.
5. Visit `https://YOUR-USERNAME.github.io/form-and-fuel/` after deployment finishes.

For local testing, use `python -m http.server 8000` inside this folder and open `http://localhost:8000` in your browser. Opening `index.html` directly works for basic testing, but the install/offline feature requires HTTP(S).

## Features

- Dashboard, goal progress and weight trend
- 12-week strength plan, set-by-set logging with weight/reps/completion
- Two run sessions per week, Peloton logging
- One-tap preset meal logging and daily macro overrides
- Daily check-ins, progress history and weekly grocery list
- Settings and JSON export/import backups
- Installable PWA and offline app shell after first online visit

## Important limitations

- All data lives in **this browser's localStorage**. It does **not sync** across phone and computer. Export backups regularly; clearing site data deletes local records.
- Hosting code publicly on GitHub Pages does **not** publish your logged fitness data. Avoid committing exported JSON backups to the public repository.
- Meal nutrition values are estimates from the spreadsheet, not exact recipes. Verify portions, oils, and labels.
- Updating app code may change functionality; keep backups before major changes.
