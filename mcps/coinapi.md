# CoinAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coinapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Unified cryptocurrency data platform — access market data across hundreds of exchanges via AI.

## Description
Equip your AI agent with institutional-grade cryptocurrency market intelligence via **CoinAPI**. This unified server provides your agent with instant access to real-time and historical pricing, volume, trades, and order book data across hundreds of crypto exchanges. Your agent can instantly fetch precise exchange rates, audit OHLCV (Open, High, Low, Close, Volume) data, and retrieve Level 2 order books without you ever manually checking an exchange. Whether you are tracking market momentum or building an automated trading strategy, your agent acts as a dedicated quantitative analyst through natural conversation.

### What you can do

- **Market Rates** — Retrieve current exchange rates between any cryptocurrency and fiat currency pair.
- **Timeseries Data** — Fetch detailed OHLCV (Open, High, Low, Close, Volume) records to analyze price actions across various timeframes.
- **Trade Activity** — Monitor the most recent executed trades on any specific exchange and symbol.
- **Order Book Depth** — Access Level 2 order book data to analyze liquidity and bid/ask spreads.
- **Asset Intelligence** — List all supported fiat and crypto assets, symbols, and integrated exchanges.

### How it works

1. Subscribe to this server
2. Enter your CoinAPI Key
3. Start managing your crypto intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Traders & Quants** — instantly retrieve exact order book depths, trades, and OHLCV data across multiple exchanges.
- **Financial Researchers** — discover macro market trends and analyze liquidity without writing custom API scripts.
- **DeFi Developers** — integrate institutional-grade pricing oracles and exchange rates into decentralized applications.
- **Portfolio Managers** — track precise valuations of diverse crypto assets against multiple fiat pairs.


## Available Tools (9)
- **list_assets**: List all assets
- **list_exchanges**: List all exchanges
- **get_ohlcv**: Get OHLCV data
- **get_latest_orderbooks**: Get latest orderbooks
- **get_latest_quotes**: Get latest quotes
- **get_exchange_rates**: Get exchange rates
- **get_specific_rate**: Get specific exchange rate
- **list_symbols**: Can be optionally filtered.

List all symbols
- **get_latest_trades**: Get latest trades


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current exchange rate for Bitcoin to USD?"

**🤖 AI Agent:**
> Fetching the latest rate for BTC/USD... Bitcoin is currently trading at approximately $65,400. Would you like me to pull the Level 2 order book for a specific exchange like Binance or Coinbase?

---

**👤 You:**
> "Show me the daily OHLCV data for Ethereum on Bitstamp."

**🤖 AI Agent:**
> Retrieving the daily OHLCV data for BITSTAMP_SPOT_ETH_USD... Yesterday, Ethereum opened at $3,450, reached a high of $3,520, and closed at $3,490, with a volume of 15,000 ETH traded.

---

**👤 You:**
> "Get the latest trades for Solana on Binance."

**🤖 AI Agent:**
> Fetching the most recent trades for BINANCE_SPOT_SOL_USDT... In the last few seconds, I see several buy orders filled around $145.20. The largest single trade was for 500 SOL. Should I check the current bid/ask quotes?


## ❓ FAQ

**Q: How do I format the symbol ID to get specific exchange data?**
CoinAPI uses a specific format: `EXCHANGE_TYPE_BASE_QUOTE`. For example, to get Bitcoin to USD on Bitstamp, use `BITSTAMP_SPOT_BTC_USD`. You can use the `list_symbols` tool to find exact identifiers.

**Q: Can I get the current price of Ethereum in Euros?**
Yes! Use the `get_specific_rate` tool. Set `asset_id_base` to 'ETH' and `asset_id_quote` to 'EUR'. This will return the real-time average conversion rate.

**Q: What timeframes are available for OHLCV data?**
The `get_ohlcv` tool supports various periods via the `period_id` parameter, such as `1MIN`, `1HRS`, `1DAY`, `1MTH`, etc. It defaults to `1DAY`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coinapi](https://vinkius.com/mcp/coinapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoinAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coinapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoinAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coinapi": {
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
