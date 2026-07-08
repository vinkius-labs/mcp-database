# Non-linear Ingredient Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/non-linear-ingredient-adjuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [baking](../categories/baking.md)

Scale baking recipes using non-linear rules for leavening, fats, and seasonings.

## Description
The Non-linear Ingredient Adjuster is a specialized culinary engine designed to handle the complex chemistry of scaling recipes. Unlike simple multiplication, this tool applies non-linear adjustments for critical categories: leavening agents are capped to prevent collapse, salt and spices are scaled at 75% to avoid overpowering flavors, and fats are adjusted to maintain texture. Use `scale_ingredients` to transform your base recipe into any size while preserving structural integrity.


## Available Tools (3)
- **get_scaling_multipliers**: Preview scaling multipliers
- **scale_ingredients**: Scale ingredients non-linearly
- **validate_recipe_input**: Validate a recipe ingredient list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Non-linear Ingredient Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to triple my cookie recipe. Here are the ingredients: [{'name': 'baking soda', 'amount': 1, 'unit': 'tsp', 'category': 'leavening'}, {'name': 'salt', 'amount': 0.5, 'unit': 'tsp', 'category': 'salt'}]. What will the new amounts be?"

**🤖 AI Agent:**
> For a 3x scale, your adjusted ingredients are: baking soda: 1.5 tsp (capped), salt: 1.125 tsp.

---

**👤 You:**
> "Check the scaling multipliers for a scale factor of 4."

**🤖 AI Agent:**
> For a scale factor of 4, the effective multipliers are: leavening: 1.5x, salt/spices: 3x, fat: 0.8x.

---

**👤 You:**
> "Is this ingredient list valid? [{'name': 'flour', 'amount': 500, 'unit': 'g', 'category': 'dry'}]"

**🤖 AI Agent:**
> Yes, the ingredient list is valid and uses a supported category.


## ❓ FAQ

**Q: How does the scaling logic work for leavening agents?**
To prevent structural failure, when the scale factor exceeds 2x, the multiplier for leavening agents like baking powder or yeast is capped at a specific limit.

**Q: Can I check multipliers before scaling my whole recipe?**
Yes, you can use the `get_scaling_multipliers` tool to preview exactly how much each category (salt, fat, leavening) will be adjusted for a specific scale factor.

**Q: Does the tool validate my ingredient list?**
Yes, the `validate_recipe_input` tool checks that all ingredients have valid names, amounts, units, and belong to supported categories like 'leavening', 'salt', or 'fat'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/non-linear-ingredient-adjuster](https://vinkius.com/mcp/non-linear-ingredient-adjuster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Non-linear Ingredient Adjuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `non-linear-ingredient-adjuster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Non-linear Ingredient Adjuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "non-linear-ingredient-adjuster": {
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
