# Agent Instructions

This repository is an HTML Bank for standalone published HTML assets.

## Required Folder Routing

Use exactly these three folders for HTML assets:

- `outreach-dashboards/` - prospect/account boards, territory views, re-engagement trackers, and internal sales dashboard views.
- `pre-call-briefs/` - single-prospect or single-meeting prep documents used before a call.
- `client-ready-assets/` - external-facing assets that could be sent to or screen-shared with a client or prospect.

Do not add new top-level HTML asset folders without explicit user approval.

## Routing Decision Rule

- Prospect/account board, territory view, re-engagement tracker, pipeline dashboard, account research board, or internal sales dashboard: `outreach-dashboards/`
- Single-prospect prep, single-meeting prep, call brief, stakeholder brief, or meeting agenda asset: `pre-call-briefs/`
- Client-sendable or screen-share-ready asset, including mockups, white papers, demo collateral, polished reports, and external leave-behinds: `client-ready-assets/`

If a file could fit multiple folders, choose based on audience: internal workflow first, meeting prep second, external-facing third.

## Filename Convention

Use:

```text
YYYY-MM-DD_account-name_asset-type.html
```

Rules:

- Use the asset date, not the upload date, when known.
- Use lowercase filenames.
- Use hyphens inside account names and asset types.
- Use underscores between date, account name, and asset type.
- Keep the `.html` extension.

## Index Requirement

Maintain a root `index.html` that lists the three folders and recent HTML files.

The preferred index behavior is auto-listing from the repository contents API so new files appear without manual link edits. If the repo remains private and the API cannot list files for public visitors, update the fallback file list inside `index.html` whenever files are added.
