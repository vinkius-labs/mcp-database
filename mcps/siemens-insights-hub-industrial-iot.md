# Siemens Insights Hub (Industrial IoT) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/siemens-insights-hub-industrial-iot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Siemens Insights Hub (formerly MindSphere) as an MCP: industrial assets, asset types, IoT time series of sensor data, latest values and event management — official Technical Token Manager auth (X-SPACE-AUTH-KEY).

## Description
**Siemens Insights Hub** (formerly MindSphere) — the industrial IoT platform of Siemens Xcelerator — as a single MCP server.

### What you can do
- **Asset management** — browse the asset hierarchy of your tenant (machines, devices, plants), their types and the aspects/variables each exposes
- **IoT time series** — sensor readings over time ranges: temperature, vibration, pressure... per asset-aspect, with from/to windows, select, sort and 2000-record pages
- **Latest values** — the current reading of every aspect variable (latestValue=true): the "what is this machine doing right now?" tool
- **Event management** — industrial events raised by assets: alarms, warnings, state changes, with MDSP filter queries

### Authentication (from the official Technical Token Manager docs)
1. Create your application credentials in the **Insights Hub Operator Cockpit** (service credentials)
2. Copy the generated **X-SPACE-AUTH-KEY** (base64-encoded authorization key)
3. The MCP mints short-lived JWTs at `POST {gateway}/[REDACTED]` with body `{appName, appVersion, hostTenant, userTenant}` — cached and auto-refreshed
4. Set your regional gateway URL (e.g. `https://gateway.eu1.mindsphere.io`)

### Who is this for?
Industrial IoT developers, predictive maintenance analytics, plant ops dashboards, OEMs building on Insights Hub and AI agents that need authoritative machine data.


## Available Tools (8)
- **get_asset_variables**: The variable names map to property set names for get_timeseries.

Get the variables (data points) an asset exposes, with last values
- **list_assets**: Each asset: assetId (32-char WID), name, typeId, parentId, location. Optionally filter by typeId or parentId. Use assetIds for time series and events.

List industrial assets registered in your Insights Hub tenant (machines, devices, plants)
- **list_asset_types**: Each type defines the aspects (property sets) and variables its assets expose — read this first to know which time series property sets exist.

List asset types: the digital twins models with their aspect definitions
- **get_asset**: The id is the 32-char assetId from list_assets.

Get full details of one asset: type, aspects, variables, location and hierarchy
- **get_timeseries**: Optional from/to (ISO datetime, from exclusive, to inclusive), limit (max 2000 per call — paginate via from), select (comma-separated variables), sort asc/desc. Without range returns the latest record.

Get IoT time series data for an asset aspect (sensor readings over a time range)
- **get_latest_timeseries**: Get the latest single record of an asset aspect (current sensor values)
- **list_events**: Supports a filter parameter (MDSP filter language, e.g. typeId eq "InsightsHub.Event" and timestamp gt ...) — pass raw MDSP filter in filter. Each event: typeId, entityId, timestamp and payload. Requires the Event Management subscription.

List industrial events raised by your assets (alarms, warnings, state changes)
- **get_event**: Use ids from list_events.

Get full details of one industrial event by id


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Siemens Insights Hub (Industrial IoT)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What machines do I have registered in Insights Hub?"

**🤖 AI Agent:**
> ⚙️ **Your Insights Hub assets**

Page 0 (50/page): Pump Station A (Pump 5X type), CNC Mill 2 (Siemens CNC type), Compressor Unit 3...

Each has a 32-char assetId. Want the variables of the CNC mill or its last temperature readings?

---

**👤 You:**
> "Show the temperature of asset X for the last 24 hours"

**🤖 AI Agent:**
> 🌡️ **Time series: asset X / BasicData (temperature)**

Last 24h, 1440 records (1/min):
- Min 22.1°C (03:40) · Max 27.8°C (14:22) · Mean 24.6°C
- Trend: +2.4°C since midnight, correlates with production cycle.

Want vibration too, or an alert if it crosses 30°C?

---

**👤 You:**
> "Any alarms raised by my assets this week?"

**🤖 AI Agent:**
> 🚨 **Events (this week)**

3 events found:
- 2026-09-05: HighVibration warning, CNC Mill 2 (spindle bearing)
- 2026-09-06: PressureDrop, Compressor Unit 3
- 2026-09-07: TemperatureHigh, Pump Station A

All are warnings, none critical. Want the full payload of any event?


## ❓ FAQ

**Q: How do I get the X-SPACE-AUTH-KEY?**
In the Insights Hub Operator Cockpit: register your application, then create its service credentials — the cockpit generates the base64-encoded authorization key. It identifies your app at the Technical Token Manager, which issues short-lived JWTs scoped to your app's roles.

**Q: Which gateway URL should I use?**
It depends on your plan/region: MindSphere-classic plans use https://gateway.eu1.mindsphere.io (also eu2, us1); Xcelerator plans use https://gateway.eu1.siemens.app. Check your Operator Cockpit — it shows the exact gateway for your tenant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/siemens-insights-hub-industrial-iot](https://vinkius.com/ai-agent-connect/siemens-insights-hub-industrial-iot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Siemens Insights Hub (Industrial IoT)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `siemens-insights-hub-industrial-iot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Siemens Insights Hub (Industrial IoT)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "siemens-insights-hub-industrial-iot": {
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
