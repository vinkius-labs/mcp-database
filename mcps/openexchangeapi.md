# OpenExchangeAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openexchangeapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Retrive real-time exchange rates — audit currency data and conversions via AI.

## Description
Empower your AI agent to orchestrate your entire financial research and currency auditing workflow with **OpenExchangeAPI**, the reliable source for global exchange rates. By connecting OpenExchangeAPI to your agent, you transform complex currency data lookups into a natural conversation. Your agent can instantly retrieve latest rates, audit historical currency trends, and perform precise conversions without you ever touching a financial terminal. Whether you are conducting market analysis or managing international payments, your agent acts as a real-time financial analyst, ensuring your intelligence is always grounded in accurate, up-to-the-minute market data.

### What you can do

- **Rate Auditing** — Retrieve real-time exchange rates for over 200 currencies and maintain a clear view of global market fluctuations.
- **Historical Oversight** — Query historical rates for any specific date to audit past financial trends and valuations.
- **Conversion Intelligence** — Perform instant currency conversions between any pairs to assist in international budgeting.
- **Temporal Intelligence** — Query exchange rate time series to monitor currency performance over specific periods.
- **Usage Monitoring** — Get real-time API usage and plan metadata to maintain strict control over your research budget.

### How it works

1. Subscribe to this server
2. Enter your Open Exchange Rates App ID
3. Start managing your financial intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — monitor global exchange rates and retrieve historical metadata straight from your workflow.
- **E-commerce Managers** — verify current rates and audit currency conversions for international storefronts.
- **Forex Traders** — perform rapid audits of market trends and currency performance through natural language.
- **Operations Leads** — automate financial data querying to orchestrate cross-functional global teams smoothly.


## Available Tools (6)
- **convert_currency**: Convert an amount from one currency to another
- **get_latest_rates**: Get the latest exchange rates for a base currency
- **get_rate_time_series**: Get historical rates over a time period
- **get_api_usage**: Get current API usage and plan details
- **list_supported_currencies**: List all supported currency codes and names
- **get_historical_rates**: Get exchange rates for a specific historical date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenExchangeAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the latest exchange rates for 'EUR' using OpenExchangeAPI."

**🤖 AI Agent:**
> I've retrieved the latest rates with EUR as the base. Notable pairs include EUR/USD at 1.08 and EUR/GBP at 0.85. Would you like the full list of supported currencies?

---

**👤 You:**
> "Convert 100 USD to BRL."

**🤖 AI Agent:**
> Conversion complete! 100 USD is currently equivalent to 495.50 BRL based on the latest market data. Would you like me to check the historical rate for this pair?

---

**👤 You:**
> "What was the exchange rate for USD/JPY on 2020-01-01?"

**🤖 AI Agent:**
> I've retrieved the historical data for January 1st, 2020. The rate for USD/JPY was approximately 108.61. I can also provide the rates for other symbols on that date if needed.


## ❓ FAQ

**Q: How do I find my OpenExchange App ID?**
Log in to your [**Open Exchange Rates dashboard**](https://openexchangerates.org/login), and you will find your App ID on the home page. Copy and paste it below.

**Q: Does it support historical data?**
Yes. The `get_historical_rates` tool allows you to retrieve the official closing rates for any date since 1999.

**Q: Can the agent perform currency conversions?**
Yes. The `convert_currency` tool calculates the conversion between two currencies based on the latest market data instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openexchangeapi](https://vinkius.com/mcp/openexchangeapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenExchangeAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openexchangeapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenExchangeAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openexchangeapi": {
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
