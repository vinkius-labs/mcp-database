# Family Breakfast Rotation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-breakfast-rotation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automated weekly breakfast scheduling based on prep time, budget, and nutrition.

## Description
This MCP server provides a complete scheduling system to manage family breakfast routines. Use `get_recipe_catalog` to browse available breakfast options, or `generate_weekly_rotation` to create an optimized plan that respects your morning time constraints, budget, and serving needs. You can also use `validate_rotation_constraints` to ensure a plan meets your strict limits and `calculate_nutrition_variety` to check the nutritional balance of your selected meals.


## Available Tools (4)
- **calculate_nutrition_variety**: Determines how well the rotation distributes food groups to ensure healthy eating
- **generate_weekly_rotation**: Creates a specific sequence of breakfasts for a set number of days
- **get_recipe_catalog**: Retrieves the list of available breakfast recipes and their base properties
- **validate_rotation_constraints**: Checks an existing rotation plan against specific user-defined thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Breakfast Rotation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 5-day breakfast rotation for 4 people with a 15-minute prep limit and a max repeat limit of 2."

**🤖 AI Agent:**
> Here is your 5-day breakfast plan: Monday: Oatmeal, Tuesday: Yogurt Parfait, Wednesday: Breakfast Burrito, Thursday: Avocado Toast, Friday: Protein Shake.

---

**👤 You:**
> "What breakfast recipes are available in the 'grain' category?"

**🤖 AI Agent:**
> The available grain-based recipes are Oatmeal, Whole Grain Toast, and Bran Muffins.

---

**👤 You:**
> "Check if this rotation plan is valid for a 20-minute time limit: {"schedule": [{"dayIndex": 0, "recipeId": "r1", "recipeName": "Pancakes", "prepTime": 25, "totalCost": 5.0}]}"

**🤖 AI Agent:**
> The rotation plan is invalid. The preparation time for Pancakes (25 minutes) exceeds your strict limit of 20 minutes.


## ❓ FAQ

**Q: How do I create a new breakfast plan?**
You can use the `generate_weekly_rotation` tool by providing the number of days, maximum prep time, number of servings, and your repeat limits.

**Q: Can I filter recipes by food type?**
Yes, use the `get_recipe_catalog` tool and provide a category like 'hot', 'cold', 'grain', or 'protein' to filter the available options.

**Q: How is the nutritional variety calculated?**
The `calculate_nutrition_variety` tool analyzes the food groups of your selected recipes to provide a diversity metric.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-breakfast-rotation](https://vinkius.com/en/ai-agent-connect/family-breakfast-rotation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Breakfast Rotation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-breakfast-rotation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Breakfast Rotation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-breakfast-rotation": {
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
