# Agro MCP Server

Monitor agricultural land using satellite imagery, weather data, and soil metrics directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/agro)

## Overview
**Category:** data-analytics
**Tools Count:** 17

## Description
Connect the **AgroMonitoring API** to your AI agent to transform how you manage precision agriculture. Access high-resolution satellite data, historical crop health indices, and hyper-local weather conditions through simple commands.

### What you can do

- **Polygon Management** — Create, list, and update areas of interest (polygons) representing your fields or farms.
- **Satellite Insights** — Search for available satellite imagery and retrieve NDVI (Normalized Difference Vegetation Index) and EVI history to track crop health over time.
- **Weather Intelligence** — Get current, forecast, and historical weather data, including accumulated temperature and precipitation metrics.
- **Soil & UV Monitoring** — Access real-time and historical soil moisture and temperature data, along with UV index tracking for optimal field management.

### How it works

1. Subscribe to this server
2. Enter your AgroMonitoring API Key
3. Start querying field data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agronomists & Farmers** — Monitor crop health and soil conditions across multiple fields without manual data entry.
- **Data Scientists** — Quickly pull historical weather and satellite indices for agricultural modeling.
- **AgTech Developers** — Integrate field-level environmental data into your development workflow via natural language.


## Available Tools
- **delete_polygon**: Delete a polygon
- **get_current_weather**: Get current weather data
- **get_current_uvi**: Get current UV Index
- **create_polygon**: Create a new polygon for an area of interest
- **get_accumulated_precipitation**: Get accumulated precipitation
- **get_accumulated_temperature**: Get accumulated temperature
- **get_forecast_uvi**: Get forecast UV Index
- **get_forecast_weather**: Get forecast weather data
- **get_historical_soil**: Get historical soil data
- **get_historical_uvi**: Get historical UV Index
- **get_current_soil**: Get current soil data
- **get_historical_weather**: Get historical weather data
- **get_ndvi_history**: Get NDVI and EVI historical data
- **get_polygon**: Get info for one polygon
- **list_polygons**: Get list of polygons
- **search_imagery**: Search for satellite imagery
- **update_polygon**: Update polygon info


## Installation & Usage

To install and use the **Agro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agro](https://vinkius.com/mcp/agro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
