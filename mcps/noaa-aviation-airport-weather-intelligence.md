# NOAA Aviation — Airport Weather Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-aviation-airport-weather-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Aviation weather data worldwide: METARs (current airport conditions), TAFs (24-hour airport forecasts), PIREPs (pilot reports of turbulence and icing), and SIGMETs/AIRMETs (significant aviation hazards) from the Aviation Weather Center.

## Description
The definitive aviation weather intelligence from the NOAA Aviation Weather Center.

### What you can do
- **METAR** — Current airport conditions (works worldwide with ICAO codes)
- **TAF** — 24-30 hour airport forecasts
- **PIREP** — Pilot reports: turbulence, icing, visibility in-flight
- **SIGMET/AIRMET** — Significant hazard areas
- **Station Info** — Airport weather station details

### Global Coverage
METARs and TAFs work worldwide using ICAO codes (KJFK, EGLL, LFPG, SBGR).


## Available Tools
- **get_metar**: Provide ICAO codes comma-separated (KJFK, EGLL, LFPG). Returns temperature, wind, visibility, clouds, pressure, weather phenomena. Optionally retrieve past hours of data.

Get METAR (current airport weather) for any airport worldwide by ICAO code
- **get_taf**: Includes forecast groups with wind, visibility, clouds, and weather changes. ICAO codes only.

Get TAF (airport weather forecast) for any airport worldwide by ICAO code
- **get_pirep**: Filter by age (hours).

Get PIREPs (Pilot Reports) for turbulence, icing, and weather conditions
- **get_sigmet**: These define areas of significant weather hazards for aviation: convection, turbulence, icing, IFR conditions, mountain obscuration.

Get SIGMETs and AIRMETs — significant aviation weather hazards
- **get_aviation_station**: Use ICAO codes (KJFK, EGLL, LFPG, SBGR).

Get aviation weather station information by ICAO code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Aviation — Airport Weather Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get current weather at London Heathrow and Paris CDG"

**🤖 AI Agent:**
> ✈️ **METAR Report**

🇬🇧 **EGLL (Heathrow)**
Temp: 14°C, Wind: 270° at 12kt
Visibility: 9999m, Clouds: SCT030
Pressure: 1018 hPa
Condition: Fair

🇫🇷 **LFPG (Paris CDG)**
Temp: 16°C, Wind: 230° at 8kt
Visibility: 9999m, Clouds: FEW040
Pressure: 1020 hPa
Condition: Clear

---

**👤 You:**
> "Any active SIGMETs for convection?"

**🤖 AI Agent:**
> ⛈️ **Active Convective SIGMETs**

1. WST 0145 — Central Plains: embedded thunderstorms with tops FL450, hail >1 inch
2. WST 0146 — Gulf Coast: developing line of storms, movement NE at 30kt
3. WST 0147 — SE United States: widespread thunderstorms

3 convective SIGMETs active. Avoid flight paths through these areas.


## ❓ FAQ

**Q: Does aviation weather work worldwide?**
METARs and TAFs work at any airport worldwide using ICAO codes. PIREPs and SIGMETs are primarily from the US Aviation Weather Center but cover international areas too.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-aviation-airport-weather-intelligence](https://vinkius.com/mcp/noaa-aviation-airport-weather-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NOAA Aviation — Airport Weather Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `noaa-aviation-airport-weather-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NOAA Aviation — Airport Weather Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "noaa-aviation-airport-weather-intelligence": {
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
