# AppVeyor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appveyor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage CI/CD pipelines, users, roles, and collaborators on AppVeyor directly from your AI agent.

## Description
Connect your **AppVeyor** account to any AI agent to streamline your DevOps workflows and team management through natural language.

### What you can do

- **Project Overview** — List all projects in your account to monitor build statuses and configurations.
- **User Management** — List, retrieve, add, update, or delete users to maintain your team's access control.
- **Role Administration** — Manage organizational roles and permissions to ensure proper security governance.
- **Collaborator Control** — Handle external collaborators by listing, adding, or modifying their access levels.
- **Account Auditing** — Quickly query user details and role assignments without navigating the web dashboard.

### How it works

1. Subscribe to this server
2. Enter your AppVeyor API Token
3. Start managing your CI/CD environment from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate user onboarding and audit project lists directly from the terminal or IDE.
- **Team Leads** — manage permissions and roles across the organization using simple voice or text commands.
- **Security Officers** — verify collaborator access and user roles to ensure compliance with internal policies.


## Available Tools (28)
- **cancel_build**: Cancel a build
- **cancel_deployment**: Cancel a deployment
- **delete_collaborator**: Delete a collaborator
- **delete_project**: Delete a project
- **delete_role**: Delete a role
- **delete_user**: Delete a user
- **get_collaborator**: Get a specific collaborator by ID
- **get_environment_settings**: Get environment settings
- **get_project_history**: Get project history
- **get_project_last_build**: Get project last build
- **get_project_settings**: Get project settings
- **get_role**: Get a specific role by ID
- **get_user**: Get a specific user by ID
- **list_collaborators**: Get all collaborators
- **list_environments**: Get all environments
- **list_projects**: Get all projects
- **list_roles**: Get all roles
- **list_users**: Get all users
- **rerun_build**: Re-run a build
- **start_build**: Start a new build
- **start_deployment**: Start a deployment
- **update_collaborator**: Update an existing collaborator
- **update_role**: Update an existing role
- **update_user**: Update an existing user
- **add_collaborator**: Add a new collaborator
- **add_project**: Add a new project
- **add_role**: Add a new role
- **add_user**: Add a new user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AppVeyor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my AppVeyor account."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'frontend-app', 'backend-api', and 'infrastructure-deploy'. Would you like details on any of them?

---

**👤 You:**
> "Show me all users and their current roles."

**🤖 AI Agent:**
> Fetching user list... I found 5 users. Most are assigned to the 'Developer' role, while 'admin@company.com' holds the 'Administrator' role. Should I list the specific permissions for the 'Developer' role?

---

**👤 You:**
> "Get details for user with ID 98765."

**🤖 AI Agent:**
> Inspecting user 98765... This user is 'John Doe', email 'john@example.com'. They were added on 2023-10-15 and currently have 'Collaborator' status. Would you like to update their role?


## ❓ FAQ

**Q: Can I see all the projects currently configured in my AppVeyor account?**
Yes, you can use the `list_projects` tool to retrieve a complete list of all projects associated with your account.

**Q: Is it possible to manage user roles and permissions through the AI?**
Absolutely. You can use `list_roles` to see existing roles and `get_role` to inspect specific permissions, helping you audit access control easily.

**Q: Can I add new team members or collaborators using this server?**
Yes, the server includes `add_user` for internal team members and `add_collaborator` for external contributors, allowing for seamless team scaling.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appveyor](https://vinkius.com/mcp/appveyor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AppVeyor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appveyor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AppVeyor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appveyor": {
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
