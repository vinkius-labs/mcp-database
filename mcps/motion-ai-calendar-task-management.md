# Motion (AI Calendar & Task Management) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/motion-ai-calendar-task-management)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/motion-ai-calendar-task-management-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/motion-ai-calendar-task-management-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your schedule via Motion — create AI-optimized tasks, track projects, and audit your timeline.

## Description
Connect your **Motion** account to any AI agent and take full control of your AI-powered scheduling, project management, and daily timeline through natural conversation.

### What you can do

- **Task Orchestration** — Create new tasks directly from your agent, allowing Motion's AI engine to automatically allocate calendar blocks based on priority (ASAP, HIGH, MEDIUM, LOW) and durations
- **Project Management** — List and retrieve projects within your workspaces to group related tasks and track high-level organizational initiatives securely
- **Timeline Optimization** — Retrieve your AI-optimized workspace schedule to understand exactly when tasks are projected to be completed after resolving all dependencies
- **Workspace Navigation** — Explore multiple workspaces to retrieve the exact GUIDs required for scoped task querying and project mapping natively
- **Live Task Mutating** — Update task priorities, due dates, or descriptions in real-time, signaling the AI engine to immediately recalculate your entire schedule
- **Cross-Workspace Relocation** — Seamlessly move tasks between different organizational containers to optimize project boundaries and resource allocation
- **Operational Cleanup** — Irreversibly delete completed or obsolete tasks to maintain a clean and relevant project log across your account

### How it works

1. Subscribe to this server
2. Enter your Motion API Key
3. Start managing your AI-powered schedule from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Busy Professionals** — automate task entry and monitor AI-optimized timelines through natural conversation without manual calendar shuffling
- **Project Leads** — manage team tasks across multiple workspaces and verify project project flows directly from your workspace
- **Knowledge Workers** — track high-priority deadlines and retrieve rapid summaries of your daily schedule to maintain high-speed productivity


## Available Tools
- **list_tasks**: Optional status filters narrow the scope.

List all tasks in a Motion workspace filtering by current lifecycle status
- **get_task**: Retrieve full details of a specific Motion task by ID
- **create_task**: Create a new task in Motion that will be auto-scheduled by AI
- **update_task**: Update configuration parameters of an existing Motion task
- **delete_task**: Delete a Motion task permanently destroying associated calendar blocks
- **move_task**: Move a specific Motion task assigning a different workspace target
- **list_projects**: List all projects in a Motion workspace. Projects are containers that group related tasks together
- **create_project**: Create a new static project in a Motion workspace
- **list_workspaces**: List all workspaces the authenticated Motion user has access to
- **get_schedule**: Get the AI-optimized timeline schedule for a workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Motion (AI Calendar & Task Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Motion workspaces"

**🤖 AI Agent:**
> I've retrieved 2 workspaces from your account: 'Engineering' (ID: ws-123) and 'Personal' (ID: ws-456). Which one would you like to list the projects or tasks for?

---

**👤 You:**
> "Create a high-priority task 'Review PR #456' in workspace 'ws-123' due tomorrow, takes 30 mins"

**🤖 AI Agent:**
> Task 'Review PR #456' created successfully! Motion AI has automatically scheduled this for tomorrow at 10:30 AM based on your current workload. New Task ID: 'task-98765'. Would you like me to show your updated schedule?

---

**👤 You:**
> "Show me the optimized schedule for my 'Engineering' workspace"

**🤖 AI Agent:**
> Retrieving AI-optimized schedule… I've identified your time blocks for today: 1) 09:00 - 'Email Triage', 2) 10:30 - 'Review PR #456', 3) 14:00 - 'Design Sync'. Motion has successfully resolved 5 tasks into your free slots. No priority conflicts detected.


## Installation & Usage

To install and use the **Motion (AI Calendar & Task Management)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/motion-ai-calendar-task-management](https://vinkius.com/mcp/motion-ai-calendar-task-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
