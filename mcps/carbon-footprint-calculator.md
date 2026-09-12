# Carbon Footprint Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/carbon-footprint-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Quantify GHG emissions for oil and gas operations using GHG Protocol and IPCC standards.

## Description
This MCP server provides a specialized engine for quantifying greenhouse gas (GHG) emissions across the lifecycle of oil and gas operations. It allows AI agents to calculate Scope 1, 2, and 3 emissions, determine emission intensity, and identify reduction opportunities. Using tools like `calculate_scope_1_emissions`, `calculate_scope_2_emissions`, and `calculate_scope_3_emissions`, agents can accurately model direct combustion, purchased energy, and value chain impacts. The `calculate_emissions_summary` tool aggregates these results to provide a complete operational efficiency overview, accounting for flaring, venting, and fugitive emissions.


## Available Tools (4)
- **calculate_emissions_summary**: Aggregates all scopes and calculates operational efficiency metrics
- **calculate_scope_1_emissions**: Quantifies all direct emissions produced by the operator's facilities
- **calculate_scope_2_emissions**: Quantifies indirect emissions from purchased energy
- **calculate_scope_3_emissions**: Quantifies downstream and upstream value chain emissions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carbon Footprint Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Scope 1 emissions for a facility with 500 units of fuel, 50 units of flaring, 10 units of venting, and 5 units of fugitive leaks."

**🤖 AI Agent:**
> The total Scope 1 emissions are 1250.5 tonnes of CO2e, consisting of fuel combustion, flaring, venting, and fugitive components.

---

**👤 You:**
> "What is the emission intensity if total GHG is 5000 tonnes and total production is 10000 barrels?"

**🤖 AI Agent:**
> The emission intensity is 0.5 tonnes of CO2e per barrel.

---

**👤 You:**
> "Calculate Scope 2 emissions for 1000 units of electricity and 200 units of thermal energy."

**🤖 AI Agent:**
> The total Scope 2 emissions are 450.0 tonnes of CO2e.


## ❓ FAQ

**Q: What emission scopes are supported?**
The server supports Scope 1 (direct), Scope 2 (indirect from purchased energy), and Scope 3 (value chain) emissions.

**Q: How are reduction opportunities identified?**
Reduction opportunities are identified by analyzing the ratio of venting and flaring to total fuel consumption via the `calculate_emissions_summary` tool.

**Q: Which standards does this follow?**
Calculations follow the Greenhouse Gas (GHG) Protocol and IPCC methodologies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/carbon-footprint-calculator](https://vinkius.com/en/ai-agent-connect/carbon-footprint-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carbon Footprint Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carbon-footprint-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carbon Footprint Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carbon-footprint-calculator": {
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
