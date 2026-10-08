# Workweek Capacity Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/workweek-capacity-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Allocates tasks across work hours using estimates, deadlines, and priority.

## Description
This MCP server provides a scheduling engine to manage weekly workload. It calculates available capacity by subtracting fixed commitments like meetings or focus blocks, then assigns tasks based on priority and deadlines. Use `allocate_tasks` to generate a schedule and `analyze_deadline_risks` to identify tasks that might miss their targets.


## Available Tools (4)
- **allocate_tasks**: Assigns tasks to the available time slots in the workweek
- **analyze_deadline_risks**: Identifies which tasks are scheduled to finish after their required deadline
- **calculate_available_capacity**: Determines the total remaining working hours in a week after subtracting fixed commitments
- **get_weekly_summary**: Provides a high-level overview of the week's utilization and workload balance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workweek Capacity Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my available capacity for a workday from 09:00 to 17:00 with a meeting from 10:00 to 11:00."

**🤖 AI Agent:**
> Your total capacity is 8 hours, and your remaining capacity after the meeting is 7 hours.

---

**👤 You:**
> "Allocate these tasks: Task A (2h, priority 1, deadline tomorrow) and Task B (3h, priority 2, deadline tomorrow) into 6 available hours."

**🤖 AI Agent:**
> Task A is scheduled from 09:00 to 11:00 and Task B is scheduled from 11:00 to 14:00. There are 1 hour of overflow.

---

**👤 You:**
> "Check if my scheduled tasks are at risk of missing their deadlines."

**🤖 AI Agent:**
> Task ID 101 is at risk as it is scheduled to finish at 17:00, but its deadline is 16:00.


## ❓ FAQ

**Q: How does the tool handle task priority?**
Tasks are processed in descending order of priority. If two tasks have the same priority, the one with the earlier deadline is scheduled first.

**Q: What is considered a 'risky task'?**
A task is flagged as risky if its scheduled end time is strictly later than its required deadline.

**Q: Can I include meetings in my capacity calculation?**
Yes, you can provide a list of commitments, including meetings and focus blocks, to determine your remaining available capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/workweek-capacity-planner](https://vinkius.com/en/ai-agent-connect/workweek-capacity-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Workweek Capacity Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workweek-capacity-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workweek Capacity Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workweek-capacity-planner": {
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
