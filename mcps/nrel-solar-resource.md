# NREL Solar Resource MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nrel-solar-resource)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nrel-solar-resource-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nrel-solar-resource-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access NREL's solar irradiance data and National Solar Radiation Database (NSRDB) information for any US location directly from your AI agent.

## Description
Connect your AI agent to the **National Renewable Energy Laboratory (NREL)** Solar Resource API to analyze solar potential and access historical radiation data through natural conversation.

### What you can do

- **Solar Irradiance** — Retrieve average solar irradiance data including Direct Normal Irradiance (DNI), Global Horizontal Irradiance (GHI), and Tilt at Latitude for specific coordinates.
- **NSRDB Queries** — Search the National Solar Radiation Database for the nearest datasets based on latitude/longitude, address, or Well-Known Text (WKT) geometry.
- **Data Sourcing** — Identify specific satellite or station-based datasets for renewable energy research and site assessment.

### How it works

1. Subscribe to this server
2. Enter your NREL API Key
3. Start querying solar data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Energy Analysts** — quickly assess the solar potential of specific geographic locations for project feasibility.
- **Researchers** — locate relevant NSRDB datasets for climate and energy studies without manual API calls.
- **Engineers** — retrieve precise irradiance metrics for solar installation planning directly in your workflow.


## Available Tools
- **get_solar_resource**: Get average solar irradiance data for a location
- **query_nsrdb_data**: Query nearest NSRDB datasets for a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NREL Solar Resource** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the average solar irradiance for latitude 34.05 and longitude -118.24?"

**🤖 AI Agent:**
> I've retrieved the solar resource data for those coordinates. The average Direct Normal Irradiance (DNI) is 6.24 kWh/m²/day, and the Global Horizontal Irradiance (GHI) is 5.12 kWh/m²/day.

---

**👤 You:**
> "Find the nearest NSRDB datasets for 'Golden, Colorado'."

**🤖 AI Agent:**
> Searching NSRDB for Golden, CO... I found several datasets. The closest station is located at 39.74, -105.17 with data available from the PSM V3 satellite model. Would you like the download links?

---

**👤 You:**
> "Query satellite-based NSRDB data for the coordinates 40.71, -74.00."

**🤖 AI Agent:**
> I've filtered the NSRDB for satellite datasets at those coordinates. I found a high-resolution satellite dataset (PSM) covering that area. It includes 30-minute interval data for solar radiation and meteorological variables.


## Installation & Usage

To install and use the **NREL Solar Resource** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nrel-solar-resource](https://vinkius.com/mcp/nrel-solar-resource)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
