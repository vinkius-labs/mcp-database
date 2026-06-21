# OneSoil MCP Server

Manage agricultural fields, monitor crop health via NDVI, and access hyper-local weather data directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/onesoil)

## Overview
**Category:** data-analytics
**Tools Count:** 9

## Description
Connect your **OneSoil** account to any AI agent to streamline precision farming and field management through natural conversation.

### What you can do

- **Field Management** — List, create, and inspect field boundaries and metadata using GeoJSON geometries.
- **Crop Monitoring** — Retrieve historical NDVI (Normalized Difference Vegetation Index) values to track vegetation health over time.
- **Satellite Insights** — List available Sentinel-2 satellite imagery for specific fields to plan scouting or analysis.
- **Hyper-local Weather** — Access current conditions, 7-day forecasts, and historical weather data based on precise field coordinates.

### How it works

1. Subscribe to this server
2. Enter your OneSoil API Key
3. Start managing your farm data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agronomists** — quickly check NDVI trends and weather history to provide better crop recommendations.
- **Farm Managers** — organize field boundaries and monitor satellite availability without switching between multiple apps.
- **AgTech Developers** — integrate precision agriculture data directly into your coding or analysis workflow.


## Available Tools
- **create_field**: Create a new field boundary
- **get_current_weather**: Provide latitude and longitude.

Get current weather for field coordinates
- **get_weather_history**: Provide latitude and longitude.

Get historical weather data for field coordinates
- **delete_field**: Remove a field
- **get_field**: Retrieve details for a specific field
- **list_images**: List available satellite images for a field
- **get_ndvi**: Get historical NDVI values for a field
- **list_fields**: List all fields in your account
- **get_weather_forecast**: Provide latitude and longitude.

Get a 7-day weather forecast for field coordinates


## Installation & Usage

To install and use the **OneSoil** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onesoil](https://vinkius.com/mcp/onesoil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
