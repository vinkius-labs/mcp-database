# DexScreener MCP Server

Real-time DEX trading data — search pairs, track prices, monitor liquidity and volume across all chains.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dexscreener)

## Overview
**Category:** defi
**Tools Count:** 7

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


## Installation & Usage

To install and use the **DexScreener** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dexscreener](https://vinkius.com/mcp/dexscreener)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
