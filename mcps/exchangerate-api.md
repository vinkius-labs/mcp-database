# ExchangeRate-API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exchangerate-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Global currency exchange platform — get real-time rates and perform conversions via AI.

## Description
Equip your AI agent with real-time financial intelligence via **ExchangeRate-API**. This unified server provides your agent with instant access to current and historical exchange rates for over 160 currencies. Your agent can search for the latest rates, audit currency pairs, and retrieve enriched metadata for any supported currency without you ever searching manually. Whether you are auditing international transactions or managing global financial operations, your agent acts as a dedicated currency analyst and conversion expert through natural conversation.

### What you can do

- **Real-time Rates** — Access the latest exchange rates for any base currency, updated in real-time.
- **Pair Conversion** — Calculate exact exchange rates or convert specific amounts between any two currency codes.
- **Historical Auditing** — Fetch exchange rates for any specific date in the past to analyze financial trends.
- **Currency Intelligence** — List all supported currencies and retrieve enriched metadata including full names and flags.
- **Data Integrity** — Retrieve reliable financial data used by thousands of companies worldwide.

### How it works

1. Subscribe to this server
2. Enter your ExchangeRate-API Key
3. Start managing your currency intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts & Accountants** — perform rapid currency conversions and audit historical rates for reporting.
- **E-commerce Managers** — monitor real-time exchange rates to optimize global pricing strategies.
- **Travelers & Digital Nomads** — get instant conversion results for their specific location and budget planning.
- **Developers** — integrate reliable currency workflows into their applications through an AI-guided interface.
- **Investment Teams** — stay updated on global currency fluctuations for organizational planning.


## Available Tools
- **get_enriched_currency_data**: g., flag, full name).

Get enriched currency information
- **get_historical_rates**: Get historical exchange rates
- **get_latest_rates**: g., USD).

Get latest exchange rates
- **convert_currency_pair**: Convert between two currencies
- **list_supported_currencies**: List all supported currencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ExchangeRate-API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 100 USD to Brazilian Real."

**🤖 AI Agent:**
> Retrieving the latest rate for USD/BRL... 100 USD is currently equivalent to approximately 500 BRL. Would you like me to check the historical rate for this pair?

---

**👤 You:**
> "Show the current exchange rates for EUR."

**🤖 AI Agent:**
> Fetching latest rates with EUR as the base currency... I've identified the exchange values for 160+ currencies, including USD (1.08), GBP (0.85), and JPY (162.50). Shall I list more?

---

**👤 You:**
> "What was the exchange rate for USD to EUR on January 1st, 2020?"

**🤖 AI Agent:**
> Retrieving historical data for 2020-01-01... On that day, 1 USD was worth approximately 0.89 EUR. I can pull the full data table for that specific date if you need.


## ❓ FAQ

**Q: How many currencies are supported by this integration?**
ExchangeRate-API supports over 160 world currencies. You can use the `list_supported_currencies` tool to see the full list of available codes and their corresponding names.

**Q: Can I perform a direct conversion between USD and EUR with a specific amount?**
Yes! Use the `convert_currency_pair` tool and provide 'USD' in the `from` parameter, 'EUR' in the `to` parameter, and your desired amount. The agent will calculate the result based on the latest rates.

**Q: Is historical exchange rate data available?**
Absolutely. You can use the `get_historical_rates` tool by providing the base currency and the specific year, month, and day. This allows you to audit financial records from any point in the past.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exchangerate-api](https://vinkius.com/mcp/exchangerate-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ExchangeRate-API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `exchangerate-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ExchangeRate-API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exchangerate-api": {
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
