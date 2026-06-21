# Bitquery (Web3 Blockchain GraphQL APIs) MCP Server

Query real-time and historical blockchain data across 40+ chains including Ethereum, Solana, and Bitcoin using GraphQL.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bitquery-web3-blockchain-graphql-apis)

## Overview
**Category:** developer-tools
**Tools Count:** 3

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


## Available Tools
- **generate_token**: The returned token should be used as the BITQUERY_ACCESS_TOKEN credential.

Generate an OAuth2 access token using Client ID and Secret
- **query_v1**: Provide a valid GraphQL query string.

Execute a GraphQL query against Bitquery V1 Historical API
- **query_v2**: Supports joins (e.g., joinCalls) and advanced filtering. Cubes include Transfers, Calls, Events, DexTrades, DexTradesByTokens, Instructions, BalanceUpdates.

Execute a GraphQL query against Bitquery V2 Streaming API


## Installation & Usage

To install and use the **Bitquery (Web3 Blockchain GraphQL APIs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bitquery-web3-blockchain-graphql-apis](https://vinkius.com/mcp/bitquery-web3-blockchain-graphql-apis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
