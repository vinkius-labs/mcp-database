# Nifty Gateway (NFT Marketplace API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nifty-gateway-nft-marketplace-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Explore and manage NFT assets via Nifty Gateway — list available nifties, browse collections, and audit your personal portfolio directly from any AI agent.

## Description
Connect the **Nifty Gateway** NFT marketplace to your AI agent to explore digital art collections and manage your portfolio through natural language.

### What you can do

- **Marketplace Discovery** — List all available Nifties (NFTs) on the platform with full pagination support to find the latest drops.
- **Detailed Inspection** — Retrieve comprehensive metadata, artist info, and attributes for specific Nifties using their unique IDs.
- **Collection Browsing** — Explore curated collections and drops to understand the latest digital art trends and creator series.
- **Portfolio Management** — Instantly list and audit the Nifties owned by your authenticated account without leaving your chat interface.

### How it works

1. Subscribe to this server
2. Enter your Nifty Gateway API Key
3. Start querying the NFT marketplace from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **NFT Collectors** — quickly check your inventory or find specific art pieces without browsing the web UI.
- **Web3 Developers** — integrate NFT data into your workflow or code editor for faster building and testing.
- **Digital Art Analysts** — track collections and marketplace trends using AI-driven queries and data extraction.


## Available Tools
- **get_collection**: Get detailed information about a specific collection
- **get_nifty**: Get detailed information about a specific Nifty
- **list_collections**: List all collections on the platform
- **list_nifties**: Supports pagination.

List all Nifties available on the platform
- **list_user_nifties**: List Nifties owned by the authenticated user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nifty Gateway (NFT Marketplace API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Nifties currently available on the platform."

**🤖 AI Agent:**
> I've retrieved the latest Nifties. There are several active listings including 'The Eternal Bloom' and 'Cyber City #402'. Would you like details on a specific one?

---

**👤 You:**
> "Get information about Nifty ID '12345'."

**🤖 AI Agent:**
> Fetching details for Nifty 12345... This is 'Neon Sunset' by Artist X. It features a vibrant 80s aesthetic and is part of the 'Retro Future' collection.

---

**👤 You:**
> "Show me the Nifties I currently own."

**🤖 AI Agent:**
> I've listed your owned Nifties. You currently have 3 assets in your wallet, including 'Golden Ticket #1' and 'Abstract Flow'. Which one should we inspect?


## ❓ FAQ

**Q: Can I see the specific details of an NFT if I have its ID?**
Yes! Use the `get_nifty` tool with the unique Nifty ID. Your agent will return detailed metadata, artist information, and current attributes associated with that specific asset.

**Q: How do I check which NFTs I currently own on Nifty Gateway?**
Simply ask the agent to run the `list_user_nifties` action. It will retrieve a complete list of all digital assets currently held in your authenticated Nifty Gateway account.

**Q: Can I browse entire collections or drops instead of individual items?**
Yes, you can use `list_collections` to see all available collections on the platform, or `get_collection` with a specific ID to see the contents and details of a particular drop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nifty-gateway-nft-marketplace-api](https://vinkius.com/mcp/nifty-gateway-nft-marketplace-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nifty Gateway (NFT Marketplace API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nifty-gateway-nft-marketplace-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nifty Gateway (NFT Marketplace API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nifty-gateway-nft-marketplace-api": {
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
