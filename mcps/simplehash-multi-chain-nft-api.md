# SimpleHash (Multi-chain NFT API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simplehash-multi-chain-nft-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/simplehash-multi-chain-nft-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/simplehash-multi-chain-nft-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access comprehensive NFT data across 50+ chains — query wallet holdings, metadata, collection details, and transfer history.

## Description
Connect to **SimpleHash**, the most comprehensive NFT API, and empower your AI agent with real-time multi-chain data. This server allows you to query NFT information across Ethereum, Polygon, Solana, Bitcoin (Ordinals), and dozens of other networks through a single interface.

### What you can do

- **Wallet Inventory** — Retrieve all NFTs owned by specific wallet addresses across multiple chains simultaneously.
- **Metadata & Media** — Fetch detailed metadata, high-resolution image URLs, and attribute data for any specific NFT.
- **Collection Insights** — Access collection-level data including descriptions, social links, and current floor prices.
- **Transfer History** — Track the movement of NFTs by querying historical transfer events for specific wallets or contracts.
- **Contract Analysis** — List all NFTs minted under a specific smart contract to understand the scope of a project.

### How it works

1. Subscribe to this server
2. Enter your SimpleHash API Key
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — instantly pull NFT metadata and ownership data into your coding environment.
- **NFT Collectors & Traders** — track portfolio movements and floor prices across different chains via natural language.
- **Data Analysts** — aggregate multi-chain transfer history and collection metrics without writing complex scrapers.


## Available Tools
- **get_collection_details**: Retrieve information about a specific NFT collection
- **get_collections_by_wallet**: Retrieve all collections that a specific wallet owns NFTs from
- **get_nft_details**: Retrieve detailed metadata and ownership information for a specific NFT
- **get_nft_transfers_by_contract**: Retrieve the transfer history for a specific contract
- **get_nft_transfers_by_wallet**: Retrieve the transfer history for a specific wallet
- **get_nfts_by_contract**: Retrieve all NFTs within a specific contract
- **get_nfts_by_wallet**: Retrieve all NFTs owned by a specific wallet address across multiple chains


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SimpleHash (Multi-chain NFT API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all NFTs owned by 0x742d35Cc6634C0532925a3b844Bc454e4438f44e on ethereum and polygon."

**🤖 AI Agent:**
> I've found 12 NFTs for that address across Ethereum and Polygon. Notable items include 2 Bored Ape Yacht Club tokens and 5 Polygon-based gaming assets. Would you like the full list or details on a specific one?

---

**👤 You:**
> "Get the metadata and image for NFT token 123 in contract 0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d on ethereum."

**🤖 AI Agent:**
> Fetching details for BAYC #123... I have the metadata: it has 'Robot Eyes' and 'Blue Fur' traits. The high-res image is available at the IPFS gateway. Would you like me to show the full attribute list?

---

**👤 You:**
> "Show me the recent transfer history for wallet 0x123... on ethereum."

**🤖 AI Agent:**
> I've retrieved the last 10 transfers for this wallet. There were 3 sales on OpenSea and 2 direct transfers in the past 48 hours. Should I break down the prices and timestamps for these events?


## Installation & Usage

To install and use the **SimpleHash (Multi-chain NFT API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplehash-multi-chain-nft-api](https://vinkius.com/mcp/simplehash-multi-chain-nft-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
