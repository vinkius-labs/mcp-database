# Taskworld MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/taskworld)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/taskworld-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/taskworld-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage Taskworld projects, tasks, and team collaboration directly from your AI agent.

## Description
Integrate **Taskworld** with your AI workflow to streamline project management and team communication. This server allows your agent to interact with your workspaces, projects, and tasks using natural language.

### Key Features

- **Workspace Management** — List all accessible workspaces and retrieve specific details for organizational oversight.
- **Project Control** — Create new projects, list existing ones, and update project details or completion status.
- **Task Lifecycle** — Create tasks with due dates and points, update assignees, and mark tasks as completed.
- **Team Collaboration** — Access and post comments on tasks to keep the conversation flowing without leaving your AI interface.
- **Task Inspection** — Retrieve comprehensive task lists from specific projects to monitor progress.

### How it works

1. Subscribe to the Taskworld server.
2. Provide your Taskworld Personal Access Token.
3. Start managing your sprints and tasks directly from Claude, Cursor, or any MCP client.

### Who is this for?

- **Project Managers** — Quickly update task statuses and check project progress across multiple workspaces.
- **Developers** — Create and update tasks or check comments while staying in your coding environment.
- **Team Leads** — Orchestrate workflows and assign tasks to team members through simple conversation.


## Available Tools
- **list_comments**: Get all comments on a task
- **complete_task**: Mark a task as finished
- **create_comment**: Post a new comment to a task or project
- **create_project**: Create a new project
- **create_task**: Create a new task
- **get_workspace**: Get details for a specific workspace
- **login**: Login to Taskworld to obtain an access token
- **list_projects**: List all projects in a workspace
- **list_tasks**: Retrieve all tasks within a project
- **update_project**: Can be used to change the title, description, or mark it as completed.

Update project details or mark as completed
- **update_task**: Can be used to change assignee, set due date, update title, etc.

Update task properties
- **list_workspaces**: List all Taskworld workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Taskworld** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Taskworld workspaces."

**🤖 AI Agent:**
> I've found 2 workspaces: 'Engineering Team' (ID: 648291) and 'Marketing Dept' (ID: 772930). Which one would you like to explore?

---

**👤 You:**
> "Show me the tasks for project 648291."

**🤖 AI Agent:**
> Fetching tasks for project 648291... I found 3 active tasks: 'Update API Documentation', 'Fix Login Bug', and 'Prepare Sprint Review'. Would you like more details on any of these?

---

**👤 You:**
> "Mark task 99283 as completed."

**🤖 AI Agent:**
> Task 99283 has been successfully marked as completed. Is there anything else I can help you with?


## Installation & Usage

To install and use the **Taskworld** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taskworld](https://vinkius.com/mcp/taskworld)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
