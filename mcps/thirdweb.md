# ThirdWeb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thirdweb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Integrate Web3 capabilities into your AI agent — manage wallets, authenticate users, and interact with smart contracts across multiple blockchains.

## Description
Connect your **ThirdWeb** account to any AI agent to build and manage Web3 applications through natural language. This server provides a comprehensive suite of tools for blockchain interaction and identity management.

### What you can do

- **Authentication & Identity** — Handle email, SMS, social, and passkey logins. Link multiple social profiles to a single wallet address using `initiate_auth` and `link_profile`.
- **Wallet Management** — Retrieve authenticated user details, search for users by address or email, and pre-generate wallets for new users via `get_user_details` and `pregenerate_wallet`.
- **Smart Contract Interaction** — Execute read-only multicalls or state-changing transactions across any supported chain using `read_contract` and `write_contract`.
- **Event Monitoring** — Query historical contract events with advanced filtering for data analysis using `query_events`.

### How it works

1. Subscribe to this server
2. Provide your ThirdWeb Secret Key and API URL
3. Start building Web3 workflows from your favorite MCP client

### Who is this for?

- **Web3 Developers** — Rapidly prototype contract interactions and test auth flows directly from the IDE.
- **DApp Operators** — Manage user profiles and monitor contract events without custom scripts.
- **Product Managers** — Query on-chain data and user details to understand platform activity.


## Available Tools (29)
- **broadcast_solana_transaction**: Broadcast a transaction on Solana
- **complete_auth**: Verify challenge and complete login
- **create_solana_wallet**: Create a Solana wallet
- **deploy_contract**: Deploy a contract using bytecode and ABI
- **execute_solana_swap**: Execute a token swap on Solana Mainnet
- **fetch_with_payment**: Proxy a request to a paid API using x402
- **get_payment_requirements**: Generate payment requirements for a resource (x402)
- **get_solana_balance**: Get Solana wallet balance
- **get_solana_swap_quote**: Get a token swap quote on Solana Mainnet
- **get_transaction_status**: Get status of a transaction
- **get_user_details**: Search for users in your project
- **get_wallet_me**: Retrieve details of the authenticated user
- **initiate_auth**: Start authentication process for email, phone, passkey, or SIWE
- **link_profile**: Tie multiple social identities to a single wallet address
- **list_solana_wallets**: List Solana wallets
- **list_transactions**: List transactions
- **pregenerate_wallet**: Create a wallet for a user before they first log in
- **query_events**: Fetch historical events for a contract
- **query_transactions**: Fetch transaction history for a contract
- **read_contract**: Execute one or more read-only calls (multicall)
- **send_raw_transactions**: Broadcast encoded transactions
- **send_solana_tokens**: Send Solana tokens
- **settle_payment**: Submit the payment on-chain (x402)
- **sign_solana_message**: Sign a message on Solana
- **sign_solana_transaction**: Sign a transaction on Solana
- **social_auth**: OAuth flow for social providers
- **unlink_profile**: Unlink a social identity from a wallet address
- **verify_payment**: Validate a signed payment payload (x402)
- **write_contract**: Execute one or more state-changing calls atomically


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ThirdWeb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read the total supply of the contract 0x123... on chain 1."

**🤖 AI Agent:**
> I've executed the `read_contract` call. The total supply for the contract on Ethereum (Chain ID: 1) is 1,000,000 tokens.

---

**👤 You:**
> "Start an email authentication for dev@example.com."

**🤖 AI Agent:**
> I've triggered `initiate_auth` via email for dev@example.com. The user should receive a verification code shortly. Please provide the code to `complete_auth` when ready.

---

**👤 You:**
> "Search for user details associated with address 0xAbc123..."

**🤖 AI Agent:**
> Using `get_user_details`, I found that this address is linked to User ID 'user_987' with the verified email 'admin@web3app.com'.


## ❓ FAQ

**Q: Can I read data from a smart contract without paying gas?**
Yes! Use the `read_contract` tool. It performs read-only calls (multicall) to the blockchain, which do not require gas or state changes.

**Q: How do I start an authentication flow for a new user?**
You can use the `initiate_auth` tool by specifying the method (email, sms, etc.) and the user's identifier. Then, use `complete_auth` with the verification code to finish the login.

**Q: Can I find a user's profile if I only have their wallet address?**
Absolutely. Use the `get_user_details` tool and provide the `address` parameter. The agent will return any associated user IDs, emails, or phone numbers linked to that wallet in your project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thirdweb](https://vinkius.com/mcp/thirdweb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ThirdWeb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thirdweb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ThirdWeb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thirdweb": {
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
