# Currency Converter Fixed MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/currency-converter-fixed)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic historical currency conversion using ECB rates.

## Description
This MCP server provides deterministic currency conversion using fixed historical exchange rates sourced from the European Central Bank (ECB). It allows AI agents to perform precise historical calculations, check exchange rates for specific dates, and monitor currency stability. Use `convert_currency` to calculate specific amounts, `get_historical_rate` to retrieve specific pair rates, and `check_currency_stability` to detect hyperinflationary trends.


## Available Tools (3)
- **check_currency_stability**: Answers "Is [currency] currently experiencing hyperinflation?"
- **convert_currency**: Answers "How much is [amount] in [source] worth in [target] on [date]?"
- **get_historical_rate**: Answers "What was the exchange rate between [source] and [target] on [date]?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Currency Converter Fixed** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much is 100 USD worth in EUR on 2023-01-15?"

**🤖 AI Agent:**
> On January 15, 2023, 100 USD was worth 92.45 EUR.

---

**👤 You:**
> "What was the exchange rate between GBP and USD on 2022-05-20?"

**🤖 AI Agent:**
> The exchange rate between GBP and USD on May 20, 2022, was 1.24.

---

**👤 You:**
> "Is the Venezuelan Bolivar experiencing hyperinflation on 2023-10-01?"

**🤖 AI Agent:**
> Yes, the currency is flagged as hyperinflationary due to extreme volatility.


## ❓ FAQ

**Q: Are these live exchange rates?**
No, this server uses fixed historical rates from the European Central Bank (ECB) to ensure deterministic and reproducible results.

**Q: How is hyperinflation detected?**
Hyperinflation is flagged if a currency's value changes by more than 50% within a 30-day period relative to a stable anchor.

**Q: Which currencies are supported?**
The server supports all currencies compliant with the ISO 4217 standard that have recorded ECB historical data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/currency-converter-fixed](https://vinkius.com/ai-agent-connect/currency-converter-fixed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Currency Converter Fixed** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `currency-converter-fixed` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Currency Converter Fixed** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "currency-converter-fixed": {
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
