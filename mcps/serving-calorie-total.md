# Serving Calorie Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serving-calorie-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates total caloric content for recipe servings.

## Description
This MCP server provides precise tools to determine the caloric content of food. It can retrieve ingredient densities using `get_ingredient_density`, calculate specific ingredient contributions with `calculate_ingredient_contribution`, list recipe components via `get_recipe_ingredient_list`, and aggregate everything to find the final sum using `calculate_total_serving_calories`.


## Available Tools (4)
- **calculate_ingredient_contribution**: Calculates how many calories a specific amount of an ingredient contributes
- **calculate_total_serving_calories**: Aggregates all ingredient contributions to find the total calories for a single serving
- **get_ingredient_density**: Retrieves the caloric density of a specific ingredient
- **get_recipe_ingredient_list**: Retrieves a list of all ingredients required for a specific recipe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serving Calorie Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the total calories in recipe ID 'pancake_001'?"

**🤖 AI Agent:**
> The total calories for recipe pancake_001 is 450 kcal.

---

**👤 You:**
> "How many calories does 50g of sugar contribute?"

**🤖 AI Agent:**
> 50g of sugar contributes 196 calories.

---

**👤 You:**
> "List all ingredients for recipe 'omelette_v2'."

**🤖 AI Agent:**
> The ingredients for omelette_v2 are: 2 eggs, 10g butter, and 5g salt.


## ❓ FAQ

**Q: How do I calculate the total calories for a recipe?**
You can use the `calculate_total_serving_calories` tool by providing the specific recipe ID.

**Q: Can I check the density of a single ingredient?**
Yes, use the `get_ingredient_density` tool to find the calories per unit for any supported ingredient.

**Q: What happens if an ingredient is not in the catalog?**
The tool will return an error if the ingredient name is unknown or missing from the registry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serving-calorie-total](https://vinkius.com/en/ai-agent-connect/serving-calorie-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serving Calorie Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serving-calorie-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serving Calorie Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serving-calorie-total": {
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
