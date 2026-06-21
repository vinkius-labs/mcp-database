# Flow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flow)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flow-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flow-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage projects, tasks, and team collaboration via AI agents with Flow (getflow.com).

## Description
Connect your **Flow** account to any AI agent and automate your project management and team collaboration through the Model Context Protocol (MCP). Flow (getflow.com) provides a clean and powerful platform for organizing work, tracking task progress, and facilitating team discussions. Now, you can manage your workspaces, projects, and individual tasks directly through natural conversation.

### What you can do

- **Project Coordination** — List all projects within your workspaces and retrieve detailed metadata, including ownership and due dates.
- **Task Management** — Create, update, and list tasks across workspaces, projects, or specific task lists. Change statuses (incomplete/completed) instantly.
- **Organized Lists** — Access and list task groups (Lists) within projects to maintain a clear hierarchy of work.
- **Team Interaction** — List all workspace members and teams, and participate in task discussions by reading or adding comments.
- **Workspace Oversight** — Get a high-level view of all the top-level workspaces you belong to.
- **Real-time Updates** — Fetch specific task details or metadata to keep your team informed and your projects on track.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flow Personal Access Token (found in Account Settings > Apps & Developers)
3. Start managing your projects and tasks from Claude, Cursor, or any MCP client

### Who is this for?

- **Project Managers** — quickly check task statuses or update project timelines while coordinating with team leads.
- **Software Teams** — automate the retrieval of task comments and metadata directly from your development environment.
- **Marketing Agencies** — manage client projects and task lists through simple AI commands to stay organized and productive.


## Available Tools
- **add_task_comment**: Post a comment
- **create_task**: Create a new task
- **get_project**: Get project details
- **get_task**: Get task details
- **list_task_lists**: List lists in project
- **list_workspace_members**: List team members
- **list_projects**: List projects in workspace
- **list_task_comments**: List task discussions
- **list_tasks**: List tasks
- **list_workspace_teams**: List workspace teams
- **list_workspaces**: List top-level workspaces
- **update_task**: ).

Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Flow projects in the 'Marketing' workspace."

**🤖 AI Agent:**
> Fetching projects... I found 4 projects in your 'Marketing' workspace, including 'Q4 Campaign' and 'Brand Guidelines'. Would you like to see the task lists for any of these?

---

**👤 You:**
> "Create a new task: 'Review final design mockup' in the 'Design' list."

**🤖 AI Agent:**
> Task created! I've added 'Review final design mockup' to your 'Design' task list. The task ID is 'task_123'. Would you like to assign it to someone or set a due date?

---

**👤 You:**
> "Add a comment to task 'task_123': 'Design looks great, proceed to coding'."

**🤖 AI Agent:**
> Comment added! Your feedback has been successfully posted to task 'task_123'. The team will see your update in the task discussion timeline.


## Installation & Usage

To install and use the **Flow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flow](https://vinkius.com/mcp/flow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
