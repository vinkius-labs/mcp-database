# Recipe Leftover Transformer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recipe-leftover-transformer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Match your leftovers to recipes to minimize food waste and cost.

## Description
The Recipe Leftover Transformer connects your kitchen inventory to a smart recipe engine. By analyzing your current leftovers, including quantities and expiry dates, it identifies the best meals to cook. Use `find_recipes_by_leftovers` to see what you can make right now, `optimize_waste_reduction` to prioritize ingredients nearing their expiration, or `calculate_recipe_cost` to see the financial impact of a meal. It even helps you scale recipes for specific serving sizes.


## Available Tools (4)
- **check_ingredient_availability**: Validates if a specific ingredient is available and checks its freshness
- **find_recipes_by_leftovers**: Identifies recipes that can be made using the current inventory of leftovers
- **calculate_recipe_cost**: Determines the financial impact of preparing a specific recipe
- **optimize_waste_reduction**: Suggests the best recipe to cook to prevent food from expiring


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recipe Leftover Transformer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What can I cook with my leftovers: 2 eggs, 100g flour, and 50ml milk?"

**🤖 AI Agent:**
> You can make simple pancakes with your eggs, flour, and milk.

---

**👤 You:**
> "Which recipe should I make to use up my milk before it expires tomorrow?"

**🤖 AI Agent:**
> The best recipe to use your milk is Creamy Oatmeal.

---

**👤 You:**
> "Is my spinach still fresh?"

**🤖 AI Agent:**
> Yes, your spinach is available and has 3 days until it expires.


## ❓ FAQ

**Q: How does the tool handle ingredients that are about to expire?**
You can use `optimize_waste_reduction` to find recipes that specifically use ingredients with the closest expiry dates, helping you reduce food waste.

**Q: Can I adjust the number of servings for a recipe?**
Yes, when using `find_recipes_by_leftovers` or `calculate_recipe_cost`, you can provide a target number of servings to scale the ingredient quantities automatically.

**Q: How much will it cost to make a recipe?**
The `calculate_recipe_cost` tool provides a summary of the additional purchase cost for any ingredients you don't currently have in your leftovers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recipe-leftover-transformer](https://vinkius.com/en/ai-agent-connect/recipe-leftover-transformer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recipe Leftover Transformer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipe-leftover-transformer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recipe Leftover Transformer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipe-leftover-transformer": {
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
