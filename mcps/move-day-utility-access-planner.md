# Move-Day Utility & Access Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/move-day-utility-access-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synchronize utility windows, logistics, and crew arrivals into a single move-day schedule.

## Description
This MCP server acts as a coordination engine for moving days. It allows you to manage activation windows for utilities, book elevator access, and schedule crew arrivals. Use `register_activity_window` to add events, `get_move_day_schedule` to view a unified timeline, and `detect_scheduling_conflicts` to identify overlapping windows or sequence errors that could disrupt your move.


## Available Tools (4)
- **get_move_day_schedule**: Provides a unified, chronological timeline of all scheduled activities for the move day
- **detect_scheduling_conflicts**: Identifies logistical overlaps or impossible sequences where activities conflict with one another
- **query_activity_by_type**: Filters and retrieves specific subsets of the move-day plan
- **register_activity_window**: Records a new time-bound event (utility, delivery, or logistics) into the planning system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Move-Day Utility & Access Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Register a utility activation window for 2024-10-15 from 08:00 to 12:00."

**🤖 AI Agent:**
> The utility activation window has been successfully registered with activity ID: util_98765.

---

**👤 You:**
> "Show me the schedule for 2024-10-15."

**🤖 AI Agent:**
> Your schedule for 2024-10-15 includes: 08:00-12:00 Utility Activation, 13:00-14:00 Elevator Booking, and 14:00-17:00 Crew Arrival.

---

**👤 You:**
> "Are there any conflicts on 2024-10-15?"

**🤖 AI Agent:**
> No scheduling conflicts or overlapping windows were detected for 2024-10-15.


## ❓ FAQ

**Q: How do I add a new appointment?**
You can use the `register_activity_window` tool to record any event, such as a utility window or an elevator booking.

**Q: Can I check for scheduling overlaps?**
Yes, the `detect_scheduling_conflicts` tool identifies overlapping windows and sequence errors to ensure your move stays on track.

**Q: How do I see my full move-day timeline?**
Use the `get_move_day_schedule` tool with the specific move date to receive a complete chronological list of all activities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/move-day-utility-access-planner](https://vinkius.com/en/ai-agent-connect/move-day-utility-access-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Move-Day Utility & Access Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `move-day-utility-access-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Move-Day Utility & Access Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "move-day-utility-access-planner": {
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
