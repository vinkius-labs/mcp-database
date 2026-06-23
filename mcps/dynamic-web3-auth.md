# Dynamic (Web3 Auth) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dynamic-web3-auth)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Manage Web3 authentication and user data via Dynamic — fetch user profiles, check wallet sanctions, and manage sessions directly from any AI agent.

## Description
Connect your **Dynamic** environment to any AI agent to streamline Web3 user management and security workflows through natural conversation.

### What you can do

- **User Management** — Fetch detailed user profiles or permanently delete users from specific environments using `get_user` and `delete_user`.
- **Security & Compliance** — Use `check_sanctions` to verify if specific wallet addresses are sanctioned across multiple chains (ETH, SOL, EVM, etc.).
- **Session Control** — Instantly terminate active user sessions with `revoke_session` to maintain environment security.
- **Infrastructure Monitoring** — List active embedded wallet versions and configured webhooks to audit your auth setup.
- **Financial Insights** — Retrieve real-time token balances for users across different networks using `get_token_balances`.

### How it works

1. Subscribe to this server
2. Enter your Dynamic API Token
3. Start managing your Web3 auth layer from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug user profiles and check token balances directly from your code editor.
- **Security & Ops Teams** — Audit wallet sanctions and revoke suspicious sessions instantly without opening the dashboard.
- **Product Managers** — Monitor webhook configurations and available event types to coordinate feature releases.


## Available Tools (8)
- **check_sanctions**: Check wallet sanctions
- **delete_user**: Delete a user from an environment
- **get_embedded_wallet_versions**: Get active embedded wallet versions
- **get_event_types**: Get available event types
- **get_token_balances**: Get token balances for a user
- **get_user**: Get a user by ID in an environment
- **get_webhooks**: Get configured webhooks
- **revoke_session**: Revoke an active user session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dynamic (Web3 Auth)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get user profile for user_id 'usr_123' in environment 'env_456'."

**🤖 AI Agent:**
> I've retrieved the profile for user 'usr_123'. They have a verified email (user@example.com) and a linked Ethereum wallet (0x123...a1b2). Their account was created on Oct 12, 2023.

---

**👤 You:**
> "Check if the wallet address 0x742d35Cc6634C0532925a3b844Bc454e4438f44e is sanctioned on the ETH chain."

**🤖 AI Agent:**
> I've performed the check. The address 0x742d... is NOT sanctioned on the Ethereum network for your current environment settings.

---

**👤 You:**
> "What are the available event types for webhooks in this environment?"

**🤖 AI Agent:**
> I've fetched the event types. You can subscribe to: 'user.created', 'wallet.authenticated', 'session.started', and 'email.verified'. Each event includes detailed metadata in its payload.


## ❓ FAQ

**Q: Can I check if a specific wallet address is sanctioned before onboarding a user?**
Yes! Use the `check_sanctions` tool by providing the wallet address and the chain (e.g., ETH, SOL). The agent will return the sanction status for that environment.

**Q: How do I retrieve the token balances for a user across different networks?**
Simply use the `get_token_balances` tool. You'll need to provide the environment ID, user ID, and an array of balance requests specifying the address and chain.

**Q: Is it possible to terminate a suspicious user session immediately?**
Yes. Use the `revoke_session` tool with the specific session ID. This will instantly invalidate the session and disconnect the user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dynamic-web3-auth](https://vinkius.com/mcp/dynamic-web3-auth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dynamic (Web3 Auth)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dynamic-web3-auth` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dynamic (Web3 Auth)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dynamic-web3-auth": {
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
