# AEMO Australian Energy MCP Server

Access Australian electricity market data — spot prices, demand, generation by fuel type, emissions, and renewable energy proportions via OpenElectricity API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aemo-australian-energy)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

## Description
Connect to **OpenElectricity API** (powered by AEMO data) and bring real-time Australian energy market intelligence to any AI agent. Monitor the National Electricity Market (NEM) and Wholesale Electricity Market (WEM), track renewable energy transition, and analyze power generation across all Australian states.

### What you can do

- **Spot Prices** — Retrieve real-time and historical wholesale electricity prices (RRP) by Australian region (NSW, VIC, QLD, SA, TAS)
- **Power Generation** — Access total network generation and breakdown by fuel technology (solar, wind, coal, gas, hydro, battery)
- **Energy Demand** — Monitor electricity demand across the NEM with 5-minute, hourly, daily, or monthly granularity
- **Facility Data** — Get generation output from specific power stations, solar farms, wind farms, and battery installations
- **Renewable Proportion** — Track what percentage of Australia's electricity comes from renewable sources in real-time
- **Regional Analysis** — Compare power generation and demand across Australian states and territories
- **Emissions Tracking** — Query pollution data including NOx, SO2, CO, PM10, PM2.5 from the National Pollutant Inventory
- **Market Updates** — Fetch commentary and updates about price spikes, outages, and notable market events
- **Facility Registry** — List all energy generation facilities with their fuel type, status, and capacity
- **Available Metrics** — Explore the full range of queryable metrics in the API
- **User Account** — Check your API plan, rate limits, and usage statistics
- **Plans & Pricing** — View available subscription tiers and features

### How it works

1. Subscribe to this server
2. Enter your OpenElectricity API Bearer token (free Community plan available)
3. Start querying Australian energy data from Claude, Cursor, or any MCP-compatible client

Your AI becomes an Australian energy analyst, helping you understand the grid, track the renewable transition, and make data-driven decisions.

### Who is this for?

- **Energy Analysts** — retrieve spot prices, generation mix, and demand forecasts for market reports
- **Sustainability Teams** — monitor renewable energy proportions and emissions for environmental reporting
- **Researchers & Academics** — access granular 5-minute interval data for energy studies and modeling
- **Homeowners with Solar** — understand when wholesale prices are negative (solar duck curve) and optimize self-consumption
- **EV Owners** — find optimal charging times when prices are low and renewable proportion is high
- **Policy Makers** — track Australia's energy transition progress and state-by-state renewable adoption


## Available Tools
- **list_facilities**: Filter by fuel technology, status, network, or facility code.

List energy facilities and generation units
- **get_facility_data**: g. "ER01" for Eraring, "BNGSF1" for Bungala Solar). Shows actual output over time.

Get generation data for a specific energy facility
- **get_market_data**: Supports interval and date range filtering.

Get market data including spot prices and demand by region
- **list_metrics**: List all available metrics in the OpenElectricity API
- **get_network_by_fueltech**: Useful for understanding the energy mix and renewable vs fossil fuel split.

Get network data grouped by fuel technology type
- **get_network_by_region**: Get network data grouped by Australian region/state
- **get_network_data**: Supports interval aggregation (5m, 1h, 1d, 7d, 1M, 1y) and date range filtering.

Get time series network data for power, energy, demand and generation
- **get_plans**: Get available API plans and pricing tiers
- **get_pollution_data**: 5, VOC) reported to the National Pollutant Inventory by energy facilities. Filter by facility, pollutant, or category.

Get pollution and emissions data from NPI (National Pollutant Inventory)
- **get_renewable_proportion**: Essential for tracking Australia's energy transition progress.

Get renewable energy proportion data
- **get_market_updates**: Get market updates and social posts from OpenElectricity
- **get_user_profile**: Get current user profile and API account details


## Installation & Usage

To install and use the **AEMO Australian Energy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aemo-australian-energy](https://vinkius.com/mcp/aemo-australian-energy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
