# NWS (National Weather Service) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nws-national-weather-service)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nws-national-weather-service-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nws-national-weather-service-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time weather data, forecasts, and active alerts directly from the National Weather Service.

## Description
Connect to the **National Weather Service (NWS)** API to retrieve precise meteorological data for any US location. This server allows AI agents to fetch point-based grid information, detailed textual forecasts, hourly updates, and critical weather alerts.

### What you can do

- **Location Mapping** — Convert coordinates into NWS grid points using `get_point` to unlock hyper-local data.
- **Forecasts** — Get detailed textual and hourly forecasts for specific grid locations via `get_forecast` and `get_hourly_forecast`.
- **Weather Alerts** — Monitor active watches, warnings, and advisories nationwide or by specific state/area with `get_active_alerts` and `get_active_alerts_by_area`.
- **Station Observations** — Access real-time data from weather stations, including the latest atmospheric readings using `get_latest_station_observation`.

### How it works

1. Subscribe to this server
2. Provide a User-Agent string (required by NWS API policy)
3. Start querying weather data in your AI agent

### Who is this for?

- **Developers & Data Scientists** — integrate live weather context into applications or analysis workflows.
- **Logistics & Operations** — monitor active alerts and forecasts to optimize travel and outdoor activities.
- **General Users** — get precise, official government weather data through natural conversation.


## Available Tools
- **get_active_alerts_by_area**: g., TX, FL, AMZ).

Get active alerts for a specific area
- **get_active_alerts**: Get all currently active weather alerts
- **get_alert**: Get details for a specific weather alert
- **get_forecast**: Get textual forecast for a specific grid location
- **get_hourly_forecast**: Get hourly forecast for a specific grid location
- **get_latest_station_observation**: Get the latest observation for a specific station
- **get_point**: Get NWS office and grid information for a latitude/longitude
- **get_station_observations**: Get observations for a specific station
- **get_stations**: Get a list of all observation stations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NWS (National Weather Service)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the weather forecast for coordinates 34.0522, -118.2437?"

**🤖 AI Agent:**
> I'll first find the NWS grid point for those coordinates... Found it: Office LOX, Grid (154, 44). Now fetching the forecast: It will be sunny today with a high near 75°F. Tonight, mostly clear with a low around 58°F.

---

**👤 You:**
> "Are there any active weather alerts in Texas right now?"

**🤖 AI Agent:**
> Checking active alerts for Texas (TX)... I found 3 active alerts: a Heat Advisory for South Texas, a Flood Watch for the Coastal Bend, and a Special Weather Statement for the Panhandle. Would you like details on any of these?

---

**👤 You:**
> "Get the latest weather observation for station KLAX."

**🤖 AI Agent:**
> Fetching the latest data for KLAX (Los Angeles International Airport)... As of 10 minutes ago: Temperature is 68°F, Humidity is 62%, Wind is from the West at 12 mph, and Visibility is 10 miles.


## Installation & Usage

To install and use the **NWS (National Weather Service)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nws-national-weather-service](https://vinkius.com/mcp/nws-national-weather-service)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
