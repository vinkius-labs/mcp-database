# World Bank Climate & Energy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/world-bank-climate-energy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Track CO2 emissions, renewable energy usage, deforestation, and electrification rates using official World Bank data.

## Description
Turn your AI into a climate change researcher by connecting it directly to the World Bank's environmental metrics.

### What you can do
- **Emissions** — Track metric tons of CO2 emissions per capita.
- **Renewables** — Measure the transition to renewable energy sources globally.
- **Conservation** — Map the shrinking or growing forest area relative to land mass.

### How it works
1. Hit subscribe.
2. Skip the authentication phase entirely (it's open data).
3. Enable your AI to perform deep climate reporting instantly.

### Who is this for?
Environmental scientists, ESG compliance officers, energy analysts, and journalists.


## Available Tools
- **get_co2_emissions**: Get CO2 emissions (metric tons per capita)
- **get_renewable_energy**: Get renewable energy consumption (% of total)
- **get_electricity_access**: Get access to electricity (% of population)
- **get_forest_area**: Get forest area (% of land area)
- **get_climate_indicator**: Get any World Bank climate/energy indicator by code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **World Bank Climate & Energy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the renewable energy consumption in Norway compared to the global average?"

**🤖 AI Agent:**
> 🌍 **Renewable Energy: Norway vs World**

Norway derives over 70% of its total energy from renewable sources — primarily hydropower — vastly exceeding the global average of approximately 18%.

---

**👤 You:**
> "Compare CO2 emissions per capita: USA versus China over the last 20 years."

**🤖 AI Agent:**
> 🌍 **CO2 Per Capita: USA vs China (2004–2024)**

The USA's per capita emissions have declined from ~20 to ~14 metric tons. China's have risen from ~4 to ~8 metric tons. While the USA still emits more per person, China's trajectory shows rapid convergence.

---

**👤 You:**
> "How has deforestation progressed in Brazil over the last 30 years?"

**🤖 AI Agent:**
> 🌍 **Forest Area: Brazil (1994–2024)**

Brazil's forest area has declined from approximately 65% to 59% of total land area over three decades, representing the loss of millions of hectares — though recent policies have begun slowing the rate of deforestation.


## ❓ FAQ

**Q: How do I get started?**
Our World Bank Open Data servers require absolutely zero authentication. You do not need to register, get an API key, or setup webhooks. Just instantly connect and your AI agent can begin querying decades of global data.

**Q: Can it track if a nation's CO2 emissions are rising?**
Yes! Your agent pulls historical CO2 per capita statistics so it can mathematically verify if a nation is adhering to its climate pledges.

**Q: Can it map national deforestation trends?**
Absolutely. The AI pulls 'forest area (% of land area)' indicators to provide accurate insights into conservation or deforestation across entire continents.

**Q: What is the scale of the data I can access?**
You have direct access to 64 years of historical data covering 196+ sovereign states and global regional aggregates, powered directly by the World Bank's robust open data initiatives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/world-bank-climate-energy](https://vinkius.com/mcp/world-bank-climate-energy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **World Bank Climate & Energy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `world-bank-climate-energy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **World Bank Climate & Energy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "world-bank-climate-energy": {
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
