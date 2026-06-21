# CoinCap MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coincap)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Get real-time cryptocurrency prices, market data, exchange rankings and OHLCV candles — no API key required.

## Description
Connect to **CoinCap** APIs and access real-time cryptocurrency market data through natural conversation — no API key needed.

### What you can do

- **Asset Prices** — Get current prices, market caps, 24h volume and supply info for any cryptocurrency
- **Asset Search** — Search for crypto by name or symbol (Bitcoin, Ethereum, Solana, etc.)
- **Historical Prices** — Retrieve price history with configurable intervals (1m to 1d)
- **Markets** — See which exchanges list specific trading pairs and their 24h volumes
- **Exchange Rankings** — Browse exchanges ranked by 24h volume with verification status
- **OHLCV Candles** — Get candlestick data for technical analysis with multiple timeframes
- **Exchange Rates** — View crypto-to-fiat conversion rates

### How it works

1. Subscribe to this server
2. No API key needed — start querying immediately
3. Get crypto data from Claude, Cursor, or any MCP-compatible client

No API key required — completely free with 30 requests/second.

### Who is this for?

- **Traders** — check real-time prices, compare exchange listings and review trading pair volumes
- **Developers** — access crypto market data without authentication for dashboards and bots
- **Researchers** — explore historical price data, exchange rankings and market trends


## Available Tools
- **get_asset**: Returns the current price in USD, market cap, 24h trading volume, price change percentages (1h, 24h, 7d), circulating supply, total supply, max supply and rank. Asset IDs are lowercase with hyphens (e.g. "bitcoin", "ethereum", "solana").

Get detailed info for a specific cryptocurrency
- **get_asset_history**: Returns daily or interval-based price snapshots. Use interval to specify the data granularity: "m1" (1 minute), "m5" (5 min), "m15" (15 min), "m30" (30 min), "h1" (1 hour), "h2" (2 hours), "h6" (6 hours), "h12" (12 hours), "d1" (1 day).

Get historical price data for a cryptocurrency
- **get_candles**: Each candle includes the open, high, low, close prices and volume for the time interval. Supports intervals: "m1", "m5", "m15", "m30", "h1", "h2", "h6", "h12", "d1". Optionally set start/end timestamps (milliseconds since epoch) for historical data.

Get OHLCV candlestick data for technical analysis
- **get_exchange**: Returns the exchange name, website, 24h volume, number of markets, rank, verification status and supported assets. Exchange IDs are lowercase (e.g. "binance", "coinbase-pro", "kraken").

Get detailed info for a specific cryptocurrency exchange
- **get_markets**: Each market includes the exchange ID, base asset ID, quote asset ID, trading pair symbol, current price, 24h volume in USD and volume percentage. Optionally filter by asset ID or exchange ID.

Get trading markets/pairs for assets or exchanges
- **get_rate**: Returns the current rate for converting the asset to its corresponding fiat currency. Base IDs are typically asset IDs like "bitcoin", "ethereum" or fiat codes like "USD".

Get a specific exchange rate
- **get_rates**: ). Returns the rate ID, symbol, currency symbol and current rate. Optionally filter by base currency.

Get exchange rates for cryptocurrencies to fiat currencies
- **list_assets**: Optionally search by name, filter by specific IDs, and paginate with limit/offset. Returns assets sorted by market cap by default.

List cryptocurrency assets with prices and market data
- **list_exchanges**: Each exchange includes its ID, name, website, 24h volume in USD, number of markets, rank and whether it's verified.

List cryptocurrency exchanges with rankings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinCap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price of Bitcoin?"

**🤖 AI Agent:**
> Bitcoin is currently trading at $87,234.50 USD. Market cap: $1.73 trillion. 24h volume: $32.4 billion. Price changed +2.1% in the last 24h. Circulating supply: 19.6 million BTC.

---

**👤 You:**
> "Show me the top 5 cryptocurrency exchanges by volume."

**🤖 AI Agent:**
> Top 5 exchanges by 24h volume: 1. Binance ($28.5B, 800+ markets, verified), 2. Coinbase Pro ($4.2B, 400+ markets), 3. Kraken ($1.8B, 600+ markets), 4. KuCoin ($1.5B, 1000+ markets), 5. OKX ($1.2B, 400+ markets).

---

**👤 You:**
> "Show me the 1-hour candlestick data for Ethereum."

**🤖 AI Agent:**
> ETH/USD 1h candles: Most recent candle closed at $3,245.60 (open: $3,220, high: $3,260, low: $3,210, volume: $45M). The trend has been upward over the last 12 hours with a 1.8% gain.


## ❓ FAQ

**Q: Do I need an API key?**
No! CoinCap's API is completely free and requires no authentication. Just subscribe and start querying. Rate limit is 30 requests/second on the free tier.

**Q: What cryptocurrencies are supported?**
CoinCap tracks thousands of cryptocurrencies including Bitcoin, Ethereum, Solana, XRP, Cardano, Dogecoin, Avalanche, Polkadot and many more. Use list_assets with the search parameter to find any coin by name or symbol.

**Q: Can I get OHLCV data for technical analysis?**
Yes! Use get_candles with the asset ID and interval (m1, m5, m15, m30, h1, h2, h6, h12, d1). Returns open, high, low, close and volume for each candle period.

**Q: Can I see which exchanges list a specific crypto?**
Yes! Use get_markets with asset_id to see all exchanges that list a specific cryptocurrency. Results include the exchange name, trading pair, current price, 24h volume and volume percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coincap](https://vinkius.com/mcp/coincap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoinCap** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `coincap` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoinCap** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coincap": {
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
