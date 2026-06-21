# TheCocktailDB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thecocktaildb-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming-entertainment](../categories/gaming-entertainment.md)

Access a massive database of cocktail recipes and ingredients — search by name, filter by alcohol content, and discover new drinks.

## Description
Connect to **TheCocktailDB** and transform your AI agent into a professional mixologist. Access thousands of recipes, ingredient details, and specialized filters to find the perfect drink for any occasion.

### What you can do

- **Search & Discovery** — Find cocktails by name, first letter, or browse random selections using `search_cocktail_by_name` and `get_random_cocktail`.
- **Ingredient Analysis** — Look up detailed information about specific ingredients and their properties with `search_ingredient_by_name`.
- **Advanced Filtering** — Narrow down choices by category, glass type, alcoholic content, or specific ingredients using tools like `filter_by_category` and `filter_by_alcoholic`.
- **Premium Features** — Access popular cocktails, latest additions, and multi-ingredient filtering with a premium API key.

### How it works

1. Subscribe to this server
2. Enter your TheCocktailDB API Key (you can use '1' for the free test tier)
3. Start exploring mixology from Claude, Cursor, or any MCP-compatible client

No more searching through disorganized recipe blogs. Your AI acts as a dedicated bartender and drink consultant.

### Who is this for?

- **Home Bartenders** — instantly find recipes based on the ingredients you have on hand
- **App Developers** — test drink data and ingredient relationships directly from your workspace
- **Food & Beverage Enthusiasts** — explore the history and composition of classic and modern cocktails


## Available Tools
- **filter_by_alcoholic**: Filter by alcoholic or non-alcoholic status
- **filter_by_category**: Filter by cocktail category
- **filter_by_glass**: Filter by glass type
- **filter_by_ingredient**: Filter cocktails by a single ingredient
- **filter_by_multi_ingredient**: Requires a Premium API key.

Filter by multiple ingredients (Premium Only)
- **get_cocktail_by_id**: Lookup full cocktail details by its ID
- **get_ingredient_by_id**: Lookup ingredient details by its ID
- **get_latest_cocktails**: Requires a Premium API key.

List the most recently added cocktails (Premium Only)
- **get_popular_cocktails**: Requires a Premium API key.

List the most popular cocktails (Premium Only)
- **get_random_cocktail**: Fetch a single random cocktail
- **get_random_selection**: Requires a Premium API key.

Fetch 10 random cocktails (Premium Only)
- **list_alcoholic_filters**: List all available alcoholic filters
- **list_categories**: List all available cocktail categories
- **list_glasses**: List all available glass types
- **list_ingredients**: List all available ingredients
- **search_cocktail_by_first_letter**: List all cocktails starting with a specific letter
- **search_cocktail_by_name**: Search for cocktails by their name
- **search_ingredient_by_name**: Search for ingredient details by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheCocktailDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a cocktail named 'Margarita' and show me the recipe."

**🤖 AI Agent:**
> I found the Margarita! It's an Ordinary Drink served in a Margarita glass. Ingredients include Tequila, Triple sec, and Lime juice. Would you like the step-by-step instructions?

---

**👤 You:**
> "What are some popular cocktails I can make?"

**🤖 AI Agent:**
> Using your premium access, I've retrieved the most popular cocktails. The list includes the Mojito, Old Fashioned, and Espresso Martini. Which one would you like to see the details for?

---

**👤 You:**
> "List all ingredients that are classified as 'Alcoholic'."

**🤖 AI Agent:**
> I've pulled the list of alcoholic filters. You can filter cocktails by categories like 'Alcoholic', 'Non_Alcoholic', and 'Optional_Alcohol'. Would you like to see drinks from one of these categories?


## ❓ FAQ

**Q: Can I find non-alcoholic drink recipes using this server?**
Yes! You can use the `filter_by_alcoholic` tool with the status 'Non_Alcoholic' to retrieve a list of mocktails and non-alcoholic beverages.

**Q: How can I get a random cocktail suggestion for inspiration?**
Simply use the `get_random_cocktail` tool. It will return full details, including ingredients and instructions, for one randomly selected drink from the database.

**Q: Is it possible to search for cocktails by a specific ingredient like Gin or Vodka?**
Absolutely. Use the `filter_by_ingredient` tool and provide the name of the ingredient to see all cocktails that include it in their recipe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thecocktaildb-extended](https://vinkius.com/mcp/thecocktaildb-extended)
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
3. Set Type to "SSE", enter `thecocktaildb-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TheCocktailDB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thecocktaildb-extended": {
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
