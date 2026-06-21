# Open-Meteo Marine Weather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo-marine-weather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Empower your AI with ocean intelligence: wave height, swell forecasts, ocean currents, tides, and sea surface temperature at 5km resolution — built for maritime professionals.

## Description
Turn your AI agent into a **maritime weather specialist** with real-time ocean data at 5km resolution.

### What you can do
- **Wave Forecasts** — Wave height, period, direction, plus wind-wave and swell components separated
- **Ocean Currents** — Current velocity, direction, and sea surface temperature
- **Daily Marine Summary** — Max wave height, dominant wave direction, and dominant period aggregated daily

### Who is this for?
Shipping companies, surfers, fisheries, coastal engineers, yacht clubs, and naval operations.


## Available Tools
- **get_marine_forecast**: Provides hourly forecast data for maritime planning.

Get marine wave forecast at 5km resolution
- **get_ocean_currents**: Get ocean current velocity and sea surface temperature
- **get_daily_marine**: Get daily marine weather summary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open-Meteo Marine Weather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the wave conditions off the coast of Hawaii right now?"

**🤖 AI Agent:**
> 🌊 **Hawaii North Shore — Current Conditions**

Wave height: 2.8m | Period: 14s
Swell: 2.4m from NW (315°)
Wind waves: 0.6m
Sea surface temp: 25.3°C

Excellent surfing conditions with clean long-period northwest swell.

---

**👤 You:**
> "Is it safe to sail across the English Channel tomorrow?"

**🤖 AI Agent:**
> ⚓ **English Channel — Tomorrow**

Wave height: 1.2m (moderate)
Wind waves: 0.8m from SW
Ocean current: 0.3 m/s eastbound
Sea temp: 14.1°C

Conditions are favorable for crossing. Expect moderate chop in the afternoon.

---

**👤 You:**
> "What's the maximum wave height expected in the North Sea this week?"

**🤖 AI Agent:**
> 🌊 **North Sea 7-Day Wave Max**

Day 1: 2.1m | Day 2: 1.8m | Day 3: 3.4m ⚠️
Day 4: 4.1m ⚠️ | Day 5: 2.6m | Day 6-7: 1.5m

Storm system on days 3-4 could produce significant wave heights. Exercise caution.


## ❓ FAQ

**Q: How accurate are the wave forecasts?**
Wave data is sourced from **ECMWF WAM, DWD EWAM, and NCEP GFS Wave** models at 5km resolution. Accuracy is excellent for open ocean but limited near coastlines due to resolution constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo-marine-weather](https://vinkius.com/mcp/open-meteo-marine-weather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open-Meteo Marine Weather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `open-meteo-marine-weather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open-Meteo Marine Weather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-meteo-marine-weather": {
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
