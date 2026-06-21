# Electricity Maps Carbon Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/electricity-maps-carbon-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal energy and carbon intelligence — get real-time electricity mix and carbon data via AI.

## Description
Equip your AI agent with real-time global energy intelligence through the **Electricity Maps** MCP server. This integration provides instant access to the carbon intensity of electricity production and the detailed power breakdown (solar, wind, nuclear, coal, etc.) for over 100 countries and regions. Your agent can retrieve the exact gCO2eq/kWh for specific zones and monitor the renewable percentage of the grid. Whether you are optimizing server workloads for sustainability, auditing corporate emissions, or researching global energy transitions, your agent acts as a dedicated energy analyst through natural conversation.

### What you can do

- **Carbon Intensity Monitoring** — Get real-time carbon intensity data for specific countries or regions.
- **Power Mix Breakdown** — Fetch the detailed mix of energy sources currently powering a specific grid.
- **Sustainability Auditing** — Compare the environmental impact of electricity across different geographical zones.
- **Renewable Tracking** — Identify the current percentage of renewable energy in the production mix.

### How it works

1. Subscribe to this server
2. Enter your Electricity Maps API Key (get it at electricitymaps.com)
3. Start monitoring global energy data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sustainability Managers** — audit and report on the carbon footprint of global operations.
- **Cloud Engineers** — optimize data center workloads based on real-time grid intensity.
- **Policy Researchers** — track the performance of national energy transitions.
- **Eco-conscious Consumers** — check the best time to use energy-intensive appliances based on grid greenness.


## Available Tools (3)
- **get_carbon_intensity**: g., DE, FR, US-CA).

Get current carbon intensity for a zone
- **get_power_production_breakdown**: ) currently powering a specific zone.

Get power production breakdown for a zone
- **list_energy_zones**: List all available energy zones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Electricity Maps Carbon Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the energy mix in France right now?"

**🤖 AI Agent:**
> Retrieving data for France (FR)... The French grid is currently powered primarily by nuclear energy, followed by wind and hydro. The current carbon intensity is quite low at 45 gCO2eq/kWh. Would you like to see the exact MW breakdown?


## ❓ FAQ

**Q: Can I check the carbon intensity in Brazil?**
Yes! Use the `get_carbon_intensity` tool with the zone code 'BR'. It will return the latest gCO2eq/kWh for the Brazilian grid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/electricity-maps-carbon-intelligence](https://vinkius.com/mcp/electricity-maps-carbon-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Electricity Maps Carbon Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `electricity-maps-carbon-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Electricity Maps Carbon Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electricity-maps-carbon-intelligence": {
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
