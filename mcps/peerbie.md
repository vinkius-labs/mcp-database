# Peerbie MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/peerbie)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/peerbie-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/peerbie-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Orchestrate your entire team's workspace, from Kanban boards to calendar events, completely driven by AI.

## Description
Turn your AI assistant into a relentless project manager. With the Peerbie integration, your agent can instantly summarize cross-project bottlenecks, assign new tasks based on team availability, publish crucial announcements to the company feed, and retrieve upcoming schedule changes—all without opening a single dashboard.

### What you can do
- Full project and task CRUD with per-project filtering
- Publish updates to the company-wide feed
- Manage team and channel directory
- Access and list upcoming calendar events
- Query full member directory with roles

### How it works
1. Log in to your Peerbie workspace
2. Request an API Key via Settings > Integrations
3. Let your AI agents start managing your entire Peerbie collaboration hub directly via Vinkius

### Who is it for?
Ideal for project managers and teams needing instant, conversational access to tasks and Peerbie company updates.


## Available Tools
- **check_peerbie_status**: Verify connectivity
- **create_post**: Create a feed post
- **create_project**: Create a project
- **create_task**: Create a task
- **get_project**: Get project details
- **get_task**: Get task details
- **get_team**: Get team details
- **list_channels**: List channels
- **list_events**: List events
- **list_feed**: List company feed
- **list_members**: List workspace members
- **list_projects**: List projects
- **list_tasks_by_project**: List tasks by project
- **list_tasks**: List all tasks
- **list_teams**: List teams
- **update_task**: Update a task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Peerbie** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all tasks assigned to me in Peerbie"

**🤖 AI Agent:**
> I've fetched your tasks. You currently have 3 pending tasks across all projects. The highest priority is 'Update marketing materials'. Would you like more details on it?

---

**👤 You:**
> "Create a task 'Review Q4 report' in the Marketing project"

**🤖 AI Agent:**
> The task 'Review Q4 report' has been successfully created in the Marketing project. I've left it unassigned. Is there anyone specific you'd like me to assign it to?

---

**👤 You:**
> "List upcoming calendar events for the team"

**🤖 AI Agent:**
> Here are the upcoming events for your team: You have the 'Weekly Standup' tomorrow at 10 AM, and 'Product Review' on Friday at 2 PM.


## Installation & Usage

To install and use the **Peerbie** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/peerbie](https://vinkius.com/mcp/peerbie)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
