# Mealie (Recipe Manager) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mealie-recipe-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Mealie recipes, meal plans, and shopping lists directly through your AI agent.

## Description
Connect your **Mealie** instance to any AI agent and take full control of your kitchen workflow. From organizing recipes to automating your weekly meal planning, your AI acts as a digital sous-chef.

### What you can do

- **Recipe Management** — List, create, and update recipes. Fetch full details using slugs to get ingredients and instructions instantly.
- **Meal Planning** — View your current meal plans and schedule new recipes for specific dates to stay organized.
- **Shopping Lists** — Manage your grocery runs by listing shopping lists and toggling items as you find them in the store.
- **Organization** — Browse through your custom categories and tags to find the perfect meal for any occasion.

### How it works

1. Subscribe to this server
2. Enter your Mealie Instance URL and Personal API Token
3. Start managing your recipes and meals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Cooks** — quickly find recipes or add ingredients to shopping lists without leaving your chat interface
- **Meal Planners** — automate the organization of your weekly food schedule through natural conversation
- **Health Enthusiasts** — keep track of your recipe database and categories for better nutritional planning


## Available Tools (13)
- **create_meal_plan**: Create a new meal plan entry
- **create_recipe**: Create a new recipe
- **create_shopping_list**: Create a new shopping list
- **delete_meal_plan**: Delete a meal plan entry
- **delete_recipe**: Remove a recipe
- **get_recipe**: Retrieve a specific recipe by its slug
- **list_categories**: List all categories
- **list_meal_plans**: Retrieve current meal plans
- **list_recipes**: List all recipes
- **list_shopping_lists**: List all shopping lists
- **list_tags**: List all tags
- **toggle_shopping_list_item**: Toggle shopping list item completion
- **update_recipe**: Update an existing recipe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mealie (Recipe Manager)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recipes in Mealie."

**🤖 AI Agent:**
> I've found 12 recipes in your Mealie instance. Some highlights include 'Spicy Taco Night', 'Homemade Sourdough', and 'Garden Salad'. Would you like the details for any of these?

---

**👤 You:**
> "Get the full recipe for the slug 'classic-lasagna'."

**🤖 AI Agent:**
> Retrieved 'Classic Lasagna'. It yields 8 servings and requires: lasagna noodles, ground beef, ricotta, and marinara sauce. The instructions involve layering and baking for 45 minutes. Should I add these ingredients to your shopping list?

---

**👤 You:**
> "Mark item ID 'milk-123' as checked in shopping list 'grocery-list-456'."

**🤖 AI Agent:**
> Done! I've updated the status of 'Milk' in your grocery list to completed.


## ❓ FAQ

**Q: How can I see the full instructions for a specific recipe?**
You can use the `get_recipe` tool by providing the recipe's unique slug. The agent will return the full details, including ingredients, steps, and yield.

**Q: Can I mark items as 'bought' on my shopping list using the AI?**
Yes! Use the `toggle_shopping_list_item` tool. You just need the shopping list ID and the item ID to check or uncheck items remotely.

**Q: Is it possible to see what I have planned for dinner this week?**
Absolutely. The `list_meal_plans` tool retrieves all scheduled entries, allowing your AI to summarize your upcoming meals for the week.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mealie-recipe-manager](https://vinkius.com/mcp/mealie-recipe-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mealie (Recipe Manager)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mealie-recipe-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mealie (Recipe Manager)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mealie-recipe-manager": {
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
