# Tailings Water Balance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tailings-water-balance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate water inventory and hydrologic stability for tailings storage facilities.

## Description
This MCP server provides specialized tools to manage the hydrologic stability and water inventory of tailings storage facilities (TSF). It models the complex interplay between tailings slurry inflow, environmental factors like precipitation and evaporation, and water recovery through reclaim rates. Use `get_water_balance_summary` to assess overall facility health, `calculate_current_inventory` to track pond volume, `evaluate_discharge_need` to prevent overtopping, and `calculate_reclaim_efficiency` to optimize water reuse. It is designed to help engineers manage water surplus, deficits, and seepage risks.


## Available Tools (4)
- **calculate_reclaim_efficiency**: Determines how much water is successfully recovered for reuse in the plant
- **calculate_current_inventory**: Determines the current state of the water volume within the tailings facility
- **evaluate_discharge_need**: Determines if the facility needs to release water to prevent overtopping
- **get_water_balance_summary**: Provides a comprehensive overview of the facility's water health


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tailings Water Balance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current water status if I start with 100,000m3, add 5,000m3 from slurry and rain, but lose 2,000m3 to evaporation and 500m3 to seepage, with a 0.5 reclaim rate and 150,000m3 capacity?"

**🤖 AI Agent:**
> The facility is Stable. The total inflow is 10,000m3, total outflow is 7,500m3, and the net water balance is 2,500m3.

---

**👤 You:**
> "Do I need to discharge water if my current pond volume is 120,000m3 and my maximum capacity is 110,000m3?"

**🤖 AI Agent:**
> Yes, you must discharge 10,000m3 to reach the target level, leaving a safety margin of 0m3.

---

**👤 You:**
> "Calculate the reclaimed volume for 50,000m3 of available water with a reclaim rate of 0.75."

**🤖 AI Agent:**
> The reclaimed volume is 37,500m3, with 12,500m3 remaining unrecovered.


## ❓ FAQ

**Q: How does this tool help prevent tailings dam failure?**
By using `evaluate_discharge_need`, you can determine exactly how much water must be released to maintain a safe pond volume and prevent overtopping.

**Q: Can I model the impact of heavy rainfall?**
Yes, you can input precipitation values into `calculate_current_inventory` or `get_water_balance_summary` to see how rainfall affects your net water balance and pond volume.

**Q: How is water recovery accounted for?**
The `calculate_reclaim_efficiency` tool allows you to model how much water is successfully recovered from the facility for reuse in the processing plant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tailings-water-balance](https://vinkius.com/en/ai-agent-connect/tailings-water-balance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tailings Water Balance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tailings-water-balance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tailings Water Balance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tailings-water-balance": {
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
