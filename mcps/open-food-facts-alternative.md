# Open Food Facts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-food-facts-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the world's largest open food database — retrieve nutrition facts, ingredients, and environmental scores for millions of products.

## Description
Connect to **Open Food Facts**, the collaborative, free, and open database of food products from around the world. This MCP server allows your AI agent to analyze millions of products to help with nutrition tracking, dietary research, and conscious shopping.

### What you can do

- **Barcode Lookup** — Instantly retrieve full product data including Nutri-Score, Eco-Score, and NOVA groups using EAN-13 barcodes.
- **Advanced Search** — Filter the global database by brands, categories, labels (like 'Organic' or 'Vegan'), and nutrient levels.
- **Ingredient Analysis** — Inspect ingredient lists and check for the presence of specific additives or allergens.
- **Nutritional Profiling** — Access detailed 100g breakdowns for energy, fats, sugars, and proteins to compare products accurately.

### How it works

1. Subscribe to this server
2. (Optional) Provide a User Agent string to identify your application
3. Start querying food data directly from your AI assistant

### Who is this for?

- **Health-Conscious Users** — quickly check if a product fits your dietary requirements or has high-quality ingredients.
- **Researchers & Developers** — access structured food data for analysis, app development, or nutritional studies.
- **Sustainability Advocates** — evaluate the environmental impact of products through the integrated Eco-Score metrics.


## Available Tools
- **get_product**: Retrieve detailed information about a specific product by its barcode
- **search_products**: Search for products using keywords and filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Food Facts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get product details for barcode 3017620422003."

**🤖 AI Agent:**
> I've retrieved the data for Nutella (400g). It has a Nutri-Score of 'E', contains ingredients like sugar and palm oil, and belongs to the 'Chocolate spreads' category. Would you like to see the full nutritional breakdown?

---

**👤 You:**
> "Search for 'Organic' dark chocolate brands."

**🤖 AI Agent:**
> I found several organic dark chocolate products. Notable brands include 'Alter Eco' and 'Green & Black's'. Would you like me to list the specific products and their cocoa percentages?

---

**👤 You:**
> "Find products in the 'Beverages' category that are 'without' additives."

**🤖 AI Agent:**
> Searching the database... I've found several additive-free beverages, including various mineral waters and pure fruit juices like 'Innocent Orange Juice'. Would you like the details for any of these?


## ❓ FAQ

**Q: How do I look up a specific food item using its barcode?**
Use the `get_product` tool and provide the barcode (EAN-13). The agent will return the product name, ingredients, Nutri-Score, and detailed nutritional facts.

**Q: Can I search for products that are specifically labeled as Organic or Vegan?**
Yes! Use the `search_products` tool and specify the `labels` parameter (e.g., 'Organic' or 'Vegan') to filter the results accordingly.

**Q: Is it possible to filter out products that contain additives?**
Absolutely. When using the `search_products` tool, set the `additives` parameter to 'without' to find products that do not contain any food additives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-food-facts-alternative](https://vinkius.com/mcp/open-food-facts-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open Food Facts** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `open-food-facts-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Food Facts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-food-facts-alternative": {
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
