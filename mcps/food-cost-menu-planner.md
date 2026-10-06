# Food Cost & Menu Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/food-cost-menu-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise ingredient costs, target menu prices, and profitability margins.

## Description
This MCP server provides essential financial tools for restaurant operators to manage profitability. Use `calculate_item_cost` to determine the total cost of a dish based on its ingredients, or `get_ingredient_yield_adjusted_cost` to account for preparation waste. You can also use `calculate_target_price` to find the ideal selling price for a specific margin, and `analyze_menu_profitability` to evaluate how current prices impact your contribution margin.


## Available Tools (4)
- **calculate_item_cost**: Determines the total cost to produce a single serving of a menu item based on its constituent ingredients
- **calculate_target_price**: g., 0.30 for 30%).

Calculates what a menu item should be priced at to hit a specific profit goal
- **get_ingredient_yield_adjusted_cost**: g., 0.85 for 85%).

Calculates the "true cost" of an ingredient by accounting for the weight lost during preparation
- **analyze_menu_profitability**: Evaluates the profitability profile of a menu item, comparing current pricing against margins


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Food Cost & Menu Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for a burger using 0.2kg of beef at $15/kg and 0.05kg of cheese at $20/kg?"

**🤖 AI Agent:**
> The total cost for the burger is $4.00.

---

**👤 You:**
> "If a steak costs $12.00 to make, what should I charge to maintain a 30% food cost?"

**🤖 AI Agent:**
> To maintain a 30% food cost, the suggested price is $40.00.

---

**👤 You:**
> "Analyze the profitability of a pasta dish that costs $5.00 and sells for $15.00."

**🤖 AI Agent:**
> The pasta dish has a food cost percentage of 33.33% and a contribution margin of $10.00.


## ❓ FAQ

**Q: How do I calculate the cost of a specific dish?**
Use the `calculate_item_cost` tool by providing a list of ingredient IDs and the quantities used in the recipe.

**Q: Can I account for ingredient waste?**
Yes, use `get_ingredient_yield_adjusted_cost` to calculate the effective cost of an ingredient after accounting for its yield percentage.

**Q: How can I set a profitable price for a new menu item?**
Use `calculate_target_price` to determine the suggested selling price based on your desired food cost percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/food-cost-menu-planner](https://vinkius.com/en/ai-agent-connect/food-cost-menu-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Food Cost & Menu Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `food-cost-menu-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Food Cost & Menu Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "food-cost-menu-planner": {
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
