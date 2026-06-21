# EIA Full Access — U.S. Energy Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eia-full-access-us-energy-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eia-full-access-us-energy-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eia-full-access-us-energy-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

The ultimate U.S. energy data Mega-Server: 34 tools covering petroleum, electricity, natural gas, coal, energy forecasts, state data, and international comparisons — every watt, barrel, and BTU from the federal government's energy agency.

## Description
The **definitive Mega-Server** for U.S. energy intelligence. Why install 6 servers when one does it all?

### What you can do
- **🛢️ Petroleum (8 tools)** — WTI/Brent, gasoline, refinery, stocks, SPR, crude imports
- **⚡ Electricity (6 tools)** — Grid demand, generation, prices, 100k+ generators
- **🔥 Natural Gas (7 tools)** — Henry Hub, storage, LNG, production, pipelines
- **⛏️ Coal (6 tools)** — Mine production, prices, quality, reserves, nuclear outages
- **🔮 Outlook (4 tools)** — STEO, AEO, IEO forecasts + international data
- **🗺️ States (3 tools)** — SEDS (1960→2024), total energy MER, emissions

### Who is this for?
Power users, energy consultants, and AI agents that need cross-commodity U.S. energy intelligence in a single integration.


## Available Tools
- **get_coal_production**: Get coal production by state, mine type, and rank
- **get_mine_production**: Source: EIA-7A and MSHA-7000-2.

Get individual mine-level coal production data
- **get_coal_prices**: Also includes price-by-rank breakdown for bituminous, subbituminous, lignite, and anthracite.

Get coal market prices by rank, region, and mine type
- **get_coal_quality**: Get coal consumption and quality data: heat content, sulfur, ash
- **get_coal_trade**: Get coal imports and exports by country, quantity, and price
- **get_coal_reserves**: Get coal reserves, productive capacity, and stocks
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
- **get_natgas_prices**: Henry Hub spot price is the benchmark for North American gas trading.

Get natural gas prices: Henry Hub, citygate, wellhead, industrial, residential
- **get_natgas_summary**: S. natural gas balance: total production, consumption, imports, exports, and storage changes.

Get natural gas supply and demand overview
- **get_natgas_reserves**: Get natural gas proved reserves and exploration data
- **get_natgas_production**: Get natural gas production: gross withdrawals, marketed production
- **get_natgas_trade**: Get natural gas imports, exports, and pipeline flows
- **get_natgas_storage**: The weekly storage report is a major market-moving event for gas trading.

Get underground natural gas storage levels
- **get_natgas_consumption**: By state and nationally.

Get natural gas consumption by sector
- **get_short_term_outlook**: Published monthly by EIA. Data range: 1974 to 2027.

Get STEO: 18-month U.S. energy price and supply projections
- **get_annual_outlook**: S. energy production, consumption, prices, and emissions using the National Energy Modeling System (NEMS). Includes reference case and side cases.

Get AEO: 30-year U.S. energy projections
- **get_international_outlook**: Covers global production, consumption, and emissions by region and fuel.

Get IEO: international energy projections
- **get_international_data**: Get country-level energy production, consumption, and emissions
- **get_petroleum_prices**: Filter by product, area, and frequency.

Get petroleum product prices: WTI, Brent, gasoline, diesel, heating oil
- **get_petroleum_summary**: S. petroleum supply/demand balance including production, imports, exports, stocks, and consumption. The weekly petroleum status report data.

Get petroleum supply and demand balance
- **get_crude_production**: Get U.S. crude oil production and reserves data
- **get_refinery_operations**: Get refinery capacity, utilization, and processing data
- **get_petroleum_trade**: Get petroleum imports, exports, and movements
- **get_petroleum_stocks**: Get petroleum stocks: commercial + Strategic Petroleum Reserve
- **get_petroleum_consumption**: Get petroleum consumption and sales by product and sector
- **get_crude_imports**: Source: EIA-814.

Get crude oil imports by country, company, type, and grade
- **get_state_energy_data**: Data from 1960 to present. The definitive source for state-level energy analysis.

Get comprehensive state-level energy data (SEDS): production, consumption, prices, expenditures
- **get_total_energy**: Includes total production, consumption, stocks, trade, prices, and CO2 emissions for petroleum, natural gas, coal, electricity, nuclear, and renewables.

Get comprehensive U.S. total energy overview (Monthly Energy Review)
- **get_nuclear_outages**: S. nuclear reactors.

Get nuclear power plant outage data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EIA Full Access — U.S. Energy Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Complete U.S. energy dashboard: oil, gas, electricity, and coal prices"

**🤖 AI Agent:**
> 🇺🇸 **U.S. Energy Dashboard**

| Commodity | Price | Trend |
|-----------|-------|-------|
| WTI Crude | $78.26/bbl | → |
| Brent | $82.10/bbl | → |
| Gasoline | $3.28/gal | ↓ |
| Henry Hub Gas | $2.84/MMBtu | ↑ |
| Electricity | 16.6¢/kWh | → |
| Coal (bit.) | $68.40/ton | ↓ |

6 commodity queries executed across petroleum, gas, electricity, and coal tools.

---

**👤 You:**
> "Which state produces the most renewable energy and what are storage levels?"

**🤖 AI Agent:**
> 🌱 **Cross-Domain Query**

Top renewable states (generation):
1. Texas — 149 TWh (wind leader)
2. California — 103 TWh (solar leader)
3. Washington — 82 TWh (hydro leader)

📦 Gas Storage: 2,584 Bcf (+11% vs 5yr avg)
🛢️ Crude Stocks: 432M bbl (commercial)

3 tools used: electricity + natgas storage + petroleum stocks

---

**👤 You:**
> "What does the STEO forecast for natural gas prices and how does it compare to coal?"

**🤖 AI Agent:**
> 🔮 **STEO Gas Forecast + Coal Comparison**

Henry Hub forecast:
- 2025 avg: $3.10/MMBtu (+9% YoY)
- Winter peak: $3.80/MMBtu

Coal delivered to power plants: $2.15/MMBtu
Gas premium over coal: 44%

Coal remains cheaper on BTU basis but gas dominates generation due to lower emissions and flexibility.


## Installation & Usage

To install and use the **EIA Full Access — U.S. Energy Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eia-full-access-us-energy-intelligence](https://vinkius.com/mcp/eia-full-access-us-energy-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
