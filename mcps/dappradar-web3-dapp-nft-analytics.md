# DappRadar (Web3 Dapp & NFT Analytics) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dappradar-web3-dapp-nft-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time Web3 data via DappRadar — analyze dapps, NFT collections, and blockchain ecosystem metrics directly from your AI agent.

## Description
Connect your **DappRadar** API to any AI agent to gain deep insights into the Web3 ecosystem. Track decentralized applications, NFT market movements, and blockchain performance through natural conversation.

### What you can do

- **Dapp Discovery** — List and filter thousands of dapps by blockchain (Ethereum, Polygon, etc.) or category (Games, DeFi, Social)
- **NFT Intelligence** — Access ranked NFT collections, metadata, and historical floor price or volume metrics
- **Historical Metrics** — Retrieve precise historical data for Users, Transactions, and Volume for any tracked dapp
- **Ecosystem Analysis** — Get aggregate stats for entire blockchain networks to understand market share and growth
- **Deep Dapp Inspection** — Fetch detailed metadata and developer information for specific decentralized projects

### How it works

1. Subscribe to this server
2. Enter your DappRadar API Key
3. Start querying Web3 analytics from Claude, Cursor, or any MCP-compatible client

No more manual searching through dashboards. Your AI acts as a Web3 data scientist, providing instant reports on the latest crypto trends.

### Who is this for?

- **Web3 Developers** — monitor competitor metrics and ecosystem health directly from your coding environment
- **Crypto Analysts** — generate instant reports on NFT collection performance and dapp user growth
- **Investors & Researchers** — track historical volume and transaction trends to identify emerging market opportunities


## Available Tools
- **get_chain_stats**: Get aggregate metrics for a specific blockchain ecosystem
- **get_dapp_metrics**: Get historical activity metrics for a specific dapp
- **get_dapp**: Get detailed information for a specific dapp
- **get_nft_collection_metrics**: Get historical metrics for a specific NFT collection
- **get_nft_collection**: Get metadata and stats for a specific NFT collection
- **list_chains**: List all blockchains supported by DappRadar
- **list_dapps**: Supports pagination and filtering by chain or category.

List all dapps tracked by DappRadar
- **list_nft_collections**: List ranked NFT collections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DappRadar (Web3 Dapp & NFT Analytics)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the top dapps in the games category on Ethereum."

**🤖 AI Agent:**
> I've retrieved the top games on Ethereum. Leading the list is 'Axie Infinity' followed by 'Illuvium'. Would you like to see detailed metrics for any of these?

---

**👤 You:**
> "Show me the historical user metrics for Uniswap."

**🤖 AI Agent:**
> Fetching historical data for Uniswap... Over the last 30 days, unique active wallets peaked at 45,000 per day with a total volume of $1.2B. Do you want the transaction count as well?

---

**👤 You:**
> "Get the floor price and sales data for the Bored Ape Yacht Club NFT collection."

**🤖 AI Agent:**
> Analyzing Bored Ape Yacht Club... The current floor price is 12.5 ETH with 15 sales recorded in the last 24 hours. The total volume for this period is 190 ETH.


## ❓ FAQ

**Q: Can I see historical volume and sales for a specific NFT collection?**
Yes! Use the `get_nft_collection_metrics` tool with the collection ID. It returns historical floor prices, volume, and sales data to help you analyze market trends.

**Q: How do I find the top performing dapps on a specific blockchain like Polygon?**
You can use the `list_dapps` tool and provide 'polygon' in the `chain` parameter. You can also filter by category like 'games' or 'defi' to narrow down your search.

**Q: Is it possible to get aggregate statistics for an entire blockchain ecosystem?**
Absolutely. Use the `get_chain_stats` tool with the name of the blockchain (e.g., 'ethereum'). It will provide aggregate metrics for that specific ecosystem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dappradar-web3-dapp-nft-analytics](https://vinkius.com/mcp/dappradar-web3-dapp-nft-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DappRadar (Web3 Dapp & NFT Analytics)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dappradar-web3-dapp-nft-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DappRadar (Web3 Dapp & NFT Analytics)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dappradar-web3-dapp-nft-analytics": {
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
