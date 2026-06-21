# The Graph (Web3 Indexing) MCP Server

Index and query blockchain data across EVM and Solana chains. Access transfers, holders, swaps, and custom subgraphs directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/the-graph-web3-indexing)

## Overview
**Category:** developer-tools
**Tools Count:** 8

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


## Installation & Usage

To install and use the **The Graph (Web3 Indexing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-graph-web3-indexing](https://vinkius.com/mcp/the-graph-web3-indexing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
