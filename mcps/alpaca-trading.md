# Alpaca Trading MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alpaca-trading)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Trade stocks and crypto, access real-time market data, and manage your Alpaca brokerage account directly through any AI agent.

## Description
Connect your **Alpaca Markets** account to your AI agent to automate trading strategies and monitor market movements through natural language.

### What you can do

- **Order Execution** — Place market, limit, or stop orders for stocks and crypto assets using `create_order` and manage them with `delete_all_orders`.
- **Market Intelligence** — Retrieve historical bars, latest quotes, and trade data for stocks and crypto using tools like `get_stocks_bars` and `get_latest_stocks_quotes`.
- **Order Tracking** — Query your order history with advanced filters like status, symbols, and timeframes via `get_orders`.
- **Account Management** — Check your broker account details and update configurations such as fractional trading or shorting permissions with `update_account_configs`.
- **Asset Discovery** — List available assets and their trading status directly from the Alpaca exchange.

### How it works

1. Subscribe to this server
2. Enter your Alpaca API Key ID and Secret Key
3. Start trading and analyzing markets from Claude, Cursor, or any MCP-compatible client

Your AI acts as a sophisticated trading terminal, capable of executing complex orders and fetching deep market analytics without you ever leaving your workflow.

### Who is this for?

- **Quant Traders** — automate the execution of strategies and fetch historical data for backtesting analysis.
- **Retail Investors** — check portfolio status and place quick trades using simple conversational commands.
- **Developers** — integrate financial market data and trading capabilities directly into coding environments.


## Available Tools (14)
- **create_broker_account**: Requires contact, identity, disclosures, and agreements objects.

Create a new broker account
- **create_order**: Create a new trading order
- **delete_all_orders**: Returns a 207 Multi-Status.

Delete all open orders
- **get_assets**: List all tradable assets
- **get_broker_account**: Get broker account by ID
- **get_crypto_bars**: Get historical bars for crypto
- **get_latest_stocks_quotes**: Get latest quotes for stocks
- **get_latest_stocks_trades**: Get latest trades for stocks
- **get_orders**: Get all orders
- **get_stocks_bars**: Get historical bars for stocks
- **get_stocks_quotes**: Get historical quotes for stocks
- **get_stocks_trades**: Get historical trades for stocks
- **issue_token**: Issue OAuth2 tokens for machine-to-machine authentication
- **update_account_configs**: Update account configurations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alpaca Trading** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Buy 10 shares of AAPL at market price."

**🤖 AI Agent:**
> I've placed a market buy order for 10 shares of AAPL. The order ID is 550e8400-e29b. Would you like to track its status?

---

**👤 You:**
> "What are the latest quotes for BTC/USD and ETH/USD?"

**🤖 AI Agent:**
> Fetching latest data... BTC/USD is currently quoted at $64,230.50 (Bid) / $64,235.00 (Ask). ETH/USD is at $3,450.10 (Bid) / $3,452.00 (Ask).

---

**👤 You:**
> "Show me my closed orders from the last 7 days."

**🤖 AI Agent:**
> I found 3 closed orders in the last week: a buy of MSFT, a sell of TSLA, and a limit order for NVDA that was filled. Would you like the specific execution prices?


## ❓ FAQ

**Q: Can I place a trade for a specific dollar amount instead of shares?**
Yes, you can use the `notional` parameter in the `create_order` tool to specify the dollar amount you wish to trade for fractional-enabled assets.

**Q: How do I see only my open orders for a specific stock?**
Use the `get_orders` tool and set the `status` to 'open' and provide the ticker in the `symbols` parameter.

**Q: Can I cancel all my pending orders at once if the market moves against me?**
Absolutely. Use the `delete_all_orders` tool to instantly cancel all open orders in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alpaca-trading](https://vinkius.com/mcp/alpaca-trading)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alpaca Trading** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `alpaca-trading` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alpaca Trading** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alpaca-trading": {
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
