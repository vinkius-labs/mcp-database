# Monday.com MCP Server

Manage any workflow visually with customizable boards, automations, and dashboards that adapt to how your team actually works.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mondaycom)

## Overview
**Category:** industry-titans
**Tools Count:** 12

## Description
Connect your **Monday.com** account to any AI agent and take full control of your team's Work OS through natural conversation. Monday.com provides a flexible and powerful platform for managing complex projects, and this integration allows you to retrieve board metadata, create automated task assignments, and monitor real-time team updates directly from your chat interface.

### What you can do

- **Board & Project Orchestration** — List all managed projects and retrieve detailed column and group metadata programmatically to ensure your team's roadmap is always synchronized.
- **Item Lifecycle Management** — Create, update, and delete board items (tasks) directly from the AI interface to maintain high-fidelity workflow automation.
- **Communication & Update Control** — List and create updates (comments) on specific items via natural language to drive better team alignment and project transparency.
- **User & Workspace Intelligence** — Access platform metadata including user profiles and workspace configurations using simple AI commands.
- **Operational Monitoring** — Track system responses and manage board structures to ensure your team's execution is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Monday.com API Token from your developer settings
3. Start managing your Work OS from Claude, Cursor, or any MCP-compatible client

No more manual logging into the dashboard to check task status or project progress. Your AI acts as a dedicated project coordinator or operations assistant.

### Who is this for?

- **Project Managers & Team Leads** — quickly retrieve project summaries and monitor task health without switching apps.
- **Operations Teams** — automate the creation of tasks and track team capacity via natural conversation.
- **Developers** — integrate real-time project data and board metadata directly within the chat.


## Available Tools
- **create_new_item**: Optional column values must be JSON.

Add row to board
- **post_item_update**: Add comment to row
- **remove_item**: Delete row
- **get_board_schema**: Get board columns
- **get_my_profile**: com user.

Get user info
- **list_boards**: List Monday.com boards
- **list_board_groups**: List board sections
- **list_board_items**: Get board rows
- **list_item_updates**: Get row comments
- **list_account_users**: com account.

List team members
- **list_workspaces**: List project containers
- **update_item_columns**: Modify row values


## Installation & Usage

To install and use the **Monday.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mondaycom](https://vinkius.com/mcp/mondaycom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
