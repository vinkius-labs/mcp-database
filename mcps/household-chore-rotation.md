# Household Chore Rotation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-chore-rotation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Distributes household chores among residents using effort points and availability.

## Description
This MCP server provides an intelligent scheduling engine to manage household tasks. It uses `get_weekly_schedule` to distribute chores based on effort points, resident availability, and historical rotation to ensure fairness. You can also use `get_resident_workload_balance` to check effort distribution, `get_unassigned_reasoning` to understand why tasks were missed, and `validate_rotation_fairness` to ensure tasks are rotating correctly among residents.


## Available Tools (4)
- **get_unassigned_reasoning**: Explains why specific chores were not assigned to any resident
- **get_weekly_schedule**: Generates a complete chore assignment plan for the upcoming week
- **validate_rotation_fairness**: Checks if the current assignment plan is effectively rotating tasks based on historical data
- **get_resident_workload_balance**: Analyzes how evenly the chore effort is distributed among the household members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Chore Rotation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a weekly chore schedule for Alice and Bob."

**🤖 AI Agent:**
> Alice is assigned: Vacuuming (5 pts), Dishwashing (3 pts). Bob is assigned: Trash (2 pts), Laundry (5 pts). Total effort: Alice 8, Bob 7.

---

**👤 You:**
> "Is the workload balanced between the residents?"

**🤖 AI Agent:**
> The workload is well-balanced with a deviation score of 0.5, as Alice has 8 points and Bob has 7 points.

---

**👤 You:**
> "Why wasn't the 'Mop Floor' chore assigned?"

**🤖 AI Agent:**
> The 'Mop Floor' chore was not assigned because all residents with availability during the required window have an exclusion for this task.


## ❓ FAQ

**Q: How does the system ensure chores are fair?**
The system uses effort points to balance the workload and `validate_rotation_fairness` to ensure tasks are distributed fairly over time.

**Q: What happens if a chore cannot be assigned?**
Unassigned chores are reported, and you can use `get_unassigned_reasoning` to find out why they couldn't be allocated.

**Q: Can I account for resident availability?**
Yes, the `get_weekly_schedule` tool incorporates resident availability and exclusions into the assignment logic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-chore-rotation](https://vinkius.com/en/ai-agent-connect/household-chore-rotation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Chore Rotation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-chore-rotation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Chore Rotation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-chore-rotation": {
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
