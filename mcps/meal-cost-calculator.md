# Meal Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meal-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total recipe expenses and individual serving costs based on ingredient unit prices.

## Description
The Meal Cost Calculator MCP connects your AI agent to precise culinary costing logic. Use `calculate_recipe_total` to find the total expense of a recipe by summing ingredient costs, `calculate_serving_split` to determine the cost per portion, and `get_cost_contribution_breakdown` to identify which ingredients are driving your expenses. It also includes `validate_measurement_units` to ensure all measurements (mass, volume, or discrete) are consistent across your recipe list.


## Available Tools (4)
- **get_cost_contribution_breakdown**: Shows which ingredients drive the cost
- **calculate_recipe_total**: Calculates the total cost of a recipe
- **calculate_serving_split**: Calculates the cost per individual serving
- **validate_measurement_units**: Validates measurement units consistency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meal Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for a recipe using 2kg of flour at $1.50/kg and 500g of sugar at $2.00/kg?"

**🤖 AI Agent:**
> $6.00

---

**👤 You:**
> "If my total recipe cost is $20 and it serves 5 people, how much does each serving cost?"

**🤖 AI Agent:**
> $4.00

---

**👤 You:**
> "Which ingredients are driving the cost in a recipe with 1kg of beef at $15/kg and 0.2kg of salt at $0.50/kg?"

**🤖 AI Agent:**
> Beef: 96.77%, Salt: 3.23%


## ❓ FAQ

**Q: How do I calculate the total cost of my recipe?**
Use the `calculate_recipe_total` tool. Provide a JSON array of ingredients, each containing its name, unit price, and the quantity used.

**Q: Can I see which ingredient is most expensive?**
Yes, use the `get_cost_contribution_breakdown` tool. It will return a list showing the percentage of the total cost contributed by each ingredient.

**Q: How do I find out the cost per serving?**
First, calculate the total recipe cost using `calculate_recipe_total`, then pass that result into the `calculate_serving_split` tool along with the number of portions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meal-cost-calculator](https://vinkius.com/mcp/meal-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meal Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meal-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meal Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meal-cost-calculator": {
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
