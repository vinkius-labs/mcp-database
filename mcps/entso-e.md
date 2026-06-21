# ENTSO-E MCP Server

Access European electricity market data via ENTSO-E — track generation, load, prices, crossborder flows, and outages across European bidding zones from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/entso-e)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

## Description
Connect your **ENTSO-E Transparency Platform API** to any AI agent and take full control of European electricity market data, generation forecasts, pricing analysis, and grid monitoring through natural conversation.

### What you can do

- **Day-Ahead Generation** — Get generation forecasts by energy source (nuclear, fossil, renewable) for any bidding zone
- **Actual Generation** — Retrieve historical generation data broken down by energy source
- **Load Forecasts** — Access day-ahead and actual electricity consumption data
- **Market Prices** — Get day-ahead electricity market clearing prices (EUR/MWh)
- **Crossborder Flows** — Monitor scheduled electricity imports and exports between zones
- **Generation Outages** — Track planned and unplanned power plant outages
- **Transmission Outages** — Monitor grid maintenance and line outages
- **Installed Capacity** — Track installed generation capacity by energy source
- **Balancing Prices** — Access upward and downward regulation prices
- **Wind & Solar Forecasts** — Get renewable energy generation forecasts

### How it works

1. Subscribe to this server
2. Enter your ENTSO-E security token (request via email to transparency@entsoe.eu)
3. Start analyzing European energy markets from Claude, Cursor, or any MCP-compatible client

No more manual XML parsing or complex API queries. Your AI acts as a dedicated European energy market analyst.

### Who is this for?

- **Energy Traders** — monitor prices, generation, and flows for trading decisions
- **Grid Operators** — track outages, balancing prices, and grid stability
- **Renewable Analysts** — analyze wind and solar forecasts against actual generation
- **Researchers** — access comprehensive European energy market data for studies


## Available Tools
- **get_actual_generation**: ) for a specific bidding zone. Essential for post-market analysis, renewable energy performance tracking, and grid balance analysis. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get actual electricity generation data by energy source for a European bidding zone
- **get_actual_load**: Essential for demand analysis, peak demand identification, and load forecasting validation. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get actual electricity load data for a European bidding zone
- **get_balancing_prices**: Essential for imbalance cost analysis, balancing market participation, and grid stability assessment. Area codes are ENTSO-E control area identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get balancing market prices for a control area
- **get_crossborder_flows**: Essential for interconnection analysis, cross-border trading, and grid congestion assessment. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get scheduled cross-border electricity flows for a bidding zone
- **get_day_ahead_generation**: ) for a specific European bidding zone. Data is provided in MW per time period (typically hourly). Essential for energy trading, grid planning, and renewable energy integration analysis. Area codes are ENTSO-E bidding zone identifiers (e.g., "10YDE-RWENET---I" for Germany, "10YFR-RTE------C" for France). Date format: YYYYMMDDHHmm in UTC. Returns XML data from the Transparency Platform.

Get day-ahead electricity generation forecasts for a European bidding zone
- **get_day_ahead_load**: Essential for energy trading, demand response planning, and grid balancing. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get day-ahead electricity load forecasts for a European bidding zone
- **get_day_ahead_prices**: Essential for energy trading, price forecasting, and market analysis. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get day-ahead electricity market prices for a European bidding zone
- **get_forecasted_generation**: Essential for energy market analysis, supply-demand balancing, and grid operation planning. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get total generation and load forecasts for a bidding zone
- **get_generation_outages**: Essential for supply security assessment, capacity planning, and market impact analysis. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get generation outage and maintenance schedules for a bidding zone
- **get_installed_generation**: ) for a specific bidding zone. Essential for capacity adequacy analysis, energy transition tracking, and infrastructure planning. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get installed generation capacity by energy source for a bidding zone
- **get_transmission_outages**: Essential for grid congestion analysis, capacity calculation, and market impact assessment. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get transmission network outage and maintenance schedules
- **get_wind_solar_forecast**: Essential for renewable energy integration analysis, grid balancing, and energy trading. Area codes are ENTSO-E bidding zone identifiers. Date format: YYYYMMDDHHmm in UTC. Returns XML data.

Get wind and solar power generation forecasts for a bidding zone


## Installation & Usage

To install and use the **ENTSO-E** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/entso-e](https://vinkius.com/mcp/entso-e)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
