# NOAA Alerts — US Severe Weather Warnings MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-alerts-us-severe-weather-warnings)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Real-time NWS severe weather alerts: tornado warnings, hurricane watches, flood advisories, winter storms, and 120+ alert types filtered by state, zone, or exact location across the United States.

## Description
Real-time access to every active NWS weather alert across the United States.

### What you can do
- **By State** — All active alerts for any US state
- **By Zone** — Focused monitoring by NWS zone
- **By Point** — Alerts affecting a specific lat/lon
- **Alert Types** — Browse 120+ event types

### Critical for
Emergency management, logistics, insurance, event planning, and any operations sensitive to severe weather.


## Available Tools
- **get_active_alerts**: Filter by state (2-letter code: TX, FL, CA), severity (Extreme, Severe, Moderate, Minor), urgency (Immediate, Expected, Future), or event type (Tornado Warning, Hurricane Warning, etc.).

Get active weather alerts by US state or severity
- **get_alerts_by_zone**: g., TXZ211, FLZ050). Zone IDs can be found via the get_point_metadata tool. Useful for focused monitoring of a specific area.

Get active weather alerts for a specific NWS zone
- **get_alerts_by_point**: Internally resolves the location to find active alerts in that area.

Get active weather alerts for a specific US latitude/longitude
- **get_alert_types**: ). Use this to discover valid event type values for filtering alerts.

List all NWS weather alert types available


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Alerts — US Severe Weather Warnings** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any active weather alerts in Texas?"

**🤖 AI Agent:**
> ⚠️ **Texas — Active Alerts (6)**

🔴 Tornado Warning — Dallas County (until 4:30 PM)
🟠 Severe Thunderstorm Warning — Tarrant County
🟡 Flash Flood Watch — Houston metro (through tonight)
🟡 Heat Advisory — Rio Grande Valley (105°F+)
🔵 Dense Fog Advisory — Gulf Coast
🔵 Rip Current Statement — Galveston

6 active alerts across 14 counties.

---

**👤 You:**
> "Show me extreme severity alerts nationwide"

**🤖 AI Agent:**
> 🔴 **Extreme Severity Alerts**

1. Tornado Emergency — Moore, OK
2. Hurricane Warning — SW Florida Coast
3. Extreme Wind Warning — Miami-Dade County

3 extreme-level alerts currently active nationwide.


## ❓ FAQ

**Q: How quickly are alerts updated?**
NWS alerts are updated in real-time. When a warning is issued or cancelled, it appears within seconds on the API. Tornado Warnings have a typical lead time of 13 minutes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-alerts-us-severe-weather-warnings](https://vinkius.com/mcp/noaa-alerts-us-severe-weather-warnings)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NOAA Alerts — US Severe Weather Warnings** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `noaa-alerts-us-severe-weather-warnings` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NOAA Alerts — US Severe Weather Warnings** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "noaa-alerts-us-severe-weather-warnings": {
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
