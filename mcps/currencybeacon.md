# CurrencyBeacon MCP Server

Access real-time and historical currency exchange rates, perform conversions, and analyze financial time-series data directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/currencybeacon)

## Overview
**Category:** data-analytics
**Tools Count:** 5

## Description
Connect **CurrencyBeacon** to your AI agent to access a robust global currency data engine. Whether you need to track live market fluctuations or audit historical financial records, this server provides the tools for precise currency analysis.

### What you can do

- **Real-Time Rates** — Get the latest mid-market exchange rates for over 160 currencies using `get_latest_rates`.
- **Historical Audits** — Retrieve specific exchange rates for any date back to 1996 with `get_historical_rates`.
- **Currency Conversion** — Convert any amount between currencies using `convert_currency`, with optional historical date support.
- **Trend Analysis** — Fetch daily historical data over a range of dates using `get_timeseries` to visualize market movements.
- **Currency Metadata** — List all supported currencies, symbols, and names via `list_currencies`.

### How it works

1. Subscribe to this server
2. Enter your CurrencyBeacon API Key
3. Start querying financial data from Claude, Cursor, or any MCP client

### Who is this for?

- **FinTech Developers** — Integrate reliable exchange rate data into applications without building complex scrapers.
- **E-commerce Managers** — Calculate international pricing and analyze historical currency impacts on sales.
- **Data Analysts** — Pull clean time-series data for financial modeling and reporting.


## Available Tools
- **convert_currency**: Convert an amount from one currency to another
- **list_currencies**: List all supported currencies
- **get_historical_rates**: Get historical exchange rates for a specific date
- **get_latest_rates**: Get real-time exchange rates
- **get_timeseries**: Max range typically 365 days.

Get daily historical exchange rates between two dates


## Installation & Usage

To install and use the **CurrencyBeacon** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/currencybeacon](https://vinkius.com/mcp/currencybeacon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
