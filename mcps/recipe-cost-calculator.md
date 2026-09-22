# Recipe Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recipe-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the exact cost per serving for any recipe based on ingredient unit prices.

## Description
This MCP server provides precise financial calculations for culinary production. It connects AI agents to ingredient inventory and recipe data to determine the cost of ingredients, total recipe expenses, and the final cost per serving. Use `get_ingredient_unit_cost` to check bulk prices, `calculate_ingredient_scaled_cost` for proportional usage costs, `calculate_recipe_total_cost` for full recipe totals, and `get_cost_per_serving` to find the cost of a single portion.


## Available Tools (4)
- **calculate_ingredient_scaled_cost**: Determine how much a specific amount of an ingredient costs based on its bulk purchase price
- **calculate_recipe_total_cost**: Sum the costs of all ingredients required for a complete recipe
- **get_cost_per_serving**: Provide the final financial metric for a single portion of a recipe
- **get_ingredient_unit_cost**: Retrieve the specific price for a single ingredient based on its purchasing unit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recipe Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cost per serving for recipe 'classic-pancake'?"

**🤖 AI Agent:**
> The cost per serving for the classic pancake recipe is $0.45.

---

**👤 You:**
> "How much does 500g of flour cost based on its bulk price?"

**🤖 AI Agent:**
> The cost for 500g of flour is $1.25.

---

**👤 You:**
> "What is the total cost to make the 'beef-stew' recipe?"

**🤖 AI Agent:**
> The total cost for the beef stew recipe is $18.50.


## ❓ FAQ

**Q: How does the server handle ingredient conversions?**
The server uses `calculate_ingredient_scaled_cost` to automatically convert recipe usage units (like grams) to the ingredient's bulk purchase unit (like kilograms) to ensure accurate pricing.

**Q: Can I adjust the number of servings for a recipe?**
Yes, you can use `get_cost_per_serving` with a `servingAdjustment` multiplier to calculate costs for different portion sizes.

**Q: What happens if an ingredient is missing from the inventory?**
If an ingredient is not found in the inventory, tools like `get_ingredient_unit_cost` will return an error indicating the ingredient is missing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recipe-cost-calculator](https://vinkius.com/en/ai-agent-connect/recipe-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recipe Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipe-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recipe Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipe-cost-calculator": {
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
