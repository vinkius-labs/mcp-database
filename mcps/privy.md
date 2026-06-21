# Privy MCP Server

Manage users and wallets via Privy — create users, search profiles, and manage embedded wallets directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/privy)

## Overview
**Category:** developer-tools
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Privy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/privy](https://vinkius.com/mcp/privy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
