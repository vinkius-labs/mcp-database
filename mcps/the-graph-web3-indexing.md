# The Graph (Web3 Indexing) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/the-graph-web3-indexing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Index and query blockchain data across EVM and Solana chains. Access transfers, holders, swaps, and custom subgraphs directly.

## Description
Connect to **The Graph** to index and retrieve real-time blockchain data across multiple ecosystems. This MCP server allows your AI agent to query decentralized data from Ethereum, Polygon, Solana, and more through standardized tools and custom GraphQL subgraphs.

### What you can do

- **EVM Data Access** — Retrieve token transfers, top holders, and DEX swap events (Uniswap, Curve) for any EVM-compatible chain.
- **Solana (SVM) Integration** — Fetch SPL token transfers, holders, and AMM swaps (Jupiter, Raydium) directly from the Solana network.
- **Historical Analysis** — Access wallet balance changes in OHLCV format to track portfolio performance over time.
- **Custom Subgraph Queries** — Execute raw GraphQL queries against any specific subgraph ID for deep, specialized data extraction.
- **Market Intelligence** — Monitor liquidity pool activities and token distribution metrics without manual block explorer searching.

### How it works

1. Subscribe to this server
2. Enter your The Graph API Token, API URL, and optional API Key
3. Start querying on-chain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug smart contract events and verify on-chain state directly from your IDE
- **Data Analysts** — aggregate token holder distributions and DEX volume metrics for research
- **DeFi Power Users** — track wallet movements and liquidity pool swaps through natural language


## Available Tools (8)
- **get_evm_historical_balances**: Get EVM historical balances
- **get_evm_holders**: Get EVM token holders
- **get_evm_swaps**: ) for EVM chains.

Get EVM DEX swaps
- **get_evm_transfers**: Get EVM token transfers
- **query_subgraph**: Requires THE_GRAPH_API_KEY.

Query a subgraph using GraphQL
- **get_svm_holders**: Get SVM (Solana) token holders
- **get_svm_swaps**: ) for Solana.

Get SVM (Solana) DEX swaps
- **get_svm_transfers**: Get SVM (Solana) token transfers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **The Graph (Web3 Indexing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the top 10 holders for the EVM token at 0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9."

**🤖 AI Agent:**
> I've retrieved the top holders for the specified token. The largest holder currently controls 12.4% of the supply, followed by a major exchange wallet with 8.2%. Would you like to see the full list of addresses and balances?

---

**👤 You:**
> "Show me recent swaps for the Solana token DezXAZ8z7PnrnMcFWRSTQC8PGL9P8be3EFr9SptT5v7."

**🤖 AI Agent:**
> I found 15 recent swap events for that token on Solana. The most significant was a 500 SOL trade on Raydium. Most activity is currently concentrated on Jupiter. Should I analyze the price impact of these trades?

---

**👤 You:**
> "Query the Uniswap V3 subgraph with ID 'ELUvFp... ' to get the latest pool prices."

**🤖 AI Agent:**
> Executing GraphQL query on the Uniswap V3 subgraph... I've successfully fetched the latest price data. The ETH/USDC pool is currently trading at $2,450.32 with $12M in 24h volume. Do you need details on any other specific pool?


## ❓ FAQ

**Q: Can I query any specific subgraph if I have its ID?**
Yes! Use the `query_subgraph` tool by providing the `subgraph_id` and your GraphQL `query` string. This allows for deep, custom data extraction beyond the standard tools.

**Q: Does this server support Solana token data?**
Absolutely. You can use `get_svm_transfers`, `get_svm_holders`, and `get_svm_swaps` to interact with SPL tokens and decentralized exchanges on the Solana network.

**Q: Can I track historical balance changes for a specific wallet?**
Yes, the `get_evm_historical_balances` tool provides historical balance data in OHLCV format for EVM chains, making it easy to analyze portfolio trends.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-graph-web3-indexing](https://vinkius.com/mcp/the-graph-web3-indexing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **The Graph (Web3 Indexing)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `the-graph-web3-indexing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **The Graph (Web3 Indexing)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "the-graph-web3-indexing": {
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
