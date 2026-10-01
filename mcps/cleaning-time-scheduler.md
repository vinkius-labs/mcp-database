# Cleaning Time Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cleaning-time-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Schedules cleaning tasks across available time blocks based on room, frequency, and priority.

## Description
This MCP server provides a specialized engine for managing cleaning workflows. It maps cleaning tasks to available time windows while respecting task priority, due dates, and room requirements. Use `get_scheduled_plan` to generate a complete schedule, `get_room_utilization` to analyze room-specific workloads, `get_overdue_report` to identify missed deadlines, and `get_capacity_analysis` to evaluate time block efficiency.


## Available Tools (4)
- **get_capacity_analysis**: Evaluates the efficiency of the provided time blocks against the workload
- **get_overdue_report**: Provides a focused view of tasks that missed their deadlines
- **get_room_utilization**: Analyzes how much cleaning time is being allocated to specific rooms
- **get_scheduled_plan**: Generates a full cleaning schedule and identifies operational gaps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cleaning Time Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a cleaning schedule for these tasks: [{'room': 'Lobby', 'duration': 60, 'frequency': 'Daily', 'due_date': '2023-10-27', 'priority': 'Critical'}] with time blocks: [{'start': '2023-10-27T08:00:00', 'end': '2023-10-27T10:00:00'}]."

**🤖 AI Agent:**
> The Lobby cleaning task has been scheduled from 08:00 to 09:00. There are 60 unscheduled minutes remaining in the time block.

---

**👤 You:**
> "What is the utilization of the Kitchen room based on the scheduled tasks?"

**🤖 AI Agent:**
> The Kitchen has been allocated a total of 120 minutes of cleaning time.

---

**👤 You:**
> "Check if we have enough capacity for our current cleaning workload."

**🤖 AI Agent:**
> The current capacity ratio is 0.75, meaning 75% of available time is utilized. No bottleneck rooms were identified.


## ❓ FAQ

**Q: How does the scheduling priority work?**
Tasks are prioritized based on their assigned level (Critical, High, Medium, Low). Higher priority tasks are assigned to available time blocks first to ensure essential maintenance is completed.

**Q: Can I identify which rooms are causing scheduling bottlenecks?**
Yes, you can use `get_capacity_analysis` to identify bottleneck rooms where the required cleaning duration exceeds the available time blocks.

**Q: How do I see tasks that were not completed on time?**
You can use `get_overdue_report` to get a list of tasks that missed their due dates and were not included in the scheduled plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cleaning-time-scheduler](https://vinkius.com/en/ai-agent-connect/cleaning-time-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cleaning Time Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cleaning-time-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cleaning Time Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cleaning-time-scheduler": {
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
