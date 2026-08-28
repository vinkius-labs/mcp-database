# Binance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/binance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Get real-time cryptocurrency prices, order books, candlesticks and trades from Binance exchange.

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


## Available Tools (8)
- **get_agg_trades**: Symbol format: BASE+QUOTE (BTCUSDT, BTCUSDC). BASE only (BTC) is converted to BTCUSDT.

Get aggregated trades, where fills at the same price and time are combined into one record. Use for efficient trade-flow analysis on high-volume pairs
- **get_exchange_info**: Symbol format: BASE+QUOTE (BTCUSDT, BTCUSDC). BASE only (BTC) is converted to BTCUSDT. Omit symbol to list all pairs.

Look up trading rules and metadata for Binance pairs: status, base/quote assets, order types and price/quantity filters. Use to discover valid symbols or check limits before trading
- **get_24h_ticker**: Symbol format: BASE+QUOTE (BTCUSDT, BTCUSDC). BASE only (BTC) is converted to BTCUSDT. Omit symbol to return all pairs.

Get 24-hour price change stats for a trading pair: price change, percent change, high, low and volume. Use for market overviews or "how did X move today"
- **get_order_book**: Symbol format: BASE+QUOTE (BTCUSDT, BTCUSDC). BASE only (BTC) is converted to BTCUSDT.

Get the live order book (bids and asks with prices and quantities) for a trading pair. Use to analyze market depth, spread and liquidity
- **get_price**: Symbol format: BASE+QUOTE (BTCUSDT, BTCUSDC). BASE only (BTC) is converted to BTCUSDT. Omit symbol to return all pairs.

Get the latest market price for a trading pair (e.g. BTCUSDT). The fastest way to answer "how much is X worth right now"
- **get_klines**: Symbol format: BASE+QUOTE (BTCUSDT, BTCUSDC). BASE only (BTC) is converted to BTCUSDT.

Get historical OHLCV candlestick data (open, high, low, close, volume) for a trading pair at a chosen interval. Use for charting and technical analysis
- **get_server_time**: Get the current Binance server time. Use to check exchange availability or align timestamps before other calls
- **get_trades**: Symbol format: BASE+QUOTE (BTCUSDT, BTCUSDC). BASE only (BTC) is converted to BTCUSDT.

Get the most recent individual trades (price, quantity, time, side) for a trading pair. Use to inspect live trade activity and order flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Binance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price of Bitcoin?"

**🤖 AI Agent:**
> BTC/USDT: $87,234.50. 24h change: +2.1% (+$1,795). 24h high: $88,100, 24h low: $85,800. 24h volume: 13,845 BTC ($1.2B).

---

**👤 You:**
> "Show me the order book for ETH/USDT."

**🤖 AI Agent:**
> ETH/USDT Order Book: Best bid $3,245.60 (15.2 ETH), Best ask $3,245.80 (8.5 ETH). Spread: $0.20 (0.006%). Top 5 bids total 125 ETH, top 5 asks total 98 ETH.

---

**👤 You:**
> "Show me the daily candlesticks for SOL/USDT for the last 30 days."

**🤖 AI Agent:**
> SOL/USDT Daily (30 candles): Current candle open $185.50, high $188.20, low $183.40, close $187.10, volume 2.5M SOL. Over the past 30 days SOL has gained +12.5% from $166.30.


## ❓ FAQ

**Q: Do I need an API key?**
No! All public market data (prices, order books, trades, klines, exchange info) is available without authentication. Just subscribe and start querying.

**Q: What trading pairs are available?**
Binance supports 1500+ trading pairs. Use get_exchange_info to see the complete list. Popular pairs include BTCUSDT, ETHUSDT, BNBUSDT, SOLUSDT and many altcoin pairs.

**Q: What candlestick intervals are available?**
15 intervals are available: 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M. Use get_klines with the interval parameter. Each candle includes open, high, low, close and volume.

**Q: Can I get historical price data?**
Yes! Use get_klines with startTime and endTime parameters (Unix timestamp in milliseconds) to retrieve historical candlestick data. You can get up to 1000 candles per request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/binance](https://vinkius.com/ai-agent-connect/binance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Binance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `binance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Binance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "binance": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
