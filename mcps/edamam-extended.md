# Edamam MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edamam-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/edamam-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/edamam-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scientific-research](../categories/scientific-research.md)

Search over 2.3 million recipes, analyze nutritional data, and access a database of 900,000+ food items directly from your AI agent.

## Description
Integrate **Edamam** into your AI workflows to access world-class nutrition and recipe data. Whether you are building a meal planner, a health app, or just looking for cooking inspiration, this server provides the tools to query millions of recipes and analyze ingredients with scientific precision.

### What you can do

- **Recipe Discovery** — Search a massive database of 2.3M+ recipes using keywords, dietary labels (vegan, keto), and cuisine types.
- **Nutrition Analysis** — Get detailed breakdowns of calories, fats, proteins, and micronutrients for any list of ingredients or full recipes.
- **Food Lookup** — Access data for over 900,000 foods, including raw ingredients, restaurant items, and packaged goods using names or UPC codes.
- **Dietary Filtering** — Filter results by health labels, allergens, and specific nutritional goals like high-protein or low-carb.

### How it works

1. Subscribe to this server
2. Enter your Edamam Application ID and Application Key
3. Start querying food and nutrition data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health & Wellness Coaches** — generate instant nutritional reports for client meal plans
- **Home Cooks & Foodies** — find recipes that match specific dietary needs or available ingredients
- **Developers** — integrate robust food data into applications without managing complex databases


## Available Tools
- **analyze_nutrition**: Get nutrition facts for a recipe
- **parse_food**: Look up food in the Food Database
- **search_recipes**: 3 million recipes by keywords, dietary restrictions, and other filters.

Search recipes by keywords and filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Edamam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for high-protein chicken recipes with an Asian cuisine type."

**🤖 AI Agent:**
> I found several high-protein Asian chicken recipes, including 'Thai Basil Chicken' and 'Ginger Soy Steamed Chicken'. Would you like the full ingredient list for one of these?

---

**👤 You:**
> "Analyze the nutrition for 100g of oats, 1 banana, and 200ml of almond milk."

**🤖 AI Agent:**
> Based on those ingredients, the total is approximately 540 calories, with 82g of carbohydrates, 12g of protein, and 14g of fat. It is also high in fiber and potassium.

---

**👤 You:**
> "Look up the nutritional data for 'Greek Yogurt' in the food database."

**🤖 AI Agent:**
> I've retrieved the data for Greek Yogurt. A standard serving contains high protein levels and active cultures. I can also provide specific brand data if you have a UPC code.


## Installation & Usage

To install and use the **Edamam** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edamam-extended](https://vinkius.com/mcp/edamam-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
