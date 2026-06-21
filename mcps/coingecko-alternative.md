# CoinGecko MCP Server

Access real-time cryptocurrency prices, market data, and on-chain analytics from the world's leading crypto data aggregator.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coingecko-alternative)

## Overview
**Category:** data-analytics
**Tools Count:** 29

## Description
Connect your **CoinGecko** API to any AI agent to transform it into a powerful financial analyst. Get instant access to thousands of tokens, global market statistics, and deep exchange data through natural conversation.

### What you can do

- **Real-time Pricing** — Fetch current prices for thousands of coins across multiple fiat and crypto currencies using `get_simple_price`.
- **Market Insights** — Analyze market caps, 24h volumes, and price changes with `list_coins_markets` to identify market trends.
- **On-chain Intelligence** — Inspect specific tokens and networks directly from the blockchain using `get_onchain_token` and `list_onchain_networks`.
- **Trending & Global Data** — Stay ahead of the curve by querying `get_trending` coins or checking the `get_global` market overview.
- **Exchange & NFT Data** — List active exchanges, check trading pairs with `get_coin_tickers`, or explore NFT floor prices and contract data.

### How it works

1. Subscribe to this server
2. Enter your CoinGecko API Key (Demo or Pro)
3. Start querying crypto data from Claude, Cursor, or any MCP-compatible client

No more manual searching through charts. Your AI can now calculate portfolio values, find trending assets, and monitor market volatility in real-time.

### Who is this for?

- **Crypto Traders** — instantly get price updates and market sentiment without leaving your terminal or chat.
- **Web3 Developers** — fetch contract addresses, platform IDs, and on-chain data directly into your coding environment.
- **Financial Analysts** — automate the collection of historical data and global market metrics for reporting.


## Available Tools
- **list_asset_platforms**: List all asset platforms
- **get_coin_history**: Get historical data at a given date
- **get_coin_market_chart_range**: Get historical market data within a range of timestamp
- **get_coin_market_chart**: Get historical market data
- **get_coin_ohlc**: Get coin OHLC data
- **get_coin_tickers**: Get coin tickers
- **get_coin**: including exchange tickers) for a coin.

Get current data for a coin
- **list_coins**: List all supported coins id, name and symbol
- **list_coins_markets**: List all supported coins price, market cap, volume, and market related data
- **get_exchange_tickers**: Get exchange tickers
- **get_exchange**: Get exchange volume in BTC and tickers
- **get_exchange_volume_chart**: Get volume chart data for an exchange
- **list_exchanges_markets**: List all supported markets id and name
- **list_exchanges**: List all exchanges
- **get_global_defi**: Get top 100 cryptocurrencies global DeFi data
- **get_global**: Get cryptocurrency global data
- **get_nft_by_contract**: Get NFT data by contract address
- **get_nft**: ) for an NFT collection.

Get current data for an NFT collection
- **list_nfts**: List all supported NFT collections
- **list_onchain_dexes**: List supported DEXes on a network
- **list_onchain_networks**: List all supported networks on GeckoTerminal
- **get_onchain_pool**: Get liquidity pool data by address
- **get_onchain_pool_trades**: Get latest trades from a pool
- **get_onchain_token**: Get token data by contract address
- **get_public_treasury**: g., bitcoin, ethereum).

Get public companies holdings for a specific coin
- **get_simple_price**: Get current price of cryptocurrencies
- **get_simple_token_price**: Get current price of tokens for a given platform
- **get_supported_vs_currencies**: Get list of supported vs currencies
- **get_trending**: Get trending search coins


## Installation & Usage

To install and use the **CoinGecko** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coingecko-alternative](https://vinkius.com/mcp/coingecko-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
