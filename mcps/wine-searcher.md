# Wine-Searcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wine-searcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search global wine pricing, critic scores, grape varieties, regions, and producer data from 100,000+ merchants worldwide through natural conversation.

## Description
Connect to **Wine-Searcher** — the world's largest wine price comparison engine — and access real-time market intelligence for any wine.

### What you can do

- **Wine Check** — Look up any wine: critic scores, grape varieties, region, alcohol content, and global average/min/max pricing
- **Market Price** — Compare real-time pricing from 100,000+ merchants: shop names, locations, and direct purchase URLs
- **Search Wines** — Full-text search across the entire Wine-Searcher database for discovery and exploration
- **Grape Info** — Detailed grape variety profiles: origins, growing regions, wine styles, and food pairings
- **Region Info** — Wine region deep-dives: climate, soil, appellations, and notable producers
- **Producer Info** — Winery profiles: key wines, price ranges, scores, and available vintages

### Who is this for?

- **Sommeliers** — Instant price checks and pairing suggestions during service
- **Wine Collectors** — Market value tracking, buying opportunities, and vintage comparison
- **Wine Importers** — Global pricing intelligence and producer research
- **Wine Retailers** — Competitive pricing analysis and inventory decisions


## Available Tools (6)
- **wine_check**: ), grape varieties, region, appellation, alcohol content, average/min/max pricing across global merchants. The primary lookup tool for any wine question.

Check wine details and scores
- **market_price**: Use for price comparison, market analysis, or finding the best deal on a specific wine.

Get global market pricing
- **search_wines**: Returns matching wines with pricing, scores, and merchant availability. Use for discovery and exploration.

Search the wine database
- **grape_info**: Perfect for sommelier education and pairing recommendations.

Get grape variety info
- **region_info**: Essential for terroir education and regional exploration.

Get wine region info
- **producer_info**: Use for winery research and brand comparison.

Get producer/winery info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine-Searcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the average price for Opus One 2021?"

**🤖 AI Agent:**
> 🍷 **Opus One 2021 — Napa Valley**

💰 **Global pricing**:
- Average: **$425**
- Range: $380 — $520
- Merchants listing: 847 worldwide

⭐ **Critic scores**:
- Wine Advocate: 97/100
- Wine Spectator: 96/100
- James Suckling: 98/100

🍇 **Blend**: Cabernet Sauvignon (79%), Merlot (7%), Cabernet Franc (6%), Petit Verdot (5%), Malbec (3%)
📍 **Appellation**: Oakville, Napa Valley
🥂 **ABV**: 14.5%

---

**👤 You:**
> "Find merchants near London selling Dom Pérignon 2012."

**🤖 AI Agent:**
> Searching Merchant listings ('search_wine_prices')...
Showing top 3 merchants for **Dom Pérignon Brut 2012** near London (UK):

1. **Berry Bros. & Rudd** (Mayfair) — £175.00 (In Stock: 12+)
   [Buy link/URL]
2. **Hedonism Wines** (Mayfair) — £182.50 (In Stock: 8)
   [Buy link/URL]
3. **Farr Vintners** (Battersea) — £168.00 (In Bond/Case only)
   [Buy link/URL]

---

**👤 You:**
> "What can you tell me about the Pomerol wine region?"

**🤖 AI Agent:**
> Looking up details ('get_region_info')...
**Pomerol (Bordeaux, France)**
- **Focus**: Red wines, primarily Merlot mixed with Cabernet Franc.
- **Terroir**: Smallest major Bordeaux appellation (800ha). Famous for its 'crasse de fer' (iron-rich clay and gravel) imparting truffle notes.
- **Top Producers**: Petrus, Le Pin, Château Lafleur, Vieux Château Certan.
- **Vintages**: 2015, 2016, 2018, 2019, 2020 are exceptional.


## ❓ FAQ

**Q: Is Wine-Searcher API free?**
Wine-Searcher offers a free trial (100 calls/day). After the trial, paid plans are available based on daily call volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wine-searcher](https://vinkius.com/mcp/wine-searcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine-Searcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-searcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine-Searcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-searcher": {
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
