# Towio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/towio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/towio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/towio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Coordinate towing and roadside assistance operations with dispatch management, GPS tracking, and job status updates.

## Description
Connect your **Towio** craft and construction account to any AI agent and simplify how you coordinate project tasks, manage your workforce, and track delivery documentation through natural conversation.

### What you can do

- **Project Oversight** — List all active construction or craft projects and retrieve detailed metadata.
- **Task Management** — Create and list tasks and to-dos to keep your job sites on schedule.
- **Workforce Coordination** — Query employee lists and staff details to manage your field team effectively.
- **Logistics & Delivery** — List and monitor delivery notes and associated documents to ensure material flow.
- **Connectivity Check** — Verify API connectivity and retrieve the current system version directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Towio API Token (found in your workspace settings)
3. Start managing your projects from Claude, Cursor, or any MCP client

### Who is this for?

- **Project Managers & Site Supervisors** — quickly check task lists and project statuses via simple AI queries.
- **Operations Managers** — coordinate employee availability and verify delivery documents directly from the workspace.
- **Business Owners** — get instant bird's-eye views of active craft projects and team structure via the AI assistant.


## Available Tools
- **list_projects**: List towio projects
- **list_tasks**: List all tasks in towio
- **create_task**: Create a new task
- **get_api_version**: Check towio API version and connectivity
- **list_delivery_documents**: List delivery documents
- **list_employees**: List company employees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Towio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my Towio workspace."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active construction sites: 'Central Park Renovations', 'Skyline Tower B', and 'Riverside Craft'. Which one would you like to check tasks for?

---

**👤 You:**
> "Show me the task list for the 'Skyline Tower B' project."

**🤖 AI Agent:**
> I've fetched the tasks. There are 5 pending items including 'Plumbing Inspection', 'Material Delivery Check', and 'Electrical Wiring'. Shall I add a new task to this list?

---

**👤 You:**
> "Create a task: 'Order 50 bags of cement' for project '88231'."

**🤖 AI Agent:**
> Success! The task 'Order 50 bags of cement' has been created for project 88231. I've logged it in your towio workspace. Would you like to assign an employee to it?


## Installation & Usage

To install and use the **Towio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/towio](https://vinkius.com/mcp/towio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
