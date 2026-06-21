# SuperTokens MCP Server

Manage authentication, users, sessions, and roles via SuperTokens Core directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/supertokens)

## Overview
**Category:** developer-tools
**Tools Count:** 18

## Description
Connect your **SuperTokens** Core instance to any AI agent to manage user lifecycles, session security, and Role-Based Access Control (RBAC) through natural language.

### What you can do

- **User Management** — Sign up new users, sign in existing ones, and retrieve detailed user profiles or link multiple accounts together.
- **Session Control** — Create, refresh, and revoke sessions (JWT or database-backed) to maintain tight security over user access.
- **RBAC & Permissions** — Create roles, define permissions, and assign them to users to manage authorization levels dynamically.
- **User Metadata** — Store and update custom JSON metadata for users to track preferences or application-specific data.
- **Account Linking** — Seamlessly link or unlink different recipe user IDs to a primary user identity.

### How it works

1. Subscribe to this server
2. Enter your SuperTokens Core URL and API Key
3. Start managing your authentication layer from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — quickly debug user sessions or update roles without writing manual scripts or using a CLI.
- **Support Teams** — inspect user metadata and account status to resolve login issues or permission errors instantly.
- **Security Engineers** — audit roles and revoke suspicious sessions directly through a conversational interface.


## Available Tools
- **assign_role_to_user**: Assign a role to a user
- **bulk_import_users**: Bulk import users
- **create_or_update_role**: Create or update a user role
- **create_session**: Create a new session for a user
- **create_or_update_tenant**: Create or update a tenant
- **delete_user_metadata**: Delete metadata for a user
- **get_tenant**: Get tenant details
- **get_user_metadata**: Get metadata for a user
- **get_user**: Get user details by ID
- **link_accounts**: Link two user accounts together
- **list_roles**: List all roles
- **list_user_roles**: List roles assigned to a user
- **refresh_session**: Refresh an existing session
- **remove_session**: Remove/revoke a session
- **signin_user**: Sign in a user
- **signup_user**: Sign up a new user
- **unlink_accounts**: Unlink a user account
- **update_user_metadata**: Update metadata for a user


## Installation & Usage

To install and use the **SuperTokens** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supertokens](https://vinkius.com/mcp/supertokens)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
