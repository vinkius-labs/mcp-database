# IEX Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iex-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iex-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iex-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical financial data, stock quotes, crypto, and market metrics directly from your AI agent.

## Description
Connect **IEX Cloud** to your AI agent to unlock professional-grade financial intelligence. This server provides a comprehensive suite of tools for market analysis, from individual stock performance to global economic indicators.

### What you can do

- **Equities & Quotes** — Get real-time prices, volume, market cap, and key statistics for any stock symbol.
- **Historical Analysis** — Fetch charting data over various time ranges and inspect detailed financial reports (income statements, balance sheets).
- **Market Insights** — List most active stocks, gainers, losers, and monitor performance across all market sectors.
- **Alternative Assets** — Access real-time quotes for cryptocurrencies and the latest foreign exchange (FX) rates.
- **Economic Indicators** — Track US Treasury yields and stay ahead with upcoming earnings release calendars.

### How it works

1. Subscribe to this server
2. Enter your IEX Cloud API Token
3. Start analyzing markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Investors & Traders** — quickly pull quotes and stats without switching to a terminal or browser.
- **Financial Analysts** — automate the retrieval of financial statements and sector performance for reports.
- **Developers** — integrate live market data into your coding workflow to build or test fintech applications.


## Available Tools
- **get_stock_chart**: Get historical price data for a stock
- **get_crypto_quote**: Get real-time quotes for cryptocurrencies
- **get_upcoming_earnings**: Get calendar of upcoming earnings releases
- **get_stock_financials**: Get income statement, balance sheet, and cash flow
- **get_fx_latest**: Get real-time foreign exchange rates
- **get_market_list**: Get market lists like most active, gainers, or losers
- **get_stock_news**: Get latest news articles for a stock
- **get_stock_quote**: Get real-time price, volume, and market cap for a stock
- **get_sector_performance**: Get performance metrics for all market sectors
- **get_stock_stats**: Get key statistics for a stock
- **get_treasury_yield**: Get US Treasury yields


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IEX Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price and market cap of NVIDIA (NVDA)?"

**🤖 AI Agent:**
> I'll check the latest quote for NVDA... The current price is $135.58 with a market cap of approximately $3.33 trillion. Trading volume today is 42.1 million shares.

---

**👤 You:**
> "Show me the latest news for Microsoft."

**🤖 AI Agent:**
> Fetching the latest headlines for MSFT... I found several recent articles, including a report on their latest AI integration and a summary of their quarterly cloud growth.

---

**👤 You:**
> "Which stocks are the top gainers in the market today?"

**🤖 AI Agent:**
> Querying the market lists... The top gainers today are led by 'TechSolutions Inc' (+12.4%) and 'BioHealth Corp' (+8.9%). Would you like details on any of these?


## Installation & Usage

To install and use the **IEX Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iex-cloud](https://vinkius.com/mcp/iex-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
