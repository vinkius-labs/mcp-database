# Wine Harvest Logistics Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-harvest-logistics-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Optimizes vineyard harvest schedules, truck logistics, and winery capacity utilization.

## Description
This MCP server provides essential tools for managing the complex orchestration of vineyard harvests. It connects AI agents to winery operations by providing capabilities to `generate_harvest_schedule` based on maturity and facility constraints, `calculate_truck_logistics` to manage transport requirements, `evaluate_crush_pad_utilization` to monitor processing limits, and `optimize_maturity_window` to ensure fruit is picked at peak ripeness.


## Available Tools (4)
- **calculate_truck_logistics**: Determines the total number of trips required to move the harvest volume
- **evaluate_crush_pad_utilization**: Analyzes how close the winery is to its maximum processing limit
- **generate_harvest_schedule**: Creates a daily plan for which vineyard blocks should be harvested based on maturity and facility capacity
- **optimize_maturity_window**: Checks if the planned harvest schedule aligns with the predicted sugar accumulation and fruit ripeness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Harvest Logistics Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a harvest schedule for blocks b1 (50 tons, 2024-09-15) and b2 (30 tons, 2024-09-18) with a crush capacity of 40 tons per day and fermentation capacity of 40 tons per day, allowed on 2024-09-14 and 2024-09-15."

**🤖 AI Agent:**
> The harvest schedule is set for 2024-09-14 (40 tons) and 2024-09-15 (40 tons).

---

**👤 You:**
> "How many truck trips are needed for 150 tons of grapes if each truck carries 25 tons?"

**🤖 AI Agent:**
> 6 trips are required to transport 150 tons of grapes.

---

**👤 You:**
> "Check the crush pad utilization if we schedule 35 tons for day 1 and 45 tons for day 2, with a daily capacity of 50 tons."

**🤖 AI Agent:**
> Day 1 utilization is 70% and Day 2 utilization is 90%. Peak utilization is 90%.


## ❓ FAQ

**Q: How does the tool handle winery capacity limits?**
The `generate_harvest_schedule` tool ensures that the daily tonnage harvested does not exceed the lower of the crush capacity or the fermentation capacity.

**Q: Can I plan for specific weather windows?**
Yes, you can provide a list of permitted harvest dates to `generate_harvest_schedule` to ensure harvesting only occurs during favorable weather windows.

**Q: How are truck trips calculated?**
The `calculate_truck_logistics` tool takes the total tonnage and the maximum capacity of your trucks to determine the exact number of trips required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-harvest-logistics-planner](https://vinkius.com/ai-agent-connect/wine-harvest-logistics-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Harvest Logistics Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-harvest-logistics-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Harvest Logistics Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-harvest-logistics-planner": {
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
