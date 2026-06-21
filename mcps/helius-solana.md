# Helius (Solana) MCP Server

Access high-performance Solana data—fetch assets, balances, transaction history, and priority fee estimates directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/helius-solana)

## Overview
**Category:** developer-tools
**Tools Count:** 14

## Description
Connect your **Helius** account to any AI agent to interact with the Solana blockchain with unprecedented speed and depth. This server leverages Helius's powerful RPC and DAS (Digital Asset Standard) API to provide real-time blockchain intelligence.

### What you can do

- **Asset Management** — Fetch detailed metadata for NFTs, cNFTs, and fungible tokens using `get_asset` or `get_asset_batch`.
- **Wallet Intelligence** — Retrieve complete balances with real-time USD pricing using `get_wallet_balances` and track history with `get_wallet_history`.
- **Ownership Tracking** — List every asset owned by a specific Solana address via `get_assets_by_owner`.
- **Network Optimization** — Get precise priority fee estimates with `get_priority_fee_estimate` to ensure your transactions land during high congestion.
- **Advanced Search** — Query the blockchain for specific assets based on collection, creator, or attributes using `search_assets`.

### How it works

1. Subscribe to this server
2. Enter your Helius API Key
3. Start querying Solana data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug smart contracts and verify on-chain state without leaving your IDE.
- **Crypto Analysts** — Perform deep wallet forensics and portfolio tracking through natural language.
- **NFT Collectors** — Manage and inspect compressed NFTs and collections with ease.


## Available Tools
- **get_asset_batch**: Get multiple assets in one call
- **get_asset_proof**: Get Merkle proof for compressed NFTs
- **get_asset**: Get detailed data for a specific Solana asset
- **get_assets_by_owner**: List all assets owned by a wallet
- **get_priority_fee_estimate**: Recommended to provide the serialized transaction.

Get precise priority fee estimates
- **get_token_accounts**: Get all token accounts for a mint or owner
- **get_transaction_history**: Get enhanced transaction history for an address
- **get_wallet_balances**: Get token and NFT balances with USD values
- **get_wallet_funded_by**: Identify the original funding source of a wallet
- **get_wallet_history**: Get complete transaction history for a wallet
- **get_wallet_identity**: sol domains.

Resolve address to known entities
- **get_wallet_transfers**: Get incoming and outgoing token transfers
- **parse_transactions**: Parse raw transactions into human-readable data
- **search_assets**: Search for assets with advanced filtering


## Installation & Usage

To install and use the **Helius (Solana)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helius-solana](https://vinkius.com/mcp/helius-solana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
