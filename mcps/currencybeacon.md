# CurrencyBeacon MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/currencybeacon)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/currencybeacon-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/currencybeacon-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical currency exchange rates, perform conversions, and analyze financial time-series data directly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CurrencyBeacon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported currencies and their symbols."

**🤖 AI Agent:**
> I've retrieved the list. CurrencyBeacon supports over 160 currencies including USD (US Dollar), EUR (Euro), JPY (Japanese Yen), and GBP (British Pound Sterling). Would you like to see the full list or check rates for specific ones?

---

**👤 You:**
> "What was the exchange rate for USD to EUR on December 25th, 2010?"

**🤖 AI Agent:**
> Checking historical records... On 2010-12-25, the exchange rate for 1 USD was approximately 0.758 EUR. Would you like to check another date or currency pair?

---

**👤 You:**
> "Convert 1500 Japanese Yen to US Dollars."

**🤖 AI Agent:**
> Using real-time mid-market rates, 1500 JPY is approximately 10.45 USD. Would you like to perform this conversion for a historical date instead?


## Installation & Usage

To install and use the **CurrencyBeacon** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/currencybeacon](https://vinkius.com/mcp/currencybeacon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
