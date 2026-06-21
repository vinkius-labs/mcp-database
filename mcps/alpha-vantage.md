# Alpha Vantage MCP Server

Access stock market data via Alpha Vantage — get real-time quotes, time series, technical indicators and crypto/forex data from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/alpha-vantage)

## Overview
**Category:** data-analytics
**Tools Count:** 13

## Description
Connect to **Alpha Vantage** APIs through any AI agent and explore global financial markets through natural conversation.

### What you can do

- **Real-Time Quotes** — Get current stock prices, volume, high/low, open and previous close
- **Time Series** — Access daily, weekly, monthly and intraday OHLCV data with 20+ years of history
- **Technical Indicators** — Calculate RSI, SMA, EMA, MACD, Bollinger Bands and 50+ other indicators
- **Company Fundamentals** — Retrieve company overview, market cap, PE ratio, EPS and earnings history
- **Sector Performance** — Monitor real-time performance of all 11 market sectors
- **News Sentiment** — Fetch news articles with sentiment scores for stock tickers
- **Crypto & Forex** — Get daily cryptocurrency and foreign exchange rate data

### How it works

1. Subscribe to this server
2. Enter your Alpha Vantage API Key (free at alphavantage.co)
3. Start exploring financial markets from Claude, Cursor, or any MCP-compatible client

No more navigating complex financial terminals to check stock prices or technical indicators. Your AI acts as a dedicated market data analyst.

### Who is this for?

- **Traders** — quickly check quotes, review time series and calculate technical indicators without opening a trading platform
- **Investors** — explore company fundamentals, earnings history and sector performance for portfolio research
- **Developers** — access market data programmatically for building financial applications and analysis tools
- **Students** — learn about technical analysis, market trends and financial data through interactive conversation


## Available Tools
- **get_company_overview**: Useful for fundamental analysis and stock screening.

Get company overview and fundamentals
- **get_crypto_daily**: Requires the crypto symbol (e.g. "BTC") and the market currency (e.g. "USD"). Returns daily price data with dates.

Get daily cryptocurrency prices
- **get_daily_time_series**: Optionally set outputsize to "compact" (last 100 data points, default) or "full" (20+ years of data). Returns daily price data with dates.

Get daily stock time series
- **get_earnings**: Useful for earnings analysis and identifying beats/misses.

Get earnings history for a stock
- **get_forex_daily**: Requires the from symbol (e.g. "EUR") and to symbol (e.g. "USD"). Returns daily OHLCV forex data with dates.

Get daily foreign exchange rates
- **get_intraday_time_series**: Optionally set interval (1min, 5min, 15min, 30min, 60min) and outputsize. Returns price data at the specified interval. Useful for day trading analysis.

Get intraday stock time series
- **get_monthly_time_series**: Each data point represents a month of trading. Useful for long-term trend analysis and portfolio review.

Get monthly stock time series
- **get_news_sentiment**: Each article includes title, summary, source, sentiment scores (bullish/bearish score) and relevance score. Optionally filter by topics and limit the number of results.

Get news sentiment for stock tickers
- **get_quote**: Returns current trading data including change and change percent. Useful for quick price checks.

Get real-time stock quote
- **get_rsi**: RSI measures momentum on a 0-100 scale; above 70 indicates overbought, below 30 indicates oversold. Optionally set interval, time period and series type (close, open, high, low).

Get Relative Strength Index (RSI) indicator
- **get_sector_performance**: Returns change percentages for each sector.

Get real-time sector performance
- **get_weekly_time_series**: Each data point represents a week of trading. Useful for medium-term trend analysis.

Get weekly stock time series
- **search_symbol**: Returns best matches with symbol, name, type and region. Useful for discovering the correct symbol before querying price data.

Search for stock symbols by keywords


## Installation & Usage

To install and use the **Alpha Vantage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alpha-vantage](https://vinkius.com/mcp/alpha-vantage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
