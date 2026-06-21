# Mnemonic MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mnemonic)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mnemonic-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mnemonic-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Deep NFT analytics and Web3 intelligence via Mnemonic — track collections, portfolios, and transfers directly from your AI agent.

## Description
Connect your **Mnemonic** account to your AI agent and unlock deep insights into the NFT ecosystem and Web3 data through natural conversation.

### What you can do

- **Portfolio Tracking** — List all NFTs owned by any wallet address and view their complete historical activity.
- **Collection Analytics** — Get real-time stats including floor price, volume, market cap, and ownership distribution.
- **Market Pricing** — Access real-time and historical pricing data for tokens across major marketplaces.
- **Transfer Monitoring** — Query historical transfer events for specific tokens or entire collections with advanced filters.
- **Token Inspection** — Retrieve complete metadata, properties, and current owners for any specific NFT.
- **Smart Contract Data** — Fetch detailed technical metadata for blockchain smart contracts and collections.

### How it works

1. Subscribe to this server
2. Enter your Mnemonic API Key
3. Start querying NFT intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — quickly inspect contract metadata or token properties while building applications.
- **NFT Collectors & Traders** — monitor portfolio health and collection stats without leaving your communication tools.
- **Data Analysts** — automate the retrieval of complex transfer and ownership data for Web3 reporting.


## Available Tools
- **get_collection_details**: Get NFT collection info
- **get_collection_distribution**: Get ownership distribution
- **get_collection_stats**: Get collection statistics
- **get_contract_metadata**: Get smart contract metadata
- **get_nft_details**: Get detailed NFT metadata
- **get_nft_owners**: Get owners of an NFT
- **get_nft_prices**: Get NFT market pricing data
- **get_wallet_history**: Get wallet transaction history
- **get_wallet_nfts**: Get all NFTs owned by a wallet
- **list_collection_tokens**: List tokens in a collection
- **list_transfers**: Query NFT transfer events
- **search_collections**: Search for NFT collections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mnemonic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all NFTs owned by the wallet 0x123..."

**🤖 AI Agent:**
> Fetching wallet portfolio... I found 12 NFTs including 3 Bored Ape Yacht Club and 2 Art Blocks. Would you like to see the floor prices for these collections?

---

**👤 You:**
> "Search for NFT collections named 'Cool Cats'."

**🤖 AI Agent:**
> I've searched for 'Cool Cats'. I found 3 matches: the primary 'Cool Cats' collection (0x1a2b...), 'Cool Cats Kittens', and 'Cool Cats Collaborations'. Which one would you like more details on?

---

**👤 You:**
> "What is the ownership distribution for the Azuki collection?"

**🤖 AI Agent:**
> Analyzing Azuki ownership... The collection has 5,400 unique owners. The top 10 holders own 15% of the total supply, indicating a highly distributed and healthy ownership base. Shall I retrieve the current floor price as well?


## Installation & Usage

To install and use the **Mnemonic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mnemonic](https://vinkius.com/mcp/mnemonic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
