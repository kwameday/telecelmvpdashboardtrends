# Telecel Marketplace Pilot — Payments & Cashback Dashboard (Static JSON + Trends)

This is a static HTML dashboard that **fetches metrics from `data.json`** (no database, no backend) and
shows **day-on-day trends** (▲ / ▼ / ↔) for key KPIs compared to the previous transaction day.

## Files
- `index.html` — UI, rendering logic, and trend calculations (fetches `data.json`).
- `data.json` — Metrics and tables (edit this file to update the dashboard).

## Deploy on Cloudflare Pages
1. Push this folder to a GitHub repo (e.g., `telecel-dashboard-json-trends`).
2. In Cloudflare → **Pages** → **Create a project** → **Connect to Git**.
3. Select your repo and use:
   - Framework preset: **None**
   - Build command: *(leave empty)*
   - Output directory: **/** (root)
4. Deploy. Your site will be live at `https://<project>.pages.dev`.

## Updating Data
- Open `data.json` in GitHub and edit values (or upload a new version).
- Commit to `main` — Cloudflare automatically redeploys and the new metrics + trends will show.
