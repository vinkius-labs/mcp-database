# CoinLore MCP Server

Access real-time cryptocurrency data, market stats, exchange info, and social metrics directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coinlore)

## Overview
**Category:** data-analytics
**Tools Count:** 11

## Description
Connect to the **CoinLore** API to empower your AI agent with comprehensive cryptocurrency market intelligence and real-time blockchain data.

### What you can do

- **Market Overview** — Get global cryptocurrency statistics including total market cap, volume, and BTC/ETH dominance.
- **Ticker Data** — Retrieve detailed price, volume, and supply data for thousands of coins using specific IDs.
- **Market Movers** — Instantly identify the top 20 gainers and losers across different timeframes (1h, 24h, 7d).
- **Historical Analysis** — Access 365 days of daily OHLCV (Open, High, Low, Close, Volume) history for deep trend analysis.
- **Exchange Intelligence** — List all supported exchanges and inspect specific trading pairs and top 100 markets.
- **Social Sentiment** — Monitor social media metrics from Twitter and Reddit to gauge community engagement for specific assets.

### How it works

1. Subscribe to this server
2. No API key is required for the public tier; simply initialize the connection
3. Start querying crypto markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders & Investors** — Quickly check market movers and coin-specific metrics without switching to a browser.
- **Data Analysts** — Fetch historical OHLCV data and global stats directly into your analysis environment.
- **Developers** — Integrate crypto pricing and metadata into your workflow using natural language commands.


## Available Tools
- **list_assets**: Get a lightweight list of all coins
- **get_coin_info**: Get static metadata for a specific coin
- **get_coin_markets**: Get top 50 exchanges and markets for a coin
- **get_exchange**: Get exchange details and top 100 trading pairs
- **list_exchanges**: Get all exchanges listed on CoinLore
- **get_global_stats**: Get overall cryptocurrency market statistics
- **get_movers**: Get top 20 winners and losers
- **get_ohlcv**: Get 365 days of daily OHLCV history
- **get_social_stats**: Get social media metrics for a coin
- **get_ticker**: Retrieve detailed tick data for specific coins
- **list_tickers**: Retrieve tick data for multiple coins


## Installation & Usage

To install and use the **CoinLore** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coinlore](https://vinkius.com/mcp/coinlore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
