# Binance (Crypto Market) MCP Server

Track cryptocurrency markets via Binance — get real-time prices, monitor 24h trends, analyze market movers, and audit trading volumes directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/binance-crypto-market)

## Overview
**Category:** money-moves
**Tools Count:** 7

## Description
Connect your AI agent to the **Binance** public API and take full control of your cryptocurrency market research and portfolio monitoring through natural conversation.

### What you can do

- **Real-Time Price Auditing** — Retrieve exact price strings for any trading pair (e.g., BTCUSDT, ETHUSDT) including 24h trend labels and emoji indicators
- **Market Overview** — List top cryptocurrencies ranked by 24h USDT volume to identify active liquidity and market hotspots natively
- **Volatility Analysis** — Inspect deep internal arrays of price fluctuations to track high/low spreads and weighted average prices limitlessly
- **Candlestick extraction** — Perform structural extraction of K-line data (OHLC) for specific time intervals to analyze historical price action
- **Market Movers** — Discover top gainers and losers in the last 24 hours to monitor radical volatility and pump/dump signals
- **Ticker Metadata** — Retrieve elaborate explicit mapping of ticker statistics including trade counts and base/quote volume vectors

### How it works

1. Subscribe to this server
2. No credentials required — this server uses Binance's public REST endpoints
3. Start monitoring the crypto market from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Traders** — monitor prices and market trends quickly without switching to trading terminals
- **Financial Analysts** — audit trading volumes and volatility across thousands of pairs using natural language
- **Portfolio Managers** — track the value of multiple assets and verify real-time price action directly from the workspace
- **Developers** — test and debug crypto market data integrations and candlestick logic through the chat


## Available Tools
- **get_price**: Accept natural names: "bitcoin", "BTC", "eth", "SOLUSDT". Returns current price + 24h change percentage. For full stats (volume, high/low, trades), use crypto.ticker instead.

Get the current price of any cryptocurrency in USDT with 24h trend
- **get_ticker**: Accept natural names (e.g. "bitcoin", "BTC", "btcusdt"). For just a quick price, use crypto.price instead.

Get full 24h statistics for any cryptocurrency trading pair on Binance
- **list_market**: Returns USDT trading pairs ranked by 24h volume. Limit is 1–50 coins. Default to 10 if the user does not specify.

Get the top cryptocurrencies by trading volume on Binance, ranked by 24h USDT volume
- **get_candles**: Supported intervals: 1m, 5m, 15m, 30m, 1h, 4h, 1d, 1w. Limit is 1–100 candles. Default to 30 daily candles (interval=1d, limit=30) unless the user specifies. Do NOT use for just a current price — use crypto.price for that.

Get OHLCV candlestick chart data for a cryptocurrency pair on Binance
- **compare_coins**: Accept comma-separated list: "BTC, ETH, SOL" or "bitcoin vs ethereum". At least 2 symbols required. Maximum 10 symbols. Ranks by 24h performance and assigns verdict (top_performer, outperforming, average, underperforming, worst_performer).

Compare multiple cryptocurrencies side by side — price, 24h change, volume, and relative performance
- **list_movers**: direction=gainers returns top positive movers, losers=negative movers, both=all sorted by absolute change. Filters to coins with at least $1M USDT volume to avoid low-liquidity noise. Limit is 1–20 per direction.

Get the top gaining and/or losing cryptocurrencies on Binance in the last 24 hours
- **get_volatility**: Fetches the last N candles and computes: amplitude %, trend direction, bull/bear ratio. Do NOT use for a simple price check — use crypto.price instead. Default: interval=1h, periods=24 (last 24 hours).

Analyse the price volatility and trend of a cryptocurrency over a given number of candles


## Installation & Usage

To install and use the **Binance (Crypto Market)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/binance-crypto-market](https://vinkius.com/mcp/binance-crypto-market)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
