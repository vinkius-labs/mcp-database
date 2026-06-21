# Stormglass MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stormglass)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access high-resolution global weather and marine data — fetch forecasts, tide levels, astronomy data, and biological marine metrics directly from any AI agent.

## Description
Connect the **Stormglass** API to your AI agent to access professional-grade environmental data for any coordinate on Earth. Perfect for maritime logistics, scientific research, and outdoor planning.

### What you can do

- **Global Weather** — Fetch high-resolution forecasts including wind speed, wave height, and air temperature for specific coordinates.
- **Tide Analysis** — Retrieve high and low tide extremes or detailed sea level height intervals for coastal locations.
- **Astronomy Data** — Get precise sunrise, sunset, moonrise, moonset, and moon phase information.
- **Marine Biology** — Access critical marine metrics like chlorophyll, oxygen levels, and phytoplankton concentrations.
- **Historical & Forecast** — Query both upcoming forecasts and historical data points using ISO 8601 timestamps.

### How it works

1. Subscribe to this server
2. Enter your Stormglass API Key
3. Start querying environmental data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Maritime & Logistics** — Monitor sea conditions and tide levels to optimize shipping routes and port operations.
- **Researchers & Scientists** — Gather biological and meteorological data for environmental studies and climate analysis.
- **Outdoor Enthusiasts** — Plan activities based on precise weather, tide, and solar/lunar cycles.


## Available Tools
- **get_astronomy_point**: Fetch astronomy data for a specific location
- **get_bio_point**: Fetch biological marine data for a specific location
- **get_tide_extremes_point**: Fetch high and low tides for a specific location
- **get_tide_sea_level_point**: Fetch sea level height at specific intervals
- **get_weather_point**: Fetch weather data for a specific coordinate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stormglass** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current wind speed and wave height for San Francisco (lat 37.7749, lng -122.4194)."

**🤖 AI Agent:**
> I've retrieved the weather data for San Francisco. Currently, the wind speed is 12 knots and the wave height is 1.5 meters according to NOAA data.

---

**👤 You:**
> "What are the high and low tides in Lisbon for the next 24 hours?"

**🤖 AI Agent:**
> Checking tide extremes for Lisbon... The next high tide is expected at 2:45 PM (1.2m) and the next low tide at 9:15 PM (0.3m).

---

**👤 You:**
> "Show me the sunrise and sunset times for Tokyo today."

**🤖 AI Agent:**
> For Tokyo today, the sun rose at 6:12 AM and is expected to set at 5:45 PM. The moon is currently in its Waxing Gibbous phase.


## ❓ FAQ

**Q: Can I get specific wave and wind data for a maritime location?**
Yes! Use the `get_weather_point` tool. You can specify parameters like `windSpeed` and `waveHeight` in the params string to get high-resolution data for your coordinates.

**Q: How do I find the next high and low tides for a coastal city?**
Simply use the `get_tide_extremes_point` tool with the latitude and longitude of the location. It will return the timing and height of the upcoming tide extremes.

**Q: Does the server provide biological data like chlorophyll levels?**
Yes, the `get_bio_point` tool allows you to fetch biological marine data including chlorophyll, iron, nitrate, oxygen, and phytoplankton levels for any coordinate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stormglass](https://vinkius.com/mcp/stormglass)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stormglass** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stormglass` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stormglass** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stormglass": {
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
