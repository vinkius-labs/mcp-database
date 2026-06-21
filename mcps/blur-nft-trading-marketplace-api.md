# Blur (NFT Trading Marketplace API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blur-nft-trading-marketplace-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time NFT market data, floor prices, and execute trades on Blur directly from your AI agent.

## Description
Connect to **Blur**, the leading NFT marketplace for pro traders, and manage your digital asset portfolio through natural language.

### What you can do

- **Market Insights** — Fetch detailed collection metadata, volume, and total supply statistics using collection slugs.
- **Floor Price Tracking** — Monitor real-time floor prices across Blur and other major marketplaces for any collection.
- **Asset Inspection** — Retrieve specific NFT metadata, token details, and current listing information.
- **Trading Execution** — Create listings (asks) and place bids (collection or token-specific) directly via signed orders.

### How it works

1. Subscribe to this server
2. Enter your Blur API Key
3. Start trading and analyzing NFT collections from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **NFT Traders** — Instantly check floor prices and execute orders without switching between browser tabs.
- **Data Analysts** — Pull collection stats and asset metadata directly into your analysis workflow.
- **Web3 Developers** — Test marketplace interactions and query NFT data straight from your code editor.


## Available Tools
- **create_ask**: Create a listing (ask) on Blur
- **create_bid**: Create a bid on Blur
- **get_asset**: Get metadata and current listings for a specific NFT
- **get_collection_floor**: Get current floor prices across marketplaces for a collection
- **get_collection**: Get metadata and stats for a specific collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blur (NFT Trading Marketplace API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current floor price for 'boredapeyachtclub' on all marketplaces?"

**🤖 AI Agent:**
> I've checked the floor prices for Bored Ape Yacht Club. On Blur, the floor is currently 12.5 ETH, while on OpenSea it's 12.6 ETH. Would you like to see more details for this collection?

---

**👤 You:**
> "Get the metadata and listings for Pudgy Penguins token ID 500."

**🤖 AI Agent:**
> Fetching asset details... Pudgy Penguin #500 is currently listed on Blur for 15.2 ETH. It has traits like 'Kimono' and 'Crown'. Would you like to place a bid on this item?

---

**👤 You:**
> "Show me the total volume and supply for the 'azuki' collection."

**🤖 AI Agent:**
> The Azuki collection has a total supply of 10,000 tokens and an all-time volume of approximately 650,000 ETH. The current floor price is 5.8 ETH. Do you need information on specific tokens in this collection?


## ❓ FAQ

**Q: Can I see floor prices on other marketplaces besides Blur?**
Yes! The `get_collection_floor` tool retrieves current floor prices across multiple marketplaces for a given collection slug, allowing for easy price comparison.

**Q: What information do I need to list an NFT for sale?**
To use the `create_ask` tool, you need the maker's wallet address, the collection contract address, token ID, price in ETH, expiration time, and a valid cryptographic signature.

**Q: How do I find the volume and total supply of a specific collection?**
Simply use the `get_collection` tool with the collection's unique slug. It will return comprehensive metadata including volume, total supply, and other key stats.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blur-nft-trading-marketplace-api](https://vinkius.com/mcp/blur-nft-trading-marketplace-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blur (NFT Trading Marketplace API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blur-nft-trading-marketplace-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blur (NFT Trading Marketplace API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blur-nft-trading-marketplace-api": {
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
