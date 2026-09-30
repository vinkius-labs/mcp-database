# Meal Plan Budget Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meal-plan-budget-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize your weekly meal plan by balancing budget, nutrition, and personal preferences.

## Description
This MCP server acts as a specialized optimization engine for meal planning. It connects your AI assistant to a sophisticated logic layer that selects the best possible meals from a catalog based on your specific constraints. By using `get_meal_catalog`, you can explore available options. The `calculate_optimized_plan` tool finds the ideal combination of meals that maximizes your preference scores while strictly adhering to your `weeklyBudget` and nutritional targets. You can also use `validate_plan_viability` to check if a specific selection is feasible, or `simulate_leftover_impact` to see how much you can save by utilizing leftovers from previous meals.


## Available Tools (4)
- **calculate_optimized_plan**: Generates the most preferred meal plan that fits within the user's budget and nutritional constraints
- **get_meal_catalog**: You can filter by category.

Retrieves the complete list of available meal options and their attributes
- **simulate_leftover_impact**: Estimates how many meals in a plan can be replaced by leftovers from previously selected meals
- **validate_plan_viability**: Checks if a specific set of meal IDs can form a valid, complete weekly plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meal Plan Budget Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me a meal plan for the week with a budget of $150, requiring 7 breakfasts, 7 lunches, and 7 dinners, with at least 2000 calories and 80g of protein per day."

**🤖 AI Agent:**
> I have generated an optimized plan for you. The total cost is $142.50, meeting your $150 budget. The plan provides 2150 calories and 85g of protein daily, and includes 3 meals that provide leftovers for future days.

---

**👤 You:**
> "What breakfast options are available in the catalog?"

**🤖 AI Agent:**
> The available breakfast options include Oatmeal with Berries, Avocado Toast, and Greek Yogurt Parfait.

---

**👤 You:**
> "Is this meal plan valid: meal_001, meal_005, meal_012 with a budget of $50 and 7 meals per category?"

**🤖 AI Agent:**
> No, this plan is not valid because the total cost of $55 exceeds your $50 budget.


## ❓ FAQ

**Q: How does the optimizer handle my budget?**
The `calculate_optimized_plan` tool ensures that the total cost of all selected meals, including the impact of leftovers, never exceeds the `weeklyBudget` you provide.

**Q: Can I filter meals by category?**
Yes, you can use the `get_meal_catalog` tool and provide a specific category like 'breakfast' to see only relevant meal options.

**Q: What are leftovers in this system?**
Some meals generate leftovers that can be used for future meals in your plan. You can use `simulate_leftover_impact` to see how these leftovers reduce your total cost and nutritional needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/meal-plan-budget-optimizer](https://vinkius.com/en/ai-agent-connect/meal-plan-budget-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meal Plan Budget Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meal-plan-budget-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meal Plan Budget Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meal-plan-budget-optimizer": {
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
