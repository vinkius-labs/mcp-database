# Meteostat MCP Server

Access historical weather data and climate statistics from thousands of weather stations and geographic points worldwide.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/meteostat)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Connect to **Meteostat** to empower your AI agent with one of the largest databases of historical weather and climate data. Whether you need to analyze past weather patterns for a specific city or interpolate data for a remote coordinate, this server provides the tools to fetch precise meteorological records.

### What you can do

- **Station Discovery** — Use `stations_nearby` to find weather stations based on GPS coordinates and radius.
- **Historical Observations** — Fetch hourly, daily, or monthly data using `stations_hourly`, `stations_daily`, or `stations_monthly` for specific stations.
- **Point Interpolation** — Get weather data for any location on Earth, even without a local station, using `point_hourly` and `point_daily` tools.
- **Climate Normals** — Access long-term averages (30-year periods) via `stations_normals` to understand regional climate baselines.
- **Metadata & Search** — Retrieve detailed station information including WMO and ICAO identifiers using `stations_meta`.

### How it works

1. Subscribe to this server
2. Enter your Meteostat RapidAPI Key
3. Start querying weather history from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — quickly pull historical weather datasets for environmental analysis or machine learning models.
- **Travel & Logistics Planners** — check historical weather patterns for specific dates and locations to optimize routing or event planning.
- **Developers** — integrate weather context into applications without building complex scrapers or data pipelines.


## Available Tools
- **point_daily**: Get historical daily point data
- **point_hourly**: Get historical hourly point data
- **point_monthly**: Get historical monthly point data
- **point_normals**: Get climate normals for a point location
- **stations_daily**: Max 10 years per request.

Get historical daily statistics for a station
- **stations_hourly**: Max 30 days per request.

Get historical hourly observations for a station
- **stations_meta**: Specify at least one identifier (id, wmo, or icao).

Get metadata for a specific weather station
- **stations_monthly**: Get historical monthly statistics for a station
- **stations_nearby**: Find nearby weather stations by geo location
- **stations_normals**: Get climate normals for a station


## Installation & Usage

To install and use the **Meteostat** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meteostat](https://vinkius.com/mcp/meteostat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
