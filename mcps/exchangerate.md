# ExchangeRate- MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exchangerate)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/exchangerate-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/exchangerate-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical currency exchange rates for 160+ currencies directly from your AI agent.

## Description
Connect your **ExchangeRate-API** account to any AI agent to perform currency conversions and financial analysis using natural language.

### What you can do

- **Latest Rates** — Get current exchange rates for any base currency to all other supported currencies.
- **Pair Conversion** — Convert specific amounts between two currencies instantly with high precision.
- **Enriched Data** — Access localization data including country names, flag URLs, and currency symbols (Business/Volume plans).
- **Historical Rates** — Retrieve exchange rate data for specific dates in the past for auditing or trend analysis.
- **Currency Support** — Programmatically list all 160+ supported currency codes and names.
- **Quota Management** — Monitor your API usage and remaining requests for the current period.

### How it works

1. Subscribe to this server
2. Enter your ExchangeRate-API Key
3. Start performing currency calculations in Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Managers** — quickly convert product prices for international markets.
- **Financial Analysts** — retrieve historical data for market trend reports without leaving the chat.
- **Travelers & Digital Nomads** — get instant conversions for expenses in any local currency.


## Available Tools
- **get_supported_codes**: Get list of all supported currency codes
- **get_enriched_data**: Requires Business/Volume plan.

Get enriched exchange rate data including localization
- **get_historical_data**: Requires Pro/Business/Volume plan.

Get historical exchange rates for a specific date
- **get_latest_rates**: Get latest exchange rates for a base currency
- **get_pair_conversion**: Get exchange rate between two specific currencies
- **get_quota**: Check remaining API request quota


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ExchangeRate-** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the current exchange rates for USD?"

**🤖 AI Agent:**
> I've fetched the latest rates for USD. Currently, 1 USD is equivalent to 0.92 EUR, 0.79 GBP, and 148.50 JPY. Would you like to see more currencies?

---

**👤 You:**
> "Convert 500 EUR to GBP."

**🤖 AI Agent:**
> Using the `get_pair_conversion` tool, 500 EUR converts to approximately 428.50 GBP based on the current mid-market rate.

---

**👤 You:**
> "What was the exchange rate for USD to EUR on January 1st, 2020?"

**🤖 AI Agent:**
> I've retrieved the historical data for 2020-01-01. On that date, the exchange rate from USD to EUR was 0.891. Would you like to check another date?


## Installation & Usage

To install and use the **ExchangeRate-** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exchangerate](https://vinkius.com/mcp/exchangerate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
