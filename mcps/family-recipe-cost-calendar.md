# Family Recipe Cost Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-recipe-cost-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate meal costs, shopping lists, and ingredient waste for your weekly meal plan.

## Description
Connect your meal planning to precise financial tracking. This MCP server allows AI agents to calculate the exact cost of your planned meals by reconciling recipe requirements against package pricing and leftover credits. Use `get_meal_plan_summary` for a high-level overview of costs, `calculate_daily_meal_cost` to find the price of a specific meal, `get_shopping_list_and_cost` to generate a purchase list, or `analyze_leftover_efficiency` to minimize food waste.


## Available Tools (4)
- **calculate_daily_meal_cost**: Calculates the specific cost of a single meal on a given day
- **get_meal_plan_summary**: Provides a high-level overview of the planned meal schedule and total projected costs
- **get_shopping_list_and_cost**: Identifies exactly which packages must be purchased to fulfill the meal plan
- **analyze_leftover_efficiency**: Evaluates how well the meal plan utilizes purchased ingredients to minimize waste


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Recipe Cost Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of my meal plan from 2024-05-01 to 2024-05-07."

**🤖 AI Agent:**
> Your meal plan summary for May 1st to May 7th shows a total shopping subtotal of $85.50 and an average cost per person of $4.25. The daily breakdown includes Monday's Spaghetti at $12.00 and Tuesday's Tacos at $15.00.

---

**👤 You:**
> "How much will the meal on 2024-05-03 cost?"

**🤖 AI Agent:**
> The meal planned for 2024-05-03 is Chicken Curry, which will cost $18.50 for 4 servings, resulting in $4.63 per person.

---

**👤 You:**
> "What is my shopping list for the period 2024-05-01 to 2024-05-07?"

**🤖 AI Agent:**
> To complete your plan, you need to buy: 1x Pasta (2.00), 1x Tomato Sauce (3.50), and 1x Chicken Breast (12.00). The final subtotal after discounts is $15.50.


## ❓ FAQ

**Q: How does the tool handle ingredient leftovers?**
The tool uses leftover credit to reduce the cost of future meals. If a package contains more than a recipe requires, the unused portion is credited to the next meal using that same ingredient.

**Q: Can I see my total shopping cost for the week?**
Yes, you can use `get_shopping_list_and_cost` to see exactly which packages you need to buy and the final subtotal after discounts.

**Q: How is the cost per person calculated?**
The cost per person is the daily meal cost divided by the number of people eating that specific meal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-recipe-cost-calendar](https://vinkius.com/en/ai-agent-connect/family-recipe-cost-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Recipe Cost Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-recipe-cost-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Recipe Cost Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-recipe-cost-calendar": {
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
