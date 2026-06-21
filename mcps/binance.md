# Binance MCP Server

Get real-time cryptocurrency prices, order books, candlesticks and trades from Binance exchange.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/binance)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
Connect to **Binance** and access the world's largest cryptocurrency exchange through natural conversation — no API key needed for public data.

### What you can do

- **Live Prices** — Get current prices for any trading pair instantly
- **24h Statistics** — View 24h price changes, volume, high/low and trade counts
- **Order Book** — Analyze market depth with bids and asks up to 5000 levels
- **Candlesticks** — Retrieve OHLCV data with 15 timeframes (1m to 1 month)
- **Recent Trades** — See the latest individual and aggregated trades
- **Exchange Info** — Explore all trading pairs, rules and filters

### How it works

1. Subscribe to this server
2. No API key needed for public market data
3. Get crypto data from Claude, Cursor, or any MCP-compatible client

No API key required for public data — completely free.

### Who is this for?

- **Traders** — check real-time prices, analyze order books and review recent trades
- **Analysts** — explore OHLC data with multiple timeframes and scan 24h market statistics
- **Developers** — access crypto market data without authentication for dashboards and bots


## Available Tools
- **get_24h_ticker**: Includes last price, 24h change (price and %), high/low, volume (base and quote), number of trades and open interest. Useful for market overview and scanning.

Get 24-hour rolling window price change statistics
- **get_server_time**: Returns Unix timestamp in milliseconds and ISO string. Useful for synchronizing with the exchange server.

Get Binance server time
- **get_agg_trades**: Each aggregated trade includes trade ID, price, quantity, first/last trade IDs, timestamp and whether buyer was maker. More efficient than individual trades for high-volume pairs. Returns up to 500 (default) or 1000 trades.

Get compressed/aggregated trades for a trading pair
- **get_exchange_info**: Returns all trading pairs, their status, base/quote assets, order types, filters (price, quantity, notional) and permissions. Optionally filter by a specific symbol.

Get exchange trading rules and symbol info
- **get_klines**: Supports intervals: 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M. Optionally set limit (max 1000, default 500) and time range with startTime/endTime (Unix timestamp ms). Useful for technical analysis and charting.

Get candlestick (OHLCV) chart data for a trading pair
- **get_order_book**: Each level includes price and quantity. The limit parameter controls the number of levels (5, 10, 20, 50, 100, 500, 1000, 5000). Useful for analyzing market depth, spread and liquidity.

Get current order book (bids and asks) for a trading pair
- **get_ticker_price**: Returns symbol and current price. If no symbol is specified, returns all pairs. Fastest way to get current prices.

Get latest price for trading pair(s)
- **get_trades**: Each trade includes trade ID, price, quantity, time, whether buyer was maker and if it was the best price match. Returns up to 500 trades (default 500, max 1000 via limit). Useful for analyzing recent market activity.

Get recent individual trades for a trading pair


## Installation & Usage

To install and use the **Binance** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/binance](https://vinkius.com/mcp/binance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
