# Sally MCP Server

Keep frontline teams connected with an employee communication platform that reaches deskless workers through mobile and chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sally)

## Overview
**Category:** productivity
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Sally** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sally](https://vinkius.com/mcp/sally)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
