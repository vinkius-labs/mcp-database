# TheMealDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/themealdb-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/themealdb-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/themealdb-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access a global database of recipes, ingredients, and meal categories to find culinary inspiration and detailed cooking instructions.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheMealDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a recipe named 'Teriyaki Chicken'."

**🤖 AI Agent:**
> I found a recipe for Teriyaki Chicken (ID: 52773). It's a Japanese dish. Would you like the full instructions and ingredients?

---

**👤 You:**
> "List all available meal categories."

**🤖 AI Agent:**
> I've retrieved the categories. You can choose from Beef, Chicken, Dessert, Lamb, Miscellaneous, Pasta, Pork, Seafood, Side, Starter, Vegan, Vegetarian, Breakfast, and Goat.

---

**👤 You:**
> "Show me some recipes from the 'Canadian' area."

**🤖 AI Agent:**
> I found several Canadian dishes, including BeaverTails, Poutine, Nanaimo Bars, and Tourtiere. Which one would you like to explore?


## Installation & Usage

To install and use the **TheMealDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/themealdb-extended](https://vinkius.com/mcp/themealdb-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
