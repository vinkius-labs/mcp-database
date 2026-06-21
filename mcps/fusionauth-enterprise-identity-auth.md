# FusionAuth (Enterprise Identity & Auth) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fusionauth-enterprise-identity-auth)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fusionauth-enterprise-identity-auth-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fusionauth-enterprise-identity-auth-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage enterprise identity, users, and applications via FusionAuth — create users, list applications, and handle authentication flows directly from any AI agent.

## Description
Connect your **FusionAuth** instance to any AI agent to streamline identity management and authentication workflows through natural conversation.

### What you can do

- **User Management** — Create, retrieve, update, and delete users. Search by ID, email, or username using the `get_user` and `create_user` tools.
- **Application Control** — List all applications and drill down into specific configurations using `list_applications` and `get_application`.
- **Role Management** — Define and retrieve application-specific roles for granular access control with `list_application_roles`.
- **Authentication Flows** — Test login and MFA sequences directly through the API using `login` and `mfa_login`.
- **Flexible Updates** — Perform full updates with `update_user` or partial modifications with `patch_user` to maintain clean user data.

### How it works

1. Subscribe to this server
2. Enter your FusionAuth URL and API Key
3. Start managing your identity stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — quickly audit user accounts, check application roles, and manage permissions without leaving the terminal or IDE.
- **Backend Developers** — test authentication flows and verify user metadata during integration directly from the code editor.
- **Security Teams** — inspect user profiles and application access levels to ensure compliance and rapid incident response.


## Available Tools
- **add_group_member**: Add a User to a Group
- **create_api_key**: Create a new API Key
- **create_application_role**: Create a new Application Role
- **create_application**: Optionally provide a specific applicationId.

Create a new Application
- **create_group**: Create a new Group
- **create_lambda**: Create a new Lambda
- **create_tenant**: Create a new Tenant
- **create_user**: Optionally provide a specific userId. Pass the user object in the JSON body.

Create a new User in FusionAuth
- **create_webhook**: Create a new Webhook
- **delete_api_key**: Delete an API Key
- **delete_group**: Delete a Group
- **delete_lambda**: Delete a Lambda
- **delete_tenant**: Delete a Tenant
- **delete_user**: Delete a User
- **delete_webhook**: Delete a Webhook
- **disable_mfa**: Disable MFA for a User
- **enable_mfa**: Enable MFA for a User
- **generate_mfa_secret**: Generate an MFA Secret
- **get_api_key**: Retrieve an API Key
- **list_application_roles**: Retrieve all Roles for an Application
- **get_application**: Retrieve a specific Application
- **list_applications**: Retrieve all Applications
- **get_group**: Retrieve a Group
- **get_identity_provider**: Retrieve an Identity Provider
- **list_identity_providers**: Retrieve all Identity Providers
- **get_lambda**: Retrieve a Lambda
- **get_system_configuration**: Retrieve System Configuration
- **get_system_health**: Retrieve System Health
- **get_system_status**: Retrieve System Status
- **get_system_version**: Retrieve System Version
- **get_tenant**: Retrieve a Tenant
- **get_user**: Provide exactly one parameter.

Retrieve a User from FusionAuth
- **get_webhook**: Retrieve a Webhook
- **idp_login**: Complete External Identity Provider Login
- **issue_jwt**: Issue a new JWT
- **login**: Authenticate a User
- **mfa_login**: Complete Multi-Factor Authentication Login
- **patch_user**: Partially update an existing User
- **refresh_jwt**: Refresh a JWT
- **register_user**: Register a User for an Application
- **remove_group_member**: Remove a User from a Group
- **revoke_refresh_tokens**: Revoke Refresh Tokens
- **start_mfa**: Start an MFA flow
- **update_api_key**: Update an API Key
- **update_group**: Update a Group
- **update_lambda**: Update a Lambda
- **update_system_configuration**: Update System Configuration
- **update_tenant**: Update a Tenant
- **update_user**: Update an existing User
- **update_webhook**: Update a Webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FusionAuth (Enterprise Identity & Auth)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our applications in FusionAuth."

**🤖 AI Agent:**
> I've retrieved your applications. You have 3 active apps: 'Main Web Portal' (ID: 8a7...), 'Mobile API' (ID: 2f1...), and 'Internal Dashboard'. Which one would you like to inspect?

---

**👤 You:**
> "Find the user with email 'admin@company.com'."

**🤖 AI Agent:**
> I found the user: Admin User (ID: 550e...). Their account is currently 'Active' and they belong to the default tenant. Would you like to see their full profile data?

---

**👤 You:**
> "Create a user with the email 'test@example.com' and username 'test_user'."

**🤖 AI Agent:**
> User 'test_user' has been created successfully with ID 9b1... and email 'test@example.com'. I can now assign roles to this user if you provide an application ID.


## Installation & Usage

To install and use the **FusionAuth (Enterprise Identity & Auth)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fusionauth-enterprise-identity-auth](https://vinkius.com/mcp/fusionauth-enterprise-identity-auth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
