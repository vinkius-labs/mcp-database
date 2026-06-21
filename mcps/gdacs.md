# GDACS MCP Server

Monitor global disaster alerts — earthquakes, cyclones, floods, volcanoes, wildfires and droughts with real-time impact estimates.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gdacs)

## Overview
**Category:** data-analytics
**Tools Count:** 12

## Description
Connect to **GDACS** (Global Disaster Alert and Coordination System) and monitor worldwide disaster activity through natural conversation — no API key needed.

### What you can do

- **Earthquake Tracking** — Monitor earthquakes worldwide with magnitude filtering, depth data and impact estimates
- **Cyclone Monitoring** — Track tropical cyclones, hurricanes and typhoons with categories, wind speeds and forecast tracks
- **Flood Alerts** — Monitor flood events with affected population estimates and severity levels
- **Volcanic Activity** — Track volcanic eruptions with ash plume data and alert levels
- **Wildfire Monitoring** — Monitor wildfires with burned area estimates and affected populations
- **Drought Tracking** — Track drought events with severity levels and population impact
- **Impact Estimates** — Get population exposure, estimated fatalities and economic losses for each event
- **Alert Levels** — View color-coded alerts (red=high, orange=medium, green=low)

### How it works

1. Subscribe to this server
2. No API key needed — start monitoring immediately
3. Explore global disaster data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Emergency Managers** — monitor real-time disaster alerts and coordinate response efforts
- **Researchers** — analyze disaster patterns, impact data and population exposure
- **Journalists** — discover breaking disaster news with verified data and impact estimates
- **Insurance Professionals** — assess catastrophe risk and estimate potential losses


## Available Tools
- **get_alert_detail**: Get details for a specific alert
- **get_alerts**: Alerts are color-coded: red (high impact), orange (medium impact), green (low impact). Supports filtering by event type and time period.

Get disaster alerts
- **get_event_detail**: Get details for a specific disaster event
- **get_event_geojson**: Returns geographic boundaries, affected areas and population exposure polygons.

Get GeoJSON data for a disaster event
- **get_event_list**: Supports filtering by event type (EQ=earthquake, TC=cyclone, FL=flood, VO=volcano, WF=wildfire, DR=drought), date range, and time period. Returns event names, types, magnitudes, alert levels, start dates and affected countries.

Search disaster events
- **get_impacts**: Returns estimated population affected, fatalities, economic losses and confidence levels.

Get impact estimates for a disaster event
- **get_latest_cyclones**: Returns cyclone names, categories, wind speeds, locations, alert levels and forecast tracks.

Get latest tropical cyclones worldwide
- **get_latest_droughts**: Returns drought locations, start dates, severity levels, alert levels and affected populations.

Get latest drought events worldwide
- **get_latest_earthquakes**: Returns magnitude, depth, location, alert level and affected countries. Optionally filter by minimum magnitude and number of days.

Get latest earthquakes worldwide
- **get_latest_floods**: Returns flood locations, start dates, alert levels, affected populations and severity estimates.

Get latest floods worldwide
- **get_latest_volcanoes**: Returns volcano names, locations, eruption types, alert levels and ash plume information.

Get latest volcanic activity worldwide
- **get_latest_wildfires**: Returns fire locations, start dates, burned areas, alert levels and affected populations.

Get latest wildfires worldwide


## Installation & Usage

To install and use the **GDACS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gdacs](https://vinkius.com/mcp/gdacs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
