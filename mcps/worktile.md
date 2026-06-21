# Worktile MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/worktile)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/worktile-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/worktile-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Collaborative project management and team communication platform — manage tasks, projects, and messages via AI.

## Description
Empower your AI agent to orchestrate your team's collaboration with **Worktile**, the leading project management and team communication suite. By connecting Worktile to your agent, you transform complex task tracking, project planning, and channel communication into a natural conversation. Your agent can instantly list your projects, create new tasks, update statuses, and even send messages to your team channels without you ever needing to navigate the Worktile web or mobile interface. Whether you are managing an agile development team or a cross-functional department, your agent acts as a real-time operations assistant, keeping your workspace organized and your communication flowing.

### What you can do

- **Project Management** — List all accessible agile projects and retrieve detailed information about your workspace.
- **Task Operations** — Create, update, and track tasks with full support for descriptions, assignees, and state changes.
- **Workflow Customization** — Browse project-specific task states to understand exactly where each item sits in your process.
- **Team Communication** — List message channels and send instant updates to your team directly through the chat interface.
- **Organization Overview** — Retrieve information about your team members and overall organization structure.

### How it works

1. Subscribe to this server
2. Enter your Worktile Client ID and Client Secret
3. Start managing your team collaboration through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Team Leads** — monitor project progress, update task statuses, and keep team members informed through natural language.
- **Product Managers** — track feature development and coordinate between different projects and channels.
- **Operations Managers** — oversee multiple team workflows and organizational structures through a unified AI interface.
- **Knowledge Workers** — manage your personal tasks and team communications directly from your AI-powered workspace.


## Available Tools
- **create_task**: Create a new Worktile task
- **get_project**: Get project details
- **get_team_info**: Get team details
- **list_channels**: List message channels
- **list_members**: List organization members
- **list_projects**: List all Worktile agile projects
- **list_task_states**: List task states for a project
- **list_tasks**: List tasks in a project
- **send_message**: Send message to channel
- **update_task**: Update an existing Worktile task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Worktile** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active projects on Worktile."

**🤖 AI Agent:**
> I've retrieved your Worktile projects. You have 3 active projects: 'Marketing Q3', 'New Product Launch', and 'Internal HR'. Which one would you like to view tasks for?

---

**👤 You:**
> "Create a task in project 'Marketing Q3' titled 'Finalize social media assets'."

**🤖 AI Agent:**
> Done! I've created the task 'Finalize social media assets' in the 'Marketing Q3' project. Would you like to assign it to a team member?

---

**👤 You:**
> "Post an update to the 'General' channel saying 'The project kickoff has been moved to 2 PM'."

**🤖 AI Agent:**
> I've posted your update to the 'General' channel. Your team has been notified that the kickoff is now at 2 PM.


## Installation & Usage

To install and use the **Worktile** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/worktile](https://vinkius.com/mcp/worktile)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
