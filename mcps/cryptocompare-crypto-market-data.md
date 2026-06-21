# CryptoCompare (Crypto Market Data) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cryptocompare-crypto-market-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cryptocompare-crypto-market-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cryptocompare-crypto-market-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Access real-time and historical cryptocurrency market data, news, and top coins directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CryptoCompare (Crypto Market Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price of BTC in USD and EUR?"

**🤖 AI Agent:**
> I've checked the latest market data. Bitcoin (BTC) is currently trading at $64,250.50 USD and €59,120.30 EUR.

---

**👤 You:**
> "Show me the daily historical data for ETH/USD for the last 7 days."

**🤖 AI Agent:**
> Retrieving historical OHLCV data for Ethereum... Here are the daily closes for the last week, showing a trend from $3,420 up to $3,550.

---

**👤 You:**
> "List the top 5 cryptocurrencies by market cap in USD."

**🤖 AI Agent:**
> The current top 5 coins by market cap are: 1. Bitcoin (BTC), 2. Ethereum (ETH), 3. Tether (USDT), 4. BNB, and 5. Solana (SOL).


## Installation & Usage

To install and use the **CryptoCompare (Crypto Market Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cryptocompare-crypto-market-data](https://vinkius.com/mcp/cryptocompare-crypto-market-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
