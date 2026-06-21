# EPA AirNow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-airnow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Monitor localized air quality indices and critical environmental forecasts directly from the Environmental Protection Agency.

## Description
The **EPA AirNow MCP Server** connects your AI agent to the beating heart of environmental tracking. Gather deep insights into regional air safety, allowing proactive mitigation of respiratory risks and wildfire smoke exposure.

### Core Capabilities

- **Real-Time AQI Observations** — Instantly check current pollutant levels (Ozone, PM2.5, PM10) to determine if the local air is safe to breathe today.
- **Regional Forecasts** — Look ahead to anticipate upcoming hazardous environmental conditions, enabling dynamic safety planning for events or communities.
- **Flexible Targeting** — Pinpoint any community instantly using standard postal codes or exact geographic coordinates to get a tight observation radius.

Ideal for health-conscious applications, community dashboards, outdoor adventure planners, and risk assessment workflows tailored to individuals with sensitivities like asthma.


## Available Tools (3)
- **get_current_aqi_by_latlon**: Get real-time Air Quality Index observation using geographic coordinates
- **get_current_aqi_by_zip**: Requires a 5-digit US ZIP Code.

Get current real-time Air Quality Index observation using a US ZIP code
- **get_forecast_aqi_by_zip**: Get future AQI forecasts for a given US ZIP code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EPA AirNow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current air quality index in Beverly Hills?"

**🤖 AI Agent:**
> I've checked the latest observations for Beverly Hills. The current AQI is 45 (Good). It's a great day for outdoor activities without any health risks.

---

**👤 You:**
> "Will the air quality be safe for a marathon in Seattle tomorrow?"

**🤖 AI Agent:**
> Let me check the AirNow forecast for Seattle tomorrow. The AQI is predicted to peak at around 55 (Moderate), largely due to PM2.5. It remains generally safe for the marathon, though unusually sensitive athletes should monitor how they feel.

---

**👤 You:**
> "Fetch the PM10 specific metrics for ZIP code 90210 safely via AirNow."

**🤖 AI Agent:**
> Retrieving specific pollutant values securely...
**Area: Beverly Hills (90210)**
- PM10 concentration reported optimally clear (AQI 22). Parameter checked actively and correctly without errors.


## ❓ FAQ

**Q: Is the environmental tracking completely real-time?**
Yes! The system taps directly into the active observation corridors of the Environmental Protection Agency, gathering insights exactly as they are reported by local atmospheric sensors.

**Q: How does it help people with asthma or sensitivities?**
The agent retrieves exact pollutant indices and maps them into clear categories, letting users instantly know when it is dangerous for sensitive groups to engage in outdoor activities.

**Q: Are the geographic queries limited by zip code only?**
No, you can query locations by ZIP code to find immediate reporting areas, or use exact latitude/longitude coordinates to pull the closest station parameters precisely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-airnow](https://vinkius.com/mcp/epa-airnow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EPA AirNow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `epa-airnow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EPA AirNow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "epa-airnow": {
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
