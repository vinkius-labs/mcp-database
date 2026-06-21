# Lunatask MCP Server

Manage tasks, habits, and notes via the Lunatask REST API (Encrypted Metadata Only).

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lunatask)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect your **Lunatask** account to any AI agent to streamline your privacy-focused productivity. This MCP server enables your agent to create, update, and manage tasks, track habits, and log journal entries directly from natural language interfaces.

### What you can do

- **Task Creation** — Add new tasks to specific Areas of Life with statuses like 'next' or 'later'
- **Habit Tracking** — Log completions for your daily habits to stay consistent with your goals
- **Encrypted Journaling** — Create secure, end-to-end encrypted journal entries directly from your conversation
- **Metadata Inspection** — List all tasks and notes to monitor your productivity structure and statuses
- **Workflow Management** — Update task priorities and move them through your personal workflow stages

### Important Note on Privacy

Lunatask uses end-to-end encryption. While this API allows creating and updating content, **it cannot read back the names or notes** of your tasks once they are stored. The agent will only see technical metadata (IDs, dates, statuses).

### How it works

1. Subscribe to this server
2. Enter your Lunatask Access Token
3. Start managing your productivity from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Privacy-Conscious Professionals** — Manage your tasks via AI without compromising the encryption of your content
- **Goal-Oriented Individuals** — Quickly track habits and log journal thoughts via natural language commands
- **Power Users** — Automate task creation and organizational metadata updates directly from your development tools


## Available Tools
- **create_journal_entry**: Add a new journal entry
- **create_new_task**: Requires a name and an area_id.

Create a new task
- **delete_task**: Delete a task
- **get_task_metadata**: Get metadata for a specific task
- **list_notes_metadata**: List metadata for all notes
- **list_tasks_metadata**: Note: Due to encryption, names and notes are not available via API.

List metadata for all tasks
- **track_habit_completion**: Log a completion for a habit
- **update_existing_task**: Update an existing task


## Installation & Usage

To install and use the **Lunatask** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lunatask](https://vinkius.com/mcp/lunatask)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
