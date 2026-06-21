# NWS (National Weather Service) MCP Server

Access real-time weather data, forecasts, and active alerts directly from the National Weather Service.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nws-national-weather-service)

## Overview
**Category:** data-analytics
**Tools Count:** 9

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


## Installation & Usage

To install and use the **NWS (National Weather Service)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nws-national-weather-service](https://vinkius.com/mcp/nws-national-weather-service)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
