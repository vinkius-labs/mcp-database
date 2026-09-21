# Irrigation Water Budget MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/irrigation-water-budget)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate garden irrigation volume and costs based on plant zones and environmental factors.

## Description
This MCP server provides precise tools for managing garden water usage. It allows you to calculate total water consumption across daily, weekly, and seasonal timelines, generate specific irrigation schedules for different plant zones, and simulate cost savings from optimized watering strategies. You can also use `validate_irrigation_feasibility` to ensure your water supply can meet the demands of your irrigation system.


## Available Tools (4)
- **calculate_consumption_metrics**: Calculates the total volume of water required across different timeframes and the total cost
- **generate_zone_schedules**: Provides a detailed breakdown of irrigation timing for each specific plant zone
- **simulate_savings_scenario**: Compares a baseline irrigation budget against a proposed optimization
- **validate_irrigation_feasibility**: Checks if the planned irrigation system is physically capable of delivering the required volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Irrigation Water Budget** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the water consumption and cost for a 50sqm zone with a flow rate of 2, duration of 15 mins, frequency of 3 times a week, and an evaporation factor of 1.2, given a weather adjustment of 1.1 and a tariff of 0.05 per liter."

**🤖 AI Agent:**
> The total seasonal consumption is 145.2 liters and the total cost is 7.26.

---

**👤 You:**
> "Generate an irrigation schedule for a zone named 'Rose Garden' with an area of 20, flow rate of 5, duration of 10, frequency of 2, and evaporation factor of 1.1, with a weather adjustment of 1.0."

**🤖 AI Agent:**
> The 'Rose Garden' zone requires 22.0 liters of water per day and will be irrigated 2 times per week.

---

**👤 You:**
> "Is my system feasible if my max flow rate is 10 and I have a zone requiring 12?"

**🤖 AI Agent:**
> No, the system is not feasible because the required flow rate exceeds the maximum capacity.


## ❓ FAQ

**Q: How do I calculate my seasonal water cost?**
Use the `calculate_consumption_metrics` tool with your zone data, weather adjustment, and water tariff to get the total seasonal cost.

**Q: Can I check if my pump is powerful enough?**
Yes, use `validate_irrigation_feasibility` by providing your zone requirements and the maximum system flow rate.

**Q: How can I reduce my water bill?**
You can use `simulate_savings_scenario` to compare your current setup against a more efficient configuration to see potential savings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/irrigation-water-budget](https://vinkius.com/en/ai-agent-connect/irrigation-water-budget)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Irrigation Water Budget** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `irrigation-water-budget` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Irrigation Water Budget** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "irrigation-water-budget": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
