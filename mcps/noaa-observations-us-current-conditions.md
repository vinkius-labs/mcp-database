# NOAA Observations — US Current Conditions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-observations-us-current-conditions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Real-time weather observations from thousands of official NWS stations: temperature, wind speed and direction, humidity, barometric pressure, visibility, and weather conditions across the United States.

## Description
Real-time sensor data from thousands of NWS stations.

### What you can do
- **Find Stations** — Locate nearby weather stations by lat/lon
- **Current Conditions** — Latest observation (temp, wind, pressure, humidity)
- **Recent History** — Observation trend over past hours
- **Station Metadata** — Details about each station
- **Radar Network** — NEXRAD radar station status


## Available Tools (5)
- **get_observation_history**: Useful for seeing temperature trends, wind changes, and weather evolution over recent hours.

Get recent observation history for a NWS station
- **get_stations**: Each station has a 4-character ID (e.g., KJFK, KLAX). US only. Use station IDs with get_latest_observation.

Find nearby NWS weather observation stations by latitude/longitude
- **get_latest_observation**: Provide a 4-character station ID such as KJFK, KLAX, KORD, KDFW.

Get current weather conditions from a specific NWS station
- **get_station_metadata**: Useful for understanding where a station is and what data it provides.

Get metadata about a specific NWS weather station
- **get_radar_stations**: List all NWS radar stations and their status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Observations — US Current Conditions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current temperature at JFK Airport?"

**🤖 AI Agent:**
> 📡 **KJFK — Current Conditions**

Temperature: 72°F (22.2°C)
Wind: SW at 12 mph, gusting 18
Humidity: 68%
Pressure: 1013.2 hPa
Visibility: 10 mi
Condition: Partly Cloudy

Observed: 2:51 PM EDT

---

**👤 You:**
> "Find the closest weather stations to downtown Chicago."

**🤖 AI Agent:**
> I found 3 official NWS reporting stations near downtown Chicago: KMDW (Midway Airport), KORD (O'Hare International), and KCGX (historical). KMDW is currently reporting 45°F and light rain.

---

**👤 You:**
> "What's the weather trend for the past 6 hours in Denver?"

**🤖 AI Agent:**
> At Denver International (KDEN) over the last 6 hours: Temperature dropped from 52°F to 34°F. Winds shifted from SW to strong N winds gusting to 35 mph, and light snow began falling in the last hour.


## ❓ FAQ

**Q: How often are observations updated?**
Most NWS stations report hourly (METAR), with some reporting every 5-15 minutes during significant weather (SPECI).

**Q: What are METAR and SPECI reports?**
METARs are routine hourly weather reports generated primarily at airports. SPECI reports are unscheduled updates issued when there is a significant change in weather conditions.

**Q: Can I check the status of a local weather radar?**
Yes, you can query the operational status of NEXRAD sites across the country to see if a station is active, down for maintenance, or scanning.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-observations-us-current-conditions](https://vinkius.com/mcp/noaa-observations-us-current-conditions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NOAA Observations — US Current Conditions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `noaa-observations-us-current-conditions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NOAA Observations — US Current Conditions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "noaa-observations-us-current-conditions": {
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
