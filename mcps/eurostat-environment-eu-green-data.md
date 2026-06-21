# Eurostat Environment — EU Green Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eurostat-environment-eu-green-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

EU environmental and energy data: greenhouse gas emissions by sector, complete energy balance sheets, electricity and gas prices, renewable energy share, waste statistics, and agricultural production for all 27 EU member states.

## Description
Track the EU Green Deal progress with official environmental and energy statistics.

### What you can do
- **Emissions** — GHG by country and sector (Paris Agreement tracking)
- **Energy Balance** — Production, imports, consumption by source
- **Energy Prices** — Electricity and gas for households and industry
- **Renewables** — Share in gross final consumption (2030 target: 42.5%)
- **Waste** — Generation, recycling, landfill by country
- **Agriculture** — Crop production, livestock (CAP data)


## Available Tools (6)
- **get_emissions**: Units: tonnes of CO2 equivalent. Breakdown by source sector (energy, agriculture, transport, industry, waste). Essential for EU Green Deal and Paris Agreement tracking.

Get EU greenhouse gas emissions by country and sector
- **get_energy_balance**: Production, imports, exports, gross consumption by energy source. The definitive view of a country energy system.

Get EU complete energy balance by country
- **get_energy_prices**: Datasets: nrg_pc_204 (electricity households), nrg_pc_205 (electricity industry), nrg_pc_202 (gas households), nrg_pc_203 (gas industry). Semi-annual data in EUR per kWh / GJ.

Get EU electricity and gas prices for households and industry
- **get_renewable_energy**: The EU target is 42.5% by 2030. Leaders: Sweden (~65%), Finland (~48%). Laggards: Luxembourg, Malta, Belgium.

Get EU renewable energy share by country
- **get_waste_statistics**: Treatment: landfill, incineration, recycling. Key for circular economy policy.

Get EU waste generation and treatment data
- **get_agriculture_data**: Covers cereals, fruits, vegetables, wine grapes, olive oil. Essential for Common Agricultural Policy (CAP) analysis.

Get EU agriculture production data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eurostat Environment — EU Green Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which EU countries have the highest share of renewable energy?"

**🤖 AI Agent:**
> 🌱 **EU Renewable Energy Share**

🇸🇪 Sweden: 65.5%
🇫🇮 Finland: 47.9%
🇱🇻 Latvia: 43.3%
🇩🇰 Denmark: 41.6%
🇪🇪 Estonia: 38.0%
...
EU27 average: 23.0%
2030 target: 42.5%

Hydro (Nordics) and wind (Denmark) drive the leaders.

---

**👤 You:**
> "Compare electricity prices for households across the EU"

**🤖 AI Agent:**
> ⚡ **Household Electricity Prices (EUR/kWh)**

Most expensive:
🇩🇪 Germany: 0.417
🇩🇰 Denmark: 0.391
🇧🇪 Belgium: 0.357

Cheapest:
🇧🇬 Bulgaria: 0.117
🇭🇺 Hungary: 0.103

EU average: 0.285

---

**👤 You:**
> "How have EU greenhouse gas emissions changed since 1990?"

**🤖 AI Agent:**
> 🌍 **EU27 GHG Emissions Trend**

1990: 5,653 Mt CO2eq (baseline)
2005: 5,152 Mt (-8.9%)
2019: 4,067 Mt (-28%)
2020: 3,723 Mt (-34%, COVID)
2022: 3,892 Mt (-31%)

EU targets: -55% by 2030, net-zero by 2050.
Energy sector: largest reduction. Agriculture: stagnant.


## ❓ FAQ

**Q: Does this include EU Green Deal data?**
Yes! GHG emissions, renewable energy share, energy efficiency, and waste recycling rates are the core metrics the European Commission uses to track Green Deal progress. This server provides all of them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eurostat-environment-eu-green-data](https://vinkius.com/mcp/eurostat-environment-eu-green-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eurostat Environment — EU Green Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eurostat-environment-eu-green-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eurostat Environment — EU Green Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eurostat-environment-eu-green-data": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
