# TheMealDB MCP Server

Access a global database of recipes, ingredients, and meal categories to find culinary inspiration and detailed cooking instructions.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/themealdb-extended)

## Overview
**Category:** knowledge-management
**Tools Count:** 13

## Description
Connect **TheMealDB** to your AI agent to transform it into a professional sous-chef. Access thousands of recipes with detailed instructions, measurements, and cultural origins.

### What you can do

- **Search & Discovery** — Find recipes by name, first letter, or browse through extensive lists of categories and geographic areas.
- **Ingredient Analysis** — Filter meals by their main components or list all available ingredients to see what you can cook.
- **Detailed Recipes** — Retrieve full cooking instructions, precise ingredient measurements, and high-quality image previews using unique meal IDs.
- **Global Cuisine** — Explore dishes by region, from Japanese and Italian to Mexican and Moroccan.
- **Premium Insights** — Access the latest database additions and bulk random selections (requires a V2 API key).

### How it works

1. Subscribe to this server
2. Enter your TheMealDB API Key (use '1' for the free tier)
3. Start asking for recipes or meal ideas in Claude, Cursor, or any MCP client

### Who is this for?

- **Home Cooks** — quickly find what to cook with the ingredients you have on hand
- **App Developers** — integrate rich culinary data into food-related applications
- **Content Creators** — gather recipe data and inspiration for food blogs or social media


## Available Tools
- **filter_by_area**: g., Canadian).

Filter meals by area
- **filter_by_category**: g., Seafood).

Filter meals by category
- **filter_by_ingredient**: For V2 premium users, multiple ingredients can be comma-separated.

Filter meals by main ingredient(s)
- **get_latest_meals**: Requires a premium API key and V2 API version.

Retrieve the most recently added meals (Premium V2 Only)
- **get_meal_by_id**: Lookup full meal details by ID
- **get_random_meal**: Lookup a single random meal
- **get_random_meals_selection**: Requires a premium API key and V2 API version.

Lookup a selection of 10 random meals (Premium V2 Only)
- **list_all_categories**: List all meal categories with descriptions
- **list_areas**: List simple browseable areas (countries/regions)
- **list_categories**: List simple browseable categories
- **list_ingredients**: List simple browseable ingredients
- **list_meals_by_first_letter**: List all meals starting with a specific letter
- **search_meals_by_name**: Search for meals by their full or partial name


## Installation & Usage

To install and use the **TheMealDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/themealdb-extended](https://vinkius.com/mcp/themealdb-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
