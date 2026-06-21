# Bitstamp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bitstamp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Trade and monitor crypto markets via Bitstamp — get tickers, order books, account balances, and manage orders.

## Description
Connect your AI agent to Bitstamp, one of the world's most established cryptocurrency exchanges. Access real-time market data and manage your private account seamlessly through natural conversation.

### What you can do

- **Market Monitoring** — Get instant tickers, order books, and recent transactions for hundreds of trading pairs (BTC, ETH, XRP, etc.)
- **Account Management** — Check your balances across all supported currencies and track your transaction history
- **Order Control** — List your open orders and cancel them when needed directly via the agent
- **Trading Pair Info** — Discover all supported pairs and their specific trading minimums and rules

### How it works

1. Subscribe to this server
2. Enter your **Bitstamp API Key** and **API Secret** (generated in your Bitstamp account settings)
3. Start managing your crypto portfolio through chat

This integration uses Bitstamp's latest V2 API with high-security HMAC-SHA256 signing for all private operations.

### Who is this for?

- **Traders** — quickly check prices and book depth during market volatility
- **Portfolio Managers** — keep track of balances and historical performance
- **Crypto Enthusiasts** — stay informed about market movements without leaving your workspace


## Available Tools
- **cancel_order**: Cancel an open order
- **get_balance**: Get account balances for all currencies
- **get_open_orders**: Get all currently open orders
- **get_order_book**: Get the current order book for a currency pair
- **get_ticker**: Get current market ticker for a currency pair
- **list_trading_pairs**: List all available trading pairs and their info
- **get_user_transactions**: Get personal transaction history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bitstamp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price of BTC/USD on Bitstamp?"

**🤖 AI Agent:**
> The current BTC/USD price is $87,250.21, with a 24h high of $88,100 and a 24h volume of 1,240 BTC.

---

**👤 You:**
> "Check my account balance."

**🤖 AI Agent:**
> You currently have 0.45 BTC and 1,200.50 USD available in your Bitstamp account.

---

**👤 You:**
> "List my open orders on Bitstamp."

**🤖 AI Agent:**
> I've retrieved your open orders. You have 2 active limit orders: a buy order for 0.1 BTC at $85,000 and a sell order for 1 ETH at $3,500.


## ❓ FAQ

**Q: Is it safe to enter my Bitstamp API keys?**
Yes. Your keys are handled securely by the Vinkius Cloud environment and are never logged or exposed. We recommend creating an API key with only 'Read' and 'Trade' permissions, excluding 'Withdraw' for maximum safety.

**Q: What currency pairs are supported?**
Bitstamp supports a wide range of pairs including BTC, ETH, XRP, LTC, BCH, and many more against USD, EUR, and GBP. Use the `list_trading_pairs` tool to see the full current list.

**Q: How do I find my Bitstamp API credentials?**
Log in to your Bitstamp account, navigate to **Settings** > **API Control**, and click **New API Key**. Make sure to save your Key and Secret immediately as they won't be shown again.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bitstamp](https://vinkius.com/mcp/bitstamp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bitstamp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bitstamp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bitstamp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bitstamp": {
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
