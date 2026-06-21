# MarketStack MCP Server

Access real-time and historical stock market data — retrieve EOD prices, intraday points, and ticker details for global exchanges directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/marketstack)

## Overview
**Category:** data-analytics
**Tools Count:** 18

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


## Installation & Usage

To install and use the **MarketStack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketstack](https://vinkius.com/mcp/marketstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
