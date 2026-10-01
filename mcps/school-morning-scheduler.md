# School Morning Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-morning-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates chronologically ordered morning routines by calculating backward from departure times.

## Description
This MCP server provides tools to build reliable morning schedules for children. By using backward scheduling, it ensures that all tasks, dependencies, and buffer minutes are accounted for relative to a fixed departure time. Use `get_routine_schedule` to create a full timeline, `validate_task_dependencies` to check for logical loops, `calculate_total_duration` to find the minimum time needed, or `simulate_buffer_impact` to see how extra safety margins affect the wake-up time.


## Available Tools (4)
- **calculate_total_duration**: Determines the minimum total time required to complete a specific subset of tasks
- **get_routine_schedule**: Generates a complete, ordered morning routine based on a departure time and a list of tasks
- **simulate_buffer_impact**: Predicts how adding extra buffer time to specific tasks will shift the overall start time
- **validate_task_dependencies**: Checks if a set of requested tasks contains any logical contradictions or impossible loops


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Morning Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a morning routine for a child who needs to leave at 08:00. Tasks: Breakfast (20m), Get Dressed (15m, depends on Breakfast), Brush Teeth (5m, depends on Get Dressed)."

**🤖 AI Agent:**
> The morning routine is: Breakfast starts at 07:20 and ends at 07:40. Get Dressed starts at 07:40 and ends at 07:55. Brush Teeth starts at 07:55 and ends at 08:00.

---

**👤 You:**
> "How much total time do I need for: Wake up (10m), Eat (20m), Pack Bag (5m)?"

**🤖 AI Agent:**
> The total required time for these tasks is 35 minutes.

---

**👤 You:**
> "If I add 5 minutes of buffer to Breakfast, how will it change my start time?"

**🤖 AI Agent:**
> Adding 5 minutes to Breakfast will move the earliest start time 5 minutes earlier.


## ❓ FAQ

**Q: How does the scheduling work?**
The server uses backward scheduling. It starts at the departure time and works backward through each task's duration and buffer to determine the necessary start times.

**Q: Can I check if my task list is valid?**
Yes, you can use the `validate_task_dependencies` tool to ensure there are no circular dependencies or impossible task loops.

**Q: What happens if a task doesn't fit in the time window?**
The `get_routine_schedule` tool will return a list of `unfitTasks` that could not be accommodated within the requested timeframe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-morning-scheduler](https://vinkius.com/en/ai-agent-connect/school-morning-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Morning Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-morning-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Morning Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-morning-scheduler": {
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
