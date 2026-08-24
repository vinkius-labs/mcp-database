# Nutrition Macro Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/nutrition-macro-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

High-precision nutritional analysis for food items and meals.

## Description
This MCP server provides high-precision nutritional analysis by aggregating macronutrients and micronutrients from food items. Using USDA FoodData Central reference values, it calculates exact totals for calories, proteins, fats, carbohydrates, and a wide array of vitamins and minerals. Users can use `calculate_meal_nutrition` to sum totals for multiple items, `calculate_daily_value_percentages` to see how a meal fits into a 2,000 kcal diet, and `get_food_reference_data` to inspect individual food profiles. It handles complex unit conversions like ounces to grams and cups to milliliters automatically.


## Available Tools (3)
- **get_food_reference_data**: Retrieves the base nutritional profile for a specific food item
- **calculate_daily_value_percentages**: Calculates the percentage of the 2,000 kcal Daily Value (%DV) for every nutrient in a given meal
- **calculate_meal_nutrition**: Calculates the absolute nutritional totals for a collection of food items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nutrition Macro Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the nutrition for 100g of chicken breast and 1 cup of cooked rice."

**🤖 AI Agent:**
> The total nutritional content for 100g of chicken breast and 1 cup of cooked rice includes 320 kcal, 35g of protein, 4g of fat, and 45g of carbohydrates.

---

**👤 You:**
> "What is the nutritional profile for 1 oz of almonds?"

**🤖 AI Agent:**
> One ounce of almonds contains approximately 164 kcal, 6g of protein, 14g of fat, and 3.5g of fiber.

---

**👤 You:**
> "How much sodium is in 2 tbsp of soy sauce?"

**🤖 AI Agent:**
> Two tablespoons of soy sauce contain approximately 1,750 mg of sodium.


## ❓ FAQ

**Q: How are nutritional totals calculated?**
Totals are calculated by normalizing all units to metric and then summing the nutritional contributions of each food item based on its quantity relative to USDA reference values.

**Q: What units are supported?**
The server supports grams (g), ounces (oz), cups, tablespoons (tbsp), and teaspoons (tsp) through automatic conversion to metric.

**Q: Can I see my Daily Value percentages?**
Yes, you can use the `calculate_daily_value_percentages` tool to determine how much each nutrient contributes to a standard 2,000 kcal daily diet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/nutrition-macro-calculator](https://vinkius.com/ai-agent-connect/nutrition-macro-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nutrition Macro Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nutrition-macro-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nutrition Macro Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nutrition-macro-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
