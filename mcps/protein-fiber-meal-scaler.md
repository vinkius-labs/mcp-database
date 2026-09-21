# Protein & Fiber Meal Scaler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/protein-fiber-meal-scaler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nutrition](../categories/nutrition.md)

Scales recipes to specific servings or target protein and fiber amounts.

## Description
This MCP server provides precise nutritional arithmetic for meal planning. It allows AI agents to adjust recipe quantities to meet specific serving sizes or hit exact protein and fiber targets. Using tools like `scale_recipe_by_servings` and `scale_recipe_by_nutrient`, agents can recalculate ingredient masses while maintaining original nutritional ratios. It also includes `get_nutrient_contributions` to analyze ingredient impact and `suggest_substitutions` to swap ingredients while preserving dietary constraints.


## Available Tools (4)
- **get_nutrient_contributions**: Analyzes a recipe to show how much each ingredient contributes to the total protein and fiber
- **scale_recipe_by_nutrient**: Adjusts a recipe's quantities to hit a specific total target for either protein or fiber
- **scale_recipe_by_servings**: Adjusts a recipe to a specific number of servings while maintaining the original ingredient proportions
- **suggest_substitutions**: Recommends an alternative ingredient to replace one in a recipe while attempting to keep the target nutrient and total mass stable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Protein & Fiber Meal Scaler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scale this recipe for 4 servings: 200g Chicken (protein: 0.3, fiber: 0.0), 100g Rice (protein: 0.02, fiber: 0.03). Original servings: 2."

**🤖 AI Agent:**
> To serve 4 people, use 400g of Chicken and 200g of Rice.

---

**👤 You:**
> "I need 50g of protein. Scale this: 100g Tofu (protein: 0.08, fiber: 0.01), 50g Spinach (protein: 0.02, fiber: 0.02). Original servings: 1."

**🤖 AI Agent:**
> To reach 50g of protein, the scaled ingredients are 500g of Tofu and 250g of Spinach.

---

**👤 You:**
> "What is the protein contribution of 100g Chicken (protein: 0.3) and 100g Broccoli (protein: 0.2) in this recipe?"

**🤖 AI Agent:**
> The Chicken contributes 60% of the total protein, and the Broccoli contributes 40%.


## ❓ FAQ

**Q: How do I scale a recipe for more people?**
Use the `scale_recipe_by_servings` tool. Provide the original ingredients, the original serving count, and your desired target servings.

**Q: Can I target a specific amount of protein?**
Yes. The `scale_recipe_by_nutrient` tool allows you to specify a target amount for either protein or fiber to adjust the recipe quantities accordingly.

**Q: How does the substitution tool work?**
The `suggest_substitutions` tool calculates a new ingredient mass to help maintain your target nutrient levels when swapping ingredients.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/protein-fiber-meal-scaler](https://vinkius.com/en/ai-agent-connect/protein-fiber-meal-scaler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Protein & Fiber Meal Scaler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `protein-fiber-meal-scaler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Protein & Fiber Meal Scaler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "protein-fiber-meal-scaler": {
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
