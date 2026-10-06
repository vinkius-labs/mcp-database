# Meal Ingredient Footprint Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meal-ingredient-footprint-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [food-science](../categories/food-science.md)

Calculate total environmental impact for ingredients and meals.

## Description
This MCP server provides tools to calculate the environmental footprint of ingredients and complete meals. It aggregates carbon emissions, water usage, packaging waste, and transport impact based on specific ingredient weights and user-provided sustainability factors. Use `calculate_ingredient_impact` to find the footprint of a single item, `calculate_meal_totals` to sum multiple ingredients, and `calculate_per_serving_footprint` to determine the impact per person.


## Available Tools (4)
- **calculate_meal_totals**: Aggregates the impact of multiple ingredients to provide the absolute footprint of the entire meal
- **calculate_ingredient_impact**: Calculates the specific environmental footprint for a single ingredient
- **calculate_per_serving_footprint**: Divides the total meal footprint by the number of servings to find the impact per person
- **summarize_footprint_report**: Generates a high-level summary comparing different impact categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meal Ingredient Footprint Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the footprint of 500g of beef with an emission factor of 25, water factor of 500, packaging factor of 10, transport factor of 2, and 100km transport distance?"

**🤖 AI Agent:**
> The footprint for 500g of beef is 12,500g of CO2e, 250,000 liters of water, 5,000g of packaging, and 1,000 units of transport impact.

---

**👤 You:**
> "Calculate the total meal impact for two ingredients: 200g of wheat (emissions: 5, water: 100, packaging: 5, transport: 1, distance: 50) and 300g of potatoes (emissions: 2, water: 50, packaging: 2, transport: 1, distance: 30)."

**🤖 AI Agent:**
> The total meal footprint is 1,600g of CO2e, 40,000 liters of water, 1,600g of packaging, and 310 units of transport impact.

---

**👤 You:**
> "If a meal has a total carbon footprint of 5000g of CO2e and serves 4 people, what is the impact per serving?"

**🤖 AI Agent:**
> The impact per serving is 1,250g of CO2e.


## ❓ FAQ

**Q: How do I calculate the impact of a single ingredient?**
You can use the `calculate_ingredient_impact` tool by providing the ingredient name, its weight in grams, and the specific intensity factors for emissions, water, packaging, and transport.

**Q: Can I see the impact per person for a recipe?**
Yes, after calculating the total meal impact, use `calculate_per_serving_footprint` to divide the totals by the number of servings.

**Q: What environmental metrics are tracked?**
The server tracks carbon emissions, water footprint, packaging waste, and transport impact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/meal-ingredient-footprint-calculator](https://vinkius.com/en/ai-agent-connect/meal-ingredient-footprint-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meal Ingredient Footprint Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meal-ingredient-footprint-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meal Ingredient Footprint Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meal-ingredient-footprint-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
