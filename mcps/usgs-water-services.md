# USGS Water Services MCP Server

Access real-time and historical water data from the USGS, including streamflow, groundwater levels, and site metadata across the US.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/usgs-water-services)

## Overview
**Category:** industry-titans
**Tools Count:** 5

## Description
Connect to the **USGS Water Services** to retrieve comprehensive hydrological data directly from the United States Geological Survey. Monitor environmental conditions, analyze historical trends, and discover monitoring stations through natural language.

### What you can do

- **Real-time Monitoring** — Use `get_instantaneous_values` to fetch near real-time data (15-minute intervals) for streamflow, water levels, and quality.
- **Historical Analysis** — Retrieve daily summaries (mean, median, max, min) using `get_daily_values` for long-term trend analysis.
- **Site Discovery** — Search for monitoring stations using `get_sites` filtered by state, county, hydrologic unit (HUC), or geographic bounding box.
- **Statistical Reports** — Generate daily, monthly, or annual statistics with `get_statistics` to understand hydrological patterns.
- **Groundwater Tracking** — Access specialized groundwater level data using `get_groundwater_levels` for aquifer monitoring.

### How it works

1. Subscribe to this server
2. This service accesses public USGS data; simply enter 'PUBLIC' as your access key to initialize
3. Start querying water data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Environmental Scientists** — quickly gather field data and historical records for research and reporting
- **Engineers & Hydrologists** — monitor streamflow and groundwater levels for infrastructure and flood planning
- **Outdoor Enthusiasts** — check real-time river conditions for fishing, boating, or safety before heading out


## Available Tools
- **get_daily_values**: You MUST provide at least one major filter.

Retrieve historical summarized daily data (mean, median, max, min)
- **get_groundwater_levels**: You MUST provide at least one major filter.

Retrieve historical manually-recorded groundwater levels
- **get_instantaneous_values**: You MUST provide at least one major filter: sites, stateCd, huc, bBox, or countyCd.

Retrieve near real-time water data (usually 15-minute intervals)
- **get_sites**: Multiple major filters can be combined (AND logic).

Search for USGS sites and metadata
- **get_statistics**: Retrieve daily, monthly, or annual statistics based on approved data


## Installation & Usage

To install and use the **USGS Water Services** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usgs-water-services](https://vinkius.com/mcp/usgs-water-services)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
