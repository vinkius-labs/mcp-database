# MarketStack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marketstack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical stock market data — retrieve EOD prices, intraday points, and ticker details for global exchanges directly from your AI agent.

## Description
Connect **MarketStack** to your AI agent to access a massive database of global stock market information. Get everything from end-of-day prices to intraday data across 70+ global exchanges.

### What you can do

- **Stock Prices** — Fetch End-of-Day (EOD) and intraday data for thousands of tickers with custom date ranges and intervals using `get_eod` and `get_intraday`.
- **Ticker Intelligence** — List all available tickers or get deep metadata for specific symbols like AAPL or MSFT with `get_ticker`.
- **Exchange Coverage** — Explore supported stock exchanges and their specific market identifiers (MIC) using `list_exchanges`.
- **Corporate Actions** — Access historical dividends and stock splits data to understand asset performance via `list_dividends` and `list_splits`.
- **Company Insights** — Retrieve SEC filings, CIK codes, and company facts for fundamental analysis using `getCompanyFacts` and `getSubmissions`.

### How it works

1. Subscribe to this server
2. Enter your MarketStack Access Key
3. Start querying market data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders & Investors** — quickly pull historical data and current prices for technical analysis without leaving your chat interface.
- **Financial Analysts** — automate the collection of dividends, splits, and company fundamentals for research reports.
- **Developers** — integrate market data into financial tools or dashboards directly from your code editor.


## Available Tools
- **get_eod**: Use symbols parameter for comma-separated tickers.

Retrieve end-of-day data for one or multiple stock tickers
- **get_cik_code**: Find the CIK for a company
- **get_company_concepts**: g., accounts_payable) for a company using its CIK code.

Retrieve specific financial concepts for a company
- **get_company_facts**: Retrieve structured financial data for a company
- **get_company_name**: Find a company name by its CIK code
- **get_exchange_tickers**: List all tickers for a specific exchange
- **get_exchange**: Get details for a specific exchange
- **get_submissions**: Retrieve SEC submissions for a company
- **get_ticker_eod**: Get EOD data for a specific ticker
- **get_ticker_intraday**: Get intraday data for a specific ticker
- **get_ticker**: Get details for a specific ticker
- **get_intraday**: Use symbols parameter for comma-separated tickers.

Retrieve intraday data points for one or multiple stock tickers
- **list_currencies**: List supported currencies
- **list_dividends**: Retrieve historical dividend data
- **list_exchanges**: List all supported stock exchanges
- **list_splits**: Retrieve historical stock split data
- **list_tickers**: List all available stock tickers
- **list_timezones**: List supported timezones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MarketStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the end-of-day stock prices for AAPL and MSFT for the last 5 days."

**🤖 AI Agent:**
> I've retrieved the EOD data for Apple (AAPL) and Microsoft (MSFT). Over the last 5 trading days, AAPL moved from $185.92 to $189.45, while MSFT showed a steady increase from $402.12 to $410.50. Would you like the specific daily breakdown?

---

**👤 You:**
> "List all stock exchanges in the United States supported by MarketStack."

**🤖 AI Agent:**
> I found several US-based exchanges: New York Stock Exchange (MIC: XNYS), NASDAQ Stock Exchange (MIC: XNAS), and Investors Exchange (MIC: IEXG). I can provide more details on any of these using their MIC codes.

---

**👤 You:**
> "Show me the intraday data for TSLA with a 1-hour interval."

**🤖 AI Agent:**
> Fetching intraday points for Tesla (TSLA) at 1-hour intervals... The data shows the price opened at $175.20 at 09:30 and reached a peak of $178.50 by 14:30. Would you like to see the volume for these periods as well?


## ❓ FAQ

**Q: Can I get intraday data for specific time intervals?**
Yes! Use the `get_intraday` tool. You can specify intervals such as '1min', '5min', '1hour', and up to '24hour' to get precise price movements throughout the trading day.

**Q: How do I find which stock exchanges are supported by this server?**
Simply run the `list_exchanges` tool. It will return a paginated list of all supported global exchanges along with their names, MIC codes, and locations.

**Q: Can I filter end-of-day data for a specific date range?**
Absolutely. Both `get_eod` and `get_ticker_eod` tools accept `date_from` and `date_to` parameters in YYYY-MM-DD format to help you analyze specific historical periods.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketstack](https://vinkius.com/mcp/marketstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MarketStack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `marketstack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MarketStack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marketstack": {
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
