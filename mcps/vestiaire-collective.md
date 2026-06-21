# Vestiaire Collective MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vestiaire-collective)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search, analyze, and manage luxury resale items on Vestiaire Collective — the global community for pre-loved fashion.

## Description
Connect your **Vestiaire Collective** seller account to any AI agent and take full control of your luxury resale business through natural conversation.

### What you can do

- **Luxury Search** — Find authenticated luxury items from brands like Hermès, Chanel, Louis Vuitton, and Gucci with precision
- **Advanced Filters** — Search by brand, category, condition, price range, color, and material to find exactly what you're looking for
- **Price Analysis** — Analyze market trends and resale value for specific luxury brands and categories to optimize your pricing
- **Inventory Management** — List and track your own selling items and dressing room status directly from your agent
- **Catalog Discovery** — Browse available brands, designers, and categories within the vast Vestiaire Collective catalog
- **Authentication & Details** — Retrieve full metadata for items including condition, price history vs. new, and material details

### How it works

1. Subscribe to this server
2. Enter your Vestiaire Collective API Key and API URL
3. Start managing your luxury fashion inventory through Claude, Cursor, or any MCP-compatible client

No more manual price tracking or inventory spreadsheets. Your AI agent becomes your personal luxury fashion consultant and sales manager.

### Who is this for?

- **Professional Sellers** — automate inventory tracking and optimize resale pricing using real-time market data
- **Luxury Collectors** — quickly find rare items and analyze price trends for investment-grade fashion pieces
- **Fashion Resellers** — manage multiple listings and monitor market demand across luxury categories
- **Stylists & Personal Shoppers** — source specific high-end pieces for clients through advanced AI-powered filtering


## Available Tools
- **analyze_price_trends**: Analyser les tendances de prix pour une marque et catégorie (valorisation du luxe)
- **get_item_details**: Consulter un article : marque, état, authentification, prix vs. neuf, taille, matière
- **list_available_brands**: Lister les marques de luxe disponibles (Hermès, Chanel, Louis Vuitton, Dior, etc.)
- **list_catalog_categories**: Lister les catégories (sacs, chaussures, vêtements, accessoires, bijoux, montres)
- **list_available_designers**: Lister les créateurs et collections
- **list_my_selling_items**: Consulter les articles en vente dans votre dressing
- **search_by_brand**: ) et catégorie.

Rechercher par marque de luxe et catégorie optionnelle
- **search_with_advanced_filters**: Fournissez les filtres sous forme de paramètres.

Recherche avancée avec filtres multiples : marque, état, prix, couleur, matière, pays
- **search_luxury_items**: Fournissez une requête textuelle.

Rechercher des articles de luxe par mots-clés (ex : "Hermès Birkin", "Chanel tweed")


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vestiaire Collective** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for vintage Hermès Birkin bags in very good condition under 15000 EUR."

**🤖 AI Agent:**
> I found 5 vintage Hermès Birkin bags matching your criteria. One is a Birkin 35 in Gold Epsom leather (Very Good Condition) for 12,500 EUR located in France. Would you like to see the full details and images for this listing?

---

**👤 You:**
> "What is the current resale trend for Chanel Flap Bags?"

**🤖 AI Agent:**
> Analyzing price history for Chanel bags… Resale value for Classic Flap Bags has increased by 12% over the last 6 months. Items in 'Never Worn' condition are currently selling at 95% of their original retail price. It's an excellent time to list your item if you're considering selling.

---

**👤 You:**
> "List all items I currently have for sale."

**🤖 AI Agent:**
> You have 3 items currently listed: 1. Louis Vuitton Speedy 30 (Status: Active, 12 likes), 2. Gucci Marmont Belt (Status: Active, 5 likes), and 3. Prada Nylon Backpack (Status: Pending Authentication). Would you like to see the performance metrics for any of these?


## ❓ FAQ

**Q: Can I monitor my own luxury listings and sales status?**
Yes. The `list_my_selling_items` tool allows your AI agent to pull a list of all items you currently have for sale in your Vestiaire Collective dressing room, along with their current status and metadata, helping you stay organized without manual tracking.

**Q: How can I find out the resale value of a luxury bag?**
Ask your agent to analyze price trends using the `analyze_price_trends` tool. Provide the brand and category, and it will surface historical price data and market trends, helping you decide on the best listing price for your item or identifying investment opportunities.

**Q: Is it possible to filter search results by item condition or material?**
Absolutely. Use the `search_with_advanced_filters` tool to narrow down results by brand, category, condition (e.g., never worn, very good), price range, color, material, and even the country of the seller for more localized results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vestiaire-collective](https://vinkius.com/mcp/vestiaire-collective)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vestiaire Collective** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vestiaire-collective` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vestiaire Collective** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vestiaire-collective": {
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
