# Aptoscan (Aptos Blockchain Explorer API) MCP Server

Explore the Aptos blockchain — check account balances, resources, transactions, and token data directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aptoscan-aptos-blockchain-explorer-api)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect to the **Aptoscan API** to inspect the Aptos blockchain in real-time. This MCP server allows any AI agent to query account states, transaction history, and token metadata without leaving the chat interface.

### What you can do

- **Account Insights** — Fetch balances, Move resources, and published modules for any Aptos address using `get_account_balance` and `get_account_resources`.
- **Transaction Tracking** — Retrieve detailed transaction data using hashes or ledger versions via `get_transaction_by_hash`.
- **Block Exploration** — Inspect specific blocks by height or transaction version to audit network activity.
- **Token & NFT Analysis** — List all tokens (NFTs and Fungible Assets) held by an account or fetch specific token metadata with `get_account_tokens`.
- **Developer Tools** — Access raw Move module data directly to analyze smart contract logic on-chain.

### How it works

1. Subscribe to this server
2. Enter your Aptoscan API Key
3. Start querying the Aptos ledger from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug transactions and inspect account resources without switching to a browser.
- **Data Analysts** — Pull on-chain data directly into your analysis workflow.
- **Crypto Enthusiasts** — Monitor wallet balances and NFT collections through natural conversation.


## Available Tools
- **get_account_balance**: Get the current balance of the specified account
- **get_account_modules**: Get all Move modules published under the specified account
- **get_account_resources**: Get all resources owned by the specified account
- **get_account_tokens**: List all tokens (NFTs and Fungible Assets) held by an account
- **get_account_transactions**: Get a list of transactions associated with a specific account
- **get_block_by_height**: Get block details by its height
- **get_block_by_version**: Get block details containing a specific transaction version
- **get_token_data**: Get metadata and supply information for a specific token
- **get_transaction_by_hash**: Get details of a specific transaction using its hash
- **get_transaction_by_version**: Get details of a transaction using its ledger version


## Installation & Usage

To install and use the **Aptoscan (Aptos Blockchain Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aptoscan-aptos-blockchain-explorer-api](https://vinkius.com/mcp/aptoscan-aptos-blockchain-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
