# Move-Out Cleaning Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/move-out-cleaning-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes cleaning task assignments based on personnel availability and deadlines.

## Description
This MCP server provides tools to manage move-out cleaning operations. It allows agents to retrieve task lists via `get_task_list`, check staff availability with `get_personnel_availability`, and verify if a schedule is possible using `validate_schedule_capacity`. The core functionality is provided by `generate_cleaning_schedule`, which creates an optimized distribution of tasks to ensure all cleaning is completed before the property deadline.


## Available Tools (4)
- **get_personnel_availability**: Provides the availability windows for all people assigned to the move-out cleaning
- **generate_cleaning_schedule**: Calculates the most efficient distribution of tasks among available people
- **validate_schedule_capacity**: Checks if the total estimated cleaning time exceeds the total available person-minutes
- **get_task_list**: Retrieves a summary of all tasks that need to be performed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Move-Out Cleaning Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check if we have enough people to clean property PROP-123 by tomorrow at 5 PM?"

**🤖 AI Agent:**
> The total task duration is 320 minutes, and your available personnel have 400 minutes of availability before the deadline. The schedule is feasible.

---

**👤 You:**
> "Generate a cleaning schedule for property PROP-456 with a deadline of 2024-12-01T18:00:00."

**🤖 AI Agent:**
> Schedule generated: Person A is assigned to Vacuuming (09:00-09:30) and Mopping (09:30-10:00). Person B is assigned to Dusting (09:00-09:15).

---

**👤 You:**
> "What tasks need to be done at property PROP-789?"

**🤖 AI Agent:**
> The tasks for property PROP-789 are: Dusting (15 min), Vacuuming (30 min), and Window Cleaning (45 min).


## ❓ FAQ

**Q: How do I know if there is enough staff to finish the cleaning?**
You can use the `validate_schedule_capacity` tool to check if the total estimated cleaning time fits within the available minutes of your personnel before the deadline.

**Q: Can I see which tasks are still unassigned?**
Yes, when you run `generate_cleaning_schedule`, the response includes an `unassignedTasks` list containing any tasks that could not be scheduled within the available time windows.

**Q: How does the scheduler handle personnel availability?**
The scheduler uses `get_personnel_availability` to identify specific time windows for each person and ensures no task is assigned outside of those windows or after the global deadline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/move-out-cleaning-scheduler](https://vinkius.com/en/ai-agent-connect/move-out-cleaning-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Move-Out Cleaning Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `move-out-cleaning-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Move-Out Cleaning Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "move-out-cleaning-scheduler": {
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
