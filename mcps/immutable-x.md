# Immutable X MCP Server

Interact with the Immutable blockchain — list activities, manage NFT collections, mint assets, and handle orderbook listings directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/immutable-x)

## Overview
**Category:** developer-tools
**Tools Count:** 17

## Description
Connect your **Immutable** developer account to any AI agent to manage Web3 gaming assets and on-chain data through natural conversation.

### What you can do

- **Activities & Events** — Retrieve on-chain events like mints, transfers, and sales using `list_activities` and `get_activity`.
- **NFT Collections** — Explore and manage NFT collections with `list_collections`, `get_collection`, and `refresh_collection_metadata`.
- **Asset Management** — Query individual NFTs with `get_nft` or `list_nfts`, and even mint new assets using `mint_nfts`.
- **Orderbook Operations** — Interact with the marketplace by listing items (`create_listing`), placing bids (`create_bid`), or fulfilling orders (`fulfill_order`).
- **Mint Tracking** — Monitor the status of minting operations with `list_mint_requests`.

### How it works

1. Subscribe to this server
2. Enter your Immutable Secret Key and Access Token
3. Start managing your blockchain assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly check on-chain data or trigger mints without leaving the code editor
- **Game Studios** — manage in-game asset collections and monitor marketplace activity
- **Crypto Analysts** — query NFT metadata and activity logs for research and reporting


## Available Tools
- **create_bid**: Create an orderbook bid
- **create_listing**: Create an orderbook listing
- **fulfill_order**: Fulfill an orderbook order
- **get_activity**: Get a specific activity by ID
- **get_collection**: Get collection details by contract address
- **get_nft**: Get NFT details by token ID
- **get_passport_profile**: Get Passport user profile (requires Access Token)
- **get_token**: Get ERC20 token by contract address
- **list_activities**: List all activities on an Immutable chain
- **list_collections**: List all NFT collections
- **list_listings**: List all orderbook listings
- **list_mint_requests**: List mint requests for a collection
- **list_nfts**: List all NFTs
- **list_tokens**: List ERC20 tokens
- **mint_nfts**: Mint NFTs (requires Secret API Key)
- **refresh_collection_metadata**: Refresh metadata for a collection
- **update_passport_username**: Update Passport username (requires Access Token)


## Installation & Usage

To install and use the **Immutable X** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/immutable-x](https://vinkius.com/mcp/immutable-x)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
