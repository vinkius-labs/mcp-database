# ThirdWeb MCP Server

Integrate Web3 capabilities into your AI agent — manage wallets, authenticate users, and interact with smart contracts across multiple blockchains.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/thirdweb)

## Overview
**Category:** developer-tools
**Tools Count:** 29

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


## Available Tools
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


## Installation & Usage

To install and use the **ThirdWeb** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thirdweb](https://vinkius.com/mcp/thirdweb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
