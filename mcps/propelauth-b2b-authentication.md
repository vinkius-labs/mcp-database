# PropelAuth (B2B Authentication) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/propelauth-b2b-authentication)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/propelauth-b2b-authentication-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/propelauth-b2b-authentication-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage B2B authentication, users, and organizations via PropelAuth — handle user provisioning, org management, and API keys directly from your AI agent.

## Description
Connect your **PropelAuth** dashboard to any AI agent to streamline B2B identity management and user operations through natural language.

### What you can do

- **User Management** — Create, fetch, update, and delete users. Manage passwords, emails, and account statuses (enable/disable) without leaving your workflow.
- **Organization Control** — Create organizations, manage memberships, and assign roles (Admin, Member, etc.) to users within specific B2B tenants.
- **API Key Governance** — Generate, validate, and monitor API keys for your end-users, including usage tracking and lifecycle management.
- **B2B Provisioning** — Invite users to organizations, change roles, and handle complex multi-tenant access structures programmatically.
- **Authentication Flows** — Create magic links, manage SAML/OIDC connections, and handle OAuth provider tokens.

### How it works

1. Subscribe to this server
2. Enter your PropelAuth API Key and Auth URL from your dashboard
3. Start managing your B2B users and orgs from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps & Security Engineers** — Automate user offboarding, audit organization memberships, and manage API key lifecycles.
- **Customer Success Managers** — Quickly look up user details, reset passwords, or manually add customers to organizations during support calls.
- **Product Developers** — Test authentication flows and verify user metadata directly from the code editor.


## Available Tools
- **add_user_to_org**: Add a user to an organization immediately
- **allow_saml**: Allow or disallow SAML for an organization
- **change_user_role_in_org**: Change a user role within an organization
- **clear_user_password**: Clear a user password
- **create_access_token**: Create an access token for testing or M2M
- **create_api_key**: Create a new end-user API key
- **create_magic_link**: Create a magic link for a user
- **create_org**: Create a new organization
- **create_saml_connection_link**: Create a SAML setup link for an organization
- **create_user**: Create a new user in PropelAuth
- **delete_api_key**: Delete an end-user API key
- **delete_org**: Delete an organization
- **delete_user**: Delete a user
- **disable_user**: Disable or block a user
- **enable_user**: Enable or unblock a user
- **get_active_api_keys**: Fetch active end-user API keys
- **get_api_key_usage**: Fetch usage statistics for API keys
- **get_custom_role_mappings**: Fetch custom role mappings
- **get_oauth_tokens**: Fetch OAuth tokens for a user
- **get_org**: Fetch an organization by ID
- **get_saml_sp_metadata**: Fetch SAML Service Provider (SP) metadata for an organization
- **get_user_by_email**: Fetch a user by email address
- **get_user_by_username**: Fetch a user by username
- **get_user**: Fetch a user by ID
- **get_users_in_org**: Fetch all users in an organization
- **go_live_saml**: Set a SAML connection to live status
- **invite_user_to_org**: Invite a user to an organization via email
- **logout_all_user_sessions**: Logout all sessions for a user
- **migrate_user**: Migrate an existing user into PropelAuth
- **query_orgs**: Query organizations
- **query_users**: Query and list users with pagination and filtering
- **refresh_provider_token**: Refresh an OAuth provider token for a user
- **remove_user_from_org**: Remove a user from an organization
- **set_oidc_idp_metadata**: Set OIDC Identity Provider (IdP) metadata
- **set_saml_idp_metadata**: Set SAML Identity Provider (IdP) metadata
- **subscribe_org_to_mapping**: Subscribe an organization to a custom role mapping
- **update_api_key**: Update an end-user API key
- **update_org**: Update an organization
- **update_user_email**: Update a user email address
- **update_user_password**: Update a user password
- **update_user**: Update user metadata
- **validate_api_key**: Validate an end-user API key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PropelAuth (B2B Authentication)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the user with email 'alex@company.com' and tell me which organizations they belong to."

**🤖 AI Agent:**
> I've located the user (ID: user_98765). They are currently a member of 'Acme Corp' (ID: org_123) with the role of 'Admin' and 'Beta Testers' (ID: org_456) as a 'Member'.

---

**👤 You:**
> "Create a new organization called 'Stark Industries' and add 'user_555' as an Admin."

**🤖 AI Agent:**
> Organization 'Stark Industries' has been created with ID `org_stark_001`. I have also successfully added user `user_555` to this organization with the 'Admin' role.

---

**👤 You:**
> "List all active API keys for organization 'org_123' and check if any have high usage."

**🤖 AI Agent:**
> I found 3 active API keys for 'org_123'. Key `pk_live_abc` has the highest usage with 1,250 calls in the last 24 hours. The other two keys show minimal activity.


## Installation & Usage

To install and use the **PropelAuth (B2B Authentication)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/propelauth-b2b-authentication](https://vinkius.com/mcp/propelauth-b2b-authentication)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
