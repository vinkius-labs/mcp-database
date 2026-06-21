# Metisscan (Metis L2 Network Explorer) MCP Server

Explore the Metis L2 network — inspect blocks, transactions, addresses, and smart contracts directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/metisscan-metis-l2-network-explorer)

## Overview
**Category:** developer-tools
**Tools Count:** 26

## Description
Connect your AI agent to the **Metis L2** ecosystem through Metisscan. Gain real-time visibility into the blockchain, from high-level network stats to granular smart contract data.

### What you can do

- **Network Monitoring** — List recent blocks and transactions or fetch the current block height using standard EVM methods.
- **Address Auditing** — Retrieve balances, transaction histories, and token holdings for any wallet or contract address.
- **Transaction Analysis** — Inspect transaction details, internal calls, and event logs to debug or track fund movements.
- **Smart Contract Insights** — Access contract source code, verification configurations, and interact with contracts via `eth_call` or `executeGraphql`.
- **Token Tracking** — List network tokens, check holders, and monitor transfers across the Metis Layer 2 ecosystem.

### How it works

1. Subscribe to this server
2. Enter your Metisscan API Key
3. Start querying the Metis L2 network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug transactions and verify contract states without leaving your IDE.
- **Data Analysts** — Extract on-chain data and token metrics for research or reporting.
- **Crypto Power Users** — Track wallet activities and monitor network congestion through natural language.


## Available Tools
- **eth_block_number**: Get the most recent block number (RPC)
- **eth_call**: Execute a message call (RPC)
- **eth_estimate_gas**: Estimate gas for a transaction (RPC)
- **eth_get_balance**: Get address balance (RPC)
- **eth_get_block_by_number**: Get block by number (RPC)
- **eth_get_code**: Get code at address (RPC)
- **eth_get_transaction_by_hash**: Get transaction by hash (RPC)
- **eth_get_transaction_receipt**: Get transaction receipt (RPC)
- **get_address_counters**: g., transaction count) for a specific address.

Get transaction and token counters for an address
- **get_address_tokens**: List token balances for an address
- **get_address**: Get details for an address
- **get_address_transactions**: List transactions for an address
- **get_block**: Get details for a specific block
- **get_block_transactions**: List transactions in a block
- **get_smart_contract**: Get details for a smart contract
- **get_smart_contract_verification_config**: Get verification configuration for a smart contract
- **get_token_holders**: List token holders
- **get_token**: Get details for a specific token
- **get_token_transfers**: List token transfers
- **get_transaction_internal_transactions**: g., contract calls) triggered by a specific transaction.

List internal transactions for a transaction
- **get_transaction_logs**: List event logs for a transaction
- **get_transaction**: Get details for a specific transaction
- **graphql_query**: Execute a GraphQL query on Metisscan
- **list_blocks**: List recent blocks on Metis L2
- **list_tokens**: List tokens on the network
- **list_transactions**: List recent transactions on Metis L2


## Installation & Usage

To install and use the **Metisscan (Metis L2 Network Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metisscan-metis-l2-network-explorer](https://vinkius.com/mcp/metisscan-metis-l2-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
