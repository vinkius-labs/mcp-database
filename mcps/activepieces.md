# Activepieces MCP Server

Automate workflows with Activepieces — manage flows, monitor executions, and handle app connections directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/activepieces)

## Overview
**Category:** productivity
**Tools Count:** 32

## Description
Connect your **Activepieces** account to any AI agent to orchestrate complex automations and monitor your business workflows through natural language.

### What you can do

- **Flow Management** — List, create, retrieve, and delete automation flows within your projects using `list_flows` and `create_flow`.
- **Execution Monitoring** — Track flow runs, check statuses, and inspect detailed step results for debugging with `list_flow_runs` and `get_flow_run`.
- **App Connections** — Manage credentials and connections for external services like Slack, Discord, or Google Sheets via `list_app_connections`.
- **Flow Operations** — Apply structural changes or status updates to existing flows programmatically using `apply_flow_operation`.
- **Organization** — List and manage folders to keep your automation workspace tidy with `list_folders`.

### How it works

1. Subscribe to this server
2. Enter your Activepieces API Key
3. Start orchestrating your automations from Claude, Cursor, or any MCP-compatible client

No more manual checking of execution logs or switching tabs to enable/disable flows. Your AI acts as a dedicated automation engineer.

### Who is this for?

- **DevOps & Automation Engineers** — monitor flow health and trigger updates directly from the terminal or chat.
- **Product Operations** — manage app connections and verify data consistency across automated workflows.
- **Marketing Teams** — check the status of lead-gen flows and ensure integrations are running smoothly.


## Available Tools
- **add_piece**: Add a custom piece to the platform
- **delete_app_connection**: Delete an app connection
- **delete_flow**: Delete a flow by ID
- **list_flow_runs**: List flow runs
- **update_folder**: Update a folder name
- **apply_flow_operation**: g., MOVE_ACTION, CHANGE_STATUS).

Apply an operation to a flow
- **configure_git_repo**: Configure Git sync for a project
- **create_flow**: Create a new flow
- **create_folder**: Create a new folder
- **upsert_app_connection**: Supports SECRET_TEXT, OAUTH2, BASIC_AUTH, CUSTOM_AUTH, etc.

Create or update an app connection
- **upsert_global_connection**: Create or update a global connection
- **create_project_release**: Create a project release
- **create_project**: Create a new project
- **delete_folder**: Delete a folder
- **delete_global_connection**: Delete a global connection
- **delete_project_member**: Remove a member from a project
- **get_flow_run**: Get detailed execution data for a flow run
- **get_flow**: Get a specific flow by ID
- **get_mcp_server**: Get MCP server configuration for AI assistants
- **invite_user**: Invite a user to the platform or project
- **list_app_connections**: List app connections
- **list_flows**: List automation flows
- **list_folders**: List folders
- **list_global_connections**: List global connections
- **list_project_members**: List members of a project
- **list_projects**: List projects
- **list_records**: List records in a table
- **list_tables**: List internal data tables
- **list_users**: List users
- **rotate_mcp_token**: Rotate MCP token for a project
- **update_project**: Update project settings
- **update_record**: Update a specific record


## Installation & Usage

To install and use the **Activepieces** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/activepieces](https://vinkius.com/mcp/activepieces)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
