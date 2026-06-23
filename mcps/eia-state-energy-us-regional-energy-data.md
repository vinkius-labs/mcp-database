# EIA State Energy — U.S. Regional Energy Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eia-state-energy-us-regional-energy-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

State-level energy data spanning 65 years: production, consumption, prices, and expenditures for ALL energy sources by state and sector (SEDS), the comprehensive Monthly Energy Review (MER), and nuclear reactor outage tracking.

## Description
The deepest state-level energy dataset in the world, covering 1960 to present.

### What you can do
- **SEDS** — Production, consumption, price, and expenditure data for ALL energy sources by state and sector. The definitive state-level energy database (1960→2024)
- **Total Energy (MER)** — The Monthly Energy Review: comprehensive overview integrating all sources
- **Nuclear Outages** — Current status of all U.S. nuclear reactors

### Who is this for?
State energy offices, regional planners, utility regulators, academic researchers, and ESG analysts needing state-level energy and emissions data.


## Available Tools (3)
- **get_state_energy_data**: Data from 1960 to present. The definitive source for state-level energy analysis.

Get comprehensive state-level energy data (SEDS): production, consumption, prices, expenditures
- **get_total_energy**: Includes total production, consumption, stocks, trade, prices, and CO2 emissions for petroleum, natural gas, coal, electricity, nuclear, and renewables.

Get comprehensive U.S. total energy overview (Monthly Energy Review)
- **get_nuclear_outages**: S. nuclear reactors.

Get nuclear power plant outage data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EIA State Energy — U.S. Regional Energy Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total energy expenditure for Texas?"

**🤖 AI Agent:**
> 💰 **Texas — Energy Expenditure**

Total: $142.3 billion
Per capita: $4,820
By sector: Industrial 48%, Transportation 28%, Residential 13%, Commercial 11%

Texas is the #1 energy-consuming state, accounting for 14% of total U.S. energy expenditure.

---

**👤 You:**
> "What is the U.S. total energy production breakdown?"

**🤖 AI Agent:**
> 🇺🇸 **U.S. Total Energy Production (MER)**

- Natural Gas: 36.2 Quad BTU (35%)
- Petroleum: 27.4 Quad (27%)
- Renewables: 13.1 Quad (13%)
- Coal: 11.2 Quad (11%)
- Nuclear: 8.1 Quad (8%)
- NGL: 6.4 Quad (6%)

Total: 102.4 Quad BTU
The U.S. is the world's largest energy producer.

---

**👤 You:**
> "Compare energy consumption between California and New York"

**🤖 AI Agent:**
> ⚖️ **California vs New York — SEDS Energy Data**

| Metric | CA | NY |
|--------|-----|-----|
| Total consumption | 7.4 Quad | 3.6 Quad |
| Per capita | 190 MMBTU | 183 MMBTU |
| Energy cost/capita | $3,920 | $4,210 |
| Renewable share | 33% | 28% |

CA consumes 2× more energy but similar per capita.


## ❓ FAQ

**Q: What is SEDS?**
**SEDS (State Energy Data System)** is EIA's comprehensive database of state-level energy statistics covering all 50 states + DC from 1960 to present. It includes production, consumption, prices, and expenditure data for ALL energy sources (petroleum, natural gas, coal, electricity, nuclear, renewables) broken down by sector.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eia-state-energy-us-regional-energy-data](https://vinkius.com/mcp/eia-state-energy-us-regional-energy-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EIA State Energy — U.S. Regional Energy Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eia-state-energy-us-regional-energy-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EIA State Energy — U.S. Regional Energy Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eia-state-energy-us-regional-energy-data": {
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
