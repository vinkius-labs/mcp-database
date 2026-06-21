# Privy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/privy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage users and wallets via Privy — create users, search profiles, and manage embedded wallets directly from any AI agent.

## Description
Connect your **Privy** application to any AI agent to streamline user onboarding and wallet management in your Web3 application through natural language.

### What you can do

- **User Management** — Create new users, search for existing ones by term or email, and retrieve full profile metadata.
- **Embedded Wallets** — Provision new wallets (Ethereum, Solana, Bitcoin, Sui) for your users individually or in batches of up to 100.
- **Wallet Operations** — Update wallet metadata, policies, and ownership, or retrieve specific wallet details via ID.
- **Blockchain Actions** — Execute RPC methods like signing messages or sending transactions directly through managed wallets.
- **Data Maintenance** — Securely delete user records when they are no longer needed.

### How it works

1. Subscribe to this server
2. Enter your Privy App ID and App Secret
3. Start managing your Web3 identity and wallet infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — quickly inspect user accounts or provision test wallets without leaving the code editor.
- **Product Managers** — search for user profiles and verify linked accounts or wallet statuses during support or planning.
- **DevOps & Security** — automate user lifecycle management and wallet policy updates via a conversational interface.


## Available Tools
- **batch_create_wallets**: Batch create wallets
- **create_user**: Create a new user object with linked accounts
- **create_wallet**: Create a new wallet
- **delete_user**: Delete a user
- **get_transaction_by_external_id**: Get a transaction by external ID
- **get_transaction**: Get a transaction
- **get_user_by_email**: Get a user by email address
- **get_user**: Get a user by ID
- **get_wallet**: Get wallet details
- **search_users**: Search for users
- **update_wallet**: Update a wallet
- **wallet_rpc**: Perform a wallet RPC action


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Privy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for users with the term 'beta-tester' in Privy."

**🤖 AI Agent:**
> I found 3 users matching 'beta-tester'. The most recent is user `did:privy:cl...` linked to `tester1@example.com`. Would you like to see their full profile details?

---

**👤 You:**
> "Create a new Ethereum wallet with the display name 'Main Treasury'."

**🤖 AI Agent:**
> Successfully created a new Ethereum wallet. ID: `wa_123...`, Address: `0x71C...`. It is now ready for use in your application.

---

**👤 You:**
> "Get the user details for email 'alice@company.com'."

**🤖 AI Agent:**
> Retrieved profile for Alice. She has a linked Google account and one embedded Solana wallet (`6xY...`). Her Privy ID is `did:privy:ck...`.


## ❓ FAQ

**Q: Can I find a user if I only have their email address?**
Yes. You can use the `get_user_by_email` tool to retrieve the full user object and linked accounts associated with that specific email address.

**Q: Is it possible to create multiple wallets for a large group of users at once?**
Absolutely. The `batch_create_wallets` tool allows you to create up to 100 wallets in a single request, which is ideal for bulk onboarding or migration tasks.

**Q: Can the AI agent perform transactions on behalf of a wallet?**
Yes, using the `wallet_rpc` tool. You can specify the `wallet_id` and the RPC method (like `eth_sendTransaction`) to execute blockchain actions through Privy's infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/privy](https://vinkius.com/mcp/privy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Privy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `privy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Privy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "privy": {
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
