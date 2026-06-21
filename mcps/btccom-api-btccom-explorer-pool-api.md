# BTC.com API (BTC.com Explorer & Pool API) MCP Server

Access real-time Bitcoin blockchain data and mining pool statistics including blocks, transactions, addresses, and worker performance.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/btccom-api-btccom-explorer-pool-api)

## Overview
**Category:** data-analytics
**Tools Count:** 13

## Description
Connect to the **BTC.com API** to integrate comprehensive Bitcoin blockchain exploration and mining pool management into your AI workflows. This server provides a dual-purpose interface for both public blockchain data and private mining operations.

### What you can do

- **Blockchain Explorer** — Query specific blocks, transactions, and unconfirmed mempool data using hashes or heights.
- **Address Analysis** — Fetch balances, UTXOs, and complete transaction history for any Bitcoin address.
- **Mining Pool Stats** — Monitor your account hashrate (15m, 24h), rejection rates, and historical performance.
- **Worker Management** — List all mining workers and inspect individual statistics to identify active, inactive, or dead units.
- **Financial Tracking** — Retrieve payment history and account-level statistics directly through your agent.

### How it works

1. Subscribe to this server
2. (Optional) Enter your BTC.com Access Key to enable Pool API features
3. Start querying Bitcoin data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Developers** — Verify transaction inputs/outputs and debug address balances without leaving the code editor.
- **Mining Operators** — Monitor farm health and hashrate stability through natural language queries.
- **Data Analysts** — Extract real-time blockchain metrics and block metadata for research and reporting.


## Available Tools
- **get_account_stats**: Requires BTC_COM_ACCESS_KEY.

Get account hashrate and stats
- **get_address_summary**: Get address summary
- **get_address_transactions**: Get address transactions
- **get_address_utxo**: Get unspent transaction outputs (UTXO) for an address
- **get_block**: Get block information by hash or height
- **get_block_transactions**: Get transactions for a specific block
- **get_hashrate_history**: Requires BTC_COM_ACCESS_KEY.

Get hashrate history
- **get_latest_block**: Get the latest block information
- **get_payment_history**: Requires BTC_COM_ACCESS_KEY.

Get payment history
- **get_transaction**: Get transaction details
- **get_unconfirmed_transactions**: Get unconfirmed transactions
- **get_worker_list**: Requires BTC_COM_ACCESS_KEY.

Get worker list
- **get_worker_stats**: Requires BTC_COM_ACCESS_KEY.

Get worker stats


## Installation & Usage

To install and use the **BTC.com API (BTC.com Explorer & Pool API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/btccom-api-btccom-explorer-pool-api](https://vinkius.com/mcp/btccom-api-btccom-explorer-pool-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
