# NOAA Climate — Historical Weather Records MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-climate-historical-weather-records)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Historical climate data from the planet's largest weather archive: GHCN-Daily temperature and precipitation records, monthly and yearly summaries, 30-year climate normals, and station search from NOAA's National Centers for Environmental Information.

## Description
The planet's largest archive of daily weather records, freely accessible.

### What you can do
- **Daily Data (GHCN-D)** — Temperature, precipitation, snow, wind for 100K+ stations
- **Monthly Summaries (GSOM)** — Monthly aggregates
- **Annual Summaries (GSOY)** — Yearly climate data
- **Climate Normals** — 30-year baseline (1991-2020)
- **Station Search** — Find stations by location or name

### Global Coverage
GHCN-Daily has worldwide stations, with densest coverage in the US, Europe, and Australia.


## Available Tools
- **get_daily_data**: This is the planet's largest archive of daily weather records. Filter by station, data types (TMAX, TMIN, PRCP, SNOW, SNWD), and date range. Stations are worldwide but densest coverage is in the US.

Get daily weather data (GHCN-Daily): temperatures, precipitation, snow
- **get_monthly_summary**: Monthly aggregates of temperature averages, precipitation totals, and degree days. Less granular than daily but ideal for climate trend analysis.

Get monthly climate summary (GSOM): average temp, total precipitation, heating degree days
- **get_yearly_summary**: Yearly temperature averages, precipitation totals, and extreme values. Perfect for long-term climate analysis spanning decades.

Get annual climate summary (GSOY): yearly averages and extremes
- **get_climate_normals**: This is the statistical baseline that defines "normal" weather for any location.

Get 30-year climate normals — the baseline for what is "normal" weather
- **search_stations**: Returns station IDs, names, and locations for use with other climate tools.

Search NCEI weather stations by location bounding box or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Climate — Historical Weather Records** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get daily temperatures for Central Park, NYC in January 2024"

**🤖 AI Agent:**
> 📊 **Central Park (USW00094728) — January 2024**

| Date | Max°C | Min°C | Precip mm |
|------|-------|-------|----------|
| Jan 1 | 4.4 | -1.1 | 0.0 |
| Jan 2 | 6.7 | 1.1 | 2.5 |
| Jan 3 | 2.2 | -3.3 | 0.0 |
| ... | ... | ... | ... |
| Jan 31 | 7.8 | 0.0 | 8.1 |

Monthly avg high: 4.8°C. Monthly precip: 89mm.

---

**👤 You:**
> "Show me the total monthly precipitation for Seattle in 2023."

**🤖 AI Agent:**
> Here is the GSOM data for Seattle (USW00024233) for 2023: Total annual precipitation was 31.5 inches. The wettest month was November with 6.2 inches, and the driest was August with 0.1 inches.

---

**👤 You:**
> "What are the 30-year climate normals for Miami?"

**🤖 AI Agent:**
> Based on the 1991-2020 normals for Miami International Airport: The average annual high is 84.4°F, the average low is 71.2°F, and the average annual precipitation is 61.9 inches.


## ❓ FAQ

**Q: How far back does the data go?**
GHCN-Daily records go back to the 1700s for some stations, with widespread coverage since the 1890s. Over 100,000 stations worldwide, with the densest network in the United States.

**Q: What is the difference between GHCN-D, GSOM, and GSOY?**
GHCN-Daily provides day-by-day records. GSOM (Global Summary of the Month) aggregates these into monthly averages and totals. GSOY (Global Summary of the Year) provides annual summaries.

**Q: Are observations available for international locations?**
Yes, while NOAA is a US agency, the GHCN incorporates data from over 100,000 stations worldwide, though the highest density remains in North America, Europe, and Australia.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-climate-historical-weather-records](https://vinkius.com/mcp/noaa-climate-historical-weather-records)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NOAA Climate — Historical Weather Records** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `noaa-climate-historical-weather-records` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NOAA Climate — Historical Weather Records** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "noaa-climate-historical-weather-records": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
