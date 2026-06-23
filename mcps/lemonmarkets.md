# lemon.markets MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lemonmarkets)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Trade European stocks and ETFs and access real-time market data via lemon.markets.

## Description
Connect your **lemon.markets** account to any AI agent to automate your stock trading and market analysis. This MCP server enables your agent to search for instruments, retrieve real-time quotes, and manage your brokerage orders directly.

### What you can do

- **Market Discovery** — Search for European stocks and ETFs by name or ISIN across major exchanges
- **Real-time Pricing** — Get the latest bid/ask quotes and price data for any tradable instrument
- **Portfolio Oversight** — List your active positions and retrieve detailed account balance information
- **Order Execution** — Place, activate, and cancel buy or sell orders directly from natural language
- **Trading History** — Monitor your order status and transaction history to track your investment performance

### How it works

1. Subscribe to this server
2. Enter your lemon.markets API Key
3. Start trading and analyzing the market from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Individual Investors** — Quickly check quotes and manage your portfolio via natural language commands
- **Financial Analysts** — Automate the retrieval of real-time market data for research and reporting
- **Developers** — Integrate stock trading and market data retrieval into custom trading bots or applications


## Available Tools (8)
- **get_brokerage_account**: markets trading account.

Get trading account information
- **activate_pending_order**: Activate a placed order to execute it
- **cancel_open_order**: Cancel an open order
- **get_latest_quote**: Get the latest bid/ask prices for an instrument
- **list_brokerage_orders**: List recent trading orders
- **place_new_order**: Note: Orders must usually be activated after creation.

Place a new buy or sell order
- **list_active_positions**: List all currently held portfolio positions
- **search_market_instruments**: g., "Apple", "Tesla", or a specific ISIN).

Search for stocks or ETFs on lemon.markets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **lemon.markets** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the ISIN for 'Volkswagen' on lemon.markets."

**🤖 AI Agent:**
> I've searched for 'Volkswagen' and found several instruments. The primary ISIN for Volkswagen AG is 'DE0007664039'. Would you like the latest quote for this asset?

---

**👤 You:**
> "Get the latest ask price for Tesla (ISIN: 'US88160R1014')."

**🤖 AI Agent:**
> The latest quote for Tesla (US88160R1014) shows an Ask price of $175.40 and a Bid price of $175.35.

---

**👤 You:**
> "List my active trading orders."

**🤖 AI Agent:**
> I've retrieved your orders. You have 2 active orders: a BUY for Apple (quantity: 10) and a SELL for BMW (quantity: 5). Both are currently in 'activated' status.


## ❓ FAQ

**Q: How do I search for an instrument if I don't have the ISIN?**
Use the `search_market_instruments` tool with a keyword like 'Apple' or 'Tesla' to retrieve a list of matching assets and their unique ISINs.

**Q: Do I need to activate an order after placing it?**
Yes, lemon.markets usually requires orders to be explicitly activated using the `activate_pending_order` tool before they are sent to the exchange.

**Q: Can I see my current portfolio positions?**
Absolutely. Use the `list_active_positions` tool to retrieve a list of all instruments you currently hold in your brokerage account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lemonmarkets](https://vinkius.com/mcp/lemonmarkets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **lemon.markets** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lemonmarkets` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **lemon.markets** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lemonmarkets": {
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
