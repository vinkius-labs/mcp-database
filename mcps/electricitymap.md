# ElectricityMap MCP Server

Access real-time and forecasted electricity carbon intensity and power breakdown data for over 200 regions worldwide.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/electricitymap)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Connect to **ElectricityMap** to empower your AI agent with global grid transparency. Track the carbon footprint of electricity in real-time, analyze historical trends, and optimize consumption based on green energy forecasts.

### What you can do

- **Real-time Intensity** — Fetch the current carbon intensity (gCO2eq/kWh) for specific zones or GPS coordinates.
- **Power Breakdown** — See exactly where electricity comes from, including solar, wind, nuclear, coal, and gas production.
- **Forecasting** — Get 24-hour forecasts for carbon intensity and power production to schedule energy-intensive tasks during green peaks.
- **Historical Analysis** — Query past data to audit carbon footprints or analyze grid behavior over time.
- **Zone Discovery** — List all supported geographical zones and their metadata to ensure precise data retrieval.

### How it works

1. Subscribe to this server
2. Enter your ElectricityMap API Key
3. Start querying global energy data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sustainability Officers** — Automate carbon reporting and monitor corporate energy footprints across global offices.
- **Software Engineers** — Build carbon-aware applications that trigger background jobs when the grid is cleanest.
- **Data Analysts** — Correlate energy production trends with climate data or market pricing.


## Available Tools
- **get_carbon_intensity_forecast**: Get forecasted carbon intensity for a zone
- **get_carbon_intensity_history**: Get historical carbon intensity for a zone
- **get_carbon_intensity_latest**: Get latest carbon intensity for a zone
- **list_zones**: List all available zones
- **get_marginal_carbon_intensity_latest**: Get latest marginal carbon intensity
- **get_power_breakdown_forecast**: Get forecasted power breakdown for a zone
- **get_power_breakdown_history**: Get historical power breakdown for a zone
- **get_power_breakdown_latest**: Get latest power breakdown for a zone


## Installation & Usage

To install and use the **ElectricityMap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/electricitymap](https://vinkius.com/mcp/electricitymap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
