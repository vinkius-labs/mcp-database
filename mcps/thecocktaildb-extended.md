# TheCocktailDB MCP Server

Access a massive database of cocktail recipes and ingredients — search by name, filter by alcohol content, and discover new drinks.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/thecocktaildb-extended)

## Overview
**Category:** gaming-entertainment
**Tools Count:** 18

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


## Installation & Usage

To install and use the **TheCocktailDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thecocktaildb-extended](https://vinkius.com/mcp/thecocktaildb-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
