# Wrike MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wrike)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wrike-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wrike-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage tasks, projects, and folders on Wrike — the most versatile work management platform for teams.

## Description
Connect your **Wrike** account to any AI agent and manage your enterprise workflows through natural conversation.

### What you can do

- **Task Monitoring** — List and browse tasks across your entire account or filter by specific folder/project IDs
- **Deep Task Analysis** — Retrieve comprehensive metadata for specific tasks, including descriptions, assignees, and custom fields
- **Project Navigation** — Browse top-level project containers and monitor their current status and organization
- **Folder Hierarchy** — Explore your organizational structure to understand how tasks are grouped and categorized
- **Team Discovery** — List all users and contacts within your Wrike workspace to find IDs for task assignment
- **Space Access** — List all available work areas (spaces) to navigate your team's different departments or functions
- **Workflow Automation** — Quickly find unique task and folder IDs required for building automated project management flows

### How it works

1. Subscribe to this server
2. Enter your Wrike Access Token
3. Start managing your tasks and projects through Claude, Cursor, or any MCP-compatible client

No more manual digging through complex project folders to find an update. Your AI agent becomes your project operations assistant.

### Who is this for?

- **Project Managers** — monitor task progress and audit project health through simple chat commands
- **Team Leads** — lookup team member IDs and browse departmental spaces without manual navigation
- **Operations Managers** — audit folder structures and verify task assignments across the workspace
- **Executive Assistants** — quickly surface task details and project statuses for reporting and coordination


## Available Tools
- **get_task_details**: Retrieves comprehensive details for a specific Wrike task
- **list_wrike_contacts**: Lists all users and contacts within the Wrike workspace
- **list_wrike_folders**: Lists all folders and projects in the Wrike account
- **list_wrike_projects**: Lists all active projects in the account
- **list_wrike_spaces**: Lists all Wrike spaces available to the authenticated user
- **list_wrike_tasks**: You can optionally provide a folder_id to scope the results.

Lists tasks in the Wrike account, optionally filtered by folder


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wrike** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Wrike projects."

**🤖 AI Agent:**
> I found 5 active projects in your account: 1. 'Product Launch 2026' (ID: IE...), 2. 'Q1 Marketing Campaign' (ID: IE...), 3. 'Internal Website Redesign' (ID: IE...), and 2 others. Which one would you like to explore?

---

**👤 You:**
> "Show me tasks in the 'Product Launch 2026' folder."

**🤖 AI Agent:**
> Searching folder 'Product Launch 2026' (ID: IE...)... I found 8 tasks. The most recent are: 1. 'Finalize Design Specs' (Status: Active), 2. 'Coordinate with Vendors' (Status: Active), and 3. 'Budget Approval' (Status: Completed). Would you like the details for any of these?

---

**👤 You:**
> "Get full details for task ID 'IEA...'."

**🤖 AI Agent:**
> Task 'Finalize Design Specs' (ID: IEA...): Description: 'Complete the UI/UX documentation for the mobile dashboard'. Status: Active, Priority: High, Assigned to: John Doe. Would you like me to check for any custom field values?


## Installation & Usage

To install and use the **Wrike** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wrike](https://vinkius.com/mcp/wrike)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
