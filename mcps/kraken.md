# Kraken MCP Server

Get real-time cryptocurrency prices, OHLC data, order books and trades from Kraken exchange.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kraken)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
Connect to **Kraken** and access real-time cryptocurrency market data through natural conversation — no API key needed for public data.

### What you can do

- **Live Tickers** — Get current prices, 24h volume, VWAP and high/low for any trading pair
- **OHLC Candles** — Retrieve candlestick data with multiple timeframes (1m to 15d)
- **Order Book** — View current bids and asks with market depth analysis
- **Recent Trades** — See the most recent completed trades with price, volume and side
- **Asset Info** — Get details about all supported cryptocurrencies and fiat currencies
- **Trading Pairs** — Explore all available trading pairs with their specifications
- **Spread Data** — Analyze bid/ask spreads for liquidity assessment

### How it works

1. Subscribe to this server
2. No API key needed for public market data
3. Get crypto data from Claude, Cursor, or any MCP-compatible client

No API key required for public data — completely free.

### Who is this for?

- **Traders** — check real-time prices, analyze order books and review recent trades
- **Analysts** — explore OHLC data, compare spreads across pairs and monitor market trends
- **Developers** — access crypto market data without authentication for dashboards and bots


## Available Tools
- **get_asset_info**: Returns asset name, alternate names, decimals, status and collateral support. Optionally filter by specific assets (comma-separated).

Get information about Kraken assets
- **get_asset_pairs**: Returns pair name, alt name, base/quote assets, lot volume decimals, pair decimals, order minimums and trading leverage. Optionally filter by a specific pair.

Get information about Kraken trading pairs
- **get_ohlc**: Each candle includes time, open, high, low, close, VWAP, volume and trade count. Supports intervals: 1 (1min), 5, 15, 30, 60 (1h), 240 (4h), 1440 (1d), 10080 (1w), 21600 (15d). Optionally provide since timestamp for incremental data.

Get OHLCV candlestick data for a trading pair
- **get_order_book**: Each level includes price and volume. The count parameter controls the number of levels returned (1-500, default 100). Useful for analyzing market depth and liquidity.

Get the current order book for a trading pair
- **get_server_time**: Returns the Unix timestamp and RFC 1123 time. Useful for synchronizing with the exchange server and verifying API connectivity.

Get Kraken server time
- **get_spread**: Returns recent spreads with bid price, ask price, time (Unix timestamp) and volume. Useful for analyzing liquidity and trading costs.

Get recent spread data for a trading pair
- **get_ticker**: Returns best bid/ask prices, last trade price, 24h volume, VWAP, high/low prices and trade counts. Pair names can be standard (XBTUSD) or alt (BTCUSD). Multiple pairs comma-separated.

Get current ticker information for trading pairs
- **get_trades**: Each trade includes price, volume, time (Unix timestamp), side (buy/sell), order type (market/limit) and misc info. Returns up to 1000 most recent trades. Optionally provide since timestamp for pagination.

Get recent trades for a trading pair


## Installation & Usage

To install and use the **Kraken** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kraken](https://vinkius.com/mcp/kraken)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
