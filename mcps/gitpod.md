# Gitpod MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitpod)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Automate cloud development environments — create, start, and manage Gitpod workspaces and organizations directly from any AI agent.

## Description
Connect your **Gitpod** account to any AI agent to orchestrate your cloud development lifecycle through natural language.

### What you can do

- **Workspace Lifecycle** — Create, start, stop, and delete workspaces using repository URLs or specific context IDs.
- **Organization Management** — List, create, and inspect organizations and their members to manage team access.
- **Configuration & Env Vars** — Manage workspace configurations and environment variables for consistent development setups.
- **Audit & Sessions** — Track workspace sessions and audit logs to monitor activity within your organizations.

### How it works

1. Subscribe to this server
2. Enter your Gitpod Personal Access Token
3. Start managing your cloud IDEs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Spin up fresh dev environments for PRs or issues without leaving the chat or editor.
- **DevOps Engineers** — Automate organization settings and environment variable management across teams.
- **Engineering Leads** — Monitor workspace usage and audit logs to maintain security and cost efficiency.


## Available Tools
- **create_and_start_workspace**: Create and start a new Gitpod workspace
- **create_configuration**: Create a new repository configuration in Gitpod
- **create_environment_variable**: Create an environment variable for a repository configuration
- **create_organization**: Create a new Gitpod organization
- **delete_configuration**: Delete a repository configuration
- **delete_environment_variable**: Delete an environment variable
- **remove_organization_member**: Remove a member from a Gitpod organization
- **delete_organization**: Delete a Gitpod organization
- **delete_workspace**: Delete a Gitpod workspace
- **get_configuration**: Get details for a specific repository configuration
- **get_organization_settings**: Get settings for a Gitpod organization
- **get_organization**: Get details for a specific Gitpod organization
- **get_workspace**: Get details for a specific Gitpod workspace
- **join_organization**: Join a Gitpod organization using an invitation ID
- **list_audit_logs**: List audit logs for an organization (Enterprise Only)
- **list_configurations**: List repository configurations in an organization
- **list_environment_variables**: List environment variables for a repository configuration
- **list_organization_members**: List members of a Gitpod organization
- **list_organizations**: List all Gitpod organizations for the authenticated user
- **list_workspace_sessions**: List workspace sessions (start/stop events) in an organization
- **list_workspaces**: List workspaces in an organization
- **start_workspace**: Start an existing Gitpod workspace
- **stop_workspace**: Stop a running Gitpod workspace
- **update_configuration**: Update a repository configuration
- **update_organization_member**: Update a member role in a Gitpod organization
- **update_organization_settings**: Update settings for a Gitpod organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gitpod** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Gitpod organizations."

**🤖 AI Agent:**
> I've found 2 organizations: 'Engineering-Team' (ID: org_123) and 'Open-Source-Projects' (ID: org_456). Which one would you like to explore?

---

**👤 You:**
> "Create and start a workspace for https://github.com/gitpod-io/gitpod."

**🤖 AI Agent:**
> Starting the `create_and_start_workspace` action... I've successfully triggered a new workspace for that repository. You can now access your cloud IDE.

---

**👤 You:**
> "Stop the workspace with ID 'ws-abc-123'."

**🤖 AI Agent:**
> I am stopping the workspace 'ws-abc-123' now. The environment will be hibernated to save resources.


## ❓ FAQ

**Q: Can I create a workspace from a repo URL?**
Yes! Use the `create_and_start_workspace` tool with the repository URL. Your agent will provision and start a cloud environment for that specific context immediately.

**Q: How do I see who is in my organization?**
Simply ask the agent to run the `list_organization_members` action with your Organization ID. It will return a list of all users and their roles within that organization.

**Q: Can I manage environment variables for my development setups?**
Yes. You can use `create_environment_variable` to set new secrets or configs, and `list_environment_variables` to review existing ones for your workspaces.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitpod](https://vinkius.com/mcp/gitpod)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gitpod** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gitpod` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gitpod** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitpod": {
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
