# Nord Pool MCP Server

Access European electricity market data via Nord Pool — query day-ahead prices, auction volumes, cross-border flows, and consumption forecasts from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nord-pool)

## Overview
**Category:** the-unthinkable
**Tools Count:** 10

## Description
Tap into the heartbeat of the European power market with **Nord Pool** — the continent's leading electricity exchange operating across 16 countries.

### What you can do

- **Day-Ahead Prices** — Retrieve clearing prices for any bidding zone (NO1, SE3, DK1, DE-LU, FR, NL, and more) in 15-minute Market Time Units
- **Yearly Price Trends** — Analyze long-term electricity price patterns and year-over-year performance for any delivery area
- **Auction Volumes** — Query traded volumes (MWh) per area to understand market depth and liquidity
- **Transmission Capacities** — Inspect Available Transmission Capacity (ATC) between interconnected bidding zones
- **Cross-Border Flows** — Track commercial auction flows and scheduled physical power transfers between regions
- **Flow-Based Constraints** — Access flow-based market coupling parameters for Core and Nordic domains
- **Consumption Forecasts** — Pull load forecasts that drive trading strategies and grid balancing decisions
- **Subscription Validation** — Verify which data products are available on your API account

### How it works

1. Subscribe to this server
2. Enter your Nord Pool API Client ID and Client Secret
3. Start querying live European electricity market data from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a real-time energy market analyst — no spreadsheets, no manual data exports, no switching between dashboards.

### Who is this for?

- **Energy Traders** — instantly pull day-ahead clearing prices and cross-border capacity to inform intraday positions
- **Portfolio Managers** — compare yearly price trends across multiple bidding zones without leaving the conversation
- **Grid Operators and Analysts** — access consumption forecasts and transmission capacities for operational planning
- **Research Teams** — automate the extraction of historical auction data for market modeling and forecasting


## Available Tools
- **get_auction_flows**: Requires both source and destination area codes. Flows reflect the scheduled energy exchange determined during the day-ahead market coupling process. Optionally filter by delivery date (YYYY-MM-DD).

Retrieve auction flows between two delivery areas
- **get_auction_volumes**: Use standard bidding zone codes separated by commas. Optionally filter by delivery date (YYYY-MM-DD). Volumes indicate the total cleared energy quantity per Market Time Unit in each area.

Retrieve day-ahead auction volumes for specified delivery areas
- **get_transmission_capacities**: Requires both source and destination area codes (e.g. NO1 to SE3). ATC represents the maximum commercial power transfer capacity allocated for the day-ahead market coupling. Optionally filter by delivery date (YYYY-MM-DD).

Retrieve Available Transmission Capacities (ATC) between two delivery areas
- **get_consumption_forecasts**: These forecasts represent the expected electricity consumption (load) for each Market Time Unit within a delivery area. Use standard bidding zone codes separated by commas. Optionally filter by delivery date (YYYY-MM-DD). Consumption forecasts are essential for production planning, trading strategy, and grid balancing decisions.

Retrieve power consumption forecasts by delivery area
- **get_day_ahead_prices**: Delivery areas are standard European bidding zone codes such as NO1, NO2, SE1, SE2, SE3, SE4, DK1, DK2, FI, EE, LV, LT, DE-LU, AT, FR, NL, BE, PL. You can pass multiple areas separated by commas. Optionally filter by a specific delivery date (YYYY-MM-DD) and currency (EUR, NOK, SEK, DKK, PLN, GBP). Prices are returned in 15-minute Market Time Units (MTU) by default since the transition to 15-min resolution in SDAC.

Retrieve day-ahead auction prices for specified delivery areas
- **get_flow_based_constraints**: Flow-based constraints define the allowable power transfer limits in flow-based market coupling regions (e.g. Core, Nordic). The domain parameter specifies which regional coupling zone to query. Optionally filter by delivery date (YYYY-MM-DD).

Retrieve flow-based constraints for a market coupling domain
- **get_scheduled_physical_flows**: These flows represent the planned physical cross-border electricity transfers, including both commercial exchanges and loop flows. Requires source and destination area codes. Optionally filter by delivery date.

Retrieve scheduled physical flows between two delivery areas
- **get_user_subscriptions**: Use this tool to verify which data products (Day-Ahead, Intraday, Power System Data, etc.) are available to the current credentials before attempting to query specific endpoints.

List the active API data subscriptions for the authenticated account
- **get_yearly_prices**: Use standard bidding zone codes (e.g. NO1, SE3, DE-LU). Optionally filter by year (YYYY) and currency. Useful for long-term price trend analysis and year-over-year comparisons.

Retrieve yearly aggregated auction prices for a delivery area
- **get_yearly_volumes**: Useful for analyzing annual energy consumption and trading patterns within a specific bidding zone.

Retrieve yearly aggregated auction volumes for a delivery area


## Installation & Usage

To install and use the **Nord Pool** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nord-pool](https://vinkius.com/mcp/nord-pool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
