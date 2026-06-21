# Suivision (Sui Blockchain Explorer API) MCP Server

Explore the Sui blockchain — query transactions, inspect accounts, analyze coins, and track on-chain objects directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/suivision-sui-blockchain-explorer-api)

## Overview
**Category:** developer-tools
**Tools Count:** 17

## Description
Connect to the **Suivision API** to gain deep visibility into the Sui Network. This MCP server allows any AI agent to act as a powerful blockchain explorer, retrieving real-time data about transactions, account balances, and smart contract packages.

### What you can do

- **Transaction Analysis** — Fetch detailed metadata for any transaction digest or list recent network activity using `get_transaction` and `list_transactions`.
- **Account Insights** — Get comprehensive overviews of Sui addresses, including coin balances and owned objects (NFTs) via `get_account_overview` and `get_account_objects`.
- **Smart Contract Inspection** — Retrieve Move package details, bytecode, and transaction history for specific protocols using `get_package_details`.
- **Coin Metadata** — Access supply information and decimals for any coin type on the network with `get_coin_metadata`.

### How it works

1. Subscribe to this server
2. Enter your Suivision API Key
3. Start querying the Sui blockchain from Claude, Cursor, or any MCP-compatible client.

No more manual searching through web explorers. Your AI acts as a dedicated blockchain analyst, providing technical data in seconds.

### Who is this for?

- **Web3 Developers** — quickly inspect package bytecode and transaction effects without leaving the IDE.
- **Crypto Analysts** — track whale movements, account balances, and coin supply metrics through natural language.
- **DeFi Users** — verify transaction statuses and object ownership on the Sui network instantly.


## Available Tools
- **get_account_coins**: List all coins owned by an account
- **get_account_objects**: List all objects owned by an account
- **get_account_overview**: Get account overview and balance
- **get_account_transactions**: List transactions associated with a specific account address
- **get_checkpoint**: Get details of a specific checkpoint
- **get_coin_metadata**: Get metadata for a specific coin type
- **get_coin_supply**: Get total supply for a specific coin type
- **get_defi_stats**: Get Sui DeFi statistics
- **get_epoch**: Get details of a specific epoch
- **get_object_details**: Get details of a specific on-chain object
- **get_package_details**: Get details of a Move package
- **get_package_transactions**: List transactions that interacted with a package
- **get_transaction**: Get detailed information about a specific transaction
- **list_checkpoints**: List recent network checkpoints
- **list_epochs**: List recent network epochs
- **list_transactions**: Supports pagination and ordering.

List recent transactions on the Sui network
- **list_validators**: List current network validators


## Installation & Usage

To install and use the **Suivision (Sui Blockchain Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/suivision-sui-blockchain-explorer-api](https://vinkius.com/mcp/suivision-sui-blockchain-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
