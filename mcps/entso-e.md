# ENTSO-E MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/entso-e)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/entso-e-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/entso-e-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access European electricity market data via ENTSO-E — track generation, load, prices, crossborder flows, and outages across European bidding zones from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ENTSO-E** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me day-ahead electricity prices for Germany tomorrow."

**🤖 AI Agent:**
> Fetching day-ahead prices for Germany (10YDE-RWENET---I)... Average price: 85.42 EUR/MWh. Peak hours (08:00-20:00): 98.15 EUR/MWh average. Off-peak: 62.30 EUR/MWh average. Highest price: 125.50 EUR/MWh at 18:00-19:00. Lowest price: 45.20 EUR/MWh at 03:00-04:00. Price drivers: High wind generation expected midday, low solar in evening driving evening peak. Would you like the hourly price breakdown?

---

**👤 You:**
> "What is the wind and solar forecast for France today?"

**🤖 AI Agent:**
> Fetching wind and solar forecast for France (10YFR-RTE------C)... Wind forecast: 8,450 MW average, peak 12,200 MW at 14:00. Solar forecast: 15,300 MW average, peak 32,500 MW at 13:00. Total renewable forecast: 23,750 MW average. Combined wind and solar expected to cover 55% of daytime demand. Strong solar generation expected between 10:00-16:00. Would you like to compare this with actual generation data?

---

**👤 You:**
> "Show me generation outages in Germany this week."

**🤖 AI Agent:**
> Checking generation outages for Germany... Found 3 active outages: 1) Nuclear plant Biblis B — 1,300 MW unavailable (planned maintenance, expected return: Friday). 2) Coal plant Neurath — 850 MW unavailable (unplanned outage, return TBD). 3) Gas plant Irsching — 400 MW unavailable (planned maintenance, expected return: Thursday). Total unavailable capacity: 2,550 MW. This represents approximately 3% of Germany's total installed capacity. Would you like impact analysis on expected prices?


## Installation & Usage

To install and use the **ENTSO-E** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/entso-e](https://vinkius.com/mcp/entso-e)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
