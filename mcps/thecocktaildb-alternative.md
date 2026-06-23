# TheCocktailDB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thecocktaildb-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Global cocktail database — search recipes, ingredients, and mixology guides via AI.

## Description
Equip your AI agent with the most comprehensive cocktail intelligence available via **TheCocktailDB**. This unified server merges thousands of drink recipes and ingredient details into a single, high-performance interface. Your agent can instantly find detailed instructions for classic and modern cocktails, retrieve ingredient metadata, and filter drinks by categories or glass types. Whether you are looking for a random inspiration or a specific recipe by ingredient, your agent acts as a dedicated global bartender and mixology expert through natural conversation.

### What you can do

- **Recipe Discovery** — Search for thousands of cocktail recipes by name or first letter to retrieve instructions and images.
- **Ingredient Auditing** — Fetch complete metadata for specific ingredients and search for them within the database.
- **Mixology Filtering** — Filter cocktails by category (e.g., Ordinary Drink, Cocktail), glass type, or alcoholic content.
- **Creative Inspiration** — Get a completely random cocktail recipe to discover new flavors and techniques.
- **Inventory Matching** — Find all drinks that use a specific ingredient you already have in your cabinet.

### How it works

1. Subscribe to this server
2. Enter your TheCocktailDB API Key (use '1' for testing)
3. Start managing your mixology intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Bartenders & Mixologists** — instantly retrieve exact measurements and ratios for thousands of drinks.
- **Home Enthusiasts** — discover new recipes based on available ingredients and learn professional techniques.
- **Content Creators** — automate the retrieval of high-quality drink images and recipe data for media production.
- **Party Organizers** — quickly compile themed drink lists by filtering categories or alcoholic filters.


## Available Tools (12)
- **filter_by_category**: Filter cocktails by category
- **filter_by_ingredient**: Filter cocktails by ingredient
- **list_alcoholic_filters**: g., Alcoholic, Non-Alcoholic).

List alcoholic filters
- **list_categories**: List cocktail categories
- **list_glasses**: List cocktail glasses
- **list_ingredients**: List all ingredients
- **get_cocktail_details**: Get cocktail details by ID
- **get_ingredient_details**: Get ingredient details by ID
- **get_random_cocktail**: Get a random cocktail
- **search_ingredient_by_name**: Search for an ingredient by name
- **search_cocktail_by_first_letter**: Search for a cocktail by first letter
- **search_cocktail_by_name**: g., Margarita).

Search for a cocktail by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheCocktailDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the recipe of a 'Margarita'."

**🤖 AI Agent:**
> I've found the Margarita recipe. It requires Tequila, Triple Sec, and Lime Juice. I have the full step-by-step instructions and a high-quality image of the final drink. Ready to start mixing?

---

**👤 You:**
> "What drinks can I make with 'Vodka'?"

**🤖 AI Agent:**
> Searching for Vodka-based drinks... I've found several popular options including the 'Moscow Mule', 'White Russian', and 'Cosmopolitan'. Would you like the recipe for any of these?

---

**👤 You:**
> "Suggest a random cocktail for tonight."

**🤖 AI Agent:**
> How about a 'Negroni'? It's a classic bitter-sweet drink made with Gin, Campari, and Sweet Vermouth. I can give you the exact proportions if you're interested.


## ❓ FAQ

**Q: Can I search for cocktails that only contain a specific ingredient like Gin?**
Yes! Use the `filter_by_ingredient` tool with 'Gin'. It will return a list of all cocktails in the database that include Gin as one of their primary components.

**Q: How do I get the full instructions and image for a specific drink?**
First, find the drink ID using `search_cocktail_by_name`. Then, use the `get_cocktail_details` tool with that ID to retrieve the high-res image URL, full ingredient list, and step-by-step instructions.

**Q: Does the integration provide non-alcoholic drink options?**
Absolutely. You can use the `list_alcoholic_filters` tool to see available filters, and then use `filter_by_category` or specific search queries to identify 'Non_Alcoholic' drinks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thecocktaildb-alternative](https://vinkius.com/mcp/thecocktaildb-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TheCocktailDB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thecocktaildb-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TheCocktailDB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thecocktaildb-alternative": {
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
