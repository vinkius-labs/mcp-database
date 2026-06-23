# Nutritional Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nutritional-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate total and per-serving macro and calorie content of recipes using weight-based nutritional density data.

## Description
The Nutritional Estimator MCP server allows AI agents to transform ingredient masses into precise nutritional insights. By leveraging a local database of nutrient densities (standardized per 100g), the tool can aggregate the total calories, proteins, fats, carbohydrates, and fiber for an entire recipe batch or a single serving. Use `search_ingredients` to find items in the registry, `get_ingredient_details` to inspect specific nutritional profiles, and `compute_recipe_nutrition` to perform complex scaling calculations based on provided weights.


## Available Tools (3)
- **compute_recipe_nutrition**: Calculate total and per-serving nutrition for a recipe
- **get_ingredient_details**: Get nutritional details for an ingredient
- **search_ingredients**: Returns a list of matches.

Search for ingredients in the database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nutritional Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me some ingredients that contain 'apple'."

**🤖 AI Agent:**
> I found the following matches: Apple (ID: apple_01), Green Apple (ID: green_apple_02), and Apple Juice (ID: apple_juice_03).

---

**👤 You:**
> "What are the nutritional details for ingredient 'chicken_breast'?"

**🤖 AI Agent:**
> For 100g of chicken breast, the nutrition profile is: 165 calories, 31g protein, 3.6g fat, 0g carbs, and 0g fiber.

---

**👤 You:**
> "Calculate the nutrition for a recipe with 200g of chicken_breast and 100g of rice, serving 2 people."

**🤖 AI Agent:**
> The total recipe contains 430 calories, 65g protein, 7.2g fat, and 78g carbs. Each of the 2 servings provides 215 calories, 32.5g protein, 3.6g fat, and 39g carbs.


## ❓ FAQ

**Q: How does the nutritional calculation work?**
The system uses a 100g reference standard. It scales the nutrient values of each ingredient by its weight in grams relative to that 100g base, then sums all contributions for the total recipe and divides by the number of servings for per-portion data.

**Q: Can I search for ingredients by partial names?**
Yes, the `search_ingredients` tool performs a case-insensitive search that matches any part of the ingredient name in the local database.

**Q: What happens if an ingredient ID is not found?**
If you provide an invalid or non-existent ID to `get_ingredient_details` or `compute_recipe_nutrition`, the tool will return a failure status with a descriptive error message.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nutritional-estimator](https://vinkius.com/mcp/nutritional-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nutritional Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nutritional-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nutritional Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nutritional-estimator": {
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
