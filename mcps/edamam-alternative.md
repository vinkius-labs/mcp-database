# Edamam MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edamam-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/edamam-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/edamam-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Manage food and nutrition — audit recipes and ingredients via AI.

## Description
Empower your AI agent to orchestrate your entire culinary research and nutritional auditing workflow with **Edamam**, the comprehensive source for food and recipe data. By connecting the Edamam API to your agent, you transform complex nutritional analysis into a natural conversation. Your agent can instantly search for thousands of recipes, audit ingredient breakdowns, and identify health-conscious meal options without you ever touching a nutrition portal. Whether you are planning a dietary regimen or conducting regional culinary research, your agent acts as a real-time nutritionist, ensuring your data is always precise and well-categorized.

### What you can do

- **Recipe Auditing** — Search for thousands of recipes by keyword or name and retrieve detailed metadata, including calorie counts and cuisine types.
- **Nutritional Oversight** — Audit the detailed breakdown of ingredients to understand total calories, weights, and nutritional markers instantly.
- **Dietary Discovery** — Query recipes based on specific diet labels such as 'high-protein' or 'low-fat' to maintain strict nutritional control.
- **Health Intelligence** — Find recipes matching health labels like 'vegan' or 'gluten-free' to assist in dietary planning.
- **Cuisine Discovery** — Retrieve recipes categorized by cuisine type to understand regional food distribution and themes.

### How it works

1. Subscribe to this server
2. Enter your Edamam App ID and App Key
3. Start managing your food intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Nutritionists & Chefs** — monitor recipe data and retrieve nutritional metadata straight from your workflow.
- **Health Enthusiasts** — verify ingredient breakdowns and audit calorie counts without manual searching.
- **Meal Planners** — perform rapid audits of dietary labels and identify matching recipes through natural language.
- **Operations Leads** — automate food data querying to orchestrate cross-functional hospitality teams smoothly.


## Available Tools
- **check_api_status**: Check if the Edamam service is operational
- **get_nutrition_details**: Get nutritional breakdown for a list of ingredients
- **search_recipes_by_cuisine**: Search for recipes by cuisine type (e.g., American, Italian)
- **search_recipes_by_diet**: Search for recipes with specific diet labels (e.g., high-protein, low-fat)
- **search_recipes_by_health**: Search for recipes with health labels (e.g., vegan, gluten-free)
- **search_recipes**: Search for food recipes by keyword or name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Edamam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'healthy chicken salad' recipes using Edamam."

**🤖 AI Agent:**
> I've retrieved several healthy chicken salad recipes! Notable options include a 'Mediterranean Chicken Salad' and a 'Grilled Lemon Chicken Salad'. Would you like the calorie count or full nutritional breakdown for any of these?

---

**👤 You:**
> "Get nutritional details for '1 cup of cooked rice' and '100g of grilled salmon'."

**🤖 AI Agent:**
> I've retrieved the nutrition details! The combination has approximately 450 calories and 35g of protein. I can provide the full breakdown of fats, carbs, and vitamins if you'd like.

---

**👤 You:**
> "Show vegan recipes for 'pasta' using Edamam."

**🤖 AI Agent:**
> I've identified 10 vegan pasta recipes. Notable matches include 'Vegan Tomato Basil Pasta' and 'Creamy Cashew Pasta'. I can provide the cuisine type and preparation time for each if you'd like.


## Installation & Usage

To install and use the **Edamam** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edamam-alternative](https://vinkius.com/mcp/edamam-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
