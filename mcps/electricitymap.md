# ElectricityMap MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/electricitymap)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/electricitymap-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/electricitymap-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and forecasted electricity carbon intensity and power breakdown data for over 200 regions worldwide.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ElectricityMap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current carbon intensity in France (FR)?"

**🤖 AI Agent:**
> I've checked the latest data for France (FR). The current carbon intensity is 45 gCO2eq/kWh, which is quite low due to high nuclear and wind production.

---

**👤 You:**
> "Show me the power breakdown for zone DK-DK1 right now."

**🤖 AI Agent:**
> The power breakdown for DK-DK1 shows that 65% of electricity is currently coming from wind, 15% from solar, and the rest from biomass and imports.

---

**👤 You:**
> "What is the forecasted carbon intensity for Germany (DE) for the next few hours?"

**🤖 AI Agent:**
> The forecast for Germany (DE) indicates that carbon intensity will drop from 350 to 280 gCO2eq/kWh over the next 4 hours as solar production increases.


## Installation & Usage

To install and use the **ElectricityMap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/electricitymap](https://vinkius.com/mcp/electricitymap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
