# Polygon.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polygonio-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/polygonio-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/polygonio-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical financial data for stocks, crypto, forex, and indices directly within your AI agent.

## Description
Connect your **Polygon.io** account to any AI agent to retrieve institutional-grade market data through simple conversation. Monitor market movements, analyze historical trends, and stay updated with financial news.

### What you can do

- **Market Exploration** — Search for ticker symbols across stocks, crypto, and forex markets with detailed filtering by exchange or asset class.
- **Historical Analysis** — Fetch aggregated OHLC (Open, High, Low, Close) and volume data for any supported ticker over custom timeframes.
- **Real-time Snapshots** — Get comprehensive snapshots of the entire U.S. stock market or specific indices to gauge current sentiment.
- **Technical Indicators** — Calculate Simple Moving Averages (SMA) and other metrics to inform trading strategies.
- **Market Intelligence** — Access tick-level trades, NBBO quotes, dividend history, and the latest financial news for any company.

### How it works

1. Subscribe to this server
2. Enter your Polygon.io API Key
3. Start querying financial markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders & Investors** — Quickly pull historical bars and market status without switching to a terminal or web dashboard.
- **Financial Analysts** — Automate the retrieval of dividends, splits, and treasury yields for research reports.
- **Developers** — Test market data queries and inspect ticker types directly from your coding environment.


## Available Tools
- **get_crypto_trades**: Retrieve tick-level trade data for crypto pairs
- **get_custom_bars**: Retrieve aggregated historical OHLC and volume data for a stock
- **get_dividends**: Retrieve historical dividends for stocks
- **get_forex_conversion**: Retrieve real-time currency conversion rates
- **get_indices_snapshot**: Retrieve snapshot data for one or more indices
- **get_market_holidays**: List future holidays affecting market hours
- **get_market_snapshot**: Retrieve a comprehensive snapshot of the entire U.S. stock market
- **get_market_status**: Check if markets are open, closed, or in pre/post-market sessions
- **get_merchant_aggregates**: Retrieve aggregated European consumer spending data
- **get_news**: Retrieve real-time structured news articles from Benzinga
- **get_options_snapshot**: Retrieve a snapshot of all options contracts for an underlying ticker
- **get_quotes**: Retrieve National Best Bid and Offer (NBBO) quotes for a stock
- **get_sma**: Retrieve Simple Moving Average (SMA) technical indicator
- **get_splits**: Retrieve historical stock splits
- **get_trades**: Retrieve tick-level trade data for a specified stock
- **get_treasury_yields**: Retrieve historical U.S. Treasury yield data (1-month to 30-year)
- **list_exchanges**: Retrieve a list of known exchanges and their identifiers
- **list_futures_contracts**: Discover listed futures contracts and specifications
- **list_options_contracts**: Retrieve an index of options contracts (active and expired)
- **list_ticker_types**: Retrieve a list of all ticker types supported
- **list_tickers**: Retrieve a comprehensive list of ticker symbols across asset classes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polygon.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active stock tickers on the NASDAQ exchange."

**🤖 AI Agent:**
> I've retrieved the active tickers for NASDAQ. There are several thousand results; some notable ones include AAPL (Apple Inc.), MSFT (Microsoft Corp.), and AMZN (Amazon.com Inc.). Would you like to filter this list further or inspect a specific ticker?

---

**👤 You:**
> "Get daily historical bars for TSLA from 2024-01-01 to 2024-02-01."

**🤖 AI Agent:**
> I have the historical data for TSLA. During this period, the price opened at $248.42 on Jan 2nd and closed at $188.86 on Feb 1st. The highest volume was recorded on Jan 25th. Would you like a summary of the average closing price?

---

**👤 You:**
> "What is the current market status and are there any upcoming holidays?"

**🤖 AI Agent:**
> The U.S. stock market is currently 'open'. Forex and Crypto markets are also active. Regarding holidays, the next market closure is for Presidents' Day on February 19th. Is there anything else you'd like to check?


## Installation & Usage

To install and use the **Polygon.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polygonio-alternative](https://vinkius.com/mcp/polygonio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
