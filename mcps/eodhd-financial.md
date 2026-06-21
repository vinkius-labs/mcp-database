# EODHD Financial MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eodhd-financial)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical stock market data — prices, fundamentals, dividends, splits and more for global exchanges.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EODHD Financial** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current price of Apple stock?"

**🤖 AI Agent:**
> AAPL.US: $198.45 (Open: $197.20, High: $199.10, Low: $196.80). Previous close: $197.50. Change: +$0.95 (+0.48%). Volume: 45.2M.

---

**👤 You:**
> "Show me Microsoft's fundamentals."

**🤖 AI Agent:**
> MSFT.US fundamentals: Market Cap: $3.1T, P/E: 36.5, EPS: $13.50, Dividend Yield: 0.72%, Beta: 0.89. 52-week high: $468.35, 52-week low: $309.45. Sector: Technology, Industry: Software.

---

**👤 You:**
> "Get prices for AAPL, MSFT and GOOGL."

**🤖 AI Agent:**
> AAPL.US: $198.45 (+0.48%), MSFT.US: $432.10 (+1.2%), GOOGL.US: $175.80 (-0.3%). All prices are real-time with volume data.


## ❓ FAQ

**Q: How do I get an EODHD API key?**
Sign up at [**eodhd.com**](https://eodhd.com/) and get your free API key from the dashboard. Free tier includes 20 calls/day.

**Q: What exchanges are supported?**
EODHD covers 60+ global exchanges including US (NYSE/NASDAQ), LSE (London), XETRA (Germany), TO (Tokyo), PA (Paris), TSX (Canada) and many more.

**Q: What is the symbol format?**
Symbols use the format TICKER.EXCHANGE (e.g. "AAPL.US" for Apple on US exchange, "BMW.XETRA" for BMW on German exchange). Use search_tickers to find the correct format.

**Q: What fundamental data is available?**
Fundamentals include: General info, Highlights, Valuation (P/E, P/B, P/S), Financials (balance sheet, income statement, cash flow), Earnings, Dividends, Shares Stats and Technical Analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eodhd-financial](https://vinkius.com/mcp/eodhd-financial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EODHD Financial** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eodhd-financial` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EODHD Financial** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eodhd-financial": {
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
