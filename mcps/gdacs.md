# GDACS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gdacs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor global disaster alerts — earthquakes, cyclones, floods, volcanoes, wildfires and droughts with real-time impact estimates.

## Description
Connect to **GDACS** (Global Disaster Alert and Coordination System) and monitor worldwide disaster activity through natural conversation — no API key needed.

### What you can do

- **Earthquake Tracking** — Monitor earthquakes worldwide with magnitude filtering, depth data and impact estimates
- **Cyclone Monitoring** — Track tropical cyclones, hurricanes and typhoons with categories, wind speeds and forecast tracks
- **Flood Alerts** — Monitor flood events with affected population estimates and severity levels
- **Volcanic Activity** — Track volcanic eruptions with ash plume data and alert levels
- **Wildfire Monitoring** — Monitor wildfires with burned area estimates and affected populations
- **Drought Tracking** — Track drought events with severity levels and population impact
- **Impact Estimates** — Get population exposure, estimated fatalities and economic losses for each event
- **Alert Levels** — View color-coded alerts (red=high, orange=medium, green=low)

### How it works

1. Subscribe to this server
2. No API key needed — start monitoring immediately
3. Explore global disaster data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Emergency Managers** — monitor real-time disaster alerts and coordinate response efforts
- **Researchers** — analyze disaster patterns, impact data and population exposure
- **Journalists** — discover breaking disaster news with verified data and impact estimates
- **Insurance Professionals** — assess catastrophe risk and estimate potential losses


## Available Tools
- **get_alert_detail**: Get details for a specific alert
- **get_alerts**: Alerts are color-coded: red (high impact), orange (medium impact), green (low impact). Supports filtering by event type and time period.

Get disaster alerts
- **get_event_detail**: Get details for a specific disaster event
- **get_event_geojson**: Returns geographic boundaries, affected areas and population exposure polygons.

Get GeoJSON data for a disaster event
- **get_event_list**: Supports filtering by event type (EQ=earthquake, TC=cyclone, FL=flood, VO=volcano, WF=wildfire, DR=drought), date range, and time period. Returns event names, types, magnitudes, alert levels, start dates and affected countries.

Search disaster events
- **get_impacts**: Returns estimated population affected, fatalities, economic losses and confidence levels.

Get impact estimates for a disaster event
- **get_latest_cyclones**: Returns cyclone names, categories, wind speeds, locations, alert levels and forecast tracks.

Get latest tropical cyclones worldwide
- **get_latest_droughts**: Returns drought locations, start dates, severity levels, alert levels and affected populations.

Get latest drought events worldwide
- **get_latest_earthquakes**: Returns magnitude, depth, location, alert level and affected countries. Optionally filter by minimum magnitude and number of days.

Get latest earthquakes worldwide
- **get_latest_floods**: Returns flood locations, start dates, alert levels, affected populations and severity estimates.

Get latest floods worldwide
- **get_latest_volcanoes**: Returns volcano names, locations, eruption types, alert levels and ash plume information.

Get latest volcanic activity worldwide
- **get_latest_wildfires**: Returns fire locations, start dates, burned areas, alert levels and affected populations.

Get latest wildfires worldwide


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GDACS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What earthquakes happened in the last 7 days?"

**🤖 AI Agent:**
> Found 12 earthquakes in the past 7 days. Notable: M6.8 Japan (orange alert, 2M people affected), M5.9 Turkey (green alert), M5.6 Indonesia (green alert). All with depth, coordinates and impact estimates.

---

**👤 You:**
> "Are there any active cyclones right now?"

**🤖 AI Agent:**
> Found 2 active tropical cyclones: Cyclone Freddy (Category 3, Mozambique channel, orange alert) with sustained winds 185km/h affecting 1.2M people. Tropical Storm 03W (Pacific, green alert) with winds 95km/h.

---

**👤 You:**
> "Show me flood alerts for the last 3 days."

**🤖 AI Agent:**
> Found 3 flood events in the past 3 days: Kenya (orange alert, 500K affected), Somalia (green alert, 150K affected), Northern Australia (green alert, localized). All with severity estimates and response status.


## ❓ FAQ

**Q: Do I need an API key?**
No! GDACS data is completely free and open. No authentication required. Just subscribe and start monitoring disasters.

**Q: What do the alert levels mean?**
GDACS uses three alert levels: Green (low impact, local effects), Orange (medium impact, significant regional effects), Red (high impact, potentially catastrophic with international response needed).

**Q: How far back can I search for events?**
You can search events from the past 1 to 30 days using the period or date_from/date_to parameters. For historical analysis, use date_from and date_to with specific dates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gdacs](https://vinkius.com/mcp/gdacs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GDACS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gdacs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GDACS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gdacs": {
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
