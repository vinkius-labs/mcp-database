# Household Sleep Window Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-sleep-window-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate household activities by finding quiet windows based on sleep schedules and noise sensitivity.

## Description
This MCP server acts as a coordination engine for managing household noise. It identifies optimal time windows for noise-sensitive tasks by analyzing the intersection of sleep schedules, room occupancy, and shared device usage. Use `get_quiet_windows` to find the best times for quiet activities, `check_task_feasibility` to verify if a specific task will disturb sleepers, `schedule_shared_device` to reserve loud appliances like washing machines, and `get_household_status` to see who is currently sleeping and which devices are active.


## Available Tools (4)
- **check_task_feasibility**: Determines if a specific task can be performed at a given time without disturbing the household
- **get_household_status**: Provides a real-time overview of who is sleeping, where, and which devices are currently active
- **get_quiet_windows**: Identifies periods of time throughout the day when the household is quietest and most suitable for noise-sensitive tasks
- **schedule_shared_device**: Reserves a slot for using a loud shared appliance while avoiding conflicts with sleep windows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Sleep Window Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is a good time to do some quiet reading today?"

**🤖 AI Agent:**
> The best quiet window for reading today is between 14:00 and 16:30, with a quietness score of 0.95.

---

**👤 You:**
> "Is it okay to run the dishwasher at 10 PM tonight?"

**🤖 AI Agent:**
> No, running the dishwasher at 10 PM is not feasible because it overlaps with the sleep window for the residents in the Living Zone.

---

**👤 You:**
> "Can I schedule the washing machine for tomorrow at 9 AM?"

**🤖 AI Agent:**
> Yes, the washing machine has been successfully scheduled for tomorrow at 09:00.


## ❓ FAQ

**Q: How do I find the best time to do laundry?**
You can use `schedule_shared_device` to reserve a slot for your washing machine, ensuring it doesn't overlap with any active sleep windows.

**Q: Can I check if my vacuuming will wake anyone up?**
Yes, use `check_task_feasibility` with the task set as noise-sensitive to see if the activity conflicts with current sleep schedules in your room or adjacent zones.

**Q: How can I see who is currently sleeping?**
Use the `get_household_status` tool to get a real-time overview of active sleepers and currently running devices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-sleep-window-planner](https://vinkius.com/en/ai-agent-connect/household-sleep-window-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Sleep Window Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-sleep-window-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Sleep Window Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-sleep-window-planner": {
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
