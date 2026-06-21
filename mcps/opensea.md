# OpenSea MCP Server

Access the world's leading NFT marketplace — query collections, track floor prices, inspect NFT metadata, and monitor wallet balances across multiple chains.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opensea)

## Overview
**Category:** ecommerce
**Tools Count:** 35

## Description
Connect **OpenSea** to your AI agent to navigate the NFT ecosystem with ease. From tracking trending collections to deep-diving into specific token traits, this server provides real-time access to the largest digital marketplace.

### What you can do

- **Market Insights** — Get trending and top collections, or fetch comprehensive stats like volume and floor prices using `get_trending_collections` and `get_collection_stats`.
- **NFT Deep-Dive** — Retrieve full metadata, rarity, and ownership details for any NFT with `get_nft` and `get_nft_metadata`.
- **Collection Analysis** — List collection traits, holders, and detailed fee structures via `get_collection_traits` and `get_collection_holders`.
- **Wallet Monitoring** — Check account profiles and fungible token balances for any wallet address with `get_account` and `get_token_balances`.
- **Multi-Chain Support** — Query data across all blockchains supported by OpenSea using `get_chains`.

### How it works

1. Subscribe to this server
2. Enter your OpenSea API Key
3. Start analyzing the NFT market from Claude, Cursor, or any MCP-compatible client

No more manual searching through marketplace tabs. Your AI acts as a dedicated floor price tracker and portfolio analyst.

### Who is this for?

- **Web3 Developers** — instantly retrieve NFT metadata and contract details directly from the code editor.
- **NFT Collectors & Traders** — monitor floor prices, volume trends, and collection holders without leaving the chat.
- **Data Analysts** — automate the retrieval of collection statistics and trait distributions for market research.


## Available Tools
- **cancel_order**: Off-chain cancellation of an order
- **generate_listing_fulfillment**: Get data to buy an NFT
- **generate_offer_fulfillment**: Get data to accept an offer
- **get_account**: Get an OpenSea account profile
- **get_best_listing_nft**: Get the lowest price listing for a specific NFT
- **get_best_offer_nft**: Get the highest offer for a specific NFT
- **get_chains**: Get all blockchain chains supported by OpenSea
- **get_collection_holders**: Get a list of wallet addresses holding items in a collection
- **get_collection_stats**: Get comprehensive statistics for a collection
- **get_collection**: Get detailed information about a collection
- **get_collection_traits**: List all available traits in a collection
- **get_drop_by_slug**: Get stages, supply, and minting details for a specific drop
- **get_drops**: List featured, upcoming, or recently minted drops
- **get_nft_metadata**: Get detailed metadata including image URLs and external links for an NFT
- **get_nft_owners**: List all owners of a specific NFT
- **get_nft**: Get metadata, traits, ownership, and rarity for a single NFT
- **get_nfts_by_account**: Get NFTs owned by a specific wallet
- **get_nfts_by_collection**: Get all NFTs in a specific collection
- **get_nfts_by_contract**: Get all NFTs for a specific smart contract
- **get_order**: Retrieve order details
- **get_swap_quote**: Get a price quote for swapping tokens
- **get_token_balances**: Get fungible token balances for a specific wallet
- **get_token**: Get metadata for a fungible token
- **get_top_collections**: Get top collections
- **get_transaction_receipt**: Check the status of a submitted swap or fulfillment
- **get_trending_collections**: Get trending collections
- **list_collections**: List collections
- **list_events**: Get historical marketplace events
- **list_listings_collection_all**: Get all active listings for a collection
- **list_offers_collection_all**: Get all active offers for a collection
- **post_criteria_offer**: Create a collection or trait-wide offer
- **post_listing**: Create a new listing
- **post_offer**: Create an offer on a single item
- **post_swap_execute**: Get executable transaction data for a swap
- **search**: Search across collections, NFTs, tokens, and accounts


## Installation & Usage

To install and use the **OpenSea** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensea](https://vinkius.com/mcp/opensea)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
