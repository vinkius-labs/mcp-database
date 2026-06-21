# Open-Meteo Flood & Rivers MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo-flood-rivers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Predict floods before they happen: GloFAS river discharge simulations at 5km, 40 years of historical data (1984–present), and 7-month forward forecasts for disaster prevention.

## Description
Arm your AI with **flood intelligence** powered by the Global Flood Awareness System (GloFAS).

### What you can do
- **River Discharge** — Real-time simulated river discharge in m³/s at 5km resolution
- **Flood Forecast** — Up to 7 months of forward river discharge predictions for early warning
- **Historical Discharge** — 40+ years of reanalysis data from 1984 for trend analysis

### Who is this for?
Disaster management agencies, civil engineers, flood insurance underwriters, environmental researchers, and agricultural water resource planners.


## Available Tools
- **get_river_discharge**: Useful for flood monitoring and water resource management.

Get river discharge data at 5km resolution
- **get_flood_forecast**: Data from GloFAS covering up to 210 days of prediction.

Get flood forecast up to 7 months ahead
- **get_historical_discharge**: Get historical river discharge data (1984–present)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open-Meteo Flood & Rivers** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current river discharge near Bangkok?"

**🤖 AI Agent:**
> 🏞️ **Chao Phraya River — Bangkok**

Current discharge: 1,245 m³/s
7-day trend: Rising (+15%)
30-day forecast: Peak expected at 1,890 m³/s

⚠️ Discharge trending above seasonal average. Monitor for flood risk.

---

**👤 You:**
> "Is there flood risk along the Rhine River in the next 3 months?"

**🤖 AI Agent:**
> 🌊 **Rhine River — 90-Day Flood Analysis**

Current: 1,100 m³/s (normal)
Month 1: Stable at 900-1,200 m³/s ✅
Month 2: Rising to 1,800 m³/s ⚠️ (spring melt)
Month 3: Peak 2,400 m³/s ⚠️ (elevated risk)

Spring snowmelt could elevate discharge significantly in months 2-3.

---

**👤 You:**
> "Compare Danube River discharge in 2002 vs today"

**🤖 AI Agent:**
> 📊 **Danube — Historical vs Current**

2002 flood peak: 10,370 m³/s (catastrophic)
Current discharge: 2,100 m³/s (normal)

2002 was one of the worst flood events in European history, with discharge 5× above current levels.


## ❓ FAQ

**Q: How accurate is the flood forecast?**
Data comes from **GloFAS v4** (Global Flood Awareness System) by Copernicus at 5km resolution. Short-term forecasts (1-30 days) are highly reliable. Seasonal forecasts (1-7 months) indicate trends but have wider uncertainty bands.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo-flood-rivers](https://vinkius.com/mcp/open-meteo-flood-rivers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open-Meteo Flood & Rivers** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `open-meteo-flood-rivers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open-Meteo Flood & Rivers** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-meteo-flood-rivers": {
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
