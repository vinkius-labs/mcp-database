# Xata MCP Server

Automate your serverless database workflows with Xata — manage organizations, projects, and branches directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/xata)

## Overview
**Category:** databases
**Tools Count:** 28

## Description
Connect your **Xata** account to any AI agent to manage your serverless data infrastructure through natural conversation.

### What you can do

- **Organization Management** — List, create, and update organizations, and manage member invitations and roles.
- **Project Control** — Create and list projects within your organizations and monitor resource limits and quotas.
- **Database Operations** — Manage branches, retrieve credentials, and execute SQL queries directly against your data.
- **Developer Workflow** — Handle API keys and GitHub integrations to streamline your deployment pipeline and repository mapping.

### How it works

1. Subscribe to this server
2. Enter your Xata API Key
3. Start managing your databases from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — quickly spin up projects and branches without leaving the terminal or IDE.
- **Data Engineers** — query data and inspect organization structures via SQL directly through the agent.
- **DevOps Managers** — automate member access, invite collaborators, and manage API key rotations.


## Available Tools
- **cancel_organization_invitation**: Cancel a pending organization invitation
- **create_branch**: Create a new database branch
- **create_org_api_key**: Create an API key for the organization
- **create_organization**: Create a new Xata organization
- **create_project**: Create a new project in an organization
- **create_user_api_key**: Create a new user API key
- **delete_user_api_keys**: Bulk delete user API keys by ID
- **execute_sql**: Execute single or batch SQL queries over HTTP
- **get_branch_credentials**: Retrieve database username and password for a branch
- **get_branch_metrics**: Query observability data (CPU, Memory, Disk, etc.) for a branch
- **get_github_repository_mapping**: Retrieve the current GitHub repository mapping for a branch
- **get_organization**: Get detailed information about a specific organization
- **get_project_limits**: Get resource limits for projects in an organization
- **install_github_app**: Link a GitHub App installation to an organization
- **invite_organization_member**: Invite a user to an organization via email
- **list_branches**: List all branches in a project
- **list_images**: List available PostgreSQL versions/images
- **list_org_api_keys**: List organization-scoped API keys
- **list_organization_invitations**: List pending or expired invitations for an organization
- **list_organization_members**: List members of an organization
- **list_organizations**: List all organizations the authenticated user belongs to
- **list_projects**: List all projects within an organization
- **list_regions**: List available regions for project deployment
- **list_user_api_keys**: List API keys for the authenticated user
- **map_github_repository**: Map a GitHub repository to a branch
- **remove_organization_member**: Remove a member from an organization
- **rotate_branch_credentials**: Trigger a password rotation for a branch
- **update_organization**: Update organization information


## Installation & Usage

To install and use the **Xata** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xata](https://vinkius.com/mcp/xata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
