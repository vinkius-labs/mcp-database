# Zerion (DeFi Portfolio) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zerion-defi-portfolio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zerion-defi-portfolio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zerion-defi-portfolio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track DeFi portfolios, NFT holdings, and transaction history across 500+ protocols and multiple chains via Zerion.

## Description
Connect your AI agent to the **Zerion** API to gain deep insights into any Web3 wallet. This server enables real-time monitoring of DeFi positions, NFT valuations, and historical performance across all major blockchains.

### What you can do

- **Portfolio Overview** — Get total value, asset distribution, and net worth for any wallet address or a set of multiple addresses.
- **DeFi & Token Positions** — Inspect specific fungible token balances and complex DeFi positions (liquidity pools, lending, etc.).
- **Transaction History** — Retrieve human-readable transaction logs to understand past on-chain activity.
- **PnL Analysis** — Calculate realized and unrealized gains to track investment performance over time.
- **NFT Analytics** — Fetch NFT portfolio values, individual holdings, and collection-grouped data.
- **Market Data** — List supported chains, dApps, and check real-time gas prices across networks.

### How it works

1. Subscribe to this server
2. Enter your Zerion API Key
3. Start querying on-chain data from Claude, Cursor, or any MCP-compatible client

No more manual searching on block explorers. Your AI acts as a personal crypto analyst, providing instant data on any wallet's health and history.

### Who is this for?

- **Crypto Investors** — quickly check your total net worth and PnL without opening multiple apps.
- **Web3 Developers** — integrate wallet balance and transaction checks directly into your development workflow.
- **Data Analysts** — aggregate data from multiple wallets to identify trends or audit holdings.


## Available Tools
- **list_chains**: List supported blockchains and metadata
- **list_dapps**: List metadata for decentralized applications
- **get_fungible**: Get token metadata, prices, and charts
- **list_gas_prices**: Get real-time gas estimates across chains
- **get_nft**: Look up specific NFTs by reference
- **get_swap_quotes**: Get quotes for same-chain swaps or cross-chain bridges
- **get_wallet_nft_collections**: Get NFT holdings grouped by collection for a wallet
- **get_wallet_nft_portfolio**: Get NFT value summary for a wallet
- **get_wallet_nft_positions**: Get individual NFT holdings for a wallet
- **get_wallet_pnl**: Get realized and unrealized gains (PnL) for a wallet
- **get_wallet_portfolio**: Get total value and distribution for a wallet
- **get_wallet_positions**: Get list of tokens and DeFi positions for a wallet
- **get_wallet_set_portfolio**: Get aggregated portfolio for multiple wallets
- **get_wallet_set_positions**: Get aggregated positions for multiple wallets
- **get_wallet_set_transactions**: Get aggregated transactions for multiple wallets
- **get_wallet_transactions**: Get human-readable transaction history for a wallet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zerion (DeFi Portfolio)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total portfolio value and asset distribution for wallet 0x71C7656EC7ab88b098defB751B7401B5f6d8976F?"

**🤖 AI Agent:**
> I've analyzed the wallet. The total net worth is approximately $42,500. The distribution is 60% ETH, 25% USDC, and 15% in various DeFi positions like Uniswap V3 liquidity pools.

---

**👤 You:**
> "Show me the last 5 transactions for address 0x123... and explain what happened."

**🤖 AI Agent:**
> Fetching transaction history... In the last 5 activities: you swapped 1 ETH for 2,500 DAI on 1inch, received 500 MATIC from an external wallet, and paid gas for a minting transaction on OpenSea. Would you like details on the gas fees for these?

---

**👤 You:**
> "What is the current PnL for wallet 0xabc... in USD?"

**🤖 AI Agent:**
> The wallet currently shows a total PnL of +$12,400. This includes $8,000 in realized gains from past sales and $4,400 in unrealized gains from your current ETH and AAVE holdings.


## Installation & Usage

To install and use the **Zerion (DeFi Portfolio)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zerion-defi-portfolio](https://vinkius.com/mcp/zerion-defi-portfolio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
