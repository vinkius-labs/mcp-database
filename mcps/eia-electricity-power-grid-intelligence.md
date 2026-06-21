# EIA Electricity — Power Grid Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eia-electricity-power-grid-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eia-electricity-power-grid-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eia-electricity-power-grid-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

U.S. power grid data: hourly demand by balancing authority, generation by fuel source, retail electricity prices by state, 100,000+ generator inventory, and individual power plant operations — from EIA-860, EIA-923, and EIA-930 surveys.

## Description
Real-time and historical intelligence on the entire U.S. power grid.

### What you can do
- **Grid Demand** — Hourly and daily demand by balancing authority (EIA-930)
- **Generation Mix** — Coal, gas, nuclear, solar, wind, hydro generation by state
- **Retail Prices** — Electricity prices (¢/kWh) by state and sector
- **Generator Inventory** — Every operable generator: capacity, fuel, location (EIA-860)
- **Plant Operations** — Individual plant generation and fuel consumption (EIA-923)
- **State Profiles** — Comprehensive state-level electricity data

### Who is this for?
Utility companies, grid operators, renewable energy developers, energy traders, ESG analysts, and infrastructure investors.


## Available Tools
- **get_electricity_prices**: Source: EIA-826, EIA-861.

Get retail electricity prices by state and sector
- **get_power_generation**: Source: EIA-923.

Get electric power generation by state, sector, and fuel source
- **get_grid_demand**: Covers all major U.S. grid operators. Source: EIA-930.

Get real-time hourly/daily electric grid demand
- **get_state_electricity_profiles**: Get comprehensive state electricity profiles
- **get_generator_inventory**: Over 100,000 generators. Source: EIA-860.

Get inventory of every operable generator in the U.S
- **get_plant_generation**: Includes net generation (MWh), fuel consumption, and heat rates. Source: EIA-923.

Get individual power plant operations by fuel and prime mover


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EIA Electricity — Power Grid Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the electricity price in California vs Texas?"

**🤖 AI Agent:**
> ⚡ **Retail Electricity Prices**

| State | Residential | Commercial | Industrial |
|-------|------------|------------|------------|
| CA | 29.8¢/kWh | 24.1¢ | 19.5¢ |
| TX | 13.2¢/kWh | 10.8¢ | 7.4¢ |

California residential prices are 2.3× higher than Texas.

---

**👤 You:**
> "What percentage of U.S. electricity comes from renewable sources?"

**🤖 AI Agent:**
> 🌱 **U.S. Generation Mix (Latest Year)**

- Natural Gas: 43.1%
- Nuclear: 18.6%
- Wind: 10.3%
- Coal: 16.2%
- Solar: 5.6%
- Hydro: 5.8%
- Other: 0.4%

**Total Renewables: 21.7%** (wind + solar + hydro)
Renewable share has doubled in the last decade.

---

**👤 You:**
> "How many solar generators are operating in Arizona?"

**🤖 AI Agent:**
> ☀️ **Arizona — Solar Generators**

Operable solar generators: 387
Total solar capacity: 6,842 MW
Largest: Agua Caliente (290 MW)
Avg capacity factor: ~28%

Arizona ranks #3 nationally in installed solar capacity.


## Installation & Usage

To install and use the **EIA Electricity — Power Grid Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eia-electricity-power-grid-intelligence](https://vinkius.com/mcp/eia-electricity-power-grid-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
