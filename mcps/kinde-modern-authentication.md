# Kinde (Modern Authentication) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kinde-modern-authentication)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kinde-modern-authentication-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kinde-modern-authentication-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage users, organizations, roles, and permissions in Kinde directly from your AI agent.

## Description
Connect your **Kinde** authentication environment to any AI agent to streamline identity management and access control through natural conversation.

### What you can do

- **User Management** — List all users, create new accounts, retrieve specific profiles, and update user information seamlessly using `list_users`, `create_user`, `get_user`, and `update_user`.
- **Organization Control** — List and create organizations to manage multi-tenant environments with `list_organizations` and `create_organization`.
- **RBAC & Permissions** — Audit available roles and permissions within your Kinde project to ensure proper access control using `list_roles` and `list_permissions`.

### How it works

1. Subscribe to this server
2. Enter your Kinde Domain and Access Token
3. Start managing your auth workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — quickly check user IDs or update test accounts without leaving the IDE
- **Support Teams** — look up user details and organization memberships to troubleshoot access issues
- **DevOps Engineers** — automate the provisioning of organizations and roles through simple prompts


## Available Tools
- **create_organization**: Create a new organization
- **create_user**: Provide user details in the data payload.

Create a new user in Kinde
- **get_user**: Retrieve user details
- **list_organizations**: List organizations in Kinde
- **list_permissions**: List available permissions
- **list_roles**: List available roles
- **list_users**: List users in Kinde
- **update_user**: Provide the user ID and the fields to update in the data payload.

Update user information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kinde (Modern Authentication)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in my Kinde environment."

**🤖 AI Agent:**
> I've retrieved the user list. You have 15 active users. Notable entries include 'John Doe' (ID: kp_123) and 'Jane Smith' (ID: kp_456). Would you like details on a specific user?

---

**👤 You:**
> "Show me all organizations configured in Kinde."

**🤖 AI Agent:**
> Fetching organizations... I found 3 organizations: 'Acme Corp' (org_1), 'Globex' (org_2), and 'Soylent Corp' (org_3).

---

**👤 You:**
> "Get the details for user ID kp_987654321."

**🤖 AI Agent:**
> Inspecting user kp_987654321... This is 'Alice Wonderland'. Email: alice@example.com. Status: Active. Last login: 2 hours ago.


## Installation & Usage

To install and use the **Kinde (Modern Authentication)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kinde-modern-authentication](https://vinkius.com/mcp/kinde-modern-authentication)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
