# AppVeyor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appveyor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/appveyor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/appveyor-mcp)
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


## Available Tools
- **add_collaborator**: Add a new collaborator
- **add_project**: Add a new project
- **add_role**: Add a new role
- **add_user**: Add a new user
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


## Installation & Usage

To install and use the **AppVeyor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appveyor](https://vinkius.com/mcp/appveyor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
