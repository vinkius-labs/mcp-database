# DNV Renewables MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dnv-renewables)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dnv-renewables-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dnv-renewables-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access wind and solar resource data, energy yield estimates, and mesoscale climate data via DNV Renewables (ex-EMD) API.

## Description
Connect to **DNV Renewables API** (formerly EMD - Energy and Market Data) and bring world-class wind and solar resource assessment intelligence to any AI agent. Access over 40 climate datasets with mesoscale data, energy yield estimates, and time series extraction for renewable energy projects.

### What you can do

- **Wind Resource Assessment** — Get wind speed, direction, and temperature data for any global location
- **Solar Resource Assessment** — Access GHI, DNI, DHI, temperature, and wind speed for PV project planning
- **Energy Yield Estimates** — Calculate estimated annual energy production (AEP) for wind turbine configurations
- **Mesoscale Climate Data** — Retrieve long-term climate model data for resource assessment
- **Dataset Catalog** — Browse 40+ available climate datasets including mesoscale, reanalysis, and atlas data
- **Data Availability** — Check what data exists for any geographic coordinates before ordering
- **Data Node Location** — Find geographic coverage areas and data nodes for specific datasets
- **Order Management** — Place data orders, track status, and download completed time series files
- **Global Coverage** — Access wind and solar data for onshore and offshore locations worldwide
- **Custom Time Periods** — Request data for specific date ranges from historical archives

### How it works

1. Subscribe to this server
2. Enter your DNV Renewables API token (requires DNV account)
3. Start querying wind, solar, and climate data from Claude, Cursor, or any MCP-compatible client

Your AI becomes a renewable energy analyst, helping you assess sites, estimate yields, and make data-driven renewable energy decisions.

### Who is this for?

- **Wind Developers** — assess wind resource potential and estimate energy yields for project development
- **Solar Developers** — evaluate solar irradiance and resource quality for PV site selection
- **Energy Consultants** — provide clients with professional-grade resource assessments
- **Researchers** — access validated mesoscale climate data for academic studies
- **Utilities** — integrate resource data into generation planning and portfolio management
- **Investors** — evaluate renewable energy project potential with professional-grade data


## Available Tools
- **check_data_availability**: Returns available datasets, time periods, and variables. Essential first step before ordering data.

Check data availability for wind and solar at a specific location
- **download_order_data**: Order must have status success. Files auto-deleted after 12 hours.

Download completed order data file
- **get_energy_yield_estimate**: Uses site-specific wind data and turbine parameters to estimate annual energy production.

Get energy yield estimate for a wind turbine at a specific location
- **get_order_status**: Orders go from pending to processing to success. Once success, a download URL is provided. Files auto-delete after 12 hours.

Check status of a previously placed data order
- **list_available_datasets**: Over 40 datasets available.

List all available climate and renewable energy datasets
- **list_all_orders**: List all data orders in your account
- **locate_data_nodes**: Useful for understanding spatial resolution and coverage.

Locate data nodes for a specific dataset
- **get_mesoscale_climate_data**: Useful for long-term climate analysis.

Get mesoscale climate data for a location
- **place_data_order**: The API processes the request and generates a downloadable file. Use getOrderStatus to check when complete.

Place an order for climate data extraction
- **get_solar_resource_data**: Essential for PV system design and energy yield analysis. Use when user needs solar irradiance data, is assessing solar resource potential, or wants solar data for PV modeling.

Get solar resource data for a specific location
- **get_wind_resource_data**: Essential for wind farm site assessment and energy yield analysis. Use when user needs wind data for a site, is assessing wind resource potential, or wants wind data for energy modeling.

Get wind resource data for a specific location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DNV Renewables** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check what wind data is available for a site at 55.5, 12.0."

**🤖 AI Agent:**
> Checking data availability... For coordinates 55.5, 12.0 (Denmark), the following datasets are available: meso-scale-wind (1989-present), ERA5 reanalysis (1950-present), Global Wind Atlas. Wind speed data at multiple hub heights (10m-200m) is available. Time series can be extracted for any period within these ranges.

---

**👤 You:**
> "Estimate energy yield for a 5MW wind turbine at 55.5, 12.0 with 120m hub height."

**🤖 AI Agent:**
> Calculating energy yield... For a 5MW turbine at 55.5, 12.0 with 120m hub height, the estimated annual energy production (AEP) is approximately 18,500-21,000 MWh/year. The site shows good wind resource with mean wind speed of 7.8 m/s at hub height. Capacity factor is estimated at 42-48%. A full P50/P75/P90 analysis would require a detailed order for complete time series.

---

**👤 You:**
> "Get solar resource data for a PV site at 35.0, -106.0 (New Mexico)."

**🤖 AI Agent:**
> Fetching solar resource data... For coordinates 35.0, -106.0 (New Mexico), the site shows excellent solar resource. Annual GHI averages approximately 2,150 kWh/m²/year. DNI is around 780 kWh/m²/year, indicating strong direct sunlight ideal for concentrating solar. The site has low cloud cover and minimal soiling concerns. Temperature averages 14°C annually, which is favorable for PV module efficiency.


## Installation & Usage

To install and use the **DNV Renewables** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dnv-renewables](https://vinkius.com/mcp/dnv-renewables)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
