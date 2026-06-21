# BugHerd MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bugherd)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bugherd-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bugherd-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage visual feedback and bug reports via BugHerd — track projects, tasks, and users directly from any AI agent.

## Description
Connect your **BugHerd** account to any AI agent and orchestrate your visual feedback, website bug tracking, and QA workflows through natural conversation.

### What you can do

- **Project Oversight** — List all your active projects and retrieve detailed metadata, including development URLs.
- **Task & Bug Management** — List all tasks in a project, retrieve detailed descriptions, and update statuses or priorities.
- **Feedback Processing** — Access the dedicated feedback queue to triage new reports from your clients or team.
- **User Coordination** — Access your directory of organization users and manage their involvement in projects.
- **Task Creation** — Create new tasks or feedback reports directly from your workspace with descriptions and priority levels.
- **Organizational Insights** — Retrieve core organization information and settings straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BugHerd API Key
3. Start managing your visual feedback from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers & QA** — quickly check task statuses or retrieve feedback details without manual portal logins.
- **Project Managers** — triage new bugs and update priorities straight from their workflow tools.
- **Designers** — monitor visual feedback and client requests using natural language.


## Available Tools
- **create_project**: Create a new BugHerd project
- **create_task**: Create a new task or feedback in a project
- **get_organization_info**: Retrieve core organization settings
- **get_project**: Get details of a specific project
- **get_task**: Get details of a specific task
- **list_feedback**: List tasks specifically in the Feedback queue
- **list_projects**: List all BugHerd projects
- **list_tasks**: List all tasks in a project
- **list_users**: List all users in the organization
- **update_task**: Update an existing task status or details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BugHerd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active projects in BugHerd."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Vinkius Redesign' (ID: proj_1), 'Client Portal' (ID: proj_2), and 'Marketing Blog' (ID: proj_3).

---

**👤 You:**
> "Show the new feedback for the 'Vinkius Redesign' project."

**🤖 AI Agent:**
> Retrieving feedback... There are 5 items in the queue, including 'Header alignment issue on mobile' and 'Button color doesn't match spec'. Which one would you like to address?

---

**👤 You:**
> "Update task task_123 in project proj_456 to status 'Doing'."

**🤖 AI Agent:**
> Task task_123 has been successfully updated to 'Doing' in the 'Vinkius Redesign' project.


## Installation & Usage

To install and use the **BugHerd** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bugherd](https://vinkius.com/mcp/bugherd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
