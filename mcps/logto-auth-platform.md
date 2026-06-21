# Logto (Auth Platform) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/logto-auth-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage users, roles, and organizations in your Logto auth tenant directly from your AI agent.

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


## Available Tools (23)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Logto (Auth Platform)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 users in my Logto tenant."

**🤖 AI Agent:**
> I've retrieved the user list. You have users like 'admin_user' (ID: user_1) and 'dev_test' (ID: user_2). Would you like to see the full details for any of them?

---

**👤 You:**
> "Create a new User role called 'Support Agent' with a description."

**🤖 AI Agent:**
> The role 'Support Agent' has been successfully created. It is now available for assignment to your users.

---

**👤 You:**
> "Show me all members of the organization with ID 'org_999'."

**🤖 AI Agent:**
> Fetching members for organization 'org_999'... I found 3 members: Alice, Bob, and Charlie. Would you like to inspect Alice's specific permissions?


## ❓ FAQ

**Q: Can I see which roles are assigned to a specific user?**
Yes! Use the `list_user_roles` tool with the target User ID to retrieve all global roles associated with that account.

**Q: Is it possible to manage multi-tenant organizations through this server?**
Absolutely. You can use `list_organizations` to see existing ones, `create_organization` to add new ones, and `list_organization_users` to audit membership.

**Q: Can I update user profiles or suspend accounts?**
Yes, the `update_user` tool allows you to modify the username, name, avatar, and the `isSuspended` status of any user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/logto-auth-platform](https://vinkius.com/mcp/logto-auth-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Logto (Auth Platform)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `logto-auth-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Logto (Auth Platform)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "logto-auth-platform": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
