# TheMealDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/themealdb-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/themealdb-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/themealdb-alternative-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **TheMealDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/themealdb-alternative](https://vinkius.com/mcp/themealdb-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
