# Covalent MCP Server

Equip your AI agent to query unified blockchain data including balances, transactions, and NFTs across 100+ chains.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/covalent)

## Overview
**Category:** databases
**Tools Count:** 10

## Description
Integrate **Covalent**, the unified API for blockchain data, directly into your AI workflow. Access real-time and historical data across Ethereum, Polygon, Binance Smart Chain, and over 100 other supported networks using natural language.

### What you can do

- **Wallet Insights** — Retrieve token balances, historical portfolio values, and transaction history for any wallet address.
- **NFT Discovery** — List NFT balances and metadata across supported chains.
- **Transaction Auditing** — Get full details and log events for specific transaction hashes.
- **Network Monitoring** — Check block details and monitor supported chain statuses.

### How it works

1. Connect the Covalent integration to your AI assistant.
2. Authorize using your Covalent API Key (found in your dashboard at covalenthq.com).
3. Query global blockchain data through intuitive conversation.

### Who is this for?

- **Web3 Developers** — Quickly audit smart contract interactions and verify transaction logs.
- **Crypto Investors** — Track portfolio performance and monitor wallet activities across multiple chains.
- **Data Analysts** — Retrieve structured on-chain data for research and reporting via chat.


## Available Tools
- **get_token_balances**: Resolves contract addresses, ticker symbols, token decimals, and current balances (formatted and raw) for the specified wallet and chain.

Get token balances for a wallet address on a specific chain
- **get_block_details**: Resolves block hashes, parent hashes, timestamps, and transaction counts for the specified chain.

Get details for a specific block height
- **get_chains_status**: Resolves block height lag, current sync status, and API availability across all supported networks.

Get the current indexing status of all supported chains
- **get_dex_pools**: Resolves liquidity pool addresses, token pairs, reserve amounts, and volume metrics for the specified DEX.

List liquidity pools for a DEX on a specific chain
- **get_nft_balances**: Resolves NFT contract names, token IDs, metadata URLs, and image links across the specified blockchain network.

Get NFT balances for a wallet address
- **get_historical_portfolio**: Resolves daily balances, asset valuations in USD, and historical price points for the specified wallet.

Get historical daily portfolio value for a wallet address
- **get_token_transfers**: Resolves sender/receiver addresses, transfer values, and transaction timestamps for the specified wallet.

Get historical token transfers for a wallet address
- **get_transaction_details**: Touches raw log events, decoded event parameters, and gas consumption metrics boundary.

Get full details and logs for a specific transaction hash
- **get_transactions**: Resolves transaction hashes, block heights, timestamps, and log events for the specified wallet on the given chain.

Get transaction history for a wallet address
- **list_supported_chains**: Resolves chain IDs, human-readable names, and supported features (NFTs, Dex, etc.) for each blockchain.

List all blockchains supported by Covalent


## Installation & Usage

To install and use the **Covalent** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/covalent](https://vinkius.com/mcp/covalent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
