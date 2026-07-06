# Dextools (DeFi Token Data API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dextools-defi-token-data-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time DeFi market data, token prices, liquidity pairs, and blockchain information across multiple networks via Dextools.

## Description
Connect your **Dextools** API account to any AI agent to analyze decentralized finance (DeFi) markets with precision. Get instant access to token metrics, liquidity pools, and price variations across dozens of supported blockchains.

### What you can do

- **Blockchain Discovery** — List all supported networks like Ethereum, BSC, Polygon, and more using the `get_blockchains` tool.
- **Token Analytics** — Fetch detailed metadata including supply, decimals, and current market valuation with `get_token`.
- **Liquidity Monitoring** — Inspect specific pool addresses to understand market depth and pair health via `get_token_liquidity`.
- **Price Tracking** — Get real-time price data and 24-hour variations for any token contract using `get_token_price`.
- **Pair Inspection** — Retrieve detailed information about specific liquidity pairs with `get_pair`.

### How it works

1. Subscribe to this server
2. Enter your Dextools API Key
3. Start querying DeFi data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DeFi Traders** — quickly verify token prices and liquidity without switching between multiple DEX explorers
- **Web3 Developers** — integrate real-time market data into your development workflow or bot logic
- **Crypto Analysts** — automate the gathering of token metrics and blockchain support lists for research reports


## Available Tools (5)
- **get_token_liquidity**: Get liquidity information for a token or pair
- **get_token_price**: Get the current price of a token
- **get_token**: Retrieve detailed information about a specific token
- **get_blockchains**: Retrieve a list of supported blockchain networks
- **get_pair**: Retrieve information about liquidity pairs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dextools (DeFi Token Data API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported blockchain networks on Dextools."

**🤖 AI Agent:**
> I've retrieved the supported chains. Dextools currently supports networks including Ethereum (ether), Binance Smart Chain (bsc), Polygon (polygon), Solana (solana), and many others. Which one would you like to explore?

---

**👤 You:**
> "Get the current price and 24h change for token 0x... on Ethereum."

**🤖 AI Agent:**
> Fetching price data... The token at that address is currently trading at $1.24 with a +5.2% increase over the last 24 hours on the Ethereum network.

---

**👤 You:**
> "Show me the liquidity information for the pair 0x... on BSC."

**🤖 AI Agent:**
> Analyzing liquidity... For the specified pair on Binance Smart Chain, the total liquidity is approximately $500,000 USD. Would you like to see the individual token reserves for this pool?


## ❓ FAQ

**Q: Can I check the current price of a token on a specific blockchain?**
Yes! Use the `get_token_price` tool by providing the blockchain identifier (e.g., 'ether') and the token's contract address. It will return the current price and 24h variation.

**Q: How do I see which networks Dextools currently supports?**
Simply run the `get_blockchains` tool. It will provide a complete list of all blockchain networks integrated with the Dextools API.

**Q: Is it possible to analyze the liquidity of a specific trading pair?**
Absolutely. You can use `get_token_liquidity` with the pair address or `get_pair` to fetch comprehensive data about liquidity pools, including volume and health metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dextools-defi-token-data-api](https://vinkius.com/mcp/dextools-defi-token-data-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dextools (DeFi Token Data API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dextools-defi-token-data-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dextools (DeFi Token Data API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dextools-defi-token-data-api": {
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
