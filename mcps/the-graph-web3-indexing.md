# The Graph (Web3 Indexing) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/the-graph-web3-indexing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/the-graph-web3-indexing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/the-graph-web3-indexing-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **The Graph (Web3 Indexing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-graph-web3-indexing](https://vinkius.com/mcp/the-graph-web3-indexing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
