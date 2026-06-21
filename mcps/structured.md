# Structured MCP Server

Connect your AI to Structured. Programmatically manage your daily planner, tasks, and routines seamlessly directly from your terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/structured)

## Overview
**Category:** productivity
**Tools Count:** 9

## Description
Integrate the powerful tracking of the **Structured** daily planner directly into your conversational AI environment. Empower your productivity by allowing your LLM to intuitively create tasks, schedule complex recurring routines, and manage your day programmatically without opening the mobile app. With this MCP connector securely attached to your Structured Pro environment, your agent can serve as an active scheduling assistant, iterating dynamically through your agenda, parsing task structures, and executing adjustments organically.

### What you can do

- **Agenda Discovery** — Audit your scheduled events querying active records using `list_tasks` and retrieve deep metadata specific assignments utilizing `get_task_details`.
- **Task Orchestration** — Drive agile agenda resolutions adding new items seamlessly executing `create_task` or adjusting timelines using `update_task`.
- **Routine Management** — Check your active multi-step routines effectively through `list_plans` and isolate their specific structural constraints engaging `get_plan_details`.
- **Profile Validations** — Safely extract your user metadata boundaries and operational statuses natively invoking `get_user_profile`.

### How it works

1. Enable the Structured MCP module configuring it logically as an active integration.
2. In the parameter matrix, bind your official `STRUCTURED_TOKEN` (provided effectively via Structured Pro settings).
3. State your objective: "Assess my planned tasks for today, generate a new activity block for 'System Architecture Review', and organize it dynamically."

### Who is this for?

- **Founders & Executives** — Manage aggressive schedules completely iteratively without breaking focus, simply dictating adjustments naturally via your AI agent.
- **Independent Creators** — Monitor creative blocks, formulate specific routines, and execute tasks dynamically interacting transparently with your daily tracking tool.
- **Software Engineers** — Bind your daily agenda directly into your IDE conversational AI securely tracking progress locally.


## Available Tools
- **list_plans**: Lists all structured plans
- **get_plan_details**: Retrieves details for a specific plan
- **create_plan**: Creates a new plan
- **get_user_profile**: Retrieves the current user profile
- **list_tasks**: Lists all tasks in Structured
- **get_task_details**: Retrieves details for a specific task
- **create_task**: Provide a title and optional start time.

Creates a new task in Structured
- **update_task**: Updates an existing task
- **delete_task**: This action is irreversible.

Permanently deletes a task


## Installation & Usage

To install and use the **Structured** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/structured](https://vinkius.com/mcp/structured)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
