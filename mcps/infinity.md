# Infinity MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/infinity)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/infinity-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/infinity-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize any kind of work with flexible boards, lists, and tables that adapt to how your team thinks and operates.

## Description
Connect your **Infinity** account to any AI agent and manage projects through natural conversation.

### What you can do

- **Workspace Management** — List all workspaces in your organization
- **Board Navigation** — Browse boards within workspaces and inspect their structure
- **Folder Organization** — Navigate folder hierarchies within boards
- **Attribute Schema** — View all custom attributes and fields configured on boards
- **Item Management** — List, create, update, and delete items (tasks/records) within boards
- **Data Access** — Read item field values and metadata

### How it works

1. Subscribe to this server
2. Enter your Infinity Access Token
3. Start managing projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — create tasks, update statuses, and organize boards through AI
- **Teams** — manage work items without switching to the dashboard
- **Operations** — automate task creation and tracking workflows


## Available Tools
- **check_api_health**: Verify Infinity API connectivity
- **create_board_item**: Values must map to attribute IDs.

Add a new item to a board
- **remove_board_item**: Delete an item from a board
- **get_current_user_profile**: Get authenticated user info
- **list_board_attributes**: List board attributes (fields)
- **list_workspace_boards**: List boards in a workspace
- **list_item_comments**: List comments on an item
- **list_board_folders**: List folders in a board
- **list_board_items**: Supports filtering by folder.

List all tasks/items in a board
- **list_board_webhooks**: List active webhooks for a board
- **list_workspaces**: List all workspaces
- **update_board_item**: Modify an existing item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infinity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all workspaces and the boards in the 'Product Development' workspace."

**🤖 AI Agent:**
> Workspaces: 4. Product Development, Marketing, Operations, HR. 'Product Development' boards: 1) 'Sprint Board' (42 items, 8 folders). 2) 'Bug Tracker' (23 items). 3) 'Feature Requests' (56 items). 4) 'Roadmap' (12 items). Total: 133 items across 4 boards. Would you like to see items or folders in a specific board?

---

**👤 You:**
> "Create a new task in the Sprint Board and list all items with 'In Progress' status."

**🤖 AI Agent:**
> Task created! 'Implement OAuth integration' in Sprint Board (item_4521). Assigned folder: 'Sprint 12'. Status: To Do. Priority: High. In Progress items (8): 'API rate limiting' (Sarah, 3 days), 'Dashboard redesign' (Mike, 5 days), 'Email notifications' (Lisa, 2 days), 5 others. Sprint Board: 42 → 43 items.

---

**👤 You:**
> "Show the attributes on the Bug Tracker board and the folder structure."

**🤖 AI Agent:**
> Bug Tracker attributes: 8 fields. Status (dropdown: Open, In Progress, Resolved, Closed), Priority (dropdown: Critical, High, Medium, Low), Assignee (person), Due Date (date), Component (dropdown: Frontend, Backend, API, Mobile), Steps to Reproduce (text), Screenshots (file), Resolution (text). Folders: 4. 'Frontend Bugs' (8 items), 'Backend Bugs' (6), 'API Issues' (5), 'Mobile' (4). Total: 23 bug reports.


## Installation & Usage

To install and use the **Infinity** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infinity](https://vinkius.com/mcp/infinity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
