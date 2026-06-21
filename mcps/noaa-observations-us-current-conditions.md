# NOAA Observations — US Current Conditions MCP Server

Real-time weather observations from thousands of official NWS stations: temperature, wind speed and direction, humidity, barometric pressure, visibility, and weather conditions across the United States.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-observations-us-current-conditions)

## Overview
**Category:** the-unthinkable
**Tools Count:** 5

## Description
Real-time sensor data from thousands of NWS stations.

### What you can do
- **Find Stations** — Locate nearby weather stations by lat/lon
- **Current Conditions** — Latest observation (temp, wind, pressure, humidity)
- **Recent History** — Observation trend over past hours
- **Station Metadata** — Details about each station
- **Radar Network** — NEXRAD radar station status


## Available Tools
- **get_stations**: Each station has a 4-character ID (e.g., KJFK, KLAX). US only. Use station IDs with get_latest_observation.

Find nearby NWS weather observation stations by latitude/longitude
- **get_latest_observation**: Provide a 4-character station ID such as KJFK, KLAX, KORD, KDFW.

Get current weather conditions from a specific NWS station
- **get_observation_history**: Useful for seeing temperature trends, wind changes, and weather evolution over recent hours.

Get recent observation history for a NWS station
- **get_station_metadata**: Useful for understanding where a station is and what data it provides.

Get metadata about a specific NWS weather station
- **get_radar_stations**: List all NWS radar stations and their status


## Installation & Usage

To install and use the **NOAA Observations — US Current Conditions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-observations-us-current-conditions](https://vinkius.com/mcp/noaa-observations-us-current-conditions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
