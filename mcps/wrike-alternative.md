# Wrike MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wrike-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wrike-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wrike-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Collaborative project management to manage tasks, projects, and team workflows with AI.

## Description
Connect your **Wrike** account to any AI agent to automate your complex project management workflows through natural conversation. Wrike provides a robust environment for enterprise-scale collaboration, task tracking, and resource management.

### What you can do

- **Project Lifecycle** — List, create, and update tasks with granular control over importance levels, statuses, and custom metadata.
- **Hierarchical Organization** — Navigate and manage the work using a structured system of folders and projects for different departments or clients.
- **Team Collaboration** — Retrieve discussion threads and post comments directly to task feeds to keep your team aligned programmatically.
- **Workspace Monitoring** — List contacts, track custom workflows, and manage task attachments to maintain a clear overview of operational progress.
- **Operational Efficiency** — Automate task assignments and progress tracking to reduce manual coordination effort.

### How it works

1. Subscribe to this server
2. Enter your Wrike Permanent Token from your account settings
3. Start managing your enterprise projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — automate the coordination of large-scale projects and team assignments via natural language.
- **Team Leads** — monitor progress across multiple folders and projects without switching applications.
- **Operations Teams** — streamline task tracking and ensure all organizational workflows are following standard procedures.


## Available Tools
- **add_task_comment**: Post comment to task
- **create_folder**: Add new folder/project
- **create_task**: Add new task
- **get_user_profile**: Get current user
- **get_task_details**: Get full task info
- **list_task_comments**: Get task discussion
- **list_team_members**: List workspace users
- **list_task_attachments**: List task files
- **list_folders_and_projects**: List hierarchy
- **list_tasks**: Can filter by status (Active, Completed, Deferred, Cancelled).

List project tasks
- **list_custom_workflows**: List task workflows
- **update_task**: Modify task info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wrike** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active tasks due this week."

**🤖 AI Agent:**
> I've retrieved your tasks for this week. You have 4 high-priority items, including 'Finalize Budget' and 'Team Sync'. Would you like more details on any of them?

---

**👤 You:**
> "Create a new high-priority task 'Draft Marketing Proposal' in project 'fld_123456'."

**🤖 AI Agent:**
> Successfully created the task 'Draft Marketing Proposal' (ID: tsk_882). I've set the priority to High as requested. Would you like to assign it to someone?


## Installation & Usage

To install and use the **Wrike** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wrike-alternative](https://vinkius.com/mcp/wrike-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
