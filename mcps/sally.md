# Sally MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sally)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sally-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sally-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Sally** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sally](https://vinkius.com/mcp/sally)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
