# Spoonacular MCP Server

Search recipes, analyze nutrition, and plan meals with AI-powered food data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/spoonacular-alternative)

## Overview
**Category:** productivity
**Tools Count:** 13

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


## Installation & Usage

To install and use the **Spoonacular** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spoonacular-alternative](https://vinkius.com/mcp/spoonacular-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
