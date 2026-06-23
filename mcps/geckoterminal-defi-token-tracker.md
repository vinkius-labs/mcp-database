# GeckoTerminal (DeFi Token Tracker) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geckoterminal-defi-token-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track DeFi tokens, liquidity pools, and DEX activity across 100+ blockchains using real-time GeckoTerminal data.

## Description
Connect **GeckoTerminal** to your AI agent to monitor the decentralized finance (DeFi) landscape in real-time. Access comprehensive data on millions of tokens and thousands of liquidity pools across all major blockchain networks.

### What you can do

- **Network & DEX Discovery** — List all supported blockchain networks and the decentralized exchanges (DEXes) operating on them.
- **Trending & New Pools** — Identify what's hot in the market by querying trending pools globally or on specific networks like Ethereum, Solana, or BSC.
- **Deep Pool Analytics** — Fetch precise pricing, liquidity depth, and 24h volume for any specific liquidity pool address.
- **Token Intelligence** — Retrieve detailed token metadata, contract information, and market caps for any DeFi asset.
- **Market Dynamics** — Access historical OHLCV data for charting and list the most recent trades to analyze whale movements and retail flow.

### How it works

1. Subscribe to this server
2. Enter your GeckoTerminal API Key (if required for higher rate limits)
3. Start analyzing the DeFi market directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DeFi Traders** — quickly find trending pairs and analyze liquidity before making a move.
- **Data Analysts** — extract historical price data and trade history for research and modeling.
- **Web3 Developers** — verify pool addresses and token metadata without leaving your coding environment.


## Available Tools (17)
- **get_multiple_pools**: Get details for multiple pools
- **get_multiple_tokens**: Get details for multiple tokens
- **get_network**: Get details for a specific network
- **get_ohlcv**: Get historical price data (OHLCV) for a pool
- **get_pool**: Get specific pool details
- **get_token_info**: Get token metadata info
- **get_token**: Get specific token details
- **list_dexes**: List DEXes on a specific network
- **list_networks**: List all supported blockchain networks
- **list_top_pools_dex**: Get top pools for a specific DEX
- **list_top_pools_for_token**: Get top pools for a specific token
- **list_top_pools_network**: Get top pools on a network
- **list_trades**: Get recent trades for a pool
- **get_new_pools_all**: Get new pools across all networks
- **get_new_pools_network**: Get new pools on a specific network
- **get_trending_pools_all**: Get trending pools across all networks
- **get_trending_pools_network**: Get trending pools on a specific network


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GeckoTerminal (DeFi Token Tracker)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported blockchain networks on GeckoTerminal."

**🤖 AI Agent:**
> I've retrieved the list of supported networks. GeckoTerminal currently supports over 100 networks, including Ethereum (eth), Solana (solana), Arbitrum (arbitrum), and Polygon (polygon_pos). Which network would you like to explore?

---

**👤 You:**
> "Show me the trending pools on the Ethereum network."

**🤖 AI Agent:**
> Fetching trending pools on Ethereum... I found several active pools. The top trending ones include PEPE/WETH on Uniswap V3 and USDC/WETH. Would you like detailed analytics for any of these specific pools?

---

**👤 You:**
> "Get token information for the contract address 0x... on Ethereum."

**🤖 AI Agent:**
> Analyzing token data... For the provided address on Ethereum, the token is identified as 'ExampleToken' (EXT). It has a current market cap of $5M and is traded primarily on Uniswap. Would you like to see the top liquidity pools for this token?


## ❓ FAQ

**Q: Can I see the trending liquidity pools on a specific network like Solana?**
Yes! Use the `get_trending_pools_network` tool with the network ID 'solana'. The agent will return a list of the most active pools currently trending on that blockchain.

**Q: How do I get historical price data (OHLCV) for a specific token pool?**
You can use the `get_ohlcv` tool. Provide the network ID and the pool address to retrieve historical open, high, low, close, and volume data for various timeframes.

**Q: Is it possible to list the most recent trades for a pair?**
Absolutely. Use the `list_trades` tool with the network ID and pool address. It will fetch the latest transaction history, including trade size and timestamps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geckoterminal-defi-token-tracker](https://vinkius.com/mcp/geckoterminal-defi-token-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GeckoTerminal (DeFi Token Tracker)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `geckoterminal-defi-token-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GeckoTerminal (DeFi Token Tracker)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geckoterminal-defi-token-tracker": {
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
