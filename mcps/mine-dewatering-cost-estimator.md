# Mine Dewatering Cost Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mine-dewatering-cost-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate capital, power, and operating costs for mine dewatering systems.

## Description
This MCP server provides specialized tools for mining engineers to estimate the financial requirements of dewatering operations. It calculates initial pump capital costs, electrical power consumption, annual operating expenditures, and long-term well lifecycle costs. By using `calculate_pump_capital_cost`, `calculate_power_consumption`, `calculate_annual_operating_cost`, and `estimate_well_lifecycle_costs`, users can model the impact of groundwater inflow and pump head on total project expenditure.


## Available Tools (4)
- **calculate_power_consumption**: Estimates the electrical load required to operate the pumps
- **calculate_annual_operating_cost**: Calculates the yearly recurring expenditure for electricity and maintenance
- **calculate_pump_capital_cost**: Determines the initial investment required for the pumping equipment
- **estimate_well_lifecycle_costs**: Projects the costs for maintaining and replacing wells over the mine life


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Dewatering Cost Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the capital cost for a pump with an inflow rate of 500 m3/h and a total head of 150 meters?"

**🤖 AI Agent:**
> The total capital cost for the pump is $125,000, which includes $100,000 for the pump itself and $25,000 for installation.

---

**👤 You:**
> "Calculate the hourly power consumption for 500 m3/h inflow, 150m head, and 0.85 efficiency."

**🤖 AI Agent:**
> The hourly power consumption is 215.4 kW.

---

**👤 You:**
> "Estimate the annual operating cost for a system using 215.4 kW at $0.15/kWh, with a maintenance factor of 0.2 and 8760 operating hours per year."

**🤖 AI Agent:**
> The total annual operating cost is $31,536, consisting of $28,671 in energy costs and $2,865 in maintenance costs.


## ❓ FAQ

**Q: What inputs are required for pump capital cost estimation?**
To use `calculate_pump_capital_cost`, you need to provide the inflow rate (volume of water per hour) and the total head (vertical lift plus friction losses in meters).

**Q: How does the tool handle well maintenance?**
The `estimate_well_lifecycle_costs` tool calculates both the annual routine maintenance and the annualized cost of replacing wells based on their expected lifespan.

**Q: Can I estimate electricity costs for the pumps?**
Yes, you can use `calculate_power_consumption` to find the electrical load and then use `calculate_annual_operating_cost` to determine the yearly energy expenditure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mine-dewatering-cost-estimator](https://vinkius.com/ai-agent-connect/mine-dewatering-cost-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Dewatering Cost Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-dewatering-cost-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Dewatering Cost Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-dewatering-cost-estimator": {
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
