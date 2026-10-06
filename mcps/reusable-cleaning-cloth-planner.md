# Reusable Cleaning Cloth Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reusable-cleaning-cloth-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate cloth inventory and laundry schedules for cleaning operations.

## Description
This MCP server provides logistical planning tools for managing reusable cleaning cloth inventory. It helps users determine the total number of cloths needed to sustain operations, plan wash cycles based on laundry capacity and drying time, and check if current stock is sufficient for upcoming tasks. Use `get_minimum_inventory_needed` to find your required stock levels and `get_wash_schedule_plan` to optimize your laundry frequency.


## Available Tools (4)
- **get_minimum_inventory_needed**: Determines the total number of cloths a user must own to sustain their operations
- **get_operational_status**: Checks if current inventory and wash capacity are sufficient to cover a specific cleaning window
- **get_total_weekly_demand**: Calculates the total number of cloths needed to complete all tasks throughout a full week
- **get_wash_schedule_plan**: Recommends how often laundry cycles should occur to maintain cloth availability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reusable Cleaning Cloth Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many cloths do I need if I use 20 cloths a week, have a wash capacity of 10, a 1-day drying time, and want a 5 cloth reserve?"

**🤖 AI Agent:**
> You need a total inventory of 25 cloths to maintain your operations and reserve.

---

**👤 You:**
> "What is my wash schedule if I need 50 cloths per week and my machine holds 15 cloths?"

**🤖 AI Agent:**
> You should run 4 wash cycles per week, with 12.5 cloths per cycle.

---

**👤 You:**
> "I have 30 cloths total. 10 are being used and 5 are in the wash. Do I have enough for a task that needs 12 cloths?"

**🤖 AI Agent:**
> Yes, you have 15 cloths available, which is sufficient for the 12 cloths required.


## ❓ FAQ

**Q: How do I know how many cloths I need to buy?**
You can use the `get_minimum_inventory_needed` tool. Provide your weekly demand, the spare reserve you want to keep, your wash capacity, and how many days it takes for cloths to dry.

**Q: Can I plan my laundry schedule?**
Yes, the `get_wash_schedule_plan` tool calculates the optimal number of wash cycles per week and the number of cloths per cycle based on your capacity.

**Q: How can I check if I have enough cloths for my next cleaning task?**
Use the `get_operational_status` tool by providing your current inventory, cloths in use, cloths being washed, and the demand for the next task.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reusable-cleaning-cloth-planner](https://vinkius.com/en/ai-agent-connect/reusable-cleaning-cloth-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reusable Cleaning Cloth Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reusable-cleaning-cloth-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reusable Cleaning Cloth Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reusable-cleaning-cloth-planner": {
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
