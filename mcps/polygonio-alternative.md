# Polygon.io MCP Server

Access real-time and historical financial data for stocks, crypto, forex, and indices directly within your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/polygonio-alternative)

## Overview
**Category:** data-analytics
**Tools Count:** 21

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


## Installation & Usage

To install and use the **Polygon.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polygonio-alternative](https://vinkius.com/mcp/polygonio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
