# Activepieces MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/activepieces)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate workflows with Activepieces — manage flows, monitor executions, and handle app connections directly from your AI agent.

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


## Available Tools (32)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Activepieces** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active automation flows in project 'proj_123'."

**🤖 AI Agent:**
> I've found 3 flows in project 'proj_123': 'Slack Notification' (ID: flow_1), 'Email Sync' (ID: flow_2), and 'Lead Router' (ID: flow_3).

---

**👤 You:**
> "Show me the last 5 runs for flow ID 'flow_1'."

**🤖 AI Agent:**
> Retrieving runs for flow_1... I found 5 recent executions. 4 succeeded and 1 failed with a timeout error. Would you like to inspect the failed run details?

---

**👤 You:**
> "Create a new flow named 'Customer Support Sync' in project 'proj_123'."

**🤖 AI Agent:**
> Flow 'Customer Support Sync' has been created successfully in project 'proj_123' with ID 'flow_new_99'. You can now start adding steps to it.


## ❓ FAQ

**Q: Can I check why a specific flow execution failed?**
Yes. Use the `get_flow_run` tool with the Run ID to retrieve detailed execution data, including step results and error messages.

**Q: How do I update the status of an existing flow?**
You can use the `apply_flow_operation` tool. It allows you to send an operation payload to change the flow's status or modify its structure.

**Q: Can I see which external apps are connected to my project?**
Yes, the `list_app_connections` tool retrieves all credentials and connections configured for a specific Project ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/activepieces](https://vinkius.com/mcp/activepieces)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Activepieces** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `activepieces` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Activepieces** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "activepieces": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
