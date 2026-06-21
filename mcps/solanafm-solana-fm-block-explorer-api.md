# SolanaFM (Solana FM Block Explorer API) MCP Server

Access Solana blockchain data via SolanaFM — inspect blocks, transactions, account metadata, and token balances directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/solanafm-solana-fm-block-explorer-api)

## Overview
**Category:** developer-tools
**Tools Count:** 6

## Description
Connect to the **SolanaFM** block explorer API to empower your AI agent with deep indexing capabilities for the Solana network.

### What you can do

- **Block Exploration** — Fetch detailed block data or ranges using slot numbers via `get_block` and `get_blocks` tools.
- **Transaction Analysis** — Retrieve full transaction details via signatures with `get_transaction` or list all transactions for a specific address using `get_account_transactions`.
- **Account Intelligence** — Inspect account metadata, state, and ownership details using `get_account_info`.
- **Token Tracking** — List all token accounts owned by a specific wallet address with `get_token_accounts`.

### How it works

1. Subscribe to this server
2. Enter your SolanaFM API Key
3. Start querying Solana data from Claude, Cursor, or any MCP-compatible client

No more manual searching through web explorers. Your AI acts as a blockchain analyst, providing real-time data on accounts, blocks, and transactions.

### Who is this for?

- **Web3 Developers** — Debug transactions and verify account states straight from the code editor to avoid breaking flow.
- **Data Analysts** — Extract blockchain metrics and block history for research and reporting without complex scripts.
- **Crypto Enthusiasts** — Monitor wallet activity and token holdings through natural conversation.


## Available Tools
- **get_account_info**: Get the metadata and state of a Solana account
- **get_account_transactions**: List transactions associated with a specific account address
- **get_block**: Get detailed information about a specific block
- **get_blocks**: Get a list of blocks within a specified range
- **get_token_accounts**: Get token accounts owned by a specific wallet address
- **get_transaction**: Get details for a specific transaction


## Installation & Usage

To install and use the **SolanaFM (Solana FM Block Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/solanafm-solana-fm-block-explorer-api](https://vinkius.com/mcp/solanafm-solana-fm-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
