# CoinDesk Bitcoin Price Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coindesk-bitcoin-price-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Universal Bitcoin intelligence — get real-time BPI prices and supported currencies via AI.

## Description
Equip your AI agent with real-time cryptocurrency intelligence through the **CoinDesk** MCP server. This integration provides instant access to the Bitcoin Price Index (BPI), the industry standard for Bitcoin valuation. Your agent can retrieve current prices in USD, GBP, and EUR, and explore the list of all supported global currencies. Whether you are tracking market moves, auditing portfolio values, or researching crypto trends, your agent acts as a dedicated financial analyst through natural conversation.

### What you can do

- **Real-time BPI** — Get the current Bitcoin price updated every minute in major currencies.
- **Currency Intelligence** — List all global currencies supported by the CoinDesk index.
- **Market Monitoring** — Stay informed about Bitcoin's valuation through official data sources.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying Bitcoin data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Investors** — monitor real-time Bitcoin prices for their portfolios.
- **Financial Analysts** — pull reliable BPI data for reports and market research.
- **Fintech Developers** — integrate official Bitcoin pricing into their AI applications.


## Available Tools (8)
- **get_bitcoin_price_global**: Get current Bitcoin price for globally recognized currencies (BPI)
- **get_bitcoin_price_custom**: g. BRL, JPY, CNY).

Get current Bitcoin price in a specific local currency
- **get_coindesk_disclaimer**: Get official CoinDesk terms and disclaimer
- **get_latest_update_time**: Get the exact UTC timestamp of the last Bitcoin trade analyzed
- **get_bitcoin_price_eur**: Get current Bitcoin price in EUR
- **get_bitcoin_price_gbp**: Get current Bitcoin price in GBP
- **get_bitcoin_price_usd**: Get current Bitcoin price in USD
- **list_supported_currencies**: List supported fiat currencies for Bitcoin tracking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinDesk Bitcoin Price Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current Bitcoin price?"

**🤖 AI Agent:**
> Retrieving the latest Bitcoin Price Index... According to CoinDesk, Bitcoin is currently trading at $65,432.10 USD. I also have the rates in GBP and EUR if you're interested.

---

**👤 You:**
> "Show me the Bitcoin price in British Pounds (GBP)."

**🤖 AI Agent:**
> Checking the BPI... Bitcoin is currently worth £51,200.45 GBP. Would you like to see the price in other currencies?

---

**👤 You:**
> "List all currencies supported by the Bitcoin index."

**🤖 AI Agent:**
> Retrieving the supported currency list... CoinDesk supports a wide range of currencies including AED, ARS, AUD, BRL, CAD, and many more. I can provide the full details if you'd like to see specific codes.


## ❓ FAQ

**Q: Can I get the current price of Bitcoin in EUR?**
Yes! Use the `get_bitcoin_price_global` tool. The response will include the current rate for USD, GBP, and EUR as provided by the CoinDesk index.

**Q: How often is the BPI updated?**
The Bitcoin Price Index (BPI) is updated every minute to reflect real-time market changes across global exchanges.

**Q: Which currencies are supported by CoinDesk?**
CoinDesk supports dozens of global currencies. Use the `list_supported_currencies` tool to see the full list of ISO codes and names supported by the index.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coindesk-bitcoin-price-index](https://vinkius.com/mcp/coindesk-bitcoin-price-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoinDesk Bitcoin Price Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coindesk-bitcoin-price-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoinDesk Bitcoin Price Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coindesk-bitcoin-price-index": {
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
