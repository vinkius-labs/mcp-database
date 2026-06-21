# Reservoir (NFT Liquidity API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reservoir-nft-liquidity-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/reservoir-nft-liquidity-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/reservoir-nft-liquidity-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access aggregated NFT liquidity, metadata, and real-time pricing across all major marketplaces via the Reservoir API.

## Description
Connect to **Reservoir**, the premier NFT liquidity aggregator, and empower your AI agent to navigate the decentralized web. This server provides comprehensive access to NFT market data, metadata, and transaction execution across Ethereum and other major chains.

### What you can do

- **Market Aggregation** — Query active listings (asks) and offers (bids) from OpenSea, LooksRare, X2Y2, and more in a single request.
- **Deep Metadata** — Retrieve detailed token information, rarity scores, and collection-level statistics including floor prices and volume.
- **Search & Discovery** — Find collections by name or contract address and list tokens based on specific owners or attributes.
- **Transaction Generation** — Generate the necessary transaction data to buy NFTs or accept offers directly through the agent.
- **Real-time Stats** — Get up-to-the-minute floor prices and market movements for any NFT collection.

### How it works

1. Subscribe to this server
2. Enter your Reservoir API Key
3. Start analyzing NFT markets and executing trades from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Integrate NFT pricing and metadata into your workflow without leaving your IDE.
- **NFT Traders** — Quickly compare prices across marketplaces and identify liquidity depth for specific collections.
- **Data Analysts** — Pull real-time market stats and ownership data for research and reporting.


## Available Tools
- **execute_buy**: Generate transactions to buy an NFT
- **execute_sell**: Generate transactions to accept an offer (fill a bid)
- **get_collection**: Get metadata and real-time stats for a collection
- **get_token**: Retrieve detailed information for a specific token
- **list_asks**: Retrieve active listings (asks) across all supported marketplaces
- **list_bids**: Retrieve active offers (bids) for tokens or collections
- **list_tokens**: Retrieve a list of tokens with various filters
- **search_collections**: Search for collections by name or contract address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir (NFT Liquidity API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the 'Azuki' collection and show me its floor price."

**🤖 AI Agent:**
> I found the Azuki collection (Contract: 0xed5af... ). The current floor price is 5.42 ETH with a 24h volume of 120 ETH. Would you like to see the top active listings?

---

**👤 You:**
> "List all tokens owned by address 0x123... sorted by rarity."

**🤖 AI Agent:**
> Fetching tokens for that address... I found 12 NFTs. The rarest is 'Bored Ape #442' followed by 'Mutant Ape #1023'. Would you like the full metadata for the Bored Ape?

---

**👤 You:**
> "Show me the active sell orders for token 0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d:1."

**🤖 AI Agent:**
> There are 3 active listings for this Bored Ape: 75 ETH on OpenSea, 74.9 ETH on LooksRare, and 76 ETH on X2Y2. I can generate a buy transaction for the cheapest one if you're ready.


## Installation & Usage

To install and use the **Reservoir (NFT Liquidity API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reservoir-nft-liquidity-api](https://vinkius.com/mcp/reservoir-nft-liquidity-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
