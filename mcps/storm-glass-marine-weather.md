# Storm Glass Marine & Weather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/storm-glass-marine-weather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal marine and weather intelligence — get global wave, tide, and bio data via AI.

## Description
Equip your AI agent with high-resolution global weather and marine intelligence through the **Storm Glass** MCP server. This integration provides real-time and forecast data from the world's leading meteorological institutions (NOAA, MET Office, DWD, and more). Your agent can retrieve precise marine weather (wave height, swell, water temp), tide extremes, astronomical data (sun/moon), and oceanic bio data (chlorophyll, iron levels). Whether you are planning offshore operations, maritime shipping, or researching environmental trends, your agent acts as a dedicated oceanographer and meteorologist through natural conversation.

### What you can do

- **Marine Point Forecasts** — Retrieve detailed wave and water data for any coordinate on Earth.
- **Tide Intelligence** — Fetch high and low tide times and heights for coastal planning.
- **Astronomical Insights** — Access sunrise, sunset, moon phases, and moonrise data.
- **Oceanic Bio Data** — Monitor chlorophyll and nutrient levels for environmental studies.

### How it works

1. Subscribe to this server
2. Enter your Storm Glass API Key (get it at stormglass.io)
3. Start querying global marine data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Maritime & Logistics Teams** — optimize routes and safety based on real-time wave and tide data.
- **Environmental Researchers** — track oceanic bio-markers and climate trends over time.
- **Offshore Engineers** — verify conditions for construction and maintenance operations.
- **Water Sports Enthusiasts** — check swell and tide data for coastal activities.


## Available Tools (3)
- **get_astronomy_data**: Get sun and moon data
- **get_marine_weather**: ) for a specific coordinate.

Get marine weather for a location
- **get_tide_extremes**: Get tide extremes for a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Storm Glass Marine & Weather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the wave height and water temp for Honolulu (21.3069, -157.8583)."

**🤖 AI Agent:**
> Retrieving marine data for Honolulu... Currently, the wave height is 1.2 meters and the water temperature is 25.4°C. The swell is coming from the North-West. Would you like to see the forecast for the next few hours?

---

**👤 You:**
> "What are the high and low tide times for London Bridge today?"

**🤖 AI Agent:**
> I've fetched the tide extremes for the London Bridge area. High tide is expected at 14:45 (3.2m) and low tide at 21:10 (0.5m). Would you like the full schedule for the week?

---

**👤 You:**
> "Get the current sunrise and moon phase for Rio de Janeiro."

**🤖 AI Agent:**
> Retrieving astronomical data... For Rio de Janeiro, sunrise was at 06:12. The current moon phase is a Waxing Gibbous (72% illumination).


## ❓ FAQ

**Q: Can I get the water temperature in the Mediterranean Sea?**
Yes! Use the `get_marine_weather` tool and provide the latitude and longitude for the specific point in the Mediterranean. It will return the latest water temperature along with other marine data.

**Q: How can I check the tide schedule for a coastal city?**
Use the `get_tide_extremes` tool with the coordinates of the target city. The response will provide the timestamps and heights for the next few high and low tide events.

**Q: Does this server provide sunrise and sunset times?**
Yes. The `get_astronomy_data` tool retrieves sunrise, sunset, moonrise, and moonset times, as well as the current moon phase for any given location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/storm-glass-marine-weather](https://vinkius.com/mcp/storm-glass-marine-weather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Storm Glass Marine & Weather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `storm-glass-marine-weather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Storm Glass Marine & Weather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "storm-glass-marine-weather": {
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
