# Family Weekly Logistics Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-weekly-logistics-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate household schedules, transport, and chores into a conflict-free weekly plan.

## Description
This MCP server acts as a coordination engine for household management. It resolves complex scheduling needs by applying hard-time conflict detection, travel buffers, and the one-owner rule. Use `generate_weekly_schedule` to create a master calendar with pickup assignments and prep tasks. You can also use `validate_transport_feasibility` to check driver availability, `optimize_meal_prep_window` to plan meal times, and `resolve_chore_conflicts` to ensure household responsibilities don't overlap with work or school.


## Available Tools (4)
- **generate_weekly_schedule**: Creates the master weekly calendar and identifies logistical gaps
- **optimize_meal_prep_window**: Calculates the necessary time windows for preparing meals
- **resolve_chore_conflicts**: Analyzes if assigned household responsibilities conflict with schedules
- **validate_transport_feasibility**: Checks if a specific subset of transport requests can be fulfilled


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Weekly Logistics Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a weekly plan for my family with 2 adults and 2 kids, including school pickups and dinner prep."

**🤖 AI Agent:**
> I have generated your weekly plan. It includes the school pickup assignments for Monday and Wednesday, the meal prep windows for Tuesday dinner, and identifies a conflict on Thursday afternoon due to a work overlap.

---

**👤 You:**
> "Check if we have enough drivers to pick up the kids from soccer on Friday."

**🤖 AI Agent:**
> All transport requests for Friday soccer pickups are feasible with the current drivers and vehicle availability.

---

**👤 You:**
> "When should I start cooking dinner to be ready by 6:00 PM?"

**🤖 AI Agent:**
> To have dinner ready by 6:00 PM, you should begin meal preparation at 5:15 PM based on the complexity of the requested meal.


## ❓ FAQ

**Q: How does the engine handle travel time?**
The engine applies mandatory travel buffers between all consecutive activities for a single person to ensure they have enough time to move between locations.

**Q: Can I check if my drivers are available for a specific trip?**
Yes, you can use the `validate_transport_feasibility` tool to verify if specific transport requests can be fulfilled given your current drivers and vehicle availability.

**Q: What happens if a chore overlaps with work?**
The `resolve_chore_conflicts` tool will identify these overlaps and list them as conflicting tasks, ensuring responsibilities are only assigned to available members.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-weekly-logistics-plan](https://vinkius.com/en/ai-agent-connect/family-weekly-logistics-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Weekly Logistics Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-weekly-logistics-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Weekly Logistics Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-weekly-logistics-plan": {
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
