# Spoonacular MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spoonacular)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/spoonacular-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/spoonacular-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

The most comprehensive recipe API — search recipes, plan meals, find dishes by ingredients, and get full nutritional analysis for everything you cook.

## Description
The **Spoonacular MCP Server** connects your AI agent to the world's leading recipe and food intelligence platform — the gold standard for recipe search, meal planning, and nutritional analysis.

### Core Capabilities

- **Smart Recipe Search** — Find recipes with powerful filters: cuisine, diet, intolerances, max calories, cooking time, and more.
- **Find by Ingredients** — Enter what's in your fridge and get recipes that maximize your available ingredients.
- **Full Nutrition** — Every recipe includes a complete nutritional breakdown: calories, protein, fat, carbs, and more.
- **Random Inspiration** — Get surprise recipe suggestions when you need cooking ideas.
- **Diet Support** — Built-in support for vegetarian, vegan, gluten-free, ketogenic, paleo, whole30, and more.

Free tier: 150 requests/day. The most widely used recipe API by professional developers worldwide.


## Available Tools
- **get_random_recipes**: Perfect for meal inspiration.

Get random recipe suggestions from Spoonacular
- **get_recipe_details**: Get complete recipe details including ingredients, instructions, and nutrition
- **find_recipes_by_ingredients**: Enter a comma-separated list of ingredients you have, and get recipe suggestions that maximize usage of your available ingredients.

Find recipes based on ingredients you have available
- **search_recipes**: Returns recipes with full nutritional breakdown, cooking time, and dietary compatibility. Cuisine options: Italian, Mexican, Chinese, Indian, Japanese, Thai, Mediterranean, etc. Diet options: vegetarian, vegan, gluten-free, ketogenic, paleo, whole30.

Search for recipes with optional filters for cuisine, diet, and nutrition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spoonacular** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What can I make with chicken, rice, and garlic?"

**🤖 AI Agent:**
> Great ingredients! I found 10 recipes you can make: Garlic Butter Chicken with Rice (uses all 3!), Chicken Fried Rice, Arroz con Pollo, and more. The top match uses all your ingredients and only needs soy sauce and butter to complete.

---

**👤 You:**
> "Find a gluten-free dessert recipe under 300 calories."

**🤖 AI Agent:**
> 🍰 **Gluten-Free Low-Calorie Desserts**

1. **Almond Flour Brownies**: 250 calories (GF, Vegetarian)
2. **Berry Chia Pudding**: 180 calories (GF, Vegan)
3. **Baked Cinnamon Apples**: 120 calories (GF, Vegan)

---

**👤 You:**
> "Show me the nutritional breakdown for spaghetti bolognese."

**🤖 AI Agent:**
> 🍝 **Nutritional Fact: Spaghetti Bolognese (Per Serving)**

- **Calories**: 450 kcal
- **Protein**: 24g
- **Fat**: 15g (Sat: 4g)
- **Carbs**: 56g (Fiber: 4g)
- **Sodium**: 850mg

*Would you like the full recipe?*


## Installation & Usage

To install and use the **Spoonacular** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spoonacular](https://vinkius.com/mcp/spoonacular)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
