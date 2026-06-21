# Spoonacular MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spoonacular-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/spoonacular-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/spoonacular-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search recipes, analyze nutrition, and plan meals with AI-powered food data.

## Description
Connect **Spoonacular** food API to any AI agent and unlock powerful recipe search, nutrition analysis, and meal planning capabilities through natural language.

### What you can do

- **Advanced Recipe Search** — Search thousands of recipes with filters for cuisine, diet, ingredients, and calories
- **Ingredient-Based Discovery** — Find recipes based on what ingredients you have available
- **Nutrition Analysis** — Get detailed nutritional breakdowns including macros, vitamins, and minerals
- **Recipe Extraction** — Extract recipes from any URL automatically
- **Taste Profiling** — Analyze taste characteristics (sweet, salty, sour, bitter, savory, spicy)
- **Dish Recognition** — Guess dish types from ingredient lists or descriptions
- **Grocery Product Search** — Find packaged food products with nutritional information

### How it works

1. Subscribe to this server
2. Enter your Spoonacular API Key (free tier available)
3. Start exploring recipes and nutrition from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **analyze_recipe**: Analyze a recipe and get enrichment data
- **extract_recipe**: Useful for importing recipes from blogs or recipe sites.

Extract recipe from a URL
- **recipes_by_ingredients**: Perfect for "what can I cook with what I have in my fridge?" scenarios. Returns recipes ranked by ingredient match.

Find recipes based on available ingredients
- **recipes_by_nutrients**: Perfect for diet-specific meal planning.

Find recipes by nutritional requirements
- **get_recipe_instructions**: Get step-by-step analyzed instructions for a recipe
- **get_recipe_info**: Get detailed information about a specific recipe
- **get_recipe_nutrition**: Get detailed nutrition data for a recipe
- **get_recipe_taste**: Get taste profile for a recipe
- **get_recipes_bulk**: Get information for multiple recipes at once
- **guess_dish_type**: Guess the dish type from ingredients or description
- **random_recipes**: Useful for meal inspiration. Can optionally filter by dietary tags.

Get random recipe suggestions
- **search_grocery_products**: Search grocery food products
- **search_recipes**: Returns recipes with basic information including title, ready time, servings, and dietary badges.

Search recipes with advanced filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spoonacular** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me vegetarian Italian recipes under 500 calories."

**🤖 AI Agent:**
> Found 8 vegetarian Italian recipes under 500 calories including 'Vegetarian Pasta Primavera' (350 cal, 25 min), 'Caprese Salad' (280 cal, 10 min), and 'Eggplant Parmesan' (420 cal, 45 min).

---

**👤 You:**
> "What can I make with chicken, rice, and broccoli?"

**🤖 AI Agent:**
> Based on chicken, rice, and broccoli, I found 5 recipes you can make. Top match: 'Chicken Rice Broccoli Stir Fry' (30 min, 380 cal) which uses all 3 ingredients perfectly.

---

**👤 You:**
> "Give me the nutrition breakdown for recipe 654959."

**🤖 AI Agent:**
> Recipe 'Spicy Garlic Shrimp' nutrition per serving: 320 calories, 28g protein, 18g fat, 15g carbs. Rich in Vitamin C (85% DV), Selenium (92% DV), and Omega-3. Low in sodium and saturated fat.


## Installation & Usage

To install and use the **Spoonacular** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spoonacular-alternative](https://vinkius.com/mcp/spoonacular-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
