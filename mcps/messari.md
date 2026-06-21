# Messari MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/messari)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Crypto market intelligence via Messari — track assets, metrics, and blockchain news.

## Description
Connect your **Messari** account to any AI agent and access deep insights into the crypto ecosystem through natural conversation.

### What you can do

- **Asset Research** — List all available crypto assets and fetch detailed metadata and qualitative profiles
- **Quantitative Metrics** — Retrieve real-time pricing, market cap, and supply data for thousands of tokens
- **Market Monitoring** — Enumerate crypto exchanges and trading pairs to understand market depth
- **News & Intelligence** — Stay updated with an aggregated feed of crypto news and significant governance events
- **Deep Inspection** — Query historical timeseries and performance data for specific blockchain protocols

### How it works

1. Subscribe to this server
2. Enter your Messari API Key
3. Start querying crypto intelligence from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_asset_details**: g. btc, eth).

Get details for a crypto asset
- **get_asset_metrics**: Get metrics for a crypto asset
- **get_asset_profile**: Get asset profile
- **get_asset_market_data**: Get market data for an asset
- **get_crypto_news**: Get crypto news feed
- **list_assets**: List crypto assets
- **list_crypto_exchanges**: List supported exchanges
- **list_governance_events**: List governance events
- **list_crypto_markets**: List all crypto markets
- **search_assets**: Search for crypto assets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Messari** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show current metrics for Bitcoin (BTC)."

**🤖 AI Agent:**
> Retrieving metrics for Bitcoin... BTC is currently trading at $65,432.10 with a market cap of $1.28T and a 24h volume of $35B.

---

**👤 You:**
> "What are the latest crypto news headlines?"

**🤖 AI Agent:**
> Fetching news feed... Recent headlines include Ethereum's latest upgrade progress and new institutional Bitcoin products.

---

**👤 You:**
> "List all DeFi assets tracked by Messari."

**🤖 AI Agent:**
> Querying DeFi assets... I found several protocols including Uniswap (UNI), Aave (AAVE), and Maker (MKR).


## ❓ FAQ

**Q: How do I find my Messari API Key?**
Log in to Messari and navigate to your account settings at https://messari.io/account/api to generate or copy your key.

**Q: What kind of crypto assets are covered?**
Messari tracks thousands of assets, including major coins like Bitcoin and Ethereum, DeFi protocols, stablecoins, and emerging tokens.

**Q: Is my data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/messari](https://vinkius.com/mcp/messari)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Messari** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `messari` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Messari** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "messari": {
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
