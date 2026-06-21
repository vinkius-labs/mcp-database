# Todoist MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/todoist-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/todoist-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/todoist-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Todoist tasks and projects — audit productivity via AI.

## Description
Empower your AI agent to orchestrate your entire productivity ecosystem with **Todoist**, the world's favorite task manager. By connecting Todoist to your agent, you transform complex to-do lists into a natural conversation. Your agent can instantly list your active tasks, audit project progress, and create new items without you ever touching a dashboard. Whether you are managing personal errands or complex team projects, your agent acts as a real-time project coordinator, ensuring your goals are always organized and on track.

### What you can do

- **Task Auditing** — List all active tasks and retrieve detailed metadata for each, including due dates and priorities.
- **Project Oversight** — List all your projects and sections to maintain a structured view of your responsibilities.
- **Lifecycle Management** — Create, update, complete, and delete tasks through natural language to keep your list current.
- **Label Management** — List all your custom labels to ensure your categorization is consistent.
- **Account Auditing** — Quickly retrieve account-wide task counts to understand your current workload.

### How it works

1. Subscribe to this server
2. Enter your Todoist API Token
3. Start managing your tasks through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Busy Professionals** — monitor daily tasks and update priorities straight from your workflow.
- **Project Managers** — verify if team tasks are being correctly created and assigned in specific projects.
- **Students** — perform rapid audits of assignment deadlines and update task descriptions without manual logins.
- **Operations Leads** — automate task querying to orchestrate cross-functional team productivity smoothly.


## Available Tools
- **close_task**: Complete a task
- **create_task**: Create a new task
- **delete_task**: Delete a task
- **get_project**: Get details for a specific project
- **get_task**: Get details for a specific task
- **list_labels**: List all user labels
- **list_projects**: List all Todoist projects
- **list_sections**: List sections in a project
- **list_tasks**: Supports filtering by project_id, section_id, label, or filter string.

List Todoist tasks
- **update_task**: Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Todoist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my tasks for today in Todoist."

**🤖 AI Agent:**
> I've retrieved your tasks for today. You have 3 items, including 'Finish report' and 'Call client'. Would you like the details for any of them?

---

**👤 You:**
> "Create a new task 'Buy groceries' for tomorrow morning."

**🤖 AI Agent:**
> Task created! 'Buy groceries' has been added to your Inbox with a due date of tomorrow at 9:00 AM.

---

**👤 You:**
> "Show me all my projects in Todoist."

**🤖 AI Agent:**
> You have 4 active projects: 'Work', 'Personal', 'Shopping', and 'Travel'. I can list the tasks inside any of these projects for you.


## Installation & Usage

To install and use the **Todoist** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/todoist-alternative](https://vinkius.com/mcp/todoist-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
