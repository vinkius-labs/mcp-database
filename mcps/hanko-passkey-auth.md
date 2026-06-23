# Hanko (Passkey Auth) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hanko-passkey-auth)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage passkey authentication and user identity via Hanko — initialize registrations, handle logins, and manage WebAuthn credentials directly.

## Description
Connect your **Hanko** instance to any AI agent to streamline passkey-based authentication and user management. This server provides a comprehensive interface for WebAuthn flows and administrative user operations.

### What you can do

- **Passkey Lifecycle** — Initialize and finalize WebAuthn registration and login flows for secure, passwordless access.
- **Credential Management** — List and delete registered WebAuthn credentials for specific users.
- **User Administration** — Create, retrieve, and list users and their associated credentials via admin tools.
- **Transaction Security** — Initialize and finalize passkey-signed transactions for sensitive operations like payments.
- **Session Validation** — Publicly validate sessions and retrieve JWKS for token verification.

### How it works

1. Subscribe to this server
2. Enter your Hanko Tenant ID and API Key
3. Start managing identity flows from your MCP-compatible client

### Who is this for?

- **Developers** — quickly test and debug WebAuthn registration and login flows without manual API calls.
- **Security Engineers** — audit user credentials and manage identity access policies through a conversational interface.
- **Product Teams** — simulate and verify user onboarding and transaction signing workflows.


## Available Tools (15)
- **admin_create_user**: Create a new user via Admin API
- **admin_get_user**: Get a user by ID via Admin API
- **admin_list_user_credentials**: List WebAuthn credentials for a user via Admin API
- **admin_list_users**: List users via Admin API
- **flow_execute**: Execute a Hanko Flow action
- **passkey_delete_credential**: Delete a WebAuthn credential
- **passkey_list_credentials**: List WebAuthn credentials for a user
- **passkey_login_finalize**: Finalize a passkey login
- **passkey_login_init**: Returns publicKey options for navigator.credentials.get().

Initialize a passkey login
- **passkey_registration_finalize**: Finalize a passkey registration
- **passkey_registration_init**: Returns publicKey options for navigator.credentials.create().

Initialize a passkey registration
- **passkey_transaction_finalize**: Finalize a passkey transaction
- **passkey_transaction_init**: g., payment confirmation) for an existing user.

Initialize a passkey transaction
- **public_get_jwks**: Get JSON Web Key Set (JWKS)
- **public_validate_session**: Validate a Hanko session token


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hanko (Passkey Auth)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Initialize a passkey registration for user 'user_789' with username 'alice_dev'."

**🤖 AI Agent:**
> I've initialized the registration. Here are the WebAuthn options for 'alice_dev' (User ID: user_789). You can now use these to call navigator.credentials.create() on your frontend.

---

**👤 You:**
> "List all registered credentials for user ID 'usr_12345'."

**🤖 AI Agent:**
> I found 2 registered credentials for user 'usr_12345'. One is a 'FaceID' passkey created on 2023-10-12, and the other is a 'YubiKey' registered on 2023-11-05.

---

**👤 You:**
> "Create a new user in Hanko with the ID 'new_customer_001'."

**🤖 AI Agent:**
> User 'new_customer_001' has been successfully created in your Hanko project. You can now proceed to initialize passkey registration for them.


## ❓ FAQ

**Q: How do I start a new passkey registration for a user?**
Use the `passkey_registration_init` tool with the user's ID and username. This will return the necessary WebAuthn options to be used on the client side.

**Q: Can I view all WebAuthn credentials associated with a specific user?**
Yes, you can use the `passkey_list_credentials` tool (or `admin_list_user_credentials` for admin access) to retrieve a list of all registered passkeys for any user ID.

**Q: Is it possible to create a user directly through the AI agent?**
Absolutely. Use the `admin_create_user` tool to provision a new user in your Hanko project by providing a unique user ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hanko-passkey-auth](https://vinkius.com/mcp/hanko-passkey-auth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hanko (Passkey Auth)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hanko-passkey-auth` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hanko (Passkey Auth)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hanko-passkey-auth": {
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
