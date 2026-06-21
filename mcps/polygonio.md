# Polygon.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polygonio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/polygonio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/polygonio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Access real-time and historical stock market data, including trades, quotes, aggregates, and company metadata directly via AI.

## Description
Connect your **Polygon.io** account to any AI agent to retrieve institutional-grade financial data through natural language. Monitor market trends, analyze historical performance, and inspect company fundamentals without leaving your chat interface.

### What you can do

- **Market Aggregates** — Fetch OHLCV (Open, High, Low, Close, Volume) bars for any ticker over custom timeframes (minute, hour, day)
- **Real-Time & Historical Trades** — Access tick-by-tick trade data to analyze precise market movements and execution prices
- **Company Fundamentals** — Retrieve detailed metadata for stock tickers, including industry classifications and company descriptions
- **Dividend Tracking** — List historical cash dividend distributions, frequencies, and ex-dividend dates for specific assets
- **Ticker Discovery** — Query the full list of supported tickers and financial instruments available on the platform

### How it works

1. Subscribe to this server
2. Enter your Polygon.io API Key
3. Start querying financial markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — quickly pull historical aggregates and dividend data for modeling and reporting
- **Traders & Quants** — inspect tick-by-tick trades and quotes (NBBO) to validate strategies directly from the terminal
- **Fintech Developers** — verify ticker metadata and market connectivity while building financial applications


## Available Tools
- **get_aggregates**: Get aggregate bars for a stock
- **get_company**: Get company details for a ticker
- **list_dividends**: List historical dividends
- **list_quotes**: Get tick-by-tick quotes (NBBO)
- **list_tickers**: io.

Query all supported tickers
- **list_trades**: Get tick-by-tick trades


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polygon.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get company details and industry for ticker NVDA."

**🤖 AI Agent:**
> I've retrieved the details for NVIDIA Corp (NVDA). They operate in the Semiconductors & Related Devices industry. Their primary business involves designing graphics processing units (GPUs) for the gaming and professional markets.

---

**👤 You:**
> "Show me the historical dividends for MSFT."

**🤖 AI Agent:**
> Fetching dividend history for Microsoft (MSFT)... I found a consistent record of quarterly cash dividends. The most recent distribution was $0.75 per share with an ex-dividend date of February 14, 2024.

---

**👤 You:**
> "Get daily aggregate bars for TSLA from 2024-01-01 to 2024-01-10."

**🤖 AI Agent:**
> I've compiled the daily aggregates for Tesla (TSLA) for that period. On Jan 2nd, it opened at $250.08 and closed at $248.42 with a volume of 104M. Would you like the full breakdown for the remaining days?


## Installation & Usage

To install and use the **Polygon.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polygonio](https://vinkius.com/mcp/polygonio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
