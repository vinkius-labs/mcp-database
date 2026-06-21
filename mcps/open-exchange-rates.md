# Open Exchange Rates MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-exchange-rates)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-exchange-rates-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-exchange-rates-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical currency exchange rates for 200+ currencies. Convert values, track time series, and analyze OHLC data directly from your AI agent.

## Description
Connect your **Open Exchange Rates** account to any AI agent to integrate global financial data into your workflows. Get accurate, reliable exchange rates for hundreds of currencies through a simple natural language interface.

### What you can do

- **Latest Rates** — Fetch real-time exchange rates relative to USD or any supported base currency.
- **Currency Conversion** — Instantly convert amounts between any two currencies using the latest market data.
- **Historical Analysis** — Retrieve exchange rates for any specific date or track trends over time with time-series data.
- **Market Insights** — Access Open-High-Low-Close (OHLC) data for detailed financial analysis and reporting.
- **Usage Monitoring** — Keep track of your API consumption and plan limits directly through the agent.

### How it works

1. Subscribe to this server
2. Enter your Open Exchange Rates App ID
3. Start querying global financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — Quickly gather historical data and OHLC metrics for market reports.
- **E-commerce Managers** — Verify current conversion rates for international pricing strategies.
- **Developers** — Test currency logic and verify API responses without leaving the code editor.


## Available Tools
- **convert_currency**: Convert any value from one currency to another
- **list_currencies**: Get a list of all available currency symbols and names
- **get_historical_rates**: Retrieve exchange rates for a specific date
- **get_latest_rates**: Retrieve the most recent exchange rates
- **get_ohlc**: Retrieve OHLC data for a specific period
- **get_time_series**: Retrieve exchange rates over a period of time
- **get_usage**: Check your App ID usage and plan limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Exchange Rates** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the latest exchange rates for EUR and GBP with USD as base."

**🤖 AI Agent:**
> I've retrieved the latest rates. Currently, 1 USD is equivalent to 0.92 EUR and 0.79 GBP.

---

**👤 You:**
> "Convert 1500 JPY to USD."

**🤖 AI Agent:**
> Based on the latest market data, 1,500 JPY is approximately 10.12 USD.

---

**👤 You:**
> "Check my current API usage and limits."

**🤖 AI Agent:**
> You have used 450 out of 1,000 requests this month. Your plan is currently active and healthy.


## Installation & Usage

To install and use the **Open Exchange Rates** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-exchange-rates](https://vinkius.com/mcp/open-exchange-rates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
