# Leiga MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leiga)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/leiga-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/leiga-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage agile projects with AI-assisted sprint planning, task prioritization, and team workload balancing that adapts in real time.

## Description
Connect your **Leiga** account to any AI agent and manage projects through natural conversation.

### What you can do

- **Project Management** — List projects, inspect details, and track progress
- **Task Tracking** — Create, update, move, and assign tasks
- **Sprint Management** — Browse sprints with capacity and velocity data
- **Team Workload** — Monitor team member assignments and availability

### How it works

1. Subscribe to this server
2. Enter your Leiga API Key
3. Start managing projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **PMs** — manage projects and sprint planning
- **Developers** — track tasks and update status
- **Team Leads** — monitor workload and progress


## Available Tools
- **create_task**: Create a new task
- **get_project_details**: Get details for a specific project
- **get_task_details**: Get details for a specific task
- **list_team_members**: List team users
- **list_projects**: List Leiga projects
- **list_tasks**: Optionally filter by project ID.

List tasks
- **list_organizational_teams**: List configured teams
- **list_workflows**: List automated workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Leiga** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all projects and the current sprint status."

**🤖 AI Agent:**
> Projects: 4. 'Platform v2' (45 tasks), 'Mobile App' (28), 'API Redesign' (18), 'DevOps' (12). Current sprint (Sprint 14): 18 tasks. Done: 8 (44%), In Progress: 6, To Do: 4. Velocity: 22 pts/sprint (avg). Capacity: 85% utilized. Deadline: Apr 30. ⚠️ 2 tasks blocked.

---

**👤 You:**
> "Create a task 'Fix auth bug' and show team workload."

**🤖 AI Agent:**
> Task created! 'Fix auth bug' — Priority: High, Sprint 14, Assigned: Sarah. Team: Sarah (6 tasks, 90% ⚠️), Mike (4 tasks, 65%), Lisa (5 tasks, 75%), James (3 tasks, 50%). Sprint points: 22/26 allocated. Sarah at capacity — consider reassigning.

---

**👤 You:**
> "Show sprint velocity trends and blocked tasks."

**🤖 AI Agent:**
> Velocity (last 5 sprints): S10: 18, S11: 20, S12: 22, S13: 24, S14: 22 (in progress). Trend: +22% improvement. Blocked: 2 tasks. 1) 'Database migration' — blocked by 'Schema review' (Mike, 2 days). 2) 'Payment integration' — blocked by 'API keys from vendor' (external).


## Installation & Usage

To install and use the **Leiga** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leiga](https://vinkius.com/mcp/leiga)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
