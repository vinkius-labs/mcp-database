# Spoonacular MCP Server

Search recipes, find meals by ingredients, and analyze nutritional data directly from your AI agent using the Spoonacular food database.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/spoonacular-extended)

## Overview
**Category:** productivity
**Tools Count:** 22

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


## Available Tools
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


## Installation & Usage

To install and use the **Spoonacular** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spoonacular-extended](https://vinkius.com/mcp/spoonacular-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
