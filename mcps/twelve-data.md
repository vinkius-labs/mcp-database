# Twelve Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twelve-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time stock quotes, crypto prices, forex rates, and technical indicators via AI.

## Description
Connect **Twelve Data** financial API to any AI agent and access real-time stock quotes, cryptocurrency prices, forex rates, and professional technical indicators through natural language.

### What you can do

- **Real-Time Quotes** — Get current price, open, high, low, volume, and change for any stock
- **Historical Data** — Retrieve OHLCV candlestick data from 1-minute to monthly intervals
- **Technical Analysis** — Calculate SMA, EMA, RSI, MACD, Bollinger Bands, and Stochastic Oscillator
- **Market Scanning** — Search and browse available stocks, crypto pairs, and forex instruments
- **Company Profiles** — Access fundamental data including market cap, P/E ratio, and sector info
- **Currency Conversion** — Get exchange rates and convert amounts between any currency pair

### How it works

1. Subscribe to this server
2. Enter your free Twelve Data API Key
3. Start analyzing markets from Claude, Cursor, or any MCP-compatible client


## Available Tools (16)
- **get_quote**: Get real-time stock quote
- **convert_currency**: Convert an amount between currencies
- **get_bollinger_bands**: Price touching upper band may indicate overbought, lower may indicate oversold.

Get Bollinger Bands
- **get_company_profile**: Get company profile and fundamentals
- **get_crypto_list**: Can filter by exchange.

List available crypto pairs
- **get_ema**: EMA gives more weight to recent prices than SMA.

Get Exponential Moving Average (EMA)
- **get_exchange_rate**: Get currency exchange rate
- **get_forex_list**: List available forex pairs
- **get_macd**: Used for trend following and momentum.

Get Moving Average Convergence Divergence (MACD)
- **get_rsi**: Values above 70 indicate overbought, below 30 indicate oversold conditions.

Get Relative Strength Index (RSI)
- **get_real_time_price**: Faster and lighter than a full quote.

Get current price only
- **get_sma**: Common periods: 20, 50, 200.

Get Simple Moving Average (SMA)
- **get_stochastic**: Values above 80 indicate overbought, below 20 indicate oversold.

Get Stochastic Oscillator
- **get_stock_list**: Can filter by exchange and partial symbol match.

List available stocks
- **get_time_series**: Supports intervals from 1min to 1month.

Get historical OHLCV candle data
- **search_symbols**: Can filter by instrument type and exchange.

Search for financial instruments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twelve Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current price of Apple stock?"

**🤖 AI Agent:**
> AAPL is currently trading at $192.45, up 1.23% (+$2.34) from yesterday's close. Open: $190.50, High: $193.10, Low: $189.80. Volume: 52.3M shares.

---

**👤 You:**
> "Show me the RSI for Tesla on the daily chart."

**🤖 AI Agent:**
> TSLA RSI (14-period) on daily chart: 58.3 — neutral territory. Not overbought (>70) or oversold (<30). The RSI has been trending upward over the past 5 sessions.

---

**👤 You:**
> "Convert 1000 USD to EUR."

**🤖 AI Agent:**
> 1,000 USD = 921.50 EUR at the current exchange rate of 0.9215. Rate updated in real-time.


## ❓ FAQ

**Q: How do I get a Twelve Data API Key?**
Visit [**Twelve Data**](https://twelvedata.com/), sign up for a free account, and copy your API key from the dashboard. Free tier includes 800 API credits/day.

**Q: What technical indicators are available?**
SMA (Simple Moving Average), EMA (Exponential MA), RSI (Relative Strength Index), MACD, Bollinger Bands, and Stochastic Oscillator — all with customizable periods.

**Q: Can I get real-time crypto and forex prices?**
Yes! Use `get_quote` or `get_real_time_price` with any symbol. Crypto pairs like BTC/USD and forex pairs like EUR/USD are supported.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twelve-data](https://vinkius.com/mcp/twelve-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twelve Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twelve-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twelve Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twelve-data": {
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
