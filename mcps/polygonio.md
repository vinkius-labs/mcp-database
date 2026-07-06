# Polygon.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polygonio)
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


## Available Tools (6)
- **list_tickers**: io.

Query all supported tickers
- **get_aggregates**: Get aggregate bars for a stock
- **get_company**: Get company details for a ticker
- **list_dividends**: List historical dividends
- **list_quotes**: Get tick-by-tick quotes (NBBO)
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


## ❓ FAQ

**Q: Can I get historical price data for a specific stock over a date range?**
Yes. Use the `get_aggregates` tool by providing the ticker, multiplier, timespan (e.g., 'day'), and the 'from' and 'to' dates. The agent will return the OHLCV bars for that period.

**Q: How do I find the description and industry of a specific company?**
Simply use the `get_company` tool with the stock ticker (e.g., 'AAPL'). It will retrieve the official company metadata, including its business description and industry classification.

**Q: Is it possible to see the most recent trades for a ticker?**
Yes! The `list_trades` tool allows you to fetch tick-by-tick trade data for a specific ticker, showing execution prices and sizes as they happen in the market.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polygonio](https://vinkius.com/mcp/polygonio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Polygon.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `polygonio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Polygon.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "polygonio": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
