# HTML Bank Site

Static GitHub-ready site generated from `dashboard.html`.

## What is in this repo

```text
index.html
README.md
manifest.json
.nojekyll
data/
  dashboard-data.json
exports/
  prospects_flat.csv
  work_now.csv
  light_research.csv
  suppress.csv
  deprioritize.csv
```

## Dashboard counts

- Total accounts: 100
- Work Now: 67
- Light Research: 30
- Suppress: 3
- Average score: 61

## Local use

Open `index.html` in a browser.

## GitHub Pages setup

1. Create/open your GitHub repo.
2. Upload the contents of this folder to the repo root. Do not upload the ZIP as the site.
3. Confirm `index.html` is at the repo root.
4. Go to Settings > Pages.
5. Set Source to Deploy from a branch.
6. Set Branch to `main` and Folder to `/root`.
7. Save and open the Pages URL once GitHub finishes deploying.

## Notes

- `.nojekyll` is included so GitHub Pages serves the static files as-is.
- The dashboard is self-contained in `index.html`.
- `/data/dashboard-data.json` and `/exports/*.csv` are included so the repo also works as a file space for analysis and seller workflows.
