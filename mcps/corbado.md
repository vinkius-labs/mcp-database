# Corbado MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/corbado)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage users, identifiers, and passkey authentication via Corbado — handle user lifecycles and auth processes directly from your AI agent.

## Description
Connect your **Corbado** project to any AI agent to streamline your identity and access management. This server allows you to manage the entire user lifecycle, from creation to session revocation, using natural language.

### What you can do

- **User Management** — Create, retrieve, update, and delete users. List all project users to audit your database.
- **Login Identifiers** — Manage email, phone, and username identifiers for any user account.
- **Passkey Orchestration** — Initiate and finalize passkey append or login flows directly through the API.
- **Session Control** — List active sessions and revoke them instantly to maintain security.
- **Auth Processes** — Initialize and monitor complex authentication processes, including SSO and identifier verification.
- **Developer Utilities** — Access JWKS, asset links, and Apple App Site Association data for your integration.

### How it works

1. Subscribe to this server
2. Enter your Corbado Project ID, API Secret, and Backend URL
3. Start managing your identity infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — quickly debug user states or reset auth processes without leaving the IDE
- **Security Engineers** — audit active sessions and manage identifiers to respond to support tickets faster
- **Product Managers** — list users and check registration statuses to monitor growth and onboarding health


## Available Tools
- **complete_auth_process**: Complete authentication process
- **create_connect_token**: Create a ConnectToken
- **create_identifier**: Create a login identifier for a user
- **create_user**: Create a new Corbado user
- **delete_connect_token**: Delete a ConnectToken
- **delete_identifier**: Delete a login identifier
- **delete_me**: Delete current user
- **delete_user**: Delete a Corbado user
- **finish_connect_login**: Finish Connect login
- **finish_identifier_verify**: Finish identifier verification
- **finish_passkey_append**: Finish passkey append
- **finish_passkey_login**: Finish passkey login
- **finish_sso**: Finish SSO (SAML2)
- **get_apple_app_site_association**: Get Apple App Site Association
- **get_assetlinks**: Get Asset Links
- **get_auth_process**: Retrieve authentication process
- **get_jwks**: Get JWKS
- **get_me**: Retrieve current user
- **get_user**: Retrieve user details
- **init_auth_process**: Initialize authentication process
- **init_connect_login**: Initialize Connect login
- **init_login**: Initialize login
- **init_signup**: Initialize signup
- **list_connect_passkeys**: List Connect passkeys
- **list_connect_tokens**: List ConnectTokens
- **list_identifiers**: List all login identifiers
- **list_sessions**: List active sessions
- **list_users**: List Corbado users
- **logout_me**: Logout current user
- **refresh_me**: Refresh session
- **reset_auth_process**: Reset authentication process
- **revoke_session**: Revoke a session
- **skip_auth_block**: Skip authentication block
- **start_connect_login**: Start Connect login
- **start_identifier_verify**: Start identifier verification
- **start_passkey_append**: Start passkey append
- **start_passkey_login**: Start passkey login
- **start_sso**: Start SSO (SAML2)
- **update_auth_identifier**: Update authentication identifier
- **update_identifier**: Update a login identifier
- **update_me**: Update current user
- **update_user**: Update a Corbado user
- **verify_signed_data**: Verify signed passkey data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corbado** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in my Corbado project."

**🤖 AI Agent:**
> I've retrieved the user list. You have 150 users in this project. The most recent users include 'John Doe' (active) and 'Jane Smith' (pending). Would you like to see more details for a specific user?

---

**👤 You:**
> "Get the details for user ID usr-123456789."

**🤖 AI Agent:**
> User 'usr-123456789' is currently 'active'. Their full name is 'Alice Vance'. They were created on October 12th, 2023. Would you like to list their identifiers or active sessions?

---

**👤 You:**
> "Add the email 'dev@example.com' as an identifier for user usr-123456789."

**🤖 AI Agent:**
> I've successfully added 'dev@example.com' as an email identifier for Alice Vance (usr-123456789). The identifier is currently in 'pending' status until verified.


## ❓ FAQ

**Q: Can I list all users in my project to check their status?**
Yes! Use the `list_users` tool to retrieve a paginated list of all users in your project, including their current status (active, pending, or disabled).

**Q: How do I add a new email or phone number to an existing user?**
You can use the `create_identifier` tool. Simply provide the `userID`, the type (email, phone, or username), and the value you want to add.

**Q: Is it possible to revoke a user's session if their account is compromised?**
Absolutely. Use the `revoke_session` tool with the specific session ID to immediately terminate that user's access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corbado](https://vinkius.com/mcp/corbado)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Corbado** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `corbado` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Corbado** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "corbado": {
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
