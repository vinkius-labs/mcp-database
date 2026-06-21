# Rarible (Multi-chain NFT Protocol) MCP Server

Access multi-chain NFT data — query items, collections, activities, and market statistics across Ethereum, Polygon, and more via Rarible.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/rarible-multi-chain-nft-protocol)

## Overview
**Category:** developer-tools
**Tools Count:** 20

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


## Installation & Usage

To install and use the **Rarible (Multi-chain NFT Protocol)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rarible-multi-chain-nft-protocol](https://vinkius.com/mcp/rarible-multi-chain-nft-protocol)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
