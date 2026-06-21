# TzKT (Tezos Indexer & Explorer API) MCP Server

Access real-time Tezos blockchain data — explore accounts, smart contracts, and transaction history directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tzkt-tezos-indexer-explorer-api)

## Overview
**Category:** developer-tools
**Tools Count:** 25

## Description
Connect to the **TzKT API**, the most advanced indexer for the Tezos blockchain. This MCP server allows your AI agent to query live on-chain data, analyze smart contract storage, and track financial operations across Mainnet and testnets.

### What you can do

- **Account Exploration** — List accounts by balance or activity and fetch detailed profiles including balance history.
- **Smart Contract Auditing** — Inspect contract code (Michelson/Micheline), current storage, and available entrypoints for any KT1 address.
- **Transaction Tracking** — Search operations by hash or list transactions with advanced filters like sender, target, and amount.
- **Financial Reporting** — Generate JSON-based activity reports for specific Tezos addresses.
- **Multi-Network Support** — Seamlessly switch between Mainnet, Ghostnet, and Shadownet.

### How it works

1. Subscribe to this server
2. (Optional) Enter your TzKT API Key for higher rate limits
3. Start querying the Tezos ledger from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug smart contracts and verify storage states directly from your IDE.
- **Data Analysts** — Extract historical balance data and transaction flows for Tezos accounts.
- **DeFi Users** — Monitor wallet activity and track specific operation hashes without leaving the chat interface.


## Available Tools
- **get_account_balance_history**: Get historical balance changes for an account
- **get_account_report**: Generate a JSON report of account activity
- **get_account**: Get detailed information for a specific account
- **get_baker_rewards**: Get baker rewards per cycle
- **get_block**: Get block details by level or hash
- **get_contract_code**: Get contract Michelson or Micheline code
- **get_contract_entrypoints**: List available contract entrypoints
- **get_contract_storage**: Get current or historical contract storage
- **get_delegator_rewards**: Get delegator rewards per cycle
- **get_head**: Get the current state of the indexer and blockchain head
- **get_operations_by_hash**: Get operations by transaction hash
- **get_statistics**: Get network-wide statistics (TPS, volume, etc.)
- **list_accounts**: Supports filtering by balance, activity, and type.

List accounts with filters
- **list_bigmap_keys**: List keys in a specific big map
- **list_bigmap_updates**: Get update history for a big map
- **list_bigmaps**: List all big maps
- **list_blocks**: List blocks with filters
- **list_contracts**: List smart contracts with filters
- **list_delegations**: List delegation operations
- **list_originations**: List contract origination operations
- **list_staking**: List staking-related operations
- **list_token_balances**: Get token balances for specific accounts
- **list_token_definitions**: Get token metadata and definitions
- **list_token_transfers**: List token transfers (FA1.2 / FA2)
- **list_transactions**: List transactions with advanced filtering


## Installation & Usage

To install and use the **TzKT (Tezos Indexer & Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tzkt-tezos-indexer-explorer-api](https://vinkius.com/mcp/tzkt-tezos-indexer-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
