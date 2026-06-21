# Irys MCP Server

Manage permanent data storage on Irys — check storage prices, query transactions via GraphQL, and manage balances across multiple tokens.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/irys)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect to **Irys**, the provenance layer for permanent data storage. This MCP server enables your AI agent to interact with Irys nodes to handle data uploads, verify storage costs, and explore historical transactions.

### What you can do

- **Storage Economics** — Use `get_price` to calculate exact costs for data storage in atomic units for tokens like Ethereum or Solana.
- **Data Discovery** — Search through permanent records using `query_transactions` with GraphQL filters for specific tags and values.
- **Account Oversight** — Monitor wallet balances with `get_balance` and manage node funding or withdrawals via `fund_account` and `withdraw_account`.
- **Transaction Metadata** — Retrieve detailed status and tags for any specific transaction ID using `get_transaction`.
- **Node Status** — Get real-time metadata about the Irys node configuration and supported features using `get_info`.

### How it works

1. Subscribe to this server
2. Provide your Irys Node URL (Mainnet or Devnet)
3. Start interacting with the permanent web through your AI agent

### Who is this for?

- **Web3 Developers** — quickly check upload prices and transaction statuses without leaving the terminal or IDE.
- **Data Analysts** — query historical data tags on the provenance layer to track on-chain activity.
- **DevOps Engineers** — automate the monitoring of Irys node balances and funding status.


## Available Tools
- **get_balance**: Get balance for a specific address
- **fund_account**: Submit a funding transaction receipt
- **get_transaction**: Retrieve metadata for a specific transaction ID
- **get_info**: Get Irys node metadata
- **get_price**: Get storage price for a specific token and data size
- **query_transactions**: Use this to find historical transactions by tag.

Search and filter transaction metadata via GraphQL
- **submit_transaction**: Submit a signed data transaction
- **withdraw_account**: Initiate a withdrawal request


## Installation & Usage

To install and use the **Irys** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/irys](https://vinkius.com/mcp/irys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
