# Mealie (Recipe Manager) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mealie-recipe-manager)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mealie-recipe-manager-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mealie-recipe-manager-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Mealie (Recipe Manager)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mealie-recipe-manager](https://vinkius.com/mcp/mealie-recipe-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
