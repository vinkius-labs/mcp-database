# ZeroHash MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zerohash)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage digital asset infrastructure via ZeroHash — list assets, manage accounts, create customers, and execute trades directly from any AI agent.

## Description
Connect your **ZeroHash** API credentials to any AI agent to orchestrate digital asset workflows through natural language. ZeroHash provides the underlying infrastructure for crypto and stablecoin liquidity, custody, and settlement.

### What you can do

- **Asset & Account Discovery** — List supported assets and check real-time balances across account groups and types using `list_assets` and `list_accounts`.
- **Customer Onboarding** — Programmatically create new customer participants with full KYC data integration via `create_customer`.
- **Trading & Liquidity** — Request real-time quotes for asset pairs and execute trades instantly using `request_quote` and `execute_quote`.
- **Transfers & Deposits** — Manage crypto deposits, create transfers, and link external accounts for seamless movement of funds.
- **Transaction Auditing** — Query trade history and fetch specific trade metadata for reporting and compliance using `list_trades` and `get_trade`.

### How it works

1. Subscribe to this server
2. Enter your ZeroHash API Key, Private Key, and Passphrase
3. Start managing your digital asset operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — Test and integrate crypto workflows directly from your IDE without switching contexts.
- **Operations Managers** — Monitor account balances and trade history through simple conversational queries.
- **Compliance Officers** — Quickly retrieve participant data and trade records for auditing and reporting purposes.


## Available Tools (12)
- **list_accounts**: List accounts and current balances
- **list_assets**: List supported assets on ZeroHash
- **create_customer**: Create a new customer participant
- **create_transfer**: Use a unique client_transfer_id for idempotency.

Create an internal transfer between participants/accounts
- **list_crypto_deposits**: List incoming crypto deposits
- **execute_quote**: Execute a previously requested quote
- **get_trade**: Retrieve detailed information for a specific trade
- **link_external_account**: Link a bank account or blockchain address
- **list_participants**: List participants
- **request_quote**: Request a quote for a trade
- **get_time**: Unauthenticated.

Get current ZeroHash server time
- **list_trades**: List trades


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZeroHash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported stablecoins on ZeroHash."

**🤖 AI Agent:**
> I've retrieved the supported stablecoins. Currently, you can trade assets like USDC (on Ethereum and Solana), USDT, and PYUSD. Would you like to see the full details for any of these?

---

**👤 You:**
> "Check my current account balances for BTC and ETH."

**🤖 AI Agent:**
> Your current balances are: 1.25 BTC in your primary trading account and 15.0 ETH in your liquidity pool account. Do you need a breakdown of other assets?

---

**👤 You:**
> "Request a quote to buy 0.5 BTC using USD."

**🤖 AI Agent:**
> I've requested a quote for buying 0.5 BTC. The current rate is 65,000 USD per BTC, totaling 32,500 USD. This quote is valid for the next 30 seconds. Would you like to execute this trade?


## ❓ FAQ

**Q: How can I check which digital assets are currently supported for trading?**
You can use the `list_assets` tool. It allows you to filter by symbol, chain code, or specific features like whether the asset is a stablecoin or if staking is enabled.

**Q: Is it possible to onboard a new customer participant directly through the AI?**
Yes, the `create_customer` tool allows you to submit all necessary participant details, including name, email, address, and KYC status, to create a new record in ZeroHash.

**Q: How do I view my current balances across different account types?**
Use the `list_accounts` tool. You can filter the results by account group, label, owner, or specific asset to get a precise view of your holdings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zerohash](https://vinkius.com/mcp/zerohash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ZeroHash** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zerohash` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ZeroHash** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zerohash": {
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
