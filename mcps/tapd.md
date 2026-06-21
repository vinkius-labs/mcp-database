# TAPD MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tapd)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tapd-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tapd-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Agile product development and collaboration platform by Tencent — manage stories, bugs, and iterations via AI.

## Description
Empower your AI agent to orchestrate your agile development lifecycle with **TAPD**, the professional collaboration platform by Tencent. By connecting TAPD to your agent, you transform complex requirement tracking, bug management, and iteration planning into a natural conversation. Your agent can instantly list your workspaces, create new stories, track defects, and even monitor sprint progress without you ever needing to navigate the complex TAPD enterprise interface. Whether you are following Scrum or Kanban, your agent acts as a real-time product assistant, keeping your development pipeline organized and your team aligned.

### What you can do

- **Workspace Management** — List all accessible workspaces and retrieve detailed information about your development environment.
- **Requirement Tracking** — Create and track stories (requirements) with full support for titles and detailed descriptions.
- **Defect Management** — List and create bugs to keep your quality assurance process moving efficiently.
- **Task Operations** — Manage granular tasks within your workspaces to stay on top of daily development activities.
- **Iteration Monitoring** — Browse workspace iterations (sprints) to track project milestones and delivery schedules.
- **Team Overview** — List workspace members to manage assignments and collaboration effectively.

### How it works

1. Subscribe to this server
2. Enter your TAPD API User and API Password
3. Start managing your agile workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — track feature requirements, audit backlogs, and monitor iteration progress through natural language.
- **Software Engineers** — manage your assigned tasks and update bug statuses directly from your AI-powered workspace.
- **QA Engineers** — report defects and monitor the resolution of bugs across multiple projects.
- **Agile Coaches** — oversee multiple team workflows and organizational structures through a unified AI interface.


## Available Tools
- **create_bug**: Create a new TAPD bug
- **create_story**: Create a new TAPD story
- **create_task**: Create a new TAPD task
- **get_workspace**: Get workspace details
- **list_bugs**: List bugs in a workspace
- **list_iterations**: List workspace iterations
- **list_members**: List workspace members
- **list_stories**: List stories in a workspace
- **list_tasks**: List tasks in a workspace
- **list_workspaces**: List all TAPD workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TAPD** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active workspaces on TAPD."

**🤖 AI Agent:**
> I've retrieved your TAPD workspaces. You have 4 active projects, including 'Cloud Infrastructure' and 'Mobile App V2'. Which one would you like to view items for?

---

**👤 You:**
> "Create a new bug in workspace 'Mobile App V2' titled 'App crashes on splash screen'."

**🤖 AI Agent:**
> Done! I've created a new bug report 'App crashes on splash screen' in the 'Mobile App V2' workspace. I've assigned it a high priority by default. Would you like to add reproduction steps?

---

**👤 You:**
> "Show me the iterations for project 'Cloud Infrastructure'."

**🤖 AI Agent:**
> I've listed the iterations for 'Cloud Infrastructure'. You have 3 iterations defined, including 'Q2 Milestone' (In Progress) and 'Security Patch v1.1' (Planned). Which one would you like to audit?


## Installation & Usage

To install and use the **TAPD** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tapd](https://vinkius.com/mcp/tapd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
