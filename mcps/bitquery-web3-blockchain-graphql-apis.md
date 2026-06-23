# Bitquery (Web3 Blockchain GraphQL APIs) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bitquery-web3-blockchain-graphql-apis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Query real-time and historical blockchain data across 40+ chains including Ethereum, Solana, and Bitcoin using GraphQL.

## Description
Connect to **Bitquery** to access comprehensive Web3 data through a unified GraphQL interface. This server allows your AI agent to fetch deep analytical insights from dozens of blockchains without needing individual node infrastructure.

### What you can do

- **Historical Analysis (V1)** — Query historical data across 40+ chains including Bitcoin, Tron, Polygon, and BNB. Perfect for auditing and long-term trend analysis.
- **Real-time Streaming (V2)** — Access live data for EVM-compatible chains and Solana. Monitor transfers, smart contract calls, and events as they happen.
- **DEX & DeFi Insights** — Use specialized cubes like `DexTrades` and `DexTradesByTokens` to track liquidity, trades, and token performance.
- **Smart Contract Inspection** — Analyze `Calls`, `Events`, and `Instructions` to understand protocol interactions and internal transactions.
- **Token Management** — Programmatically generate OAuth2 access tokens using your Client ID and Secret to maintain secure, automated connectivity.

### How it works

1. Subscribe to this server
2. Enter your Bitquery Access Token (or generate one using your credentials)
3. Start querying blockchain data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Debug smart contract calls and verify on-chain events directly from your IDE.
- **Data Analysts** — Perform cross-chain analysis and extract DeFi market metrics using natural language.
- **Security Researchers** — Audit historical transactions and track fund movements across multiple protocols.


## Available Tools (3)
- **generate_token**: The returned token should be used as the BITQUERY_ACCESS_TOKEN credential.

Generate an OAuth2 access token using Client ID and Secret
- **query_v1**: Provide a valid GraphQL query string.

Execute a GraphQL query against Bitquery V1 Historical API
- **query_v2**: Supports joins (e.g., joinCalls) and advanced filtering. Cubes include Transfers, Calls, Events, DexTrades, DexTradesByTokens, Instructions, BalanceUpdates.

Execute a GraphQL query against Bitquery V2 Streaming API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bitquery (Web3 Blockchain GraphQL APIs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Execute a V1 query to get the last 5 blocks from the Bitcoin network."

**🤖 AI Agent:**
> I've retrieved the latest 5 Bitcoin blocks using `query_v1`. The most recent block height is 834291 with 3,421 transactions. Would you like to see the details of a specific block?

---

**👤 You:**
> "Use query_v2 to find the latest 10 DEX trades on Ethereum Mainnet."

**🤖 AI Agent:**
> Fetching real-time DEX trades via `query_v2`... I found 10 recent trades on Uniswap V3 and Curve. The largest trade was 45.2 ETH for USDC. Should I analyze the price impact of these trades?

---

**👤 You:**
> "Generate a new access token using my client ID 'cid_123' and secret 'sec_456'."

**🤖 AI Agent:**
> I have successfully generated a new OAuth2 token using `generate_token`. You can now use this Bearer token for your subsequent GraphQL queries. Remember to keep this token secure.


## ❓ FAQ

**Q: What is the difference between query_v1 and query_v2?**
Use `query_v1` for historical data across 40+ legacy and non-EVM chains (like Bitcoin). Use `query_v2` for real-time streaming and advanced filtering on EVM chains and Solana, supporting complex joins like 'joinCalls'.

**Q: How do I obtain an access token if I only have a Client ID and Secret?**
You can use the `generate_token` tool. Provide your Bitquery Client ID and Secret, and the tool will return a Bearer token that you can use as your `BITQUERY_ACCESS_TOKEN` credential.

**Q: Can I query data from multiple regions?**
Yes. Both `query_v1` and `query_v2` support an optional `region` parameter. You can choose between 'global', 'asia', or 'us' to optimize latency based on your location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bitquery-web3-blockchain-graphql-apis](https://vinkius.com/mcp/bitquery-web3-blockchain-graphql-apis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bitquery (Web3 Blockchain GraphQL APIs)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bitquery-web3-blockchain-graphql-apis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bitquery (Web3 Blockchain GraphQL APIs)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bitquery-web3-blockchain-graphql-apis": {
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
