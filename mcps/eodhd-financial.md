# EODHD Financial MCP Server

Access real-time and historical stock market data — prices, fundamentals, dividends, splits and more for global exchanges.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/eodhd-financial)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Connect to **EODHD Financial Data** and access professional-grade stock market data through natural conversation.

### What you can do

- **Real-Time Prices** — Get current stock prices with change, volume and previous close
- **Historical EOD Data** — Download end-of-day price history with OHLCV data
- **Fundamentals** — Access P/E ratios, market cap, earnings, financial statements and analyst targets
- **Dividends** — View dividend payment history with ex-dividend dates and amounts
- **Stock Splits** — Track stock split history with split ratios
- **Ticker Search** — Find stock symbols by company name across global exchanges
- **Multi-Ticker** — Get prices for multiple stocks in one call

### How it works

1. Subscribe to this server
2. Enter your EODHD API Key (free tier with 20 calls/day)
3. Start exploring financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Investors** — track stock prices, research fundamentals and monitor dividend payments
- **Traders** — access real-time prices and historical OHLCV data for technical analysis
- **Analysts** — pull fundamental data, financial ratios and earnings reports


## Available Tools
- **get_dividends**: Returns ex-dividend date, payment date, record date, declaration date and dividend amount per share. Symbol format: TICKER.EXCHANGE. Supports date range filtering.

Get dividend history for a stock
- **get_eod_data**: Supports daily, weekly and monthly periods. Symbol format: TICKER.EXCHANGE (e.g. "AAPL.US"). Use date_from and date_to for date range filtering.

Get historical end-of-day stock data
- **get_exchange_symbols**: Returns symbol codes, names, country and exchange info. Common exchanges: "US" (NYSE/NASDAQ), "XETRA" (Germany), "LSE" (London), "TO" (Tokyo), "PA" (Paris).

Get all symbols for a specific exchange
- **get_fundamentals**: Symbol format: TICKER.EXCHANGE. Use filter parameter to request specific sections (e.g. "General,Highlights,Valuation").

Get fundamental data for a stock
- **get_historical_dividends**: Provide comma-separated symbols (e.g. "AAPL.US,MSFT.US,GOOGL.US"). Returns dividend dates and amounts for all matching tickers.

Get historical dividends for multiple tickers
- **get_historical_splits**: Provide comma-separated symbols. Returns split dates and ratios for all matching tickers.

Get historical stock splits for multiple tickers
- **get_multi_price**: Provide comma-separated symbols (e.g. "AAPL.US,MSFT.US,GOOGL.US"). Returns price, change and change percent for each.

Get real-time prices for multiple tickers
- **get_realtime_price**: Symbol format: TICKER.EXCHANGE (e.g. "AAPL.US" for Apple, "MSFT.US" for Microsoft, "BMW.XETRA" for BMW). Returns current price, open, high, low, close, volume, previous close, change and change percent.

Get real-time stock price
- **get_splits**: Returns split date and split ratio (e.g. "2:1" for a 2-for-1 split). Symbol format: TICKER.EXCHANGE.

Get stock split history for a stock
- **search_tickers**: Returns matching symbols with exchange, name, country and type. Useful for finding the correct symbol format for other API calls.

Search for stock tickers by name or symbol


## Installation & Usage

To install and use the **EODHD Financial** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eodhd-financial](https://vinkius.com/mcp/eodhd-financial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
