# Family Meal Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-meal-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates a seven-day meal schedule optimized for budget, dietary needs, and household availability.

## Description
This MCP server acts as a planning engine that generates a complete seven-day meal calendar. It optimizes recipe selection against specific household constraints such as food budget, dietary requirements, and available time windows. Use `get_meal_plan` to create a full weekly schedule, `validate_recipe_compliance` to check dietary restrictions, `calculate_weekly_cost` to manage spending, and `check_schedule_availability` to ensure prep blocks fit your schedule.


## Available Tools (4)
- **calculate_weekly_cost**: Determines the total cost of a proposed set of meals
- **check_schedule_availability**: Verifies if the required meal preparation can be fit into the household's free time
- **get_meal_plan**: Generates a full seven-day meal calendar based on all provided constraints
- **validate_recipe_compliance**: Checks if a specific recipe is compatible with the household's dietary restrictions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Meal Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 7-day meal plan for a budget of $150, including vegan recipes and a household schedule for weekday evenings."

**🤖 AI Agent:**
> Here is your 7-day vegan meal plan within the $150 budget: Monday: Lentil Stew, Tuesday: Chickpea Curry, Wednesday: Quinoa Salad, Thursday: Tofu Stir-fry, Friday: Vegetable Pasta, Saturday: Bean Tacos, Sunday: Roasted Veggie Bowl.

---

**👤 You:**
> "Check if a recipe with peanuts is compliant with a nut-free dietary constraint."

**🤖 AI Agent:**
> No, the recipe is not compliant because it contains peanuts, which violates the nut-free constraint.

---

**👤 You:**
> "What is the total cost for these three recipes: Beef Stew, Chicken Salad, and Pasta?"

**🤖 AI Agent:**
> The total cost for the selected recipes is $45.50.


## ❓ FAQ

**Q: How does the budget constraint work?**
The engine ensures the sum of all unique ingredient costs for the selected recipes does not exceed your specified budget.

**Q: Can I use leftovers to save money?**
Yes, if you enable the leftover option in `get_meal_plan`, the engine will prioritize recipes that can be used for subsequent meals to reduce costs and prep time.

**Q: How are dietary restrictions handled?**
You can use `validate_recipe_compliance` to check individual recipes or include constraints in `get_meal_plan` to ensure all selected meals meet your needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-meal-calendar](https://vinkius.com/en/ai-agent-connect/family-meal-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Meal Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-meal-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Meal Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-meal-calendar": {
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
