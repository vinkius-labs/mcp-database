# Bybit MCP Server

Access real-time crypto market data — tickers, klines, orderbook, trades, funding rates and open interest.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bybit)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Connect to **Bybit** and access real-time cryptocurrency market data through natural conversation — no API key needed for public market data.

### What you can do

- **Tickers** — Get real-time prices, 24h change, high/low and volume for any trading pair
- **Klines** — Fetch candlestick/OHLCV data for technical analysis across all timeframes
- **Orderbook** — View current market depth (bids and asks) for any pair
- **Recent Trades** — See the latest executed trades with price, size and side
- **Mark/Index Price** — Get mark price and index price candlesticks for derivatives
- **Funding Rates** — Check historical funding rates for perpetual contracts
- **Open Interest** — Track open interest changes over time
- **Instruments** — Browse all available trading pairs and contract specifications

### How it works

1. Subscribe to this server
2. No API key needed for public market data
3. Start exploring crypto market data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders** — check real-time prices, orderbook depth and recent trades before executing
- **Analysts** — access OHLCV data, funding rates and open interest for technical analysis
- **Developers** — integrate crypto market data into trading bots and dashboards


## Available Tools
- **get_funding_history**: Funding rates are paid every 8 hours between long and short positions. Positive rate means longs pay shorts. Categories: "linear", "inverse". Limit: 1-200 records.

Get funding rate history for perpetual contracts
- **get_index_price_kline**: Index price is the composite price from multiple exchanges. Categories: "linear", "inverse".

Get index price candlestick data
- **get_instruments**: Categories: "spot", "linear", "inverse", "option". Filter by symbol or base coin.

Get trading instruments (pairs/contracts) info
- **get_kline**: Intervals: 1,3,5,15,30,60,120,240,360,720 (minutes), D (daily), W (weekly), M (monthly). Use start and end timestamps (milliseconds) for historical data. Limit: 1-1000 candles. Categories: "spot", "linear", "inverse".

Get candlestick (kline) data for technical analysis
- **get_mark_price_kline**: Mark price is used for liquidation calculations. Intervals same as kline. Categories: "linear", "inverse".

Get mark price candlestick data for derivatives
- **get_open_interest**: Open interest shows total number of open positions. Intervals: 5min, 15min, 30min, 1h, 4h, 1d. Categories: "linear", "inverse".

Get open interest history for a derivatives contract
- **get_orderbook**: Returns price levels and quantities. Limit: 1-200 (spot), 1-500 (linear/inverse/option). Useful for analyzing market depth and liquidity.

Get the current orderbook (bids and asks) for a symbol
- **get_recent_trades**: Returns trade price, size, side (Buy/Sell), timestamp and trade ID. Useful for seeing current market activity and order flow. Limit: 1-1000 trades.

Get recent executed trades for a symbol
- **get_server_time**: Useful for synchronizing requests and verifying API connectivity.

Get the current Bybit server time
- **get_tickers**: Categories: "spot" (spot trading), "linear" (USDT/USDC perpetual & futures), "inverse" (inverse perpetual & futures), "option" (options). Filter by specific symbol (e.g. "BTCUSDT") or base coin (e.g. "BTC").

Get real-time market tickers (prices) for any category


## Installation & Usage

To install and use the **Bybit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bybit](https://vinkius.com/mcp/bybit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
