# Family Errand Route Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-errand-route-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes family outings by synchronizing errands, schedules, and carrying limits.

## Description
This MCP server provides a specialized routing engine for families. It synchronizes errand locations, store operating hours, children's fixed schedules, and physical carrying capacities into a single, executable plan. Use `get_optimized_plan` to generate a full sequential itinerary that respects appointment windows and weight limits, or `validate_errand_feasibility` to check if a new task fits your current timeline.


## Available Tools (4)
- **calculate_travel_impact**: Determines the time cost and weight impact of moving between two points
- **get_optimized_plan**: Generates the full sequential itinerary for a family outing based on all constraints
- **identify_fallbacks**: Identifies which secondary tasks can be swapped in if a primary location is closed
- **validate_errand_feasibility**: Checks if a single specific errand can be integrated into an existing schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Errand Route Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an optimized plan for 3 errands: Grocery (weight 10), Pharmacy (weight 2), and Post Office (weight 1), with a carrying capacity of 15 and driving as the mode."

**🤖 AI Agent:**
> Your optimized plan is: 1. Grocery (09:00-09:30, Owner: Mom, Items: Milk, Bread), 2. Pharmacy (09:45-10:00, Owner: Mom, Items: Vitamins), 3. Post Office (10:15-10:30, Owner: Dad, Items: Package).

---

**👤 You:**
> "Is it possible to add a doctor's appointment at 14:00 if I have a school pickup at 14:30?"

**🤖 AI Agent:**
> No, the doctor's appointment is not possible because its duration overlaps with the fixed school pickup schedule.

---

**👤 You:**
> "Calculate the travel impact between the Grocery store and the Pharmacy using cycling."

**🤖 AI Agent:**
> The travel time is 12 minutes and the weight impact is 0.


## ❓ FAQ

**Q: How does the tool handle weight limits?**
The `get_optimized_plan` tool ensures that the cumulative weight of items carried does not exceed your specified carrying capacity between any two locations.

**Q: Can I check if a specific errand is possible?**
Yes, you can use `validate_errand_feasibility` to check if a task fits within your existing schedule and the location's opening hours.

**Q: What happens if a store is closed?**
You can use `identify_fallbacks` to find suitable secondary tasks that fit within the time window vacated by the primary errand.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-errand-route-planner](https://vinkius.com/en/ai-agent-connect/family-errand-route-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Errand Route Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-errand-route-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Errand Route Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-errand-route-planner": {
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
