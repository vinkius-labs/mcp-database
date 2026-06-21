# DappRadar (Web3 Dapp & NFT Analytics) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dappradar-web3-dapp-nft-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dappradar-web3-dapp-nft-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dappradar-web3-dapp-nft-analytics-mcp)
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


## Installation & Usage

To install and use the **DappRadar (Web3 Dapp & NFT Analytics)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dappradar-web3-dapp-nft-analytics](https://vinkius.com/mcp/dappradar-web3-dapp-nft-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
