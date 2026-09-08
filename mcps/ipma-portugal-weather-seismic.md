# IPMA Portugal Weather & Seismic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ipma-portugal-weather-seismic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Official Portuguese weather authority: district forecasts, coastal sea state, active weather warnings, real-time earthquakes (including Azores), UV index and 200+ live station observations — zero-auth.

## Description
The **official Portuguese Institute for Sea and Atmosphere (IPMA)** as a single MCP server — the authoritative source for weather, ocean and seismic data in Portugal.

### What you can do
- **Official forecasts** — daily weather for all 35 districts and islands (min/max temp, precipitation probability, wind) for today, tomorrow and the day after
- **Sea state** — wave height, period and sea surface temperature for 12 coastal zones, from Figueira da Foz to the islands
- **Safety warnings** — active official warnings: rain, wind, thunderstorm, fog, heat, coastal agitation, with colour levels (green/yellow/orange/red)
- **Earthquakes** — real-time seismicity for mainland Portugal (area 7) and Azores/Madeira (area 3), including volcanic activity near São Jorge
- **Live stations** — temperature, humidity, wind, pressure, radiation and precipitation from 200+ automatic weather stations
- **UV index** — hourly UV forecast per location for sun-protection decisions

### Why IPMA and not a global API?
Global weather APIs model Portugal; IPMA measures it — with national radar, tide gauges, seismographs and the official warning system that Portuguese civil protection actually uses. When a Portuguese municipality closes beaches due to Agitação Marítima or an earthquake is felt in Lisbon, this is the data source behind it.

### Who is this for?
Travel and beach planning, agriculture, marine and nautical operations, civil-protection-aware agents, journalism and anyone who needs authoritative Portuguese weather, ocean or seismic data.


## Available Tools (8)
- **get_uv_index**: iUv >= 11 extreme, 8-10 very high, 6-7 high, 3-5 moderate. Use for sun-protection advice.

Current UV index forecast by hour interval for Portuguese locations
- **get_weather_forecast**: Day defaults to 0 (today); valid values 0, 1 or 2. Decode idWeatherType with get_weather_codes.

Official IPMA daily weather forecast for all Portuguese districts and islands
- **get_sea_forecast**: Day defaults to 0 (today); valid values 0, 1 or 2. Essential for beach, fishing and nautical activities.

Official IPMA sea state forecast for the Portuguese coast and islands
- **get_warnings**: ), level (green/yellow/orange/red) and validity window. Empty array means no active warnings. Check before travel, agriculture or marine operations.

Current official IPMA weather warnings for Portugal (rain, wind, storm, heat, fog, sea)
- **get_earthquakes**: Area 7 = mainland Portugal (default), area 3 = Azores and Madeira (includes volcanic seismicity from São Jorge). Returns the latest activity list.

Recent earthquakes detected by IPMA in mainland Portugal, Azores and Madeira
- **get_station_observations**: Very large payload — latest_only=true returns only the most recent hour (recommended).

Live observations from 200+ IPMA weather stations across Portugal
- **list_locations**: Districts have idRegiao 1-2; sea zones come from the separate coastal list.

List all IPMA locations: 35 districts/islands and 12 coastal sea zones with coordinates
- **get_weather_codes**: Use to translate numeric codes from get_weather_forecast and get_station_observations into human text.

Decode IPMA weather type, wind and precipitation codes into descriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IPMA Portugal Weather & Seismic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it safe to go to the beach in Nazaré this weekend? Check warnings and sea state"

**🤖 AI Agent:**
> 🏖️ **Nazaré beach safety check**

⚠️ Warnings: Yellow warning for Agitação Marítima (coastal agitation) on the Centro coast until Sunday 10:00
🌊 Sea forecast: wave height max 3.5m, period 13s, SST 17.5°C
☀️ UV index: 6 (high) between 12h-15h — use protection

Verdict: swimming not recommended due to rough seas; beach walks fine. Re-check Saturday morning.

---

**👤 You:**
> "Were there any earthquakes in the Azores in the last days?"

**🤖 AI Agent:**
> 🌋 **Azores seismicity (IPMA area 3)**

Latest event: 2026-09-07 08:27, magnitude 2.1 (L), SE Terceira, depth 12km
Activity: 76 events in the current series, mostly low-magnitude volcanic-tectonic swarms
Largest recent: M 3.4 north of São Jorge

This matches the ongoing São Jorge volcanic monitoring. No event above M 3.5 in the last 48h.

---

**👤 You:**
> "What's the weather forecast for Faro tomorrow and should I pack an umbrella?"

**🤖 AI Agent:**
> 🌤️ **Faro tomorrow (IPMA day 1)**

🌡️ Min 18°C / Max 28°C
🌧️ Precipitation probability: 10%
💨 Wind: W, class 2 (weak)
☀️ Weather type: partly cloudy (code 3)

No umbrella needed — pack sunscreen instead, UV will be high.


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. The IPMA open-data API is fully public — every tool in this MCP works without any authentication or account.

**Q: How is this different from global weather APIs like Open-Meteo?**
IPMA is Portugal's official meteorological authority: it operates the national observation network and issues the official warnings used by Portuguese civil protection. This MCP adds what global APIs do not have: official warnings, official sea reports, real-time earthquakes and live station observations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ipma-portugal-weather-seismic](https://vinkius.com/ai-agent-connect/ipma-portugal-weather-seismic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IPMA Portugal Weather & Seismic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ipma-portugal-weather-seismic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IPMA Portugal Weather & Seismic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ipma-portugal-weather-seismic": {
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
