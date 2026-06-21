# Twelve Data MCP Server

Access real-time stock quotes, crypto prices, forex rates, and technical indicators via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/twelve-data)

## Overview
**Category:** data-analytics
**Tools Count:** 16

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


## Available Tools
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
- **get_quote**: Get real-time stock quote
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


## Installation & Usage

To install and use the **Twelve Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twelve-data](https://vinkius.com/mcp/twelve-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
