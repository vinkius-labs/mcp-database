# Wine Pairing & Sommelier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wine-pairing-sommelier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Get expert wine pairings for any dish, discover wines by description, and find top-rated bottles with prices — your AI sommelier.

## Description
The **Wine Pairing & Sommelier MCP Server** transforms your AI agent into a knowledgeable wine expert. Powered by comprehensive wine data, it handles everything from food-wine pairing to specific bottle recommendations.

### Core Capabilities

- **Food → Wine** — Enter any dish or ingredient and get expert wine pairing suggestions.
- **Wine → Dish** — Already have a wine? Discover the perfect dishes to pair with it.
- **Wine Descriptions** — Learn about any wine variety: flavor profile, origin, and characteristics.
- **Product Recommendations** — Get specific bottle suggestions with ratings, prices, and purchase links.

Uses the Spoonacular API key (same as Spoonacular MCP). An essential companion for hospitality, dining, and lifestyle AI applications.


## Available Tools
- **get_dish_for_wine**: g. merlot, chardonnay, pinot noir, riesling) and get expert dish pairing recommendations.

Find the perfect dish to pair with a wine
- **get_wine_description**: Get a detailed description of a wine type
- **get_wine_pairing**: g. steak, salmon, pasta, chocolate) and get expert wine pairing recommendations with specific product suggestions, ratings, and prices.

Find the perfect wine to pair with a dish or ingredient
- **recommend_wines**: Get specific wine product recommendations with ratings and prices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Pairing & Sommelier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What wine pairs best with grilled salmon?"

**🤖 AI Agent:**
> For grilled salmon, I recommend a Pinot Noir or a dry Chardonnay. The salmon's rich, oily texture pairs beautifully with the earthiness of Pinot Noir, while Chardonnay's buttery notes complement the grilled flavor. A top pick: Domaine Drouhin Oregon Pinot Noir 2021 — rated 4.2/5, around $32.

---

**👤 You:**
> "What dishes pair well with an Argentinian Malbec?"

**🤖 AI Agent:**
> Argentinian Malbec is a bold, full-bodied red that pairs perfectly with:
🥩 **Grilled Steaks** (especially ribeye or sirloin)
🍔 **Gourmet Burgers** with blue cheese
🍖 **BBQ Pork Ribs** or brisket
The wine's dark fruit notes and smokiness complement charred and heavily seasoned meats.

---

**👤 You:**
> "Give me a description of a typical New Zealand Sauvignon Blanc."

**🤖 AI Agent:**
> Querying wine database ('get_wine_description')...
**New Zealand Sauvignon Blanc** (typically from Marlborough):
- **Profile**: Highly aromatic, crisp, and high in acidity.
- **Tasting Notes**: Overt notes of passion fruit, gooseberry, grapefruit, and fresh-cut grass or bell pepper (jalapeño descriptors are common).
- **Style**: Unoaked, best consumed young.
- **Pairings**: Goat cheese, asparagus, fresh seafood.


## ❓ FAQ

**Q: What wines are covered?**
The database covers all major wine varieties including Cabernet Sauvignon, Merlot, Pinot Noir, Chardonnay, Sauvignon Blanc, Riesling, Malbec, Prosecco, Champagne, and dozens more from wine regions worldwide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wine-pairing-sommelier](https://vinkius.com/mcp/wine-pairing-sommelier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Pairing & Sommelier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wine-pairing-sommelier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Pairing & Sommelier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-pairing-sommelier": {
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
