# Spoonacular MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spoonacular-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search recipes, find meals by ingredients, and analyze nutritional data directly from your AI agent using the Spoonacular food database.

## Description
Connect the **Spoonacular** food and recipe API to your AI agent to transform it into a professional culinary assistant. Access a massive database of recipes, ingredients, and nutritional information through natural conversation.

### What you can do

- **Advanced Recipe Search** — Find recipes by cuisine, diet, or intolerances using natural language with the `search_recipes` tool.
- **Ingredient-Based Discovery** — Use `find_recipes_by_ingredients` to input what's in your fridge and get recipes that maximize your available items.
- **Nutritional Analysis** — Filter meals by calories, protein, or carbs using `find_recipes_by_nutrients` to meet specific health goals.
- **Recipe Extraction** — Convert any cooking blog post into structured data with the `extract_recipe` tool.
- **Meal Planning & Variety** — Generate random ideas with `get_random_recipes` or find alternatives using `get_similar_recipes` to diversify your menu.

### How it works

1. Subscribe to this server
2. Enter your Spoonacular API Key
3. Start cooking with Claude, Cursor, or any MCP-compatible client

No more manual searching through ad-heavy recipe blogs. Your AI acts as a digital sous-chef that knows exactly what you can cook with the ingredients you have.


## Available Tools (22)
- **add_to_meal_plan**: Add an item to a user's meal plan
- **autocomplete_ingredient_search**: Autocomplete ingredient names
- **autocomplete_recipe_search**: Autocomplete recipe titles based on a partial query
- **search_recipes**: Search through thousands of recipes using advanced filtering
- **compute_ingredient_amount**: Compute the amount of an ingredient needed to reach a target nutritional goal
- **extract_recipe**: Extract recipe data from any website URL
- **find_recipes_by_ingredients**: Find recipes that maximize usage of ingredients you have
- **find_recipes_by_nutrients**: Find recipes by nutritional requirements
- **generate_meal_plan**: Generate a meal plan
- **get_ingredient_information**: Get information about a specific ingredient
- **get_ingredient_substitutes**: Get substitutes for a specific ingredient
- **get_meal_plan_week**: Get a meal plan for a specific week
- **get_menu_item_information**: Get information about a specific menu item
- **get_product_information**: Get information about a specific grocery product
- **get_random_recipes**: Get random recipes
- **get_recipe_information**: Get full information about a specific recipe
- **get_shopping_list**: Get a user's shopping list
- **get_similar_recipes**: Find recipes similar to the given recipe ID
- **search_ingredients**: Search for ingredients
- **search_menu_items**: Search for restaurant menu items
- **search_products_by_upc**: Search for a grocery product by its UPC code
- **search_grocery_products**: Search for grocery products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spoonacular** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for healthy Mediterranean dinner recipes that are gluten-free."

**🤖 AI Agent:**
> I've found several Mediterranean options using `search_recipes`. Top results include 'Grilled Greek Chicken' and 'Quinoa Tabbouleh'. Would you like the full instructions for one of these?

---

**👤 You:**
> "I have salmon, asparagus, and lemon. What can I cook?"

**🤖 AI Agent:**
> Using `find_recipes_by_ingredients`, I found a 'Sheet Pan Lemon Herb Salmon' recipe that uses all three. It only requires 2 additional pantry staples. Should I get the full recipe info?

---

**👤 You:**
> "Find recipes with at least 30g of protein and less than 500 calories."

**🤖 AI Agent:**
> I've queried `find_recipes_by_nutrients` for those specific macros. I found a 'High-Protein Turkey Chili' (35g protein, 420 cal). Would you like to see the ingredient list?


## ❓ FAQ

**Q: Can I find recipes based on specific ingredients I already have?**
Yes! Use the `find_recipes_by_ingredients` tool. Just list your ingredients, and the agent will return recipes that maximize the use of what you have while minimizing missing items.

**Q: How do I get the full nutritional breakdown of a specific recipe?**
You can use the `get_recipe_information` tool with the recipe ID and set `includeNutrition` to true. This provides calories, macros, and vitamins for the dish.

**Q: Can the AI extract a recipe from a website link?**
Absolutely. Use the `extract_recipe` tool and provide the URL. The agent will parse the website and return a structured recipe with ingredients and instructions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spoonacular-extended](https://vinkius.com/mcp/spoonacular-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spoonacular** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spoonacular-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spoonacular** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spoonacular-extended": {
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
