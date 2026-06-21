# NOAA Alerts — US Severe Weather Warnings MCP Server

Real-time NWS severe weather alerts: tornado warnings, hurricane watches, flood advisories, winter storms, and 120+ alert types filtered by state, zone, or exact location across the United States.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-alerts-us-severe-weather-warnings)

## Overview
**Category:** the-unthinkable
**Tools Count:** 4

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


## Installation & Usage

To install and use the **NOAA Alerts — US Severe Weather Warnings** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-alerts-us-severe-weather-warnings](https://vinkius.com/mcp/noaa-alerts-us-severe-weather-warnings)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
