# DexScreener MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dexscreener)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dexscreener-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dexscreener-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [defi](../categories/defi.md)

Real-time DEX trading data — search pairs, track prices, monitor liquidity and volume across all chains.

## Description
Connect **DexScreener** to any AI agent and get instant access to real-time DEX market data across all major blockchains. Search tokens, check prices, monitor liquidity, and discover trending tokens — all through natural conversation.

### What you can do
- **Token Search** — Find any token or trading pair by name, symbol, or address
- **Price Tracking** — Get real-time prices in USD and native tokens
- **Liquidity & Volume** — Check 24h volume, liquidity depth, and market cap
- **Trending Tokens** — Discover boosted and trending tokens getting community attention
- **Multi-Chain** — Query data across Solana, Ethereum, BSC, Base, Arbitrum, and more
- **Batch Queries** — Check up to 30 tokens at once for portfolio snapshots

### How it works
1. Subscribe to this server
2. No authentication needed — DexScreener API is free and public
3. Start searching tokens and tracking prices from Claude, Cursor, or any MCP client

### Who is this for?
- **Traders** — Quick price checks, liquidity monitoring, and token discovery
- **Researchers** — Track new tokens, compare DEX volumes, and analyze trends
- **DeFi Users** — Find the best liquidity pools and check token prices before swapping


## Available Tools
- **get_multiple_tokens**: Useful for batch checking prices, comparing multiple tokens, or building portfolio snapshots. All tokens must be on the same chain.

Get data for multiple tokens at once (up to 30)
- **get_pair**: Returns exact price, liquidity, volume, and market cap data. Use this after finding a pair through search to get the precise pair address, or if you already know the contract address.

Get specific trading pair by chain and pair address
- **get_token_boosts**: Shows which tokens are getting community attention right now. Useful for spotting trending and hyped tokens.

Get currently boosted/trending tokens
- **get_token_pairs**: Useful for finding all markets where a token is traded, comparing prices across DEXes, and identifying the most liquid pair for a token.

Get all trading pairs for a specific token
- **get_token_profiles**: Shows new tokens being tracked on the platform. Useful for discovering newly listed tokens before they gain traction.

Get latest token profiles on DexScreener
- **get_top_boosts**: Shows which tokens have the most community promotion activity. Useful for identifying tokens with strong community backing and marketing efforts.

Get top boosted tokens by total boost amount
- **search_pairs**: Returns up to 30 matching pairs with price, volume, liquidity, and DEX information. Use token symbols like "SOL", "PEPE", or pair names like "SOL/USDC". Essential for discovering new tokens and tracking existing ones across all supported chains.

Search for trading pairs on DexScreener


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DexScreener** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for PEPE token pairs and show me the top result."

**🤖 AI Agent:**
> 📊 **PEPE/ETH** on Ethereum: $0.00000842 | 24h Vol: $45.2M | Liquidity: $12.8M | MC: $3.5B. Top pair on Uniswap V2 with $8.1M daily volume.

---

**👤 You:**
> "What are the top boosted tokens right now?"

**🤖 AI Agent:**
> 🔥 Top 3 boosted: 1) **$NEON** (Solana) - 15.2k boosts, 2) **$CAT** (BSC) - 12.8k boosts, 3) **$MOON** (Base) - 9.4k boosts.

---

**👤 You:**
> "Check prices for SOL, ETH, and MATIC on Ethereum."

**🤖 AI Agent:**
> 📊 Prices: **SOL** $142.50 (↑3.2%), **ETH** $2,450.30 (↑1.8%), **MATIC** $0.72 (↓0.5%). All showing normal trading volume.


## Installation & Usage

To install and use the **DexScreener** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dexscreener](https://vinkius.com/mcp/dexscreener)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
