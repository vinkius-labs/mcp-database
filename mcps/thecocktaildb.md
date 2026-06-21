# TheCocktailDB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thecocktaildb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search cocktail recipes by name, ingredient, or category — with full mixing instructions, measurements, glass type, and cocktail images.

## Description
The **TheCocktailDB MCP Server** transforms your AI agent into a knowledgeable bartender with access to 600+ cocktail recipes from around the world.

### Core Capabilities

- **Cocktail Search** — Find any drink by name with full ingredient lists, exact measurements, and mixing instructions.
- **Ingredient Filter** — Enter any spirit (Vodka, Gin, Rum, Tequila, Whiskey) and discover every cocktail that uses it.
- **Category Browse** — Explore by type: Cocktail, Shot, Ordinary Drink, Coffee/Tea, Punch/Party Drink, and more.
- **Random Inspiration** — Get a surprise cocktail for "what should I mix tonight?" moments.
- **Glass Guide** — Every recipe specifies the correct glass type for authentic presentation.

Zero authentication required. Perfect for bartending assistants, hospitality chatbots, and cocktail discovery apps.


## Available Tools
- **browse_cocktail_category**: Browse cocktails by category (Cocktail, Shot, Ordinary Drink, etc.)
- **find_cocktails_by_ingredient**: g. Vodka, Gin, Rum, Tequila, Whiskey, Bourbon, Champagne, Kahlua) and get all cocktails that use it.

Find cocktails that use a specific ingredient
- **get_cocktail_details**: Get full cocktail recipe details by CocktailDB ID
- **get_random_cocktail**: Perfect for bartender inspiration or "what should I drink?" moments.

Get a random cocktail recipe for inspiration
- **search_cocktails**: Returns full recipes with ingredients, measures, glass type, and step-by-step instructions. Try: Margarita, Mojito, Old Fashioned, Negroni, Mai Tai, Piña Colada.

Search for cocktail recipes by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheCocktailDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How do I make a Margarita?"

**🤖 AI Agent:**
> Classic Margarita recipe: 🧊 Rub the rim of a cocktail glass with lime juice, dip in coarse salt. Shake 1½ oz Tequila, 1 oz Lime Juice, and ½ oz Triple Sec with ice. Strain into the prepared glass. Garnish with a lime wheel. Serve in a Cocktail Glass.

---

**👤 You:**
> "Show me a cocktail that includes Campari."

**🤖 AI Agent:**
> Here is the 'Negroni': Combine 1 oz Gin, 1 oz Campari, and 1 oz Sweet Vermouth over ice. Stir it well and strain into a rocks glass. Garnish with a fresh orange peel.

---

**👤 You:**
> "Give me a random drink recommendation."

**🤖 AI Agent:**
> How about a 'Dark and Stormy'? It requires 2 oz Dark Rum poured over ice, topped high with Ginger Beer. Served in a Highball glass with a lime wedge.


## ❓ FAQ

**Q: Do I need an API key?**
No. TheCocktailDB provides free open access. No registration or API key required.

**Q: Are measurements standardized across all recipes?**
Measurements on TheCocktailDB typically default to imperial measurements (oz, parts, dashes). They match exactly what the database provides.

**Q: Can I search for non-alcoholic mocktails?**
Definitely! The DB maintains a 'Non-Alcoholic' category you can filter by when asking for a refreshing drink with zero ABV.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thecocktaildb](https://vinkius.com/mcp/thecocktaildb)
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
3. Set Type to "SSE", enter `thecocktaildb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TheCocktailDB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thecocktaildb": {
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
