# BANK AGENT Prospect Cockpit

Static GitHub Pages-ready dashboard for the BANK AGENT prospecting workflow.

## Entry point

- `index.html` - open this file locally or publish it with GitHub Pages.

## Clean file structure

```text
bank_agent_file_space/
├── index.html
├── README.md
├── manifest.json
├── .nojekyll
├── data/
│   └── dashboard-data.json
├── exports/
│   ├── prospects_flat.csv
│   ├── work_now.csv
│   ├── light_research.csv
│   ├── account_research.csv
│   └── deprioritize.csv
└── html/
    └── dashboard_original.html
```

## What this does

This package turns the uploaded prospect dashboard into a lightweight static site. It is meant to work as a seller command center:

- **Work Now** - send-ready records.
- **Light Research** - good targets that need quick validation or contact enrichment.
- **Account Research** - unclear-fit records that need account-level checking first.
- **Deprioritize** - low-signal records to keep out of daily selling motion.

## Import summary

- Generated at: May 30, 2026, 5:41 PM EDT
- Source file named in dashboard: `RECENT CONNECTS - ICP.xlsx`
- Total prospects: 88
- Ready to send: 1
- Light research: 76
- Account research: 2
- Deprioritize: 9

## GitHub Pages setup

1. Create a new GitHub repository, for example `bank-agent-prospect-cockpit`.
2. Upload the full contents of this folder to the repository root.
3. Make sure `index.html` is at the repository root.
4. In GitHub, go to **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/root` folder.
7. Save. GitHub will publish the static site and provide a Pages URL.

## Local use

Double-click `index.html` to open the dashboard in your browser.

## Data and export files

- `data/dashboard-data.json` contains the extracted embedded dashboard data.
- `exports/prospects_flat.csv` contains all flattened records.
- `exports/work_now.csv` contains records marked `Ready to send`.
- `exports/light_research.csv` contains records marked `Light research`.
- `exports/account_research.csv` contains records marked `Account research`.
- `exports/deprioritize.csv` contains records marked `Deprioritize`.

## QA notes

- The dashboard has embedded CSS, JavaScript, and JSON, so it can run as a standalone static page.
- LinkedIn URLs and public-profile text came from the supplied export context; this package does not scrape LinkedIn.
- Most records are research-gated because contact email/phone data is missing in the embedded data.
- Outreach drafts should be reviewed before sending.
