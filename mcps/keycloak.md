# Keycloak MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keycloak)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/keycloak-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/keycloak-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage identity and access control — list realms, manage users, configure clients, and handle security roles directly from your AI agent.

## Description
Connect your **Keycloak** instance to any AI agent to streamline your Identity and Access Management (IAM) workflows. This server provides comprehensive tools to audit, configure, and maintain your security infrastructure through natural language.

### What you can do

- **Realm Administration** — List, import, and export realms, or monitor admin events to audit changes across your infrastructure.
- **User Management** — Create, update, or delete users, reset passwords, and inspect user group memberships without leaving your chat interface.
- **Client Configuration** — Manage OIDC/SAML clients, retrieve client secrets, and regenerate credentials instantly.
- **Groups & Roles** — Organize your security hierarchy by managing groups and assigning roles at both realm and client levels.
- **Session Control** — Force global logouts across entire realms to mitigate security threats in real-time.

### How it works

1. Subscribe to this server
2. Provide your Keycloak Base URL and a valid Admin Access Token
3. Start managing your IAM infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps & SREs** — Quickly audit realm events and manage client configurations during deployments.
- **Security Administrators** — Perform emergency password resets or session terminations via simple commands.
- **Backend Developers** — Setup test users and retrieve client credentials directly within the IDE flow.


## Available Tools
- **create_auth_flow**: Create an authentication flow
- **create_client**: Create a new client
- **create_group**: Create a top-level group
- **create_role**: Create a realm-level role
- **create_user**: Create a new user
- **delete_client**: Delete a client
- **delete_group**: Delete a group
- **delete_realm**: Delete a realm
- **delete_user**: Delete a user
- **get_client_secret**: Get client secret
- **get_client**: Get client representation
- **get_group**: Get group representation
- **get_realm**: Get realm representation
- **get_role**: Get a role by name
- **get_user**: Get user representation
- **import_realm**: Import a realm
- **list_admin_events**: Get admin events for a realm
- **list_auth_flows**: Get authentication flows
- **list_client_roles**: Get client-level roles
- **list_clients**: Get all clients in the realm
- **list_groups**: Get group hierarchy
- **list_realms**: Get accessible realms
- **list_required_actions**: Get required actions
- **list_roles**: Get realm-level roles
- **list_user_groups**: Get user groups
- **list_users**: Get users in a realm
- **logout_all_users**: Remove all user sessions in a realm
- **partial_export_realm**: Partial export of a realm
- **regenerate_client_secret**: Regenerate client secret
- **reset_user_password**: Reset user password
- **update_client**: Update a client
- **update_group**: Update a group
- **update_realm**: Update realm information
- **update_user**: Update a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keycloak** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all realms available in our Keycloak instance."

**🤖 AI Agent:**
> I've retrieved the realms. You have 3 active realms: 'master', 'production-apps', and 'staging-environment'.

---

**👤 You:**
> "Get the details for user ID '550e8400-e29b' in the 'production-apps' realm."

**🤖 AI Agent:**
> Fetching user data... User 'john.doe' found. Email: john@example.com, Status: Enabled, Created: 2023-10-12.

---

**👤 You:**
> "Create a new group called 'Engineering-Leads' in the 'master' realm."

**🤖 AI Agent:**
> Group 'Engineering-Leads' has been successfully created in the 'master' realm.


## Installation & Usage

To install and use the **Keycloak** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keycloak](https://vinkius.com/mcp/keycloak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
