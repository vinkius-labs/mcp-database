# Casdoor (IAM) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/casdoor-iam)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/casdoor-iam-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/casdoor-iam-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage identity and access control via Casdoor — list users, manage organizations, and configure applications directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Casdoor (IAM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations in my Casdoor instance."

**🤖 AI Agent:**
> I've retrieved the organizations. You currently have: 'built-in', 'marketing-dept', and 'engineering-team'. Would you like to see the users for any of these?

---

**👤 You:**
> "Get the profile for user 'built-in/admin'."

**🤖 AI Agent:**
> Fetching details for 'built-in/admin'... The user is active, with the display name 'System Administrator' and email 'admin@example.com'.

---

**👤 You:**
> "Add a new user named 'dev_user' to the 'engineering' organization."

**🤖 AI Agent:**
> I have successfully created the user 'dev_user' in the 'engineering' organization. Would you like to set an email or display name for this user?


## Installation & Usage

To install and use the **Casdoor (IAM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/casdoor-iam](https://vinkius.com/mcp/casdoor-iam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
