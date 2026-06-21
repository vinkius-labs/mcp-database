# TheMealDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/themealdb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/themealdb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/themealdb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search international recipes by name, category, cuisine, or ingredient — with full cooking instructions, measurements, and video tutorials.

## Description
The **TheMealDB MCP Server** gives your AI agent instant access to an international recipe database spanning dozens of cuisines — from Japanese sushi rolls to Italian pasta, Mexican tacos, and Indian curries.

### Core Capabilities

- **Recipe Search** — Find meals by name with complete ingredient lists, exact measurements, and step-by-step cooking instructions.
- **Category Browse** — Explore by food type: Beef, Chicken, Dessert, Pasta, Seafood, Vegetarian, Vegan, Breakfast, and more.
- **Cuisine Filter** — Discover recipes from 27+ national cuisines including American, Chinese, French, Indian, Italian, Japanese, Mexican, Thai, and Vietnamese.
- **Random Inspiration** — Get a surprise recipe whenever someone asks "what should I cook tonight?"
- **Video Tutorials** — Most recipes include YouTube tutorial links for visual learners.

Zero authentication required. Perfect for meal planning assistants, cooking chatbots, food blogs, and recipe recommendation engines.


## Available Tools
- **get_meal_details**: Get complete details of a specific meal by its TheMealDB ID
- **get_meals_by_cuisine**: Available areas: American, British, Canadian, Chinese, Croatian, Dutch, Egyptian, Filipino, French, Greek, Indian, Irish, Italian, Jamaican, Japanese, Kenyan, Malaysian, Mexican, Moroccan, Polish, Portuguese, Russian, Spanish, Thai, Tunisian, Turkish, Vietnamese.

Browse meals by cuisine/country of origin
- **get_meals_by_category**: Available categories: Beef, Chicken, Dessert, Lamb, Miscellaneous, Pasta, Pork, Seafood, Side, Starter, Vegan, Vegetarian, Breakfast, Goat.

Browse meals by category such as Beef, Chicken, Dessert, Pasta, Seafood, or Vegetarian
- **get_random_meal**: Great for inspiration or "what should I cook tonight?" scenarios.

Get a random recipe from TheMealDB
- **search_meals**: Returns full recipe details including ingredients, measures, instructions, and YouTube tutorials. Try queries like "Arrabiata", "Chicken", "Sushi", "Pad Thai".

Search TheMealDB for recipes by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheMealDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me an Italian pasta recipe."

**🤖 AI Agent:**
> I found several Italian pasta recipes! The top result is Pasta Carbonara — a classic Roman dish made with eggs, Pecorino cheese, guanciale, and black pepper. Ready in 30 minutes, serves 4. Would you like the full recipe with measurements?

---

**👤 You:**
> "Find a quick pasta recipe that takes less than 30 minutes."

**🤖 AI Agent:**
> Scanning TheMealDB ('search_meals')...
I recommend the 'Spaghetti Carbonara' (Meal ID: 52982). It takes about 25 minutes.
Main ingredients: Spaghetti, Pancetta, Eggs, Parmesan.
Do you want me to list the full cooking instructions?

---

**👤 You:**
> "Give me a list of highly rated vegetarian meals from Indian cuisine."

**🤖 AI Agent:**
> Filtering categorical clusters ('filter_by_category' & 'filter_by_area')...
Here are some classic Indian vegetarian dishes from the database:
1. 'Dal Makhani' (Black Lentils)
2. 'Matar Paneer' (Peas and Cheese)
3. 'Baingan Bharta' (Roasted Eggplant)
Let me know if you need the recipe for one of these.


## Installation & Usage

To install and use the **TheMealDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/themealdb](https://vinkius.com/mcp/themealdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
