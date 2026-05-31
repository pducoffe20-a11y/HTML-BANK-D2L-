# HTML Bank

HTML Bank stores standalone HTML assets and publishes them through GitHub Pages so each file can be opened as a live shareable page.

Use it for generated sales dashboards, pre-call briefs, and client-facing HTML assets.

## Live Site

GitHub Pages should publish from the `main` branch and the `/ (root)` folder.

Root index:

```text
https://pducoffe20-a11y.github.io/HTML-BANK---Engine/
```

Direct file links use this pattern:

```text
https://pducoffe20-a11y.github.io/HTML-BANK---Engine/FOLDER/FILENAME.html
```

Example:

```text
https://pducoffe20-a11y.github.io/HTML-BANK---Engine/outreach-dashboards/2026-05-30_d2l-brightspace_prospect-execution-dashboard.html
```

## Folder Structure

Use exactly these three folders for HTML assets:

```text
outreach-dashboards/
pre-call-briefs/
client-ready-assets/
```

- `outreach-dashboards/` - prospect/account boards, territory views, re-engagement trackers, and internal sales dashboard views.
- `pre-call-briefs/` - single-prospect or single-meeting prep documents used before a call.
- `client-ready-assets/` - external-facing assets that could be sent to or screen-shared with a client or prospect.

## Routing Rule

- If the file is primarily for prospecting, account research, pipeline review, territory planning, or re-engagement, put it in `outreach-dashboards/`.
- If the file prepares for one specific prospect, meeting, stakeholder, or call, put it in `pre-call-briefs/`.
- If the file is polished and safe enough to send or show externally, put it in `client-ready-assets/`.

When in doubt, choose based on audience: internal selling workflow goes in `outreach-dashboards/`, meeting prep goes in `pre-call-briefs/`, and external-facing material goes in `client-ready-assets/`.

## Filename Convention

Use this format:

```text
YYYY-MM-DD_account-name_asset-type.html
```

Examples:

```text
2026-05-31_brightspace_outreach-dashboard.html
2026-05-31_prima-shaunda-ragland_pre-call-brief.html
2026-05-31_acme-demo-mockup_client-ready-asset.html
```

Rules:

- Use lowercase words.
- Use hyphens inside account names and asset types.
- Use underscores between the date, account name, and asset type.
- Keep the `.html` extension.

## GitHub Pages Setup

1. Open the repo: `pducoffe20-a11y/HTML-BANK---Engine`.
2. Go to `Settings`.
3. In the left sidebar, click `Pages`.
4. Under `Build and deployment`, set `Source` to `Deploy from a branch`.
5. Set the branch to `main`.
6. Set the folder to `/ (root)`.
7. Click `Save`.
8. Wait a minute or two for GitHub to publish the site.

Note: the repo is currently private. If you want public, no-login preview links and automatic index listing through the GitHub API, make sure GitHub Pages is available for this private repo on your plan or make the repository public.

## Upload With The GitHub Website

1. Decide which folder the file belongs in using the routing rule above.
2. Open that folder in GitHub.
3. Click `Add file`.
4. Click `Upload files`.
5. Drag your `.html` file into the upload area.
6. Check the filename. Rename it first if it does not follow `YYYY-MM-DD_account-name_asset-type.html`.
7. Click `Commit changes`.
8. Wait about 1-3 minutes for GitHub Pages to refresh.
9. Open the live preview link using the URL pattern above.

## Upload With Terminal

Use this path if you already have the repo on your computer.

```bash
cd path/to/HTML-BANK---Engine
cp "/path/to/your/file.html" outreach-dashboards/2026-05-31_account-name_asset-type.html
git add outreach-dashboards/2026-05-31_account-name_asset-type.html
git commit -m "Add account-name asset"
git push
```

Change the folder and filename before running the commands.

## Index Page

The root `index.html` is the bank index. It lists the three folders and attempts to auto-load recent `.html` files from each folder.

When a new HTML file is added to one of the three folders, the index should update automatically if the repository contents API is publicly readable. If the repository remains private and the public API cannot list files, update the fallback list inside `index.html` or make the repository public.
