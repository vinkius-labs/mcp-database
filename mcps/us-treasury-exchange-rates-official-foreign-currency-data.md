# U.S. Treasury Exchange Rates — Official Foreign Currency Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-treasury-exchange-rates-official-foreign-currency-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-treasury-exchange-rates-official-foreign-currency-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-treasury-exchange-rates-official-foreign-currency-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access the U.S. Treasury's official exchange rates for over 170 foreign currencies. Used by the government for financial reporting. Retrieve current rates or query historical exchange rates by country.

## Description
U.S. Treasury FX data.

### 2 Tools
- **Exchange Rates** — Latest official rates for 170+ currencies
- **Historical FX** — Currency history for specific countries

### Zero Auth


## Available Tools
- **get_treasury_exchange_rates**: Updated quarterly. Covers 170+ currencies against the U.S. dollar. These are the official rates used for government accounting and reporting.

Get official Treasury exchange rates for 170+ currencies
- **get_exchange_rate_for_currency**: Use the currency name or country (e.g., "Euro", "Japan-Yen", "Brazil-Real", "United Kingdom-Pound"). Updated quarterly.

Get Treasury exchange rate history for a specific currency
- **query_treasury_dataset**: treasury.gov. Provide the API endpoint path (e.g., /v2/accounting/od/debt_to_penny). Supports filter, sort, fields, and pagination parameters. See fiscaldata.treasury.gov for all available datasets.

Query any Treasury Fiscal Data dataset by endpoint path


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Treasury Exchange Rates — Official Foreign Currency Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the official Treasury exchange rate for the Euro?"

**🤖 AI Agent:**
> 📊 **Treasury Exchange Rates**

The EUR/USD rate for March 2026 is:
- 1 EUR = 1.085 USD
(Reported by the U.S. Treasury as 0.921 EUR per 1 USD)

---

**👤 You:**
> "Show the historical exchange rate for Brazil over the last year"

**🤖 AI Agent:**
> 📊 **Historical Rates: Brazil (Real)**

- Mar 2026: 4.95 BRL
- Dec 2025: 4.85 BRL
- Sep 2025: 5.02 BRL
- Jun 2025: 4.79 BRL

---

**👤 You:**
> "What is the Treasury rate for Japanese Yen?"

**🤖 AI Agent:**
> 📊 **Treasury Exchange Rates**

Official exchange rate for Japan (Yen) as of Mar 2026:
- 151.34 JPY per 1 USD


## Installation & Usage

To install and use the **U.S. Treasury Exchange Rates — Official Foreign Currency Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-treasury-exchange-rates-official-foreign-currency-data](https://vinkius.com/mcp/us-treasury-exchange-rates-official-foreign-currency-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
