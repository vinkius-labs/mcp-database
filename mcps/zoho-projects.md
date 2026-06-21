# Zoho Projects MCP Server

Manage projects, tasks, and milestones via the Zoho Projects V3 API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-projects)

## Overview
**Category:** productivity
**Tools Count:** 9

## Description
Connect your **Zoho Projects** account to any AI agent to streamline your project management and team collaboration. This MCP server enables your agent to interact with portals, projects, and tasks directly through natural language interfaces using the latest V3 API.

### What you can do

- **Project Oversight** — List all projects within your portals and retrieve detailed configurations and metadata
- **Task Management** — List, retrieve, create, and update tasks across your projects with support for partial updates
- **Milestone Tracking** — Monitor project milestones and their associated target dates to stay on schedule
- **Team Visibility** — List all users and participants registered for a specific project to manage responsibilities
- **Organization Control** — List task lists and portals to maintain a clear picture of your entire project management hierarchy

### How it works

1. Subscribe to this server
2. Enter your Zoho Client ID, Client Secret, and Data Center Domain
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — Quickly update task statuses and monitor project health via natural language commands
- **Team Leads** — Move tasks through the pipeline and assign responsibilities without opening the dashboard
- **Developers** — Integrate project management data and task automation into your daily development workflow


## Available Tools
- **create_project**: Requires a portal ID and a project name.

Create a new project in a portal
- **create_task**: Requires portal ID, project ID, and task name.

Create a new task in a project
- **list_milestones**: List all milestones in a project
- **list_portals**: Use this to identify the portal ID for subsequent project and task calls.

List all Zoho Projects portals
- **list_projects**: List all projects in a portal
- **list_task_lists**: List all task lists in a project
- **list_tasks**: List all tasks in a project
- **update_task**: Update an existing task
- **list_project_users**: List all users associated with a project


## Installation & Usage

To install and use the **Zoho Projects** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-projects](https://vinkius.com/mcp/zoho-projects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
