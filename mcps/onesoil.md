# OneSoil MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onesoil)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/onesoil-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/onesoil-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage agricultural fields, monitor crop health via NDVI, and access hyper-local weather data directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneSoil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my fields in OneSoil."

**🤖 AI Agent:**
> I've retrieved your fields. You have 3 active boundaries: 'North Corn' (ID: 123), 'South Soy' (ID: 456), and 'East Wheat' (ID: 789). Which one would you like to inspect?

---

**👤 You:**
> "Get the NDVI history for field 123."

**🤖 AI Agent:**
> Retrieving NDVI data for field 123... I found 10 historical data points. The vegetation index peaked at 0.82 in mid-July, indicating healthy growth during that period.

---

**👤 You:**
> "What is the 7-day weather forecast for lat 53.9, lon 27.5?"

**🤖 AI Agent:**
> Fetching the forecast for those coordinates... Expect clear skies for the next 3 days with temperatures between 18°C and 24°C, followed by light rain on Thursday.


## Installation & Usage

To install and use the **OneSoil** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onesoil](https://vinkius.com/mcp/onesoil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
