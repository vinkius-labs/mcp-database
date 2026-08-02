# Finnhub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/finnhub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time financial data — audit stocks, crypto, and market news via AI.

## Description
Empower your AI agent to orchestrate your entire financial research and market auditing workflow with **Finnhub**, the comprehensive platform for real-time stock and crypto data. By connecting Finnhub to your agent, you transform complex market querying into a natural conversation. Your agent can instantly retrieve stock quotes, audit company profiles, and monitor market news without you ever touching a financial terminal. Whether you are conducting investment research or tracking crypto trends, your agent acts as a real-time financial analyst, ensuring your intelligence is always grounded in live market data.

### What you can do

- **Stock Auditing** — Retrieve real-time price quotes for thousands of global stocks and maintain a clear view of market changes.
- **Company Oversight** — Audit comprehensive company profiles and basic financial metrics to understand organizational health.
- **Market Intelligence** — Search for stock and crypto symbols to identify relevant assets for your portfolio instantly.
- **News Discovery** — Monitor latest market news across various categories, including general, forex, and crypto, to stay on top of trends.
- **Crypto Monitoring** — List supported crypto symbols for dozens of exchanges to maintain strict control over digital asset data.

### How it works

1. Subscribe to this server
2. Enter your Finnhub API Key
3. Start managing your financial intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — monitor market performance and retrieve company metadata straight from your workflow.
- **Investors & Traders** — verify stock quotes and audit market news without manual searching.
- **Data Engineers** — perform rapid audits of financial symbols and identify asset markers through natural language.
- **Operations Leads** — automate financial data querying to orchestrate cross-functional investment teams smoothly.


## Available Tools (6)
- **list_crypto_symbols**: List supported crypto symbols for an exchange
- **get_basic_financials**: Get basic financial metrics for a company
- **get_market_news**: Get latest market news in a category
- **get_company_profile**: Get general information about a company by symbol
- **get_stock_quote**: Get real-time quote data for a specific stock symbol
- **search_symbols**: Search for stock or crypto symbols by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Finnhub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current stock quote for 'AAPL' (Apple) using Finnhub."

**🤖 AI Agent:**
> I've retrieved the quote for AAPL! The current price is $185.20, with a daily high of $186.50. The change for the day is +1.5%. Would you like to see the company profile or basic financials?

---

**👤 You:**
> "Show the latest news in the 'crypto' category."

**🤖 AI Agent:**
> I've retrieved the latest crypto market news. Notable headlines include updates on Bitcoin ETFs and new Ethereum upgrades. I can provide the links to the full articles if you'd like.

---

**👤 You:**
> "What are the basic financial metrics for 'MSFT' (Microsoft)?"

**🤖 AI Agent:**
> I've retrieved the financial metrics for Microsoft. Notable data includes a P/E ratio of 35.2 and a current dividend yield. I can provide the full breakdown of valuation and profitability markers if you'd like.


## ❓ FAQ

**Q: How do I find my Finnhub API Key?**
Log in to your [**Finnhub dashboard**](https://finnhub.io/dashboard), and you will find your API Key on the main page. Copy and paste it below.

**Q: Does it support real-time stock prices?**
Yes. The `get_stock_quote` tool provides real-time pricing data for supported exchanges globally.

**Q: Can the agent show news for a specific category?**
Yes. Use the `get_market_news` tool providing the `category` parameter (e.g., 'forex' or 'crypto'). Your agent will retrieve latest headlines for that vertical instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/finnhub](https://vinkius.com/mcp/finnhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Finnhub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `finnhub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Finnhub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "finnhub": {
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
