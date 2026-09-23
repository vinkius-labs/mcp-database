# Renovation Progress Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/renovation-progress-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and calculate completion percentages for renovation projects.

## Description
This MCP server provides tools to monitor renovation project lifecycles. Use `get_project_progress` to calculate the exact completion percentage, `list_all_projects` to view all active jobs, `get_task_details` to inspect specific task statuses, and `get_project_summary` for a high-level overview of workload scale and task distribution.


## Available Tools (4)
- **get_project_progress**: Calculates the current completion percentage for a specific renovation project
- **get_project_summary**: Provides a high-level overview of a project's health and scale
- **get_task_details**: Retrieves the specific status and details of individual tasks within a project
- **list_all_projects**: Retrieves a list of all renovation projects currently being tracked


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Renovation Progress Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the progress of project PRJ-123?"

**🤖 AI Agent:**
> Project PRJ-123 is 75% complete, with 15 out of 20 tasks finished.

---

**👤 You:**
> "List all my renovation projects."

**🤖 AI Agent:**
> You have 3 active projects: Kitchen Remodel (PRJ-001), Bathroom Update (PRJ-002), and Basement Finish (PRJ-003).

---

**👤 You:**
> "Give me a summary for project PRJ-999."

**🤖 AI Agent:**
> Project PRJ-999 is a medium-sized project with a 40% completion ratio. Status breakdown: 4 pending, 2 in-progress, and 3 completed.


## ❓ FAQ

**Q: How is the progress percentage calculated?**
The progress is calculated by dividing the number of finished tasks by the total number of tasks in the project.

**Q: Can I see the status of a specific task?**
Yes, you can use the `get_task_details` tool to retrieve the current state and description of any task within a project.

**Q: What information is included in the project summary?**
The `get_project_summary` tool provides the completion ratio, the workload scale (small, medium, or large), and a breakdown of task statuses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/renovation-progress-tracker](https://vinkius.com/en/ai-agent-connect/renovation-progress-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Renovation Progress Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `renovation-progress-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Renovation Progress Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "renovation-progress-tracker": {
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
