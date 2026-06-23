# Sally MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sally)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Keep frontline teams connected with an employee communication platform that reaches deskless workers through mobile and chat.

## Description
Connect your **Sally** instance to any AI agent and take full control of your API-first project management through natural conversation.

### What you can do

- **Projects** — Create, list, and inspect projects with full metadata.
- **Tasks** — Full CRUD with priorities (P1-P4), statuses, labels, and assignees.
- **Comments** — Add comments to any task for collaboration and status updates.
- **Kanban Board** — Retrieve the aggregated board view showing tasks organized by status columns.
- **Timesheets** — Access timesheet reports with tracked hours and billing information.
- **Profile** — Verify your authenticated identity and workspace permissions.

### How it works

1. Subscribe to this server
2. Enter your Sally API key, instance URL, and workspace slug
3. Start managing projects from Claude, Cursor, or any MCP client

### Who is this for?

- **Project Managers** — create tasks, track progress, and review board status through AI commands.
- **AI Developers** — automate agent-driven task management in a system designed for human+agent collaboration.
- **Operations Teams** — monitor project velocity and timesheet data without switching tools.


## Available Tools (12)
- **add_comment**: Comments are visible to all project members.

Add a comment to a task
- **get_board**: Get the Kanban board view
- **create_project**: Create a new project
- **create_task**: Optionally set priority (P1-P4), status, and labels.

Create a new task in a project
- **get_profile**: Get the authenticated user profile
- **get_project**: Get details of a specific project
- **get_task**: Get full details of a specific task
- **check_sally_health**: Check Sally instance health
- **list_projects**: List all projects in the workspace
- **list_tasks**: Optionally filter by project ID to see tasks for a specific project.

List tasks, optionally filtered by project
- **get_timesheet_report**: Get timesheet report for the workspace or project
- **update_task**: Only provided fields are changed.

Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sally** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my Sally workspace."

**🤖 AI Agent:**
> I found 3 active projects: 'Product Launch' (5 tasks, 2 in progress), 'API Redesign' (12 tasks, 4 in review), and 'Onboarding Flow' (8 tasks, 1 blocked). Would you like to see the board or tasks for any of these?

---

**👤 You:**
> "Create a P2 task 'Implement auth middleware' in project proj_abc123 with labels 'backend, security'."

**🤖 AI Agent:**
> Done! Task 'Implement auth middleware' created in project 'API Redesign' with priority P2 and labels [backend, security]. The new task ID is task_xyz789. Want me to add any comments or sub-tasks?

---

**👤 You:**
> "Show me the Kanban board for project proj_abc123."

**🤖 AI Agent:**
> Here's the board for 'API Redesign': **Backlog** (3 tasks), **In Progress** (4 tasks, including 'Implement auth middleware' P2), **In Review** (2 tasks), **Done** (3 tasks). Would you like to update the status of any task?


## ❓ FAQ

**Q: Can I create a task with priority, labels, and status in one step?**
Yes! Use `create_task` with the project ID, title, priority (P1-P4), status name, and comma-separated labels. The task is created instantly with all metadata.

**Q: How do I view my Kanban board from the AI agent?**
Use `get_board` to retrieve the aggregated board data. Optionally pass a project ID to scope it to a specific project. Tasks are grouped by their status columns.

**Q: Does Sally require a hosted instance or cloud account?**
Sally is a self-hosted, API-first project management system. You need your own Sally instance URL, an API key (atpm_ prefix), and your workspace slug to connect.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sally](https://vinkius.com/mcp/sally)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sally** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sally` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sally** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sally": {
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
