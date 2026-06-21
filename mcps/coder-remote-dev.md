# Coder (Remote Dev) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coder-remote-dev)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Coder remote development environments, monitor deployment stats, and interact with AI Bridge sessions directly from your AI agent.

## Description
Connect your **Coder** deployment to any AI agent to orchestrate remote development infrastructure and monitor workspace health through natural language.

### What you can do

- **Deployment Monitoring** — Retrieve build info, deployment statistics, and check for available updates to keep your infrastructure current.
- **AI Bridge Management** — List connected AI clients, available models, and active sessions to understand how AI is being utilized in your workspaces.
- **Agent Operations** — Stream logs from specific workspace agents and manage application statuses to troubleshoot remote environments instantly.
- **Infrastructure Config** — Access SSH configurations and deployment settings to ensure seamless connectivity for your engineering team.
- **Session Insights** — Fetch threads and interceptions from AI sessions to audit and optimize AI-assisted development workflows.

### How it works

1. Subscribe to this server
2. Enter your Coder URL and Session Token
3. Start managing your remote dev clusters from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — monitor deployment health and configuration without leaving the terminal or chat interface.
- **Platform Teams** — manage AI Bridge sessions and model availability across the organization's remote workspaces.
- **Software Developers** — quickly retrieve SSH configs and agent logs to debug environment issues without context switching.


## Available Tools
- **get_agent_debug_magicsock**: Get Tailscale magicsock debug info (local agent API)
- **get_agent_debug_manifest**: Get the startup manifest from the server (local agent API)
- **get_agent_external_auth**: Get external authentication tokens for the agent
- **get_agent_logs**: Stream logs from a specific agent
- **get_ai_session_threads**: Get threads for an AI session
- **get_api_root**: Get basic API information
- **get_app_auth_redirect**: Redirect to a URI with an encrypted API key
- **get_app_host**: Get the base host for applications
- **get_appearance**: Get dashboard branding and banners
- **get_audit_logs**: Get a paginated list of audit logs
- **get_build_info**: Get Coder build info
- **get_chat_messages**: Get messages for a chat session
- **get_deployment_config**: Get deployment configuration
- **get_deployment_stats**: Get deployment statistics
- **get_external_auth_device**: Initiate device-based OAuth
- **get_insights_daus**: Get Daily Active User stats
- **get_insights_templates**: Get usage data for templates
- **get_insights_user_activity**: Get activity duration per user
- **get_notifications_inbox**: List user notifications
- **get_notifications_settings**: Get global notification settings
- **get_notifications_templates**: List available notification templates
- **get_prebuild_settings**: Get prebuild settings
- **get_ssh_config**: Get SSH configuration
- **get_update_check**: Check for Coder updates
- **get_user_profile**: Get user profile
- **get_workspace_acl**: Get workspace ACLs
- **get_workspace_build_logs**: Get logs for a specific build
- **get_workspace_build_params**: List parameters used for the build
- **get_workspace_build**: Get details of a specific build
- **get_workspace**: Get workspace metadata
- **list_ai_clients**: List connected AI Bridge clients
- **list_ai_interceptions**: List AI interceptions
- **list_ai_models**: List available AI models
- **list_ai_sessions**: List active AI Bridge sessions
- **list_chats**: List user chat sessions
- **list_external_auth**: List linked external accounts (e.g., GitHub)
- **list_groups**: List groups
- **list_licenses**: List enterprise licenses
- **list_org_members**: List members of an organization
- **list_org_provisioner_daemons**: List active provisioner daemons
- **list_org_provisioner_jobs**: List jobs for the organization provisioners
- **list_org_roles**: List assignable roles in an organization
- **list_organizations**: List organizations
- **list_tasks**: Manage long-running AI tasks
- **list_template_examples**: List starter template examples
- **list_template_versions**: List versions for a template
- **list_templates**: List all templates
- **list_user_secrets**: List user secrets
- **list_user_tokens**: List user tokens
- **list_users**: List users
- **list_workspace_port_shares**: List port shares for a workspace
- **list_workspaces**: g., owner:me).

List workspaces
- **login_user**: Authenticate a user with email and password
- **register_agent_log_source**: Register a new log source
- **send_agent_logs**: Send logs to the server
- **update_agent_app_status**: Update status of an application running on the agent
- **update_appearance**: Update dashboard branding and banners
- **update_organization**: Update an organization
- **update_prebuild_settings**: Update prebuild settings
- **update_user_profile**: Update user profile
- **update_workspace_acl**: Update workspace ACLs
- **update_workspace_autostart**: Update workspace autostart schedule
- **update_workspace_autoupdates**: Update workspace autoupdates schedule
- **upload_file**: Upload a file (tar or zip)
- **add_license**: Add an enterprise license
- **auth_workspace_agent**: Authenticate agent using cloud provider identity
- **cancel_workspace_build**: Cancel a pending or running build
- **check_auth**: Check if user has permission to perform actions
- **create_chat_message**: Send a message to a chat session
- **create_chat**: Start a new AI chat session
- **create_group**: Create a group in an organization
- **create_organization**: Create an organization
- **create_user_secret**: Create a user secret
- **create_user_task**: Create a long-running AI task for a user
- **create_user_token**: Create a user token
- **create_user**: Create a user
- **create_workspace_port_share**: Create a port share for a workspace
- **create_workspace**: Create a workspace
- **delete_license**: Delete an enterprise license
- **delete_user**: Delete a user
- **download_file**: Download a file by ID
- **get_agent_connection**: Get DERP and connection details for an agent
- **get_agent_containers**: List running containers and devcontainers
- **get_agent_debug_logs**: Get the last 10MiB of agent logs (local agent API)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coder (Remote Dev)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current Coder deployment statistics and build info."

**🤖 AI Agent:**
> I've retrieved the deployment data. You have 12 active workspaces and 8 active sessions. The current build version is v2.10.2. Would you like to check for updates?

---

**👤 You:**
> "List all active AI Bridge sessions and their available models."

**🤖 AI Agent:**
> Found 3 active AI sessions. Available models include GPT-4o, Claude 3.5 Sonnet, and Llama 3. Would you like to see the thread history for a specific session?

---

**👤 You:**
> "Get the SSH configuration for my Coder instance."

**🤖 AI Agent:**
> I've fetched the SSH config. The hostname prefix is 'coder.' and the suffix is '.dev'. You can use these to configure your local SSH client for workspace access.


## ❓ FAQ

**Q: Can I check the health and usage of my Coder deployment?**
Yes. Use the `get_deployment_stats` tool to retrieve workspace and session statistics, providing a clear overview of your infrastructure's current state.

**Q: How do I see which AI models are available in my Coder instance?**
Simply run the `list_ai_models` tool. It will return a list of all AI models currently configured and available through the Coder AI Bridge.

**Q: Can I view logs for a specific workspace agent to debug issues?**
Yes! Use the `get_agent_logs` tool with the target `agent_id`. This allows you to stream and inspect logs directly from the remote environment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coder-remote-dev](https://vinkius.com/mcp/coder-remote-dev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coder (Remote Dev)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `coder-remote-dev` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coder (Remote Dev)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coder-remote-dev": {
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
