# Casdoor (IAM) MCP Server

Manage identity and access control via Casdoor — list users, manage organizations, and configure applications directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/casdoor-iam)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Casdoor** IAM instance to any AI agent to streamline your identity and access management workflows through natural conversation.

### What you can do

- **User Management** — Create, update, delete, and retrieve detailed profiles for users across your organizations using the `add_user`, `update_user`, and `delete_user` tools.
- **Organization Oversight** — List all organizations and fetch specific configuration details for your IAM hierarchy with `list_organizations` and `get_organization`.
- **Application Control** — Query and manage applications registered within your Casdoor instance using `list_applications` and `get_application`.
- **Identity Inspection** — Instantly retrieve the profile of the currently authenticated user to verify permissions via `get_userinfo`.

### How it works

1. Subscribe to this server
2. Enter your Casdoor Endpoint, Client ID, and Client Secret
3. Start managing your identity infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — Automate user provisioning and organization audits without leaving the terminal or IDE.
- **Security Teams** — Quickly inspect user permissions and application configurations for compliance and security reviews.
- **Full-stack Developers** — Manage test users and application settings directly while coding to maintain development flow.


## Available Tools
- **add_user**: Requires owner (organization) and name (username).

Add a new user
- **delete_user**: Requires the owner (organization) and name (username) of the user to delete.

Delete a user
- **get_application**: Get a specific application
- **get_organization**: Get a specific organization
- **get_user**: Get a specific user by ID
- **list_applications**: List applications in an organization
- **list_organizations**: List all organizations
- **list_users**: List users in an organization
- **update_user**: The ID parameter must be formatted as <organization>/<username>.

Update an existing user
- **get_userinfo**: Get the profile of the authenticated user


## Installation & Usage

To install and use the **Casdoor (IAM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/casdoor-iam](https://vinkius.com/mcp/casdoor-iam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
