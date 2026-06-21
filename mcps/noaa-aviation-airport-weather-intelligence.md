# NOAA Aviation — Airport Weather Intelligence MCP Server

Aviation weather data worldwide: METARs (current airport conditions), TAFs (24-hour airport forecasts), PIREPs (pilot reports of turbulence and icing), and SIGMETs/AIRMETs (significant aviation hazards) from the Aviation Weather Center.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-aviation-airport-weather-intelligence)

## Overview
**Category:** the-unthinkable
**Tools Count:** 5

## Description
The definitive aviation weather intelligence from the NOAA Aviation Weather Center.

### What you can do
- **METAR** — Current airport conditions (works worldwide with ICAO codes)
- **TAF** — 24-30 hour airport forecasts
- **PIREP** — Pilot reports: turbulence, icing, visibility in-flight
- **SIGMET/AIRMET** — Significant hazard areas
- **Station Info** — Airport weather station details

### Global Coverage
METARs and TAFs work worldwide using ICAO codes (KJFK, EGLL, LFPG, SBGR).


## Available Tools
- **get_metar**: Provide ICAO codes comma-separated (KJFK, EGLL, LFPG). Returns temperature, wind, visibility, clouds, pressure, weather phenomena. Optionally retrieve past hours of data.

Get METAR (current airport weather) for any airport worldwide by ICAO code
- **get_taf**: Includes forecast groups with wind, visibility, clouds, and weather changes. ICAO codes only.

Get TAF (airport weather forecast) for any airport worldwide by ICAO code
- **get_pirep**: Filter by age (hours).

Get PIREPs (Pilot Reports) for turbulence, icing, and weather conditions
- **get_sigmet**: These define areas of significant weather hazards for aviation: convection, turbulence, icing, IFR conditions, mountain obscuration.

Get SIGMETs and AIRMETs — significant aviation weather hazards
- **get_aviation_station**: Use ICAO codes (KJFK, EGLL, LFPG, SBGR).

Get aviation weather station information by ICAO code


## Installation & Usage

To install and use the **NOAA Aviation — Airport Weather Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-aviation-airport-weather-intelligence](https://vinkius.com/mcp/noaa-aviation-airport-weather-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
