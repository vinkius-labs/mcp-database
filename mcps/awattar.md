# Awattar MCP Server

Access real-time electricity prices from aWATTar — retrieve EPEX Spot market data and optimized YAML stats for home automation directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/awattar)

## Overview
**Category:** iot-hardware
**Tools Count:** 2

## Description
Connect to **aWATTar** to monitor electricity market prices and optimize your smart home energy consumption. This server provides direct access to EPEX Spot stock prices and specialized data formats for automation systems.

### What you can do

- **Market Price Tracking** — Fetch real-time and historical EPEX Spot electricity prices to understand market trends and costs.
- **Home Automation Integration** — Get price statistics and hourly thresholds formatted in YAML, specifically designed for LOXONE and other smart home controllers.
- **Smart Scheduling** — Access tomorrow's prices (updated daily at 14:00 CET) to schedule high-consumption appliances during the cheapest hours.
- **Data Analysis** — Retrieve market data for specific time intervals using epoch timestamps for precise energy reporting.

### How it works

1. Subscribe to this server
2. Configure your access credentials if required by your region
3. Start querying energy data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Smart Home Enthusiasts** — feed real-time price data into Loxone or Home Assistant to automatically save on energy bills.
- **Sustainability Advocates** — shift energy usage to times when renewable production is high and prices are low.
- **IoT Developers** — build energy-aware applications using clean, structured market data directly in your development workflow.


## Available Tools
- **get_current_yaml**: Get current aWATTar price statistics in YAML format
- **get_market_data**: Prices for the next day are typically updated daily at 14:00 (CET/CEST).

Get aWATTar market data (electricity prices)


## Installation & Usage

To install and use the **Awattar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/awattar](https://vinkius.com/mcp/awattar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
