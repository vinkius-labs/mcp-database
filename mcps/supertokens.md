# SuperTokens MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/supertokens)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage authentication, users, sessions, and roles via SuperTokens Core directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SuperTokens** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for user ID 'user-123'."

**🤖 AI Agent:**
> I've retrieved the details for user 'user-123'. They are registered with email 'dev@example.com' and currently have 2 active sessions.

---

**👤 You:**
> "Assign the 'editor' role to user 'user-456'."

**🤖 AI Agent:**
> Successfully assigned the 'editor' role to 'user-456'. They now have the associated permissions for that role.

---

**👤 You:**
> "List all available roles in the system."

**🤖 AI Agent:**
> Here are the roles currently configured in your SuperTokens instance: 'admin', 'editor', and 'viewer'.


## ❓ FAQ

**Q: Can I retrieve specific user information using their ID?**
Yes, by using the `get_user` tool with the specific User ID, you can fetch the full profile, including email and account linking status.

**Q: How do I assign a specific role like 'admin' to a user?**
You can use the `assign_role_to_user` tool. Just provide the User ID and the role name to update their permissions immediately.

**Q: Is it possible to update custom user data or preferences?**
Absolutely. The `update_user_metadata` tool allows you to pass a JSON object to store or update custom information for any user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supertokens](https://vinkius.com/mcp/supertokens)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SuperTokens** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `supertokens` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SuperTokens** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supertokens": {
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
