# Userfront MCP Server

Manage users, multi-tenant structures, and authentication sessions directly through Userfront's identity platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/userfront)

## Overview
**Category:** developer-tools
**Tools Count:** 40

## Description
Connect your **Userfront** workspace to your AI agent to streamline identity management and user operations. This MCP server allows you to handle complex authentication workflows, tenant hierarchies, and user data through simple natural language commands.

### What you can do

- **User Lifecycle** — Create, update, delete, and invite users. Use the `create_or_update_user` tool for seamless upserts.
- **Advanced Search** — Find specific users across your tenant using the `find_users` query with custom filters.
- **Multi-Tenancy** — Manage complex organizational structures by creating and updating tenants or child tenants using `create_child_tenant`.
- **Session Monitoring** — Track active security contexts by retrieving user sessions with `get_user_sessions`.
- **Status Management** — Programmatically activate users or modify metadata to control access levels.

### How it works

1. Subscribe to this server
2. Enter your Userfront API Key
3. Start managing your identity infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & Security Engineers** — Quickly audit user sessions or manage tenant access without leaving the terminal or IDE.
- **Product Managers** — Invite new beta users or check user growth metrics through conversational queries.
- **Customer Support** — Instantly find user records, update emails, or reset statuses to resolve tickets faster.


## Available Tools
- **create_api_key**: Create a new API key
- **create_child_tenant**: Create a child tenant
- **create_custom_jwt**: Create a custom JWT access token for a user
- **create_or_update_user**: Create or update a user
- **create_role**: Create a new role
- **create_tenant_role**: Create a role (tenant level)
- **create_tenant**: Create a new tenant
- **create_user_import**: Create a user import
- **create_user**: Create a new user
- **delete_api_key**: Delete an API key
- **delete_role**: Delete a role
- **delete_tenant**: Delete a tenant and its descendants
- **delete_user_import**: Delete import record
- **delete_user**: Delete a user record
- **find_tenants**: Search tenants
- **find_users**: Uses POST /users/find.

Search users within a tenant
- **generate_link_credentials**: Generate link credentials for custom flows
- **get_jwks**: Get JSON Web Key Set (JWKS)
- **get_jwt_available_claims**: Read possible JWT claims
- **get_jwt_format**: Read JWT format
- **get_tenant**: Read a tenant record
- **get_user_import**: Check import status
- **get_user_sessions**: Read a user's sessions
- **get_user**: Read a user record
- **invalidate_api_key**: Invalidate an API key
- **invite_role**: Invite a user to a role
- **invite_user**: Invite a user by email
- **list_api_keys**: List API keys of a specific type
- **list_jwt_keys**: List JWT public keys
- **list_roles**: List all roles
- **list_tenant_roles**: List roles (tenant level)
- **logout_user**: Invalidate user sessions
- **mark_user_active**: Mark a user as active
- **process_user_import**: Start processing the import
- **set_tenant_user_roles**: Set user roles (tenant level)
- **set_user_roles**: Set roles for a user (application-wide)
- **update_jwt_format**: Create/update custom JWT format
- **update_tenant**: Update a tenant
- **update_user**: Update a user record
- **verify_api_key**: Verify an API key


## Installation & Usage

To install and use the **Userfront** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/userfront](https://vinkius.com/mcp/userfront)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
