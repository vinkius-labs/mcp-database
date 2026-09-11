# Mine Power Consumption Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mine-power-consumption-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate electricity demand and costs for mining operations.

## Description
This MCP server provides specialized tools for modeling power consumption in mining environments. It allows users to calculate peak demand, annual energy usage, and total electricity costs by analyzing equipment inventories and load factors. Use `query_equipment_consumption` to analyze specific machine groups, `calculate_total_utility_cost` to determine bills including demand charges, `simulate_annual_profile` for yearly budgeting, or `compare_load_scenarios` to evaluate how different utilization levels impact costs.


## Available Tools (4)
- **compare_load_scenarios**: Evaluates how changing the operational load affects the total cost
- **query_equipment_consumption**: Calculates the specific energy consumption and peak demand for a selected subset of equipment
- **simulate_annual_profile**: Provides a high-level yearly projection of power needs and costs based on a full inventory
- **calculate_total_utility_cost**: Determines the total monetary cost of electricity for a period, accounting for both usage and peak penalties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Power Consumption Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated energy consumption for equipment IDs 'crusher-01' and 'conveyor-05' with a load factor of 0.8 over 100 hours?"

**🤖 AI Agent:**
> The total energy consumption for those units is 4500 kWh with a peak demand of 50 kW.

---

**👤 You:**
> "Calculate the total utility cost if I have 50000 kWh consumed, a peak demand of 200 kW, an energy rate of 0.12, a demand charge of 15, and a power factor of 0.96."

**🤖 AI Agent:**
> The total utility cost is $8,950.00, consisting of $6,000.00 in usage costs and $2,950.00 in demand charges.

---

**👤 You:**
> "How will my costs change if I increase the load factor from 0.7 to 0.9 for my current equipment set?"

**🤖 AI Agent:**
> Increasing the load factor from 0.7 to 0.9 will increase your estimated annual cost from $120,000 to $155,000 due to higher energy usage and increased peak demand charges.


## ❓ FAQ

**Q: How does this model account for demand charges?**
The model uses the `calculate_total_utility_cost` tool to factor in both energy consumption and peak demand charges, ensuring a realistic estimation of utility bills.

**Q: Can I compare different operational scenarios?**
Yes, you can use `compare_load_scenarios` to evaluate how varying load factors affect your total estimated costs and peak demand.

**Q: What inputs are required for annual projections?**
To run `simulate_annual_profile`, you need the full equipment inventory, an average load factor, annual energy and demand rates, and the expected power factor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mine-power-consumption-model](https://vinkius.com/en/ai-agent-connect/mine-power-consumption-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Power Consumption Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-power-consumption-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Power Consumption Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-power-consumption-model": {
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
