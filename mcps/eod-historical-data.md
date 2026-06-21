# EOD Historical Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eod-historical-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eod-historical-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eod-historical-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access global financial market data — historical EOD, intraday, real-time prices, and deep fundamentals for stocks, ETFs, and indices.

## Description
Connect your **EOD Historical Data (EODHD)** account to any AI agent to retrieve professional-grade financial market data through natural language.

### What you can do

- **Historical EOD Data** — Fetch daily, weekly, or monthly OHLCV data for stocks, ETFs, and indices globally using `get_eod_historical`.
- **Intraday & Real-Time** — Access minute-by-minute historical intervals or live price snapshots with `get_intraday_historical` and `get_real_time`.
- **Deep Fundamentals** — Retrieve extensive financial statements, ratios, and company metadata for over 70+ exchanges using `get_fundamentals`.
- **Insider Transactions** — Track SEC Form 4 filings and insider trading activity for US companies with `get_insider_transactions`.
- **Bulk Data & Screener** — Download fundamental data for entire exchanges or search for assets using specific criteria.

### How it works

1. Subscribe to this server
2. Enter your EODHD API Token
3. Start analyzing markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders & Investors** — quickly pull historical trends and fundamental ratios to validate investment theses.
- **Financial Analysts** — automate the collection of financial statements and insider trading reports.
- **Developers** — integrate high-quality market data directly into your coding environment for backtesting and tool building.


## Available Tools
- **get_bulk_fundamentals**: Get bulk fundamental data for an exchange
- **get_calendar_dividends**: Get upcoming dividends calendar
- **get_calendar_earnings**: Get upcoming earnings calendar
- **get_calendar_ipos**: Get upcoming IPOs calendar
- **get_calendar_splits**: Get upcoming splits calendar
- **get_commodities**: Get historical prices for commodities
- **get_dividends**: Get dividends history for a symbol
- **get_eod_historical**: Get End-Of-Day (EOD) historical data for a symbol
- **get_exchange_symbol_list**: Get list of tickers for an exchange
- **get_exchanges_list**: Get list of supported exchanges
- **get_fundamentals**: Get fundamental data for a single symbol
- **get_id_mapping**: Resolve identifiers like CUSIP, ISIN, FIGI to symbols
- **get_insider_transactions**: Get insider transactions (SEC Form 4)
- **get_intraday_historical**: Get Intraday historical data for a symbol
- **get_news**: Get financial news feed
- **get_news_word_weights**: Get news word weights for a ticker
- **get_real_time**: Get Live (Delayed) OHLCV data
- **get_screener**: Filter the stock market based on metrics and signals
- **search_assets**: Search for assets by ticker, name, or ISIN
- **get_sentiments**: Get financial news sentiment
- **get_splits**: Get splits history for a symbol
- **get_technical_indicators**: Get technical indicators for a symbol
- **get_user**: Get EODHD user account details and API limits
- **get_ust_bill_rates**: Get US Treasury Bill Rates
- **get_ust_real_yield_rates**: Get US Treasury Real Yield Rates
- **get_ust_yield_rates**: Get US Treasury Yield Rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EOD Historical Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the historical EOD data for AAPL.US for the last 30 days."

**🤖 AI Agent:**
> I've retrieved the EOD historical data for Apple Inc. (AAPL) on the US exchange. Over the last 30 days, the price moved from $185.20 to $192.45 with an average daily volume of 55M shares.

---

**👤 You:**
> "Show me the fundamental data and key ratios for TSLA.US."

**🤖 AI Agent:**
> Fetching fundamentals for Tesla... I have the latest balance sheet and income statement. Key metrics include a P/E Ratio of 45.2, Debt-to-Equity of 0.12, and a Profit Margin of 14.5%. Would you like to see the full cash flow statement?

---

**👤 You:**
> "What are the latest insider transactions for Microsoft (MSFT.US)?"

**🤖 AI Agent:**
> I found 3 recent insider transactions for MSFT. The most notable was a sale of 10,000 shares by a Senior VP on 2023-10-15 at an average price of $330.10. Two other directors exercised options earlier this month.


## Installation & Usage

To install and use the **EOD Historical Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eod-historical-data](https://vinkius.com/mcp/eod-historical-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
