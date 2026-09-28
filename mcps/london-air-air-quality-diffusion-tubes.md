# London Air: Air Quality & Diffusion Tubes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/london-air-air-quality-diffusion-tubes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Keyless London air data: city-wide monthly averages for 14 pollutants (NO, NO2, NOx, O3, PM10, PM2.5, SO2 — roadside and background, 2008 to today), time-of-day profiles, and the 2024 diffusion-tube study across all 33 boroughs.

## Description
Three official London air-quality datasets — keyless, straight from the London open-data platform (data.london.gov.uk).

### What you can do
- **air_quality_monthly / air_quality_by_hour / air_quality_overview** — the city-wide series: 139 months × 14 indicators (NO, NO2, NOx, O3, PM10, PM2.5, SO2 in roadside and background, in µg/m³), with the time-of-day cut (month × hour, each with a 14-indicator block) and a per-indicator min/max/mean overview
- **diffusion_boroughs / diffusion_borough_lookup / diffusion_sites / diffusion_overview** — the 2024 diffusion-tube study: per-borough site counts, the share of sites above the UK legal limit and the WHO guideline, the full site register for one borough (site ID, name, type, Easting/Northing, monthly means January to December) and the city-wide totals

### Who is this for
Anyone tracking London's air against the legal limits or the WHO guideline, comparing boroughs, or pulling the raw monthly and hourly series. Diffusion tubes are low-cost passive samplers that integrate exposure over months — cheaper and steadier than the fixed monitoring stations behind the first three tools. Borough names in the lookup accept plain forms ("Camden", "City of London") and resolve the source file's odd stored spellings for you.


## Available Tools (7)
- **air_quality_by_hour**: Filter by month (e.g. "Jan-08") and/or hour ("9" or "09:00"). Page with limit/offset.

London air-pollutant means broken down by hour of day
- **air_quality_monthly**: 5, sulphur dioxide) in ug/m3, roadside and background networks, January 2008 to August 2019 (139 months). Use air_quality_by_hour for the 24-hour breakdown. Page with limit/offset.

London-wide monthly mean air-pollutant concentrations, roadside and background
- **air_quality_overview**: A compact way to see which pollutants trend highest/lowest.

Per-pollutant min/max/mean across the London monthly air-quality series
- **diffusion_borough_lookup**: borough is required and is matched case-insensitively, with or without the LB/RB prefix ("barnet", "LB Barnet" and "Barnet" all work; use "Waltham Forest" or "Kensington & Chelsea" for the misspelled sheets).

Look up one London borough in the 2024 diffusion-tube summary
- **diffusion_boroughs**: Sorted by tube count; pass top to keep only the first N (max 33).

2024 diffusion-tube air-monitoring summary per London borough
- **diffusion_overview**: City-wide totals from the 2024 diffusion-tube summary
- **diffusion_sites**: ), OSGB easting/northing (x_m, y_m), month-by-month means (jan-dec, ug/m3) and the raw vs bias-adjusted annual means. borough is required. Page with limit/offset.

The 2024 diffusion-tube monitoring sites of one London borough


## 💬 Prompt Examples

Here are some examples of how you can interact with the **London Air: Air Quality & Diffusion Tubes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the average roadside NO2 in London for the last 12 months?"

**🤖 AI Agent:**
> Call air_quality_monthly with limit 12 and offset pointing at the end of the series (or just read the last 12 rows of the 139-month series), then average the no2_roadside column; air_quality_overview gives the all-series mean for context.

---

**👤 You:**
> "Which borough has the highest share of diffusion-tube sites above the WHO guideline?"

**🤖 AI Agent:**
> Run diffusion_boroughs with a large top — each row carries sites_exceeding_who and its share of the borough's sites; the first row is the borough with the highest WHO exceedance share.

---

**👤 You:**
> "List the diffusion-tube sites in Camden."

**🤖 AI Agent:**
> Call diffusion_sites with borough 'Camden' — one row per site with its ID, name, sensor type, Easting/Northing and the twelve monthly means; page with limit/offset for longer registers.


## ❓ FAQ

**Q: Do I need an API key?**
No. data.london.gov.uk publishes every dataset as an anonymous file download (CSV or Excel). This MCP defines no credentials and needs nothing configured.

**Q: Which indicators are in the monthly series?**
Fourteen, in pairs: NO, NO2, NOx, O3, PM10, PM2.5 and SO2, each measured roadside and in background (units µg/m³). air_quality_overview returns the min, max and mean of every one of them across the whole series.

**Q: What is a diffusion tube?**
A low-cost passive sampler: air diffuses through a cap into a sorbent, and the 12-month average is reported per site. Because it integrates exposure over months rather than minutes, it is ideal for mapping long-term neighbourhood-level pollution across all 33 London boroughs.

**Q: Why do some borough names look misspelled in the source?**
The 2024 study stores two boroughs with typos ('LB Waltham' for Waltham Forest, 'RB Kensignton & Chelsea'). diffusion_borough_lookup accepts the plain friendly names — 'Waltham Forest', 'Kensington and Chelsea', 'City of London' — and resolves them to the stored sheet names automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/london-air-air-quality-diffusion-tubes](https://vinkius.com/en/ai-agent-connect/london-air-air-quality-diffusion-tubes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **London Air: Air Quality & Diffusion Tubes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `london-air-air-quality-diffusion-tubes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **London Air: Air Quality & Diffusion Tubes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "london-air-air-quality-diffusion-tubes": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
