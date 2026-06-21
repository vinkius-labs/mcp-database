# Open-Meteo Air Quality MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo-air-quality)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Monitor the air your users breathe: PM2.5, PM10, ozone, pollen counts, and official AQI indexes (European & US) — real-time pollutant intelligence for health-conscious AI agents.

## Description
Give your AI the power to **assess air safety** with real-time pollutant data at 11km resolution.

### What you can do
- **Pollutant Concentrations** — PM2.5, PM10, O₃, NO₂, SO₂, CO, dust, and ammonia in μg/m³
- **AQI Indexes** — Both European (0-100+) and US (0-500) Air Quality Indexes with per-pollutant breakdowns
- **Pollen Forecast** — Birch, grass, alder, ragweed, olive, and mugwort pollen counts for allergy planning
- **UV Index** — Clear-sky and actual UV index for sun exposure safety

### Who is this for?
Health apps, allergy sufferers, outdoor sports planners, environmental agencies, and parents monitoring playground safety.


## Available Tools (4)
- **get_air_quality**: 5, PM10, ozone, nitrogen dioxide, sulphur dioxide, and carbon monoxide concentrations for any location.

Get air quality pollutant concentrations
- **get_aqi_index**: Get Air Quality Index (European and US standards)
- **get_pollen_forecast**: Get pollen and allergen forecast
- **get_uv_index**: Get UV index forecast


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open-Meteo Air Quality** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the air quality in Beijing safe for outdoor exercise today?"

**🤖 AI Agent:**
> 💨 **Beijing — Air Quality Report**

US AQI: 156 (Unhealthy) ⚠️
PM2.5: 68 μg/m³ | PM10: 124 μg/m³
Ozone: 45 μg/m³ | NO₂: 38 μg/m³

❌ **Not recommended** for outdoor exercise. Sensitive groups should avoid all outdoor exertion.

---

**👤 You:**
> "What's the pollen forecast for Berlin this week?"

**🤖 AI Agent:**
> 🌿 **Berlin — Pollen Forecast**

Birch: HIGH (78 grains/m³) ⚠️
Grass: Moderate (32 grains/m³)
Alder: Low (5 grains/m³)
Ragweed: None detected

Birch allergy sufferers should take antihistamines and limit outdoor exposure.

---

**👤 You:**
> "What's the UV index in Sydney right now?"

**🤖 AI Agent:**
> ☀️ **Sydney — UV Index**

Current UV: 9.2 (Very High) 🔴
Clear-sky UV: 10.1
Recommendation: Apply SPF 50+, wear protective clothing, avoid sun between 10am-2pm.


## ❓ FAQ

**Q: What's the difference between European AQI and US AQI?**
The **European AQI** ranges 0-100+ with thresholds set by the EEA. The **US AQI** ranges 0-500 with EPA thresholds. Both are provided simultaneously so your AI can serve users in any region with their local standard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo-air-quality](https://vinkius.com/mcp/open-meteo-air-quality)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open-Meteo Air Quality** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `open-meteo-air-quality` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open-Meteo Air Quality** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-meteo-air-quality": {
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
