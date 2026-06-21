# Logto (Auth Platform) MCP Server

Manage users, roles, and organizations in your Logto auth tenant directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/logto-auth-platform)

## Overview
**Category:** fort-knox
**Tools Count:** 23

## Description
Connect your **Logto** authentication platform to any AI agent and take full control of your identity management and access control workflows.

### What you can do

- **User Management** — List, fetch, update, or delete users from your tenant with full metadata access.
- **RBAC & Permissions** — Create and list global roles and API resources to manage granular access control.
- **Organizations** — Handle multi-tenant structures by creating organizations and managing their memberships.
- **Security & Verification** — Verify user passwords and manage account-level security settings.
- **Account API** — Access and update the current user's profile and MFA settings using end-user tokens.

### How it works

1. Subscribe to this server
2. Provide your Logto Management API credentials (Endpoint, App ID, and App Secret)
3. Start managing your auth infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & Security Engineers** — Quickly audit user lists, roles, and resource permissions without leaving the terminal.
- **Full-stack Developers** — Manage test users and organization structures directly from the code editor.
- **Support Teams** — Inspect user metadata and account statuses to resolve identity-related tickets faster.


## Available Tools
- **bind_mfa_verification**: Bind a new MFA factor (TOTP, WebAuthn)
- **create_organization**: Create a new organization
- **create_resource**: Create a new API resource
- **create_role**: Create a new role
- **delete_user**: Delete a Logto user
- **get_user**: Get details for a specific Logto user
- **list_mfa_verifications**: List registered MFA factors for the current user
- **get_my_account**: Retrieve current user profile (Account API)
- **list_organization_users**: List members of an organization
- **list_organizations**: List organizations in Logto
- **remove_mfa_verification**: Remove an MFA factor
- **list_resources**: List API resources in Logto
- **list_roles**: List global roles in Logto
- **send_verification_code**: Send email/SMS code for verification
- **update_my_account_primary_email**: Update or link primary email
- **update_my_account_profile**: Update extended profile (address, etc.)
- **update_my_account_password**: Update user password
- **update_my_account**: Update basic profile (username, name, avatar)
- **update_user**: Update an existing Logto user
- **list_user_roles**: List roles assigned to a user
- **list_users**: List Logto users
- **verify_password**: Verify password to get a verification ID
- **verify_user_password**: Verify a user password (Management API)


## Installation & Usage

To install and use the **Logto (Auth Platform)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/logto-auth-platform](https://vinkius.com/mcp/logto-auth-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
