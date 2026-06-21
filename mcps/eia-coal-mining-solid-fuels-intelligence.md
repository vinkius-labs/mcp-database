# EIA Coal & Mining — Solid Fuels Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eia-coal-mining-solid-fuels-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

U.S. coal industry data: mine-level production for every operating mine, market prices by rank (bituminous, subbituminous, lignite, anthracite), quality metrics (heat, sulfur, ash), international trade, reserves, and nuclear facility outages.

## Description
Deep intelligence on U.S. coal production and the solid fuels market.

### What you can do
- **Mine Production** — Individual mine-level data: name, company, county, output, coal rank
- **Aggregate Production** — National and state totals by mine type and rank
- **Market Prices** — Sales prices by rank, region, and mine type
- **Coal Quality** — Heat content (BTU/lb), sulfur (%), ash (%) by sector
- **International Trade** — Exports/imports by country, rank, and customs district
- **Reserves** — Recoverable reserves, productive capacity, and stocks
- **Nuclear Outages** — Plant-level outage events for U.S. nuclear reactors

### Who is this for?
Mining companies, coal traders, utility procurement teams, environmental regulators, and energy transition analysts.


## Available Tools
- **get_coal_production**: Get coal production by state, mine type, and rank
- **get_mine_production**: Source: EIA-7A and MSHA-7000-2.

Get individual mine-level coal production data
- **get_coal_prices**: Also includes price-by-rank breakdown for bituminous, subbituminous, lignite, and anthracite.

Get coal market prices by rank, region, and mine type
- **get_coal_quality**: Get coal consumption and quality data: heat content, sulfur, ash
- **get_coal_trade**: Get coal imports and exports by country, quantity, and price
- **get_coal_reserves**: Get coal reserves, productive capacity, and stocks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EIA Coal & Mining — Solid Fuels Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the largest coal mines in the U.S.?"

**🤖 AI Agent:**
> ⛏️ **Top 5 U.S. Coal Mines by Production**

1. North Antelope Rochelle (WY) — 96M short tons
2. Black Thunder (WY) — 68M
3. Antelope Mine (WY) — 38M
4. Belle Ayr (WY) — 28M
5. Cordero Rojo (WY) — 26M

Wyoming's Powder River Basin dominates U.S. production.

---

**👤 You:**
> "What is the current price of bituminous coal?"

**🤖 AI Agent:**
> 🪨 **Bituminous Coal — Market Price**

Average: $68.40/short ton
Appalachia: $82.50/ton
Illinois Basin: $52.30/ton
Western: $14.80/ton (subbituminous)

Prices vary dramatically by region and coal rank.

---

**👤 You:**
> "Are there any nuclear plant outages right now?"

**🤖 AI Agent:**
> ☢️ **Current Nuclear Outages**

3 reactors currently offline:
1. Byron Unit 2 (IL) — Refueling, ETA: 45 days
2. Calvert Cliffs Unit 1 (MD) — Planned maintenance
3. South Texas Unit 2 (TX) — Unplanned, investigating

90 of 93 commercial reactors operating.


## ❓ FAQ

**Q: Does this include nuclear data?**
Yes! In addition to comprehensive coal data, this server includes EIA nuclear outage tracking for all U.S. commercial nuclear reactors. For nuclear generation data, see the Electricity server.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eia-coal-mining-solid-fuels-intelligence](https://vinkius.com/mcp/eia-coal-mining-solid-fuels-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EIA Coal & Mining — Solid Fuels Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eia-coal-mining-solid-fuels-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EIA Coal & Mining — Solid Fuels Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eia-coal-mining-solid-fuels-intelligence": {
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
