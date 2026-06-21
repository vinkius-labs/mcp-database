# CoinGate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coingate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Accept cryptocurrency payments from customers worldwide with instant fiat settlement and multi-coin checkout support.

## Description
Connect your **CoinGate** account to any AI agent and take full control of your cryptocurrency payment operations and financial workflows through natural conversation.

### What you can do

- **Order Orchestration** — List and create new cryptocurrency payment orders programmatically, including monitoring price, currency, and real-time payment status
- **Payout Management** — Access and monitor your payout history and account balances to ensure efficient fund management across your crypto portfolio
- **Exchange Rate Intelligence** — Retrieve real-time exchange rates for Bitcoin, Ethereum, and dozens of other digital and fiat currencies directly through your agent
- **Shopper Relationship Management** — Access customer metadata and transaction histories to maintain a perfectly coordinated relationship ecosystem
- **Account Visibility** — Monitor your account profile and verification status directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your CoinGate dashboard (Settings > API)
3. Start managing your crypto business from Claude, Cursor, or any MCP client

No more manual address checking or digging through complex blockchain explorers. Your AI acts as your dedicated crypto operations and payment coordinator.

### Who is this for?

- **Web3 & Fintech Merchants** — instantly retrieve order statuses and update payment details using natural language commands
- **Finance Teams** — monitor payout histories and exchange rates without leaving your communication tools
- **Developers** — integrate automated crypto order creation and balance tracking into custom workflows through simple AI queries


## Available Tools
- **create_order**: Pass data as a JSON string.

Create a new payment order
- **get_account_info**: Get account profile details
- **get_order**: Get order details
- **get_exchange_rates**: Get current crypto exchange rates
- **list_orders**: List all crypto payment orders
- **list_payouts**: List all payouts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinGate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active payment orders in my CoinGate account."

**🤖 AI Agent:**
> I've retrieved your orders. You currently have 3 active transactions, including an order for 0.005 BTC (Status: Pending) and one for 150.00 EUR. Would you like the checkout URL for either of these?

---

**👤 You:**
> "What is the current BTC to USD exchange rate?"

**🤖 AI Agent:**
> Scanning market... The current exchange rate for BTC/USD is $65,420.50. I've also checked the EUR rate, which is €60,150.00. Shall I check your payout history for these assets?

---

**👤 You:**
> "Create a new 50 EUR payment order titled 'Service Fee'."

**🤖 AI Agent:**
> Order created successfully! I've initialized the 50.00 EUR payment order for 'Service Fee'. The Order ID is 'ord_789'. You can share this checkout link with the client: [Payment URL].


## ❓ FAQ

**Q: How do I find my CoinGate API Token?**
Log in to your account, navigate to the **API** section in your dashboard, and generate a new Bearer Token for your integration.

**Q: Which cryptocurrencies are supported for payments?**
CoinGate supports Bitcoin (BTC), Ethereum (ETH), Litecoin (LTC), and many other digital assets, plus major fiat currencies.

**Q: Can the agent check real-time exchange rates?**
Yes! The `get_exchange_rates` tool retrieves the most current market rates for all supported assets in the CoinGate ecosystem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coingate](https://vinkius.com/mcp/coingate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoinGate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `coingate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoinGate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coingate": {
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
