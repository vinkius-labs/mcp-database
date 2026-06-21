# CryptoCompare (Crypto Market Data) MCP Server

Access real-time and historical cryptocurrency market data, news, and top coins directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cryptocompare-crypto-market-data)

## Overview
**Category:** finance-accounting
**Tools Count:** 13

## Description
Connect your **CryptoCompare** account to any AI agent to access institutional-grade cryptocurrency market data through natural conversation.

### What you can do

- **Real-time Pricing** — Fetch current prices for single or multiple cryptocurrencies across various fiat and crypto pairs using `get_price` and `get_price_multi`.
- **Historical Data** — Retrieve OHLCV (Open, High, Low, Close, Volume) data at daily, hourly, or minute intervals with `get_historical_daily`, `get_historical_hourly`, and `get_historical_minute`.
- **Market Insights** — List top coins by market cap and identify the highest volume trading pairs for any asset using `get_top_mktcap` and `get_top_pairs`.
- **News & Sentiment** — Stay updated with the latest crypto news, categorized feeds, and industry updates via `get_latest_news`.
- **Global Coverage** — Access a comprehensive list of all supported coins and exchanges in the CryptoCompare ecosystem.

### How it works

1. Subscribe to this server
2. Enter your CryptoCompare API Key
3. Start querying crypto markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders & Investors** — Get instant price checks and historical trends without leaving your workflow.
- **Developers** — Integrate market data into your code or research directly from your IDE.
- **Analysts** — Perform deep market cap and volume analysis using natural language queries.


## Available Tools
- **get_historical_daily**: Get daily historical OHLCV data
- **get_historical_hourly**: Get hourly historical OHLCV data
- **get_historical_minute**: Get minute historical OHLCV data
- **get_latest_news**: Get the latest cryptocurrency news
- **get_price_multi_full**: Get full 24h market data for multiple cryptocurrencies
- **get_price_multi**: Get the current price of multiple cryptocurrencies
- **get_price**: Get the current price of any cryptocurrency in any other currency
- **get_top_mktcap**: Get top coins by market cap
- **get_top_pairs**: Get top trading pairs by volume
- **list_all_coins**: List all supported cryptocurrencies
- **list_all_exchanges**: List all supported exchanges
- **list_news_categories**: List available news categories
- **list_news_feeds**: List available news feeds


## Installation & Usage

To install and use the **CryptoCompare (Crypto Market Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cryptocompare-crypto-market-data](https://vinkius.com/mcp/cryptocompare-crypto-market-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
