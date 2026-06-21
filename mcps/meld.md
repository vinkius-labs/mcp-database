# Meld MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meld)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Unified API for digital assets via Meld — track blockchain networks, assets, and exchange rates.

## Description
Connect your **Meld** account to any AI agent and take full control of your digital asset intelligence and blockchain operations through natural conversation.

### What you can do

- **Network Orchestration** — List and inspect supported blockchain and financial networks and their statuses
- **Asset Management** — Retrieve detailed metadata and real-time pricing for cryptocurrencies and digital tokens
- **Rate Tracking** — Access real-time exchange rates between fiat currencies and various digital assets
- **Wallet & Transaction Monitoring** — List linked wallets, fetch balances, and track recent transaction histories securely
- **Market Research** — Search for specific digital assets by name or symbol to get current market data

### How it works

1. Subscribe to this server
2. Enter your Meld API Key and API Secret
3. Start managing your digital assets from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_account_info**: Get account information
- **get_asset**: Get details for a specific asset
- **get_exchange_rates**: Get real-time exchange rates
- **get_network**: Get details for a specific network
- **get_wallet_details**: Get details for a specific wallet
- **list_assets**: List all digital assets
- **list_networks**: List all digital asset networks
- **list_transactions**: List recent transactions
- **list_wallets**: List all linked wallets
- **search_assets**: Search for digital assets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meld** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported blockchain networks in Meld."

**🤖 AI Agent:**
> Retrieving networks... I found several supported networks including Ethereum, Polygon, and Bitcoin.

---

**👤 You:**
> "Get current exchange rate for BTC to USD."

**🤖 AI Agent:**
> Fetching exchange rates... 1 BTC is currently worth approximately 65,000 USD.

---

**👤 You:**
> "Show recent transactions for my account."

**🤖 AI Agent:**
> Querying transactions... You have 3 recent transactions, including a deposit of 0.5 ETH yesterday.


## ❓ FAQ

**Q: How do I find my Meld API Key and Secret?**
Log in to Meld, go to your Dashboard settings, and navigate to the API section to generate your key and secret.

**Q: What networks are supported by Meld?**
Meld supports a wide range of blockchain and traditional financial networks. Use the `list_networks` tool to see the current list.

**Q: Is my asset data secure?**
Absolutely. Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meld](https://vinkius.com/mcp/meld)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meld** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `meld` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meld** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meld": {
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
