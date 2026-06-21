# IsThereAnyDeal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/isthereanydeal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Track game prices, find the best deals, and check historical lows across multiple digital stores using the IsThereAnyDeal API.

## Description
Connect your AI agent to **IsThereAnyDeal** to access real-time gaming commerce data. Compare prices across dozens of digital stores, track price history, and never miss a sale again.

### What you can do

- **Game Search** — Search for any game title to find its unique 'Plain ID' used for price tracking
- **Price Comparison** — Fetch current prices for games across all supported stores (Steam, GOG, Epic, etc.) in specific regions or countries
- **Historical Lows** — Check the lowest price ever recorded for a game to know if a current deal is truly worth it
- **Global Deals** — List the best active deals across the entire IsThereAnyDeal platform with customizable filters
- **ID Conversion** — Convert store-specific IDs (like Steam AppIDs) into ITAD Plain IDs for seamless integration

### How it works

1. Subscribe to this server
2. Enter your IsThereAnyDeal API Key
3. Start querying game prices and deals from Claude, Cursor, or any MCP-compatible client

Your AI acts as a personal shopping assistant for your gaming library, helping you optimize your budget and find the best time to buy.


## Available Tools
- **get_deals**: Get current best deals
- **get_historical_low**: Get historical lowest price for games
- **get_plain_id**: Get the ITAD Plain ID for a game
- **get_prices**: Get current prices for games
- **search_games**: Search for games by title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IsThereAnyDeal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the game 'Elden Ring' and find its Plain ID."

**🤖 AI Agent:**
> I found 'Elden Ring' with the Plain ID: `elden-ring`. You can now use this ID to check prices or historical lows.

---

**👤 You:**
> "What are the current prices for 'cyberpunk-2077' in the US region?"

**🤖 AI Agent:**
> Checking prices for Cyberpunk 2077 in the US... It's currently $29.99 on Steam (50% off) and $29.99 on GOG. The best price is currently available on both stores.

---

**👤 You:**
> "Show me the historical lowest price for 'the-witcher-3-wild-hunt'."

**🤖 AI Agent:**
> The historical low for The Witcher 3: Wild Hunt was $7.99 (80% off) recorded on Steam and GOG. Compared to the current price of $9.99, you are very close to the all-time low.


## ❓ FAQ

**Q: How do I find the correct ID for a game to check its price?**
Use the `search_games` tool with the game title. It will return a list of matching games along with their 'Plain ID', which you can then use in other tools like `get_prices` or `get_historical_low`.

**Q: Can I see the best deals currently available globally?**
Yes! Use the `get_deals` tool. You can optionally filter by region (e.g., 'us', 'eu1'), country, or specific shops to find exactly what you're looking for.

**Q: Is it possible to convert a Steam AppID to an IsThereAnyDeal ID?**
Absolutely. Use the `get_plain_id` tool, specifying 'steam' as the shop and the AppID as the game parameter. It will return the corresponding ITAD Plain ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/isthereanydeal](https://vinkius.com/mcp/isthereanydeal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IsThereAnyDeal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `isthereanydeal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IsThereAnyDeal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "isthereanydeal": {
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
