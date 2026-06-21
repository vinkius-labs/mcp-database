# ClickUp MCP Server

Bring tasks, docs, goals, and team communication together in one workspace that replaces scattered project management tools.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/clickup-alternative)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **ClickUp** account to any AI agent and take full control of your project hierarchy and task management workflows through natural conversation.

### What you can do

- **Hierarchy Orchestration** — Navigate through your entire ClickUp structure, from Workspaces and Spaces to Folders and Lists programmatically
- **Task Lifecycle Management** — Create, update, and manage tasks in real-time, including monitoring status, priority, and detailed metadata directly through your agent
- **Deep Task Intelligence** — Retrieve complete task details, including descriptions, assigned users, and custom fields to maintain high-fidelity project records
- **Workflow Automation** — Programmatically list tasks within specific lists or filter folderless lists to understand your team's progress and individual workloads
- **Administrative Oversight** — List all accessible workspaces and team members to ensure perfectly coordinated collaboration and permission management

### How it works

1. Subscribe to this server
2. Retrieve your **Personal API Token** from the ClickUp dashboard (Settings > Apps)
3. Start managing your productivity pipeline from Claude, Cursor, or any MCP client

No more manual toggling between lists or digging through complex status folders. Your AI acts as your dedicated project coordinator and task architect.

### Who is this for?

- **Project Managers** — instantly retrieve task lists and update project statuses using natural language commands
- **Software Teams** — manage complex sprints and automate task assignment without leaving your creative workspace
- **Operations Leads** — monitor team capacity and orchestrate folder structures through simple AI queries


## Available Tools
- **create_task**: Requires a task name. Optional status and description can be provided.

Create a new task in a List
- **delete_task**: Delete a specific task
- **get_task_details**: Note: Do not include the # prefix.

Get details for a specific task
- **list_folderless_lists**: List Lists not contained in a Folder
- **list_folders**: Folders help organize multiple lists.

List all Folders in a Space
- **list_lists**: Lists contain the actual tasks.

List all Lists in a Folder
- **list_spaces**: Spaces are large groupings of folders and lists.

List all Spaces in a Workspace
- **list_tasks**: Supports pagination to handle large numbers of tasks.

List tasks within a List
- **list_workspaces**: Workspaces are the top-level unit in ClickUp.

List all ClickUp Workspaces
- **update_task**: Can update the name, description, or status.

Update an existing task


## Installation & Usage

To install and use the **ClickUp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickup-alternative](https://vinkius.com/mcp/clickup-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
