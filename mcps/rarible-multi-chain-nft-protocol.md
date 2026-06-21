# Rarible (Multi-chain NFT Protocol) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rarible-multi-chain-nft-protocol)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rarible-multi-chain-nft-protocol-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rarible-multi-chain-nft-protocol-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access multi-chain NFT data — query items, collections, activities, and market statistics across Ethereum, Polygon, and more via Rarible.

## Description
Connect to the **Rarible Multi-chain NFT Protocol** and empower your AI agent with real-time access to the decentralized NFT ecosystem across multiple blockchains.

### What you can do

- **NFT Discovery** — Fetch detailed metadata, ownership history, and media for any NFT using `get_item` or perform complex queries with `search_items`.
- **Collection Insights** — Retrieve comprehensive data on NFT collections, including owner lists and multi-chain availability using `get_collection` and `get_all_collections`.
- **Market Activity** — Track real-time mints, transfers, and sales across the ecosystem with `get_all_activities` or filter by specific users and items.
- **Trading & Orders** — Inspect active sell orders and bids with `get_sell_orders_by_item` and `get_bid_orders_by_item` to understand market depth.
- **Analytics & Rankings** — Access high-level market intelligence, including volume rankings, user stats, and buyer/seller trends via `get_volume_ranking` and `get_user_ranking`.

### How it works

1. Subscribe to this server
2. Enter your Rarible API Key
3. Start querying NFT data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — instantly pull NFT metadata and order book data directly into your coding environment.
- **Data Analysts** — track market trends, volume rankings, and wallet activities without manual API integration.
- **NFT Collectors & Traders** — monitor floor prices, bids, and collection activities through natural conversation.


## Available Tools
- **get_activities_by_collection**: Get activities for a collection
- **get_activities_by_item**: Get activities for an item
- **get_activities_by_user**: Get activities for a user
- **get_all_activities**: ).

Get all activities
- **get_all_collections**: Get all NFT collections
- **get_bid_orders_by_item**: Get bid orders for an NFT
- **get_bid_orders_by_maker**: Get user bid orders
- **get_buyers_stats**: Get collection buyer stats
- **get_collection**: Get collection by ID
- **get_collections_by_owner**: Get collections owned by user
- **get_item**: Get NFT by ID
- **get_items_by_collection**: Get NFTs from a collection
- **get_items_by_owner**: Get NFTs owned by a user
- **get_order**: Get order by ID
- **get_sell_orders_by_item**: Get sell orders for an NFT
- **get_sell_orders_by_maker**: Get user sell orders
- **get_sellers_stats**: Get collection seller stats
- **get_user_ranking**: Get user volume ranking
- **get_volume_ranking**: Get collection volume ranking
- **search_items**: Uses POST under the hood but is a read-only query.

Complex search for NFT items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rarible (Multi-chain NFT Protocol)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for the NFT ETHEREUM:0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d:1"

**🤖 AI Agent:**
> I've retrieved the details for Bored Ape #1. It is part of the Bored Ape Yacht Club collection, currently owned by address 0x..., and features traits like 'Golden Fur' and 'Laser Eyes'.

---

**👤 You:**
> "Show me the top 5 NFT collections by volume on Ethereum."

**🤖 AI Agent:**
> Based on the latest volume rankings, the top 5 collections are: 1. Bored Ape Yacht Club, 2. Mutant Ape Yacht Club, 3. Azuki, 4. DeGods, and 5. Captainz.

---

**👤 You:**
> "List all NFTs owned by ETHEREUM:0x1234567890abcdef1234567890abcdef12345678"

**🤖 AI Agent:**
> I found 12 NFTs in this wallet across Ethereum and Polygon, including 2 items from the 'Pudgy Penguins' collection and 1 'Art Blocks' piece.


## Installation & Usage

To install and use the **Rarible (Multi-chain NFT Protocol)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rarible-multi-chain-nft-protocol](https://vinkius.com/mcp/rarible-multi-chain-nft-protocol)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
