# ProjectManager MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/projectmanager)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/projectmanager-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/projectmanager-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate project planning and tracking via ProjectManager — manage projects, tasks, and timesheets directly from any AI agent.

## Description
Connect your **ProjectManager.com** account to any AI agent and simplify your project orchestration, task management, and resource allocation through natural conversation.

### What you can do

- **Project Management** — List all projects, retrieve detailed status metadata, and monitor project health and progress
- **Task Control** — Query tasks for any project, retrieve detailed descriptions, and create new tasks programmatically
- **Resource Intelligence** — List team resources, including members and equipment, to choose the right context for each task
- **Time Tracking** — Access a history of recorded timesheets to stay on top of your project billing and capacity
- **Direct Control** — Manage your entire project portfolio directly from your agent without manual dashboard navigation

### How it works

1. Subscribe to this server
2. Enter your ProjectManager API Key from your account settings
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_project**: Create a new project
- **create_project_task**: Add a new task
- **get_project_details**: Get details for a specific project
- **get_task_details**: Get details for a specific task
- **list_dashboards**: List all dashboards
- **list_projects**: List ProjectManager projects
- **list_team_resources**: List team resources
- **list_tags**: List all project tags
- **list_tasks**: Optionally filter by project ID.

List tasks
- **list_timesheets**: List recorded timesheets
- **update_task**: Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProjectManager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in ProjectManager."

**🤖 AI Agent:**
> I've retrieved your projects. You have 5 active projects, including 'New Product Launch' (80% complete) and 'Website Redesign'.

---

**👤 You:**
> "Show me all overdue tasks across all projects with their assignees and original deadlines."

**🤖 AI Agent:**
> 23 overdue tasks across 6 projects. Critical (5+ days late): "API Integration Testing" on Mobile App (assigned: James Park, due May 5). "UX Research Report" on Website Redesign (Sarah Chen, due May 3). "Database Schema Review" on Data Migration (Lisa Wang, due May 1). Medium priority (2-4 days late): 8 tasks across 4 projects. Low priority (1 day late): 12 tasks. Total hours at risk: 156. 3 project milestones are impacted by these delays.

---

**👤 You:**
> "Create 3 new tasks for the Website Redesign project assigned to the design team due next Friday."

**🤖 AI Agent:**
> 3 tasks created in Website Redesign project. Task 1: "Homepage Hero Section Mockup" assigned to Sarah Chen, priority: High, estimated: 8 hours. Task 2: "Navigation Menu Redesign" assigned to Alex Rivera, priority: Medium, estimated: 6 hours. Task 3: "Mobile Responsive Layouts" assigned to Lisa Wang, priority: High, estimated: 12 hours. All due: Friday, May 23rd. Total estimated effort: 26 hours. Calendar notifications sent to all assignees.


## Installation & Usage

To install and use the **ProjectManager** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/projectmanager](https://vinkius.com/mcp/projectmanager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
