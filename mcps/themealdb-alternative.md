# TheMealDB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/themealdb-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search recipes, browse ingredients, and discover meals from global cuisines via AI.

## Description
Connect **TheMealDB** open database to any AI agent and instantly search recipes, browse ingredients, and discover meals from global cuisines.

### What you can do

- **Recipe Search** — Search for meals by name and retrieve complete recipes with ingredients and step-by-step instructions
- **Cuisine Discovery** — Filter meals by cuisine area (Italian, Indian, Mexican, etc.)
- **Category Browsing** — Explore meals organized by category (Beef, Chicken, Seafood, Dessert, etc.)
- **Ingredient Lookup** — Find meals by main ingredient and discover all available ingredients
- **Random Inspiration** — Get random meal suggestions for culinary inspiration

### How it works

1. Subscribe to this server
2. No API key required — TheMealDB is free and open
3. Start searching recipes from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **list_ingredients**: List all available ingredients
- **lookup_meal**: Get full details of a meal by ID
- **search_by_letter**: Search meals by first letter
- **search_meals**: Returns up to 100 results with basic info.

Search for meals by name
- **filter_by_area**: Filter meals by cuisine area
- **filter_by_category**: Filter meals by category
- **filter_by_ingredient**: Filter meals by main ingredient
- **get_random_meal**: Perfect for meal inspiration or discovery.

Get a random meal suggestion
- **list_areas**: List all cuisine areas
- **list_categories**: List all meal categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheMealDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for chicken recipes."

**🤖 AI Agent:**
> Found 15 chicken recipes including 'Chicken Enchilada Casserole', 'Chicken & Mushroom Hotpot', and 'Jerk Chicken'. Would you like the full recipe for any of these?

---

**👤 You:**
> "Give me a random meal idea for dinner."

**🤖 AI Agent:**
> Today's random suggestion: 'Beef Wellington' - a classic British dish with beef fillet coated in pâté and duxelles, wrapped in puff pastry. It's from the Beef category and serves 8 people.

---

**👤 You:**
> "Show me all Italian cuisine meals."

**🤖 AI Agent:**
> Found 12 Italian meals including 'Spaghetti Bolognese', 'Chicken Alfredo Primavera', 'Osso Buco alla Milanese', and 'Mediterranean Pasta Salad'.


## ❓ FAQ

**Q: Do I need an API key to use TheMealDB?**
No! TheMealDB is completely free and open. No API key is required to search and retrieve recipes.

**Q: Can I get full recipe details with ingredients and instructions?**
Yes! Use the `lookup_meal` tool with a meal ID to retrieve the full recipe including all ingredients with measurements, category, area, and detailed instructions.

**Q: How do I find recipes by ingredient?**
Use the `filter_by_ingredient` tool with the ingredient name. It returns all meals that have that ingredient as their main component.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/themealdb-alternative](https://vinkius.com/mcp/themealdb-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TheMealDB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `themealdb-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TheMealDB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "themealdb-alternative": {
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
