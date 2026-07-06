# Intrinio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/intrinio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical financial market data via Intrinio API.

## Description
Empower your AI agents with Intrinio's comprehensive financial data. This MCP server allows you to retrieve real-time and historical stock prices, access financial statements, search for companies, and track earnings releases and IPO calendars directly through the Intrinio API. Ideal for financial analysis, portfolio monitoring, and market research.


## Available Tools (10)
- **get_financials**: Returns line items and values. Essential for fundamental financial analysis and performance vetting.

Retrieves financial statements for a company
- **get_ipo_calendar**: Useful for identifying new market entrants and investment opportunities.

Retrieves the IPO calendar
- **get_security**: Returns exchange info, security type, and identifiers. Use this to distinguish between different types of instruments traded under similar names.

Retrieves details for a specific security
- **get_stock_prices**: Use this to analyze market performance and price trends over time.

Retrieves historical stock prices for a security
- **list_companies**: Returns company names, tickers, and internal IDs. Use this to discover tickers before querying specific stock prices or financial statements.

Lists all companies covered by Intrinio
- **list_indices**: g., S&P 500, Dow Jones) tracked by Intrinio. Use this to identify index identifiers before querying index performance data.

Lists stock market indices
- **list_news**: Useful for monitoring market-moving events and recent announcements from public companies.

Lists latest financial news
- **search_companies**: Use this when the user provided a partial company name and you need to locate the correct ticker or ID.

Searches for companies by name or ticker
- **get_company**: g., "AAPL") or ID. Returns headquarters address, employee counts, and business descriptions. Useful for providing a profile overview of a company.

Retrieves details for a specific company
- **get_earnings_releases**: Essential for tracking reporting seasons and anticipating market volatility for specific tickers.

Lists upcoming and past earnings releases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Intrinio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List financial statements for Apple (AAPL)."

**🤖 AI Agent:**
> I'll fetch the financial data for Apple Inc. for you.

---

**👤 You:**
> "Get the latest stock price for Microsoft."

**🤖 AI Agent:**
> I'll retrieve the current stock price for Microsoft (MSFT).

---

**👤 You:**
> "Search for companies in the 'Software' industry."

**🤖 AI Agent:**
> I'll look up companies in the software sector using Intrinio.


## ❓ FAQ

**Q: How do I get Intrinio API credentials?**
Log in to your Intrinio account, go to Account > API Keys, and copy your API Key. Ensure you have an active subscription for the data feeds you need.

**Q: Which markets are covered?**
Intrinio provides extensive coverage of US and international stock exchanges, indices, and financial data.

**Q: Can I see real-time stock prices?**
Yes, the get_stock_prices tool provides access to real-time and historical pricing data, depending on your subscription plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/intrinio](https://vinkius.com/mcp/intrinio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Intrinio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `intrinio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Intrinio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "intrinio": {
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
