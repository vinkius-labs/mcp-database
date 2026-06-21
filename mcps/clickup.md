# ClickUp MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickup)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clickup-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clickup-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage tasks and projects via ClickUp — track work, monitor spaces, and manage team productivity directly from any AI agent.

## Description
Connect your **ClickUp** account to any AI agent and take full control of your project management and productivity through natural conversation. Streamline how you manage tasks, subtasks, and complex workflows natively.

### What you can do

- **Workspace Oversight** — List and retrieve details for all workspaces (teams) you belong to natively
- **Hierarchy Intelligence** — Access and monitor spaces, folders, and lists to understand project structures flawlessly
- **Task Management** — List and retrieve detailed information for tasks, including statuses and priorities, securely
- **Workflow Logistics** — Create new tasks and manage subtasks to keep your team organized flawlessly
- **Productivity Tracking** — Access your own user profile and team member information securely
- **Integrated Visibility** — Retrieve detailed task metadata including descriptions and due dates directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ClickUp Personal API Token (obtained from Settings > Apps)
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor task progress and team capacity using natural language
- **Team Leads** — audit project hierarchies and task statuses without opening the complex dashboard
- **Developers** — quickly look up task details and create new to-dos straight from their chat interface
- **Ops Teams** — verify workspace configurations and monitor organizational productivity


## Available Tools
- **create_new_task**: Create a new task in a specific list
- **get_my_clickup_profile**: Retrieve information about the authenticated user
- **get_task_details**: Get detailed information for a specific task
- **list_space_folders**: List all folders within a space
- **list_space_lists**: List all lists within a space
- **list_workspace_spaces**: List all spaces within a workspace
- **list_list_tasks**: List all tasks in a specific list
- **list_clickup_workspaces**: List all workspaces (teams) the user belongs to


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickUp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my ClickUp workspaces."

**🤖 AI Agent:**
> Retrieving your ClickUp workspaces... I found 2: 'Product Team' (ID: 1234) and 'Marketing Dept' (ID: 5678). Which one would you like to see the spaces for?

---

**👤 You:**
> "Show me the tasks in the 'Q2 Launch' list."

**🤖 AI Agent:**
> Checking tasks in Q2 Launch... I found 5 items: 'Update Landing Page' (To Do), 'Finalize Copy' (In Progress), 'Security Audit' (Closed), and 2 others. Should I include subtasks?

---

**👤 You:**
> "Create a new task called 'Prepare presentation' in list 'wf_123'."

**🤖 AI Agent:**
> Creating task 'Prepare presentation'... The task has been successfully created in ClickUp. You can find it under the ID 'task_abc123'. Would you like to add a description or a due date?


## Installation & Usage

To install and use the **ClickUp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickup](https://vinkius.com/mcp/clickup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
