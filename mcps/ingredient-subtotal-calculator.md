# Ingredient Subtotal Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ingredient-subtotal-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise ingredient costs and recipe totals.

## Description
This MCP server provides specialized tools for culinary cost management. It allows AI agents to retrieve individual ingredient prices using `get_ingredient_price`, calculate specific costs with `calculate_ingredient_subtotal`, and determine the full cost of a recipe via `sum_recipe_total`. You can also use `validate_ingredient_list` to verify ingredient availability before processing.


## Available Tools (4)
- **calculate_ingredient_subtotal**: Calculates the cost for a specific quantity of one ingredient
- **get_ingredient_price**: Retrieves the cost of a specific ingredient
- **sum_recipe_total**: The ingredients parameter should be a JSON string representing an array of objects with ingredientName and quantity.

Calculates the total cost for a list of multiple ingredients
- **validate_ingredient_list**: Checks if a list of ingredients can be successfully priced


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ingredient Subtotal Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does 500 grams of flour cost?"

**🤖 AI Agent:**
> 500 grams of flour costs $0.50.

---

**👤 You:**
> "What is the total cost for 2 eggs and 100g of sugar?"

**🤖 AI Agent:**
> The total cost for 2 eggs and 100g of sugar is $0.85.

---

**👤 You:**
> "Check if salt, pepper, and saffron are available."

**🤖 AI Agent:**
> Yes, all requested ingredients are available in the catalog.


## ❓ FAQ

**Q: How do I calculate the total cost of a recipe?**
You can use the `sum_recipe_total` tool by providing a list of ingredients and their respective quantities.

**Q: Can I check if an ingredient is available in the catalog?**
Yes, use the `validate_ingredient_list` tool to check if all ingredients in your list exist in the database.

**Q: What happens if an ingredient is not found?**
If an ingredient is missing from the catalog, the tools will return an error indicating the specific missing item.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ingredient-subtotal-calculator](https://vinkius.com/en/ai-agent-connect/ingredient-subtotal-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ingredient Subtotal Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ingredient-subtotal-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ingredient Subtotal Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ingredient-subtotal-calculator": {
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
