# Blockchair (Universal Blockchain Search Engine & API) MCP Server

Query blocks, transactions, and addresses across multiple blockchains like Bitcoin and Ethereum using Blockchair's universal API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/blockchair-universal-blockchain-search-engine-api)

## Overview
**Category:** developer-tools
**Tools Count:** 11

## Description
Connect to **Blockchair**, the most advanced universal blockchain search engine, and explore decentralized data across 20+ networks including Bitcoin, Ethereum, and Litecoin through natural conversation.

### What you can do

- **Multi-Chain Stats** — Get real-time network health, difficulty, and block height for any supported blockchain using `get_blockchain_stats`.
- **Deep Address Inspection** — Retrieve balances, transaction history, and UTXO sets for specific wallet addresses with `get_address`.
- **SQL-like Filtering** — Query blocks and transactions using advanced filters (e.g., filter by fee, time, or value) via `filter_transactions` and `filter_blocks`.
- **Token & Contract Data** — Check ERC-20 token balances and inspect internal Ethereum contract calls using specialized tools.
- **HD Wallet Support** — Analyze entire HD wallets using extended public keys (xpub) with the `get_xpub` tool.

### How it works

1. Subscribe to this server
2. Enter your Blockchair API Key
3. Start querying blockchain data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug transactions and verify contract states without leaving your IDE or code editor.
- **Data Analysts** — Extract specific blockchain datasets using powerful filtering tools for research or reporting.
- **Crypto Enthusiasts** — Track wallet balances and monitor network congestion through simple natural language prompts.


## Available Tools
- **filter_blocks**: Example q: time(2023-01-01..2023-01-02),transaction_count(100..)

Query blocks using SQL-like filters
- **filter_transactions**: Example q: fee(10000..), s: fee(desc)

Query transactions using SQL-like filters
- **get_address**: Retrieve balance, history, and UTXO set for an address
- **get_block**: Retrieve details about a specific block
- **get_contract_calls**: Get Ethereum contract internal transactions
- **get_erc20_token_address**: Get the balance of a specific ERC-20 token for an address
- **get_blockchain_stats**: for the specified blockchain.

Get general information about a blockchain
- **get_transaction**: Retrieve details about a specific transaction
- **get_xpub**: Retrieve data for an entire HD wallet (xpub)
- **push_transaction**: Broadcast a raw hex-encoded transaction to the network
- **validate_address**: Check if an address is valid for a specific chain


## Installation & Usage

To install and use the **Blockchair (Universal Blockchain Search Engine & API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockchair-universal-blockchain-search-engine-api](https://vinkius.com/mcp/blockchair-universal-blockchain-search-engine-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
