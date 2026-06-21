# Sunsama MCP Server

Connect your AI to Sunsama. Actively manage your day, orchestrate tasks, and balance your work natively from the terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sunsama)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Integrate the mindful focus of the **Sunsama** daily planner directly into your conversational AI environment. Empower your engineering or administrative focus by allowing your LLM to intuitively pull tasks, filter backlog activities, and assign contexts dynamically without constant tab-switching. With this MCP connector attached securely to your workspace, your conversational agent functions as an objective scheduling assistant, seamlessly tracking and resolving your agenda.

### What you can do

- **Agenda Discovery** — Query your scheduled events actively using `list_tasks` and retrieve deep contextual dependencies of an item utilizing `get_task_details`.
- **Task Orchestration** — Add new action items seamlessly via `create_task` or modify ongoing assignments intuitively using `update_task`.
- **Taxonomy Mapping** — Review your organizational frameworks executing `list_channels` and `list_contexts` to accurately file items according to team domains.
- **Profile Confirmations** — Safely extract your user metadata boundaries and operational statuses natively invoking `get_user_profile`.

### How it works

1. Enable the Sunsama MCP module orchestrator as an active system integration.
2. Bind your verified `SUNSAMA_API_KEY` directly from your workspace parameters precisely to your environment matrix.
3. Instruct your artificial intelligence concisely: "Analyze my pending tasks for today, generate a new assigned block under the 'Development' channel, and mark yesterday's review as completed."

### Who is this for?

- **Founders & Executives** — Mitigate schedule conflicts iteratively without breaking focus, directing agenda adjustments via an analytical AI agent.
- **Software Engineers** — Centralize your daily planned agenda cleanly inside your IDE or local conversational CLI, reporting progress directly in real-time.
- **Project Managers** — Consolidate activities safely tracking team deliverables and personal timelines without bloated secondary interfaces.


## Available Tools
- **list_tasks**: You can filter by date.

Lists all tasks in Sunsama
- **create_task**: Provide text and an optional planned date.

Creates a new task in Sunsama
- **delete_task**: This action is irreversible.

Permanently deletes a task
- **get_user_profile**: Retrieves the current user profile
- **get_task_details**: Retrieves details for a specific task
- **list_channels**: g., "Work", "Personal").

Lists available Sunsama channels
- **list_contexts**: Lists available Sunsama contexts
- **update_task**: Updates an existing task


## Installation & Usage

To install and use the **Sunsama** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sunsama](https://vinkius.com/mcp/sunsama)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
