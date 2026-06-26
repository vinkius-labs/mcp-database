# Batch Cooking Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/batch-cooking-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Consolidate ingredients from multiple recipes into a single, organized shopping list.

## Description
The Batch Cooking Planner is an essential tool for meal prepping. It allows you to select multiple recipes and specify the number of servings for each, then automatically aggregates all ingredients into a single shopping list. The system handles scaling quantities based on your target portions and organizes everything by food category like Proteins, Vegetables, and Dairy. Use `generate_shopping_list` to merge items and `scale_recipe` to see individual ingredient adjustments.


## Available Tools (3)
- **scale_recipe**: Scale a recipe to a target number of servings
- **generate_shopping_list**: Generate a consolidated shopping list from multiple recipes
- **get_category_counts**: ).

Get the count of unique ingredients in each food category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Batch Cooking Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to cook 10 portions of recipe 'beef-stew' and 5 portions of 'chicken-salad'. What is my shopping list?"

**🤖 AI Agent:**
> Your consolidated shopping list includes: Proteins: Beef (500g), Chicken (250g); Vegetables: Carrots (3 units), Lettuce (1 head); Dairy: Butter (20g).

---

**👤 You:**
> "How many ingredients are in the Protein category?"

**🤖 AI Agent:**
> There are currently 12 unique ingredients registered under the Protein category.

---

**👤 You:**
> "Scale the 'pasta-carbonara' recipe for 4 people."

**🤖 AI Agent:**
> For 4 portions of pasta-carbonara, you will need: Pasta (400g), Eggs (4 units), Pancetta (150g), Pecorino Romano (50g).


## ❓ FAQ

**Q: How does the consolidation process work?**
The `generate_shopping_list` tool takes your recipe selections and sums quantities for ingredients that have both the same name and the same unit of measurement.

**Q: Can I scale a single recipe without merging it with others?**
Yes, you can use the `scale_recipe` tool to see exactly how much of each ingredient you need for a specific number of portions.

**Q: How are ingredients categorized?**
Ingredients are automatically grouped into categories such as Proteins, Vegetables, Dairy, Pantry, and Fruit to make your shopping trip more efficient.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/batch-cooking-planner](https://vinkius.com/mcp/batch-cooking-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Batch Cooking Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `batch-cooking-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Batch Cooking Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "batch-cooking-planner": {
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
