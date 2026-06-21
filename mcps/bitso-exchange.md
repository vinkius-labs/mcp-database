# Bitso Exchange MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bitso-exchange)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Trade dynamically on Mexico's biggest Crypto Exchange. Access live balances, order books, and command trades programmatically.

## Description
Connect your heavy lifting quantitative **Bitso Platform Account** to the Vurb ecosystem forcing pure algorithmic logic to handle your portfolio bounds instead of manually refreshing charts.

### What you can do

- **Order Book Recon** — Pull tickers aggressively verifying spreads on massive pairs covering MXN, ARS, COP, or BRL prior to execution.
- **Wallet Tracking** — Constantly check available account capacity scanning fiat pools vs digital alt-coins natively inside your prompt.
- **Market Execution** — Place strict Limit or fast Market Orders bypassing phone apps directly routing straight to the official exchange backend.
- **Risk Management** — Cancel rogue open Maker orders immediately dropping them off the book if the market tanks!

### How it works

1. Append the node 
2. Extract your isolated 'Read/Write' Dev API Keys originating internally from Bitso.
3. Type your fiscal move into Claude and watch the ledger morph.

### Who is this for?

- **Local Traders** — Building strategies against fast USD-BRL deviations bridging crypto pools.
- **Web3 Architects** — Monitoring LatAm on/off ramps dynamically tied to system tests.
- **Power Holders** — Looking securely at account standing limits or balances without dealing with the slow GUI interfaces.


## Available Tools
- **cancel_order**: Cancel a live unfulfilled order
- **create_order**: Submit a new trading order
- **get_account_status**: Get regulatory account status limits
- **get_funding_destination**: Reveal inbound funding crypto address
- **get_ticker**: Get trading ticker information
- **list_available_books**: g., btc_mxn, eth_brl, usdc_ars) on the exchange.

List natively traded market books
- **list_balances**: List trading account balances
- **list_ledger**: Examine raw ledger account flows
- **list_open_orders**: List active hanging orders
- **list_order_trades**: Extract executions mapped to an Order ID
- **list_trades**: Review historical executed trades
- **list_withdrawals**: Monitor executed funds external withdrawals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bitso Exchange** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the ticker data right now looking heavily over the XRP to Mexican Peso book pair."

**🤖 AI Agent:**
> Target captured. The `xrp_mxn` book signals an active spread. Last executed price stands at $12.30 MXN, touching a 24H High roughly cresting near $12.80 with an aggregated voluminous 24H activity. Ready to position capital?

---

**👤 You:**
> "Issue a firm LIMIT buy. Let's bid placing around 0.1 Ether spending native BRL strictly on the eth_brl active ledger."

**🤖 AI Agent:**
> Processing command. Creating authenticated request. Your Limit Buy order successfully cleared local nodes towards Bitso's Maker tab binding ID `ox9...abc`. Tracking shows resting order unfulfilled. Need to list open positions?

---

**👤 You:**
> "Show my withdrawals"

**🤖 AI Agent:**
> I've retrieved your recent withdrawal history. You have 3 completed withdrawals this month: 0.05 BTC to an external wallet, 1,500 MXN via SPEI, and 200 XRP to another exchange.


## ❓ FAQ

**Q: Can I trust adding my Secret HMAC trading key into the agent flow safely?**
Yes. We wrap Bitso API requirements inside protected `sensitive: true` attributes isolating them visibly. Best practice dictates creating a Key exclusively with Trading power turning OFF 'Withdrawals'.

**Q: Do I have to calculate the complicated Bitso signatures by hand before calling createOrder?**
Absolutely not! The magic of these servers is that the internal code natively binds your keys and calculates the digest. You just ask to 'Buy BTC'.

**Q: Are ledger pulls real-time?**
Yes. Every time you call a tool like `get_ticker` or `get_order_book`, the agent fetches the most current data directly from Bitso's production API endpoints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bitso-exchange](https://vinkius.com/mcp/bitso-exchange)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bitso Exchange** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bitso-exchange` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bitso Exchange** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bitso-exchange": {
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
