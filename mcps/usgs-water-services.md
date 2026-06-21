# USGS Water Services MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usgs-water-services)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/usgs-water-services-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/usgs-water-services-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access real-time and historical water data from the USGS, including streamflow, groundwater levels, and site metadata across the US.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USGS Water Services** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all active USGS water monitoring sites in Florida."

**🤖 AI Agent:**
> I've found several active sites in Florida. For example, site 02236000 (ST. JOHNS RIVER NEAR COCOA, FL) and site 02248000 (ST. JOHNS RIVER NEAR DE LAND, FL). Would you like to see the full list or details for a specific one?

---

**👤 You:**
> "Get the last 7 days of water level data for site 08313000."

**🤖 AI Agent:**
> Retrieving data for site 08313000 (RIO GRANDE AT OTOWI BRIDGE, NM)... Over the last 7 days, the gage height has fluctuated between 3.12 and 3.45 feet. Would you like a more detailed breakdown of the 15-minute intervals?

---

**👤 You:**
> "What are the daily mean statistics for discharge at site 01646500?"

**🤖 AI Agent:**
> For site 01646500 (POTOMAC RIVER NEAR WASH, DC), the daily mean discharge for today's date historically is 12,400 cubic feet per second (cfs). The record high for this day was 85,000 cfs in 1996.


## Installation & Usage

To install and use the **USGS Water Services** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usgs-water-services](https://vinkius.com/mcp/usgs-water-services)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
