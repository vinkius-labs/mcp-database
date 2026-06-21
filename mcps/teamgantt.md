# TeamGantt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teamgantt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan projects with intuitive Gantt charts that show deadlines, dependencies, and team workloads in one visual timeline.

## Description
Connect your **TeamGantt** account to any AI agent and simplify how you manage your project timelines, task assignments, and team resources through natural conversation.

### What you can do

- **Project Oversight** — List all projects in your account and retrieve detailed metadata and configuration for specific Gantt charts.
- **Task Management** — Create, update, and delete tasks with full control over start/end dates and completion percentages.
- **Timeline Coordination** — Create dependencies between tasks to ensure your project logic remains sound and automated.
- **Resource Tracking** — List available resources (people and equipment) to optimize team allocation across projects.
- **Milestone Planning** — List and query major project goals (milestones) and sub-task checklists.
- **Account Visibility** — Fetch your user profile and verify account configurations directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your TeamGantt API Token (found in your account settings under API)
3. Start managing your timelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — quickly check task progress and update project timelines via simple AI commands.
- **Operations Teams** — coordinate resource assignments and verify dependencies directly from the workspace.
- **Engineering Leads** — monitor milestones and update task completion percentages via the AI assistant.


## Available Tools
- **link_tasks_dependency**: g. Task A must finish before Task B starts).

Create Gantt link
- **create_new_task**: Add task to project
- **remove_task**: Delete task
- **get_task_checklist**: List sub-tasks
- **get_account_profile**: Get user info
- **get_project_details**: Get project info
- **get_task_info**: Get task details
- **list_project_milestones**: List major goals
- **list_projects**: List TeamGantt projects
- **list_available_resources**: List users and labels
- **list_project_tasks**: List tasks in project
- **update_task_fields**: ).

Update task status/dates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TeamGantt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my TeamGantt account."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active timelines: 'Website Launch Q4', 'New Product Development', and 'Marketing Content Plan'. Which one would you like to check tasks for?

---

**👤 You:**
> "Show me the tasks for 'Website Launch Q4' (ID: 10293)."

**🤖 AI Agent:**
> I've fetched the tasks. There are 5 pending items including 'Hero Section Design' (50%), 'Fix login bug' (0%), and 'API Integration' (85%). Shall I update the progress for any of these?

---

**👤 You:**
> "Mark task '88231' as 100% complete."

**🤖 AI Agent:**
> Task updated! I've set the progress for task 88231 to 100% and updated its status to 'completed' in your TeamGantt project. Your timeline has been synchronized.


## ❓ FAQ

**Q: Can I see all the tasks in a project via AI?**
Yes! Use the `list_project_tasks` tool and provide the Project ID. Your agent will retrieve all tasks, milestones, and groups for that specific Gantt chart.

**Q: How do I update the progress of a task using the agent?**
Use the `update_task_fields` action. Provide the Task ID and the `percentComplete` value (0-100) to update the task's status instantly.

**Q: Is it possible to link two tasks with a dependency via AI?**
Absolutely. Use the `link_tasks_dependency` tool. Provide the ID of the predecessor and the successor tasks to create a Gantt link between them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teamgantt](https://vinkius.com/mcp/teamgantt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TeamGantt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `teamgantt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TeamGantt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "teamgantt": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
