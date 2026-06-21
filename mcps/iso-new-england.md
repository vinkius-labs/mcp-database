# ISO New England MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iso-new-england)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iso-new-england-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iso-new-england-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access real-time and historical energy market data via ISO New England API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ISO New England** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current system load in ISO New England?"

**🤖 AI Agent:**
> I'll fetch the real-time system load data for you.

---

**👤 You:**
> "Show me the current fuel mix for electricity generation."

**🤖 AI Agent:**
> I'll retrieve the real-time generation fuel mix from ISO-NE.

---

**👤 You:**
> "Get the latest locational marginal prices (LMP)."

**🤖 AI Agent:**
> I'll look up the current 5-minute LMP data for the New England grid.


## Installation & Usage

To install and use the **ISO New England** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iso-new-england](https://vinkius.com/mcp/iso-new-england)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
