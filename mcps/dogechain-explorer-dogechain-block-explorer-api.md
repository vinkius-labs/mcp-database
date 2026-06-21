# Dogechain Explorer (Dogechain Block Explorer API) MCP Server

Automate Dogecoin blockchain analysis via Dogechain — check address balances, inspect transactions, and query block data directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dogechain-explorer-dogechain-block-explorer-api)

## Overview
**Category:** developer-tools
**Tools Count:** 17

## Description
Connect the **Dogechain** block explorer to your AI agent to monitor the Dogecoin network in real-time. Perform deep on-chain analysis, verify wallet balances, and track transaction flows through natural language.

### What you can do

- **Address Auditing** — Retrieve real-time balances, total coins received/sent, and transaction counts for any Dogecoin address.
- **Transaction Tracking** — Fetch detailed metadata for specific transaction hashes, including inputs, outputs, and confirmation status.
- **Block Inspection** — Query block data by height or hash and stay updated with the latest network activity using the best block hash tool.
- **UTXO Management** — List unspent transaction outputs (UTXOs) to understand wallet liquidity and prepare for transaction building.
- **Quick Validation** — Instantly check if a Dogecoin address is valid or decode it to its public key hash.

### How it works

1. Subscribe to this server
2. Enter 'public' or your Dogechain API key if applicable
3. Start querying the blockchain from Claude, Cursor, or any MCP-compatible client

No more manual searching on web explorers. Your AI acts as a blockchain analyst, providing raw data and insights directly in your workflow.

### Who is this for?

- **Crypto Traders & Whales** — Monitor wallet movements and verify large transactions without leaving your chat interface.
- **Blockchain Developers** — Debug transaction inputs/outputs and verify address balances during integration testing.
- **Data Analysts** — Extract on-chain metrics and block history for research and reporting.


## Available Tools
- **get_address_balance**: Get balance for a Dogecoin address
- **get_address_received**: Get total received amount for an address
- **get_address_sent**: Get total sent amount for an address
- **get_address_transaction_count**: Get transaction count for an address
- **get_address_transactions**: Results are paginated (10 per page).

Get recent transactions for an address
- **get_address_unspent**: Results are paginated (10 per page).

Get unspent outputs (UTXOs) for an address
- **get_best_block_hash**: Get the best block hash
- **get_block**: Get detailed block information
- **get_transaction**: Get detailed transaction information
- **q_address_balance**: Quick query: Get current balance
- **q_address_to_hash**: Quick query: Get public key hash
- **q_check_address**: Quick query: Check if address is valid
- **q_decode_address**: Quick query: Decode address
- **q_get_block_count**: Quick query: Get current block height
- **q_get_difficulty**: Quick query: Get last block difficulty
- **q_get_received_by_address**: Quick query: Get total amount ever received
- **q_get_sent_by_address**: Quick query: Get total amount ever sent


## Installation & Usage

To install and use the **Dogechain Explorer (Dogechain Block Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dogechain-explorer-dogechain-block-explorer-api](https://vinkius.com/mcp/dogechain-explorer-dogechain-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
