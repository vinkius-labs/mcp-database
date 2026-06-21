# OpenSea MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opensea)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Access the world's leading NFT marketplace — query collections, track floor prices, inspect NFT metadata, and monitor wallet balances across multiple chains.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenSea** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the trending NFT collections on OpenSea right now."

**🤖 AI Agent:**
> I've fetched the trending collections. Currently, 'Pudgy Penguins' and 'Azuki' are seeing high activity. Would you like to see the specific stats for one of them?

---

**👤 You:**
> "Get the floor price and volume stats for the 'boredapeyachtclub' collection."

**🤖 AI Agent:**
> The Bored Ape Yacht Club currently has a floor price of 12.5 ETH with a total volume of 1.2M ETH. There have been 45 sales in the last 24 hours.

---

**👤 You:**
> "Check the profile and token balances for wallet address 0x123..."

**🤖 AI Agent:**
> For wallet 0x123..., the profile name is 'CryptoCollector'. The account holds 2.5 ETH and 500 USDC. Would you like to see their NFT holdings as well?


## ❓ FAQ

**Q: Can I check the floor price and volume for a specific NFT collection?**
Yes! Use the `get_collection_stats` tool with the collection slug. The agent will return real-time metrics including floor price, total volume, and sales counts.

**Q: How do I retrieve the image and metadata for a specific NFT?**
You can use the `get_nft_metadata` tool by providing the chain, contract address, and token ID. It returns detailed metadata including image URLs and external links.

**Q: Can I see which wallets hold the most items in a collection?**
Yes, the `get_collection_holders` tool provides a list of wallet addresses that currently hold items within a specific collection slug.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensea](https://vinkius.com/mcp/opensea)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenSea** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `opensea` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenSea** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opensea": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
