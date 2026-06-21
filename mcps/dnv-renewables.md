# DNV Renewables MCP Server

Access wind and solar resource data, energy yield estimates, and mesoscale climate data via DNV Renewables (ex-EMD) API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dnv-renewables)

## Overview
**Category:** the-unthinkable
**Tools Count:** 11

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


## Installation & Usage

To install and use the **DNV Renewables** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dnv-renewables](https://vinkius.com/mcp/dnv-renewables)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
