# ISO New England MCP Server

Access real-time and historical energy market data via ISO New England API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/iso-new-england)

## Overview
**Category:** the-unthinkable
**Tools Count:** 10

## Description
Empower your AI agents to monitor the New England power grid with the ISO-NE Web Services API. This MCP server allows you to retrieve real-time system load, generation fuel mix, locational marginal prices (LMP), and market forecasts directly through the official ISO New England API. Ideal for energy analysis, grid monitoring, and market research.


## Available Tools
- **get_actual_interchange**: g., NYISO, Hydro-Quebec). Essential for understanding net imports and exports of electricity.

Retrieves actual interchange data
- **get_day_ahead_lmp**: Useful for anticipating energy costs and market planning.

Retrieves day-ahead Locational Marginal Prices (LMP)
- **get_fuel_mix**: g., Natural Gas, Nuclear, Renewables). Use this to analyze the environmental impact and energy sources powering the grid.

Retrieves real-time generation fuel mix
- **get_hourly_lmp**: Use this for historical price analysis or when 5-minute granularity is not required.

Retrieves hourly Locational Marginal Prices (LMP)
- **get_hourly_load**: Use this for analyzing long-term consumption patterns and demand forecasting performance.

Retrieves hourly load data
- **get_lmp**: Returns prices in USD/MWh. Essential for tracking energy market volatility and cost of power at specific locations.

Retrieves 5-minute Locational Marginal Prices (LMP)
- **get_regulation**: Includes clearing prices and capacity requirements. Useful for analyzing grid stability services.

Retrieves regulation requirements and clearing prices
- **get_reserve**: Essential for auditing grid resilience capacity.

Retrieves reserve requirements and clearing prices
- **get_seven_day_forecast**: Essential for anticipating grid stress and planning energy procurement.

Retrieves the seven-day load forecast
- **get_system_load**: Returns current load in megawatts (MW). Essential for monitoring grid stress and power consumption trends.

Retrieves real-time system load data


## Installation & Usage

To install and use the **ISO New England** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iso-new-england](https://vinkius.com/mcp/iso-new-england)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
