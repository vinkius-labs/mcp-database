# Open Food Facts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-food-facts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Scan barcodes and search packaged food products for complete nutritional data, Nutri-Score grades, allergens, and ingredient analysis.

## Description
The **Open Food Facts MCP Server** connects your AI agent to the world's largest open food product database — over 2 million products from 150+ countries.

### Core Capabilities

- **Barcode Scanner** — Instantly look up any packaged food product by its EAN/UPC barcode to get complete nutritional information.
- **Product Search** — Find products by name, brand, or category across the entire global database.
- **Nutri-Score** — Official A-to-E nutritional quality grading used across Europe.
- **NOVA Classification** — Food processing level indicator (1=unprocessed to 4=ultra-processed).
- **Allergen Detection** — Comprehensive allergen warnings including gluten, dairy, nuts, soy, and more.

Zero authentication required. Open source, community-driven data. Essential for health apps, dietary assistants, and grocery shopping tools.


## Available Tools (2)
- **scan_food_barcode**: Returns Nutri-Score, NOVA classification, full macronutrient profile, allergens, and ingredient list.

Scan a food product barcode to get complete nutritional and allergen information
- **search_food_products**: Returns nutritional information, Nutri-Score grades, NOVA processing levels, and allergen data for each product.

Search the Open Food Facts database for packaged food products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Food Facts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan barcode 3017620422003"

**🤖 AI Agent:**
> That's Nutella! Here's what I found: Nutri-Score E, NOVA Group 4 (ultra-processed). Per 100g: 539 kcal, 31g fat, 57g carbs, 6g protein. Contains hazelnuts, milk, and soy. Ingredients: sugar, palm oil, hazelnuts (13%), cocoa, skimmed milk powder, whey powder, lecithin, vanillin.

---

**👤 You:**
> "Search for vegan protein bars with a Nutri-Score of A."

**🤖 AI Agent:**
> I found several options! For instance, 'Misfits Vegan Protein Bar' often scores well. Another high-ranking product is 'Trek High Protein Flapjack' which features a good Nutri-Score due to its balance of fiber and plant protein.

---

**👤 You:**
> "What is the NOVA group for a standard can of Coca-Cola?"

**🤖 AI Agent:**
> A standard can of Coca-Cola is classified under NOVA Group 4, which means it is an ultra-processed food product. It also holds a Nutri-Score of E due to its high sugar content.


## ❓ FAQ

**Q: What is Nutri-Score?**
Nutri-Score is a front-of-pack nutrition label that rates food products from A (healthiest) to E (least healthy). It's widely used across Europe and helps consumers make informed dietary choices at a glance.

**Q: What is the NOVA classification?**
The NOVA classification assigns a score from 1 to 4 depending on how much a food is processed. 1 means unprocessed/minimally processed foods, while 4 indicates ultra-processed food and drink products.

**Q: Is the allergen data reliable?**
The allergen data is derived from product labels uploaded by contributors. While extensive, you should always double-check physical packaging for severe allergies as formulations can change.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-food-facts](https://vinkius.com/mcp/open-food-facts)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `open-food-facts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Food Facts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-food-facts": {
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
