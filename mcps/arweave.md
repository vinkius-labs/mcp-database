# Arweave MCP Server

Interact with the Arweave permaweb — query network info, check wallet balances, inspect transactions, and calculate storage costs directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/arweave)

## Overview
**Category:** developer-tools
**Tools Count:** 13

## Description
Connect to the **Arweave** network and manage permanent data storage through natural conversation. This MCP server allows your AI agent to query the blockweave, check transaction statuses, and interact with the permaweb ecosystem.

### What you can do

- **Network Monitoring** — Get real-time network status, height, and peer information using `get_network_info` and `get_peers`.
- **Transaction Inspection** — Retrieve transaction metadata, status, and raw data using unique IDs with `get_transaction` and `get_transaction_data`.
- **Wallet Management** — Check balances in Winstons and find the last transaction for any wallet address via `get_wallet_balance`.
- **Storage Economics** — Calculate the exact cost to store data on the permaweb with `get_storage_price`.
- **Advanced Querying** — Use `query_graphql` to search for specific data and tags across the entire network.

### How it works

1. Subscribe to this server
2. (Optional) Provide a custom Arweave Gateway URL
3. Start querying the permaweb from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly check transaction confirmations and network status without leaving the terminal or IDE.
- **Data Analysts** — query the permaweb using GraphQL to extract insights from permanent data.
- **Crypto Users** — monitor wallet balances and storage costs for permanent file uploads.


## Available Tools
- **get_block_by_hash**: Retrieve a block by its hash
- **get_block_by_height**: Retrieve a block by its height
- **get_storage_price**: Get the cost in Winstons to store data
- **get_transaction_data**: Retrieve the data associated with a transaction
- **get_transaction_offset**: Get the byte offset and size of the transaction data
- **get_transaction_status**: g., pending, confirmed).

Get the status of a transaction
- **get_transaction**: Retrieve a transaction by its ID
- **get_wallet_balance**: Get the balance of a wallet address in Winstons
- **get_wallet_last_tx**: Get the ID of the last transaction sent by the wallet
- **get_network_info**: Get current Arweave network status
- **get_peers**: Get a list of peer addresses known to the node
- **query_graphql**: Execute a GraphQL query against the Arweave network
- **submit_transaction**: Submit a new transaction to the network


## Installation & Usage

To install and use the **Arweave** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arweave](https://vinkius.com/mcp/arweave)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
