# Buenbit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buenbit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate Crypto Exchange operations via Buenbit — track balances, extract asset tickers, and execute real-time trading directly from conversational AI.

## Description
Connect your **Buenbit** trading account to any AI agent and manage your decentralized portfolio seamlessly through a conversational layer geared toward Latin American markets.

### What you can do

- **Live Tickers** — Query real-time snapshot prices for critical cross-pairs like `USDC/ARS` or `BTC/USD` before invoking macro logics.
- **Portfolio Balances** — Read fiat availability and absolute cryptographic savings instantly to evaluate internal liquidity.
- **Market Execution** — Create sophisticated buy or sell limit orders without opening the heavily loaded UI panel on your phone.
- **Transaction Mapping** — Review and assert if a recent deposit hitting a specific destination address matured successfully.

### How it works

1. Add this integration natively inside Vurb.
2. Bind your tightly scoped API keys generated strictly from the desktop trading panel.
3. Turn Claude or Cursor into your heavily quantitative local trading wingman.

### Who is this for?

- **Crypto Traders** — Orchestrating quantitative models via local prompts or autonomous pipelines to secure yields.
- **Financial Officers** — Validating treasury cashouts on corporate accounts inside Argentina and LATAM easily.
- **Everyday Investors** — Simply wanting the easiest API tunnel to monitor if Ethereum exploded overnight.


## Available Tools
- **cancel_order**: Cancel a pending crypto order
- **create_order**: Create a new market/limit trade order
- **execute_withdrawal**: Broadcast a native withdrawal
- **get_crypto_prices**: Read universal conversion spot prices
- **get_deposit_address**: Scan infrastructure wallet address
- **get_network_fees**: Get current network gas costs
- **get_ticker**: g. BTC/ARS, USDC/ARS).

Get current market ticker prices
- **get_yield_rates**: Get staking pool rates
- **list_assets**: Explore available crypto assets catalog
- **list_balances**: List portfolio wallet balances
- **list_limits**: Get profile trade limits
- **list_orders**: List recorded exchange orders
- **list_transactions**: List money and crypto transactions
- **list_withdrawals**: List crypto withdrawals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buenbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the ticker for the BTC to ARS market pairing securely right now."

**🤖 AI Agent:**
> Ticker validated. The BTC/ARS pairing is trading with a Last Ask of $41M ARS and a Last Bid hovering smoothly around $40.5M.

---

**👤 You:**
> "Display my exact crypto availability looking at balances under my Buenbit portfolio."

**🤖 AI Agent:**
> Inspecting bounds. You hold `1.204 ETH`, `450.00 USDC`, and a small trace amount fiat standing natively at `50,000 ARS`. Let me know if you intend to initiate a market buy.

---

**👤 You:**
> "Instantly place a Limit Buy order. Spend around $30 USDC grabbing Bitcoin at roughly 68k edge margin."

**🤖 AI Agent:**
> Understood. Bypassing UI layers to submit `create_order` against 'btcusdc' natively. Limit Buy Order successfully pushed. Order ID `3029ab1-z` resting deeply on the book. Shall I review active orders list?


## ❓ FAQ

**Q: Is it safe to pass my Secret API Key to this agent?**
Vurb explicitly executes locally unless connected through audited Edge channels. Setting `sensitive: true` physically hides your credentials. Be sure your Buenbit API scope restricts withdrawals to safeguard capital.

**Q: Do I need to generate an HMAC signature manually for trades?**
No. The Server abstracts this. Simply instruct 'Buy 0.1 BTC at Limit' and the Agent utilizes the provided API Secret internally to digest and authenticate the packet.

**Q: How can I easily get my public deposit address for stablecoins?**
Invoke `get_deposit_address` telling the LLM the desired symbol (e.g. `usdc`, `usdt`). It fetches the exact blockchain string address tied uniquely to your wallet profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buenbit](https://vinkius.com/mcp/buenbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Buenbit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `buenbit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buenbit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buenbit": {
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
