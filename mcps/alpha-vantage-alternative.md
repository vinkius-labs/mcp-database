# Alpha Vantage MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alpha-vantage-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/alpha-vantage-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/alpha-vantage-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical stock market data, financial statements, and economic indicators directly from your AI agent.

## Description
Connect **Alpha Vantage** to your AI agent to transform it into a powerful financial analyst. Access a comprehensive suite of market data, from intraday stock prices to deep fundamental analysis and global economic indicators.

### What you can do

- **Stock Time Series** — Fetch intraday, daily, weekly, and monthly OHLCV data for global equities with optional adjustments for splits and dividends.
- **Fundamental Data** — Retrieve company overviews, income statements, balance sheets, and cash flow reports to perform deep-dive equity research.
- **Market Intelligence** — Monitor real-time news sentiment and analyze market trends using advanced technical indicators.
- **Economic Indicators** — Access key macroeconomic data points like GDP, CPI, and unemployment rates directly within your conversation.
- **Forex & Crypto** — Get real-time currency exchange rates and digital currency data to track global market movements.

### How it works

1. Subscribe to this server
2. Enter your Alpha Vantage API Key
3. Start querying market data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — automate the collection of financial ratios and statements for valuation models.
- **Traders & Quants** — pull high-resolution intraday data and technical indicators directly into your research environment.
- **Developers** — integrate market data into your workflow without leaving your code editor.


## Available Tools
- **get_balance_sheet**: Get annual and quarterly balance sheets
- **get_cash_flow**: Get annual and quarterly cash flow statements
- **time_series_daily_adjusted**: Get daily adjusted time series for a stock
- **time_series_daily**: Get daily OHLCV time series for a stock
- **get_digital_currency_daily**: Get daily time series for a cryptocurrency
- **get_economic_indicator**: Get macroeconomic indicators (GDP, CPI, Unemployment, etc.)
- **get_currency_exchange_rate**: Get real-time exchange rate for physical/digital currencies
- **get_income_statement**: Get annual and quarterly income statements
- **time_series_intraday**: Get intraday OHLCV time series for a stock
- **time_series_monthly_adjusted**: Get monthly adjusted time series for a stock
- **time_series_monthly**: Get monthly time series for a stock
- **get_news_sentiment**: Get live and historical news sentiment scores
- **get_overview**: Get company overview and financial ratios
- **get_sma**: Get Simple Moving Average (SMA) technical indicator
- **time_series_weekly_adjusted**: Get weekly adjusted time series for a stock
- **time_series_weekly**: Get weekly time series for a stock


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alpha Vantage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the intraday price action for IBM with 5-minute intervals."

**🤖 AI Agent:**
> I've retrieved the 5-minute intraday data for IBM. The latest price is $182.45 (at 15:55:00). The volume for the last interval was 124,500 shares. Would you like to see the trend for the last hour?

---

**👤 You:**
> "Get the latest income statement and balance sheet for Apple (AAPL)."

**🤖 AI Agent:**
> Fetching financial statements for AAPL... In the last fiscal year, Apple reported total revenue of $383.28B with a net income of $96.99B. Their balance sheet shows total assets of $352.58B. Should I break down the quarterly figures?

---

**👤 You:**
> "What are the current economic indicators for US GDP and inflation?"

**🤖 AI Agent:**
> Accessing economic indicators... The latest Real GDP growth rate is 3.4% (annualized), and the Consumer Price Index (CPI) shows a year-over-year inflation rate of 3.2%. Would you like to see the historical trend for either of these?


## Installation & Usage

To install and use the **Alpha Vantage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alpha-vantage-alternative](https://vinkius.com/mcp/alpha-vantage-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
