# Pantry Meal Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pantry-meal-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan meals based on your current pantry inventory and ingredient substitutions.

## Description
Pantry Meal Builder connects your AI assistant to your kitchen inventory. Use `find_feasible_meals` to discover recipes you can cook right now with what you have, or `calculate_scaled_requirements` to adjust ingredient amounts for a specific number of guests. It also supports ingredient swaps via `check_substitution_validity` and provides a categorized view of your stock using `get_pantry_summary`.


## Available Tools (4)
- **get_pantry_summary**: Provides an overview of what is currently available in the pantry, organized by category
- **calculate_scaled_requirements**: Determines the exact quantities of ingredients needed for a specific number of servings
- **check_substitution_validity**: Determines if a specific ingredient can be replaced by another
- **find_feasible_meals**: Identifies which recipes can be cooked given the current pantry contents and allowed substitutions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pantry Meal Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What meals can I make with flour, eggs, and milk?"

**🤖 AI Agent:**
> You can make Pancakes or Crepes with your current ingredients.

---

**👤 You:**
> "How much flour do I need for a recipe serving 6 people?"

**🤖 AI Agent:**
> You will need 450 grams of flour for 6 servings.

---

**👤 You:**
> "Can I use honey instead of sugar in this recipe?"

**🤖 AI Agent:**
> Yes, honey is a valid substitute for sugar in this recipe.


## ❓ FAQ

**Q: How do I know if a recipe is cookable?**
You can use `find_feasible_meals` to check which recipes match your current pantry items and any allowed substitutions.

**Q: Can I adjust recipes for more people?**
Yes, use `calculate_scaled_requirements` to get the exact quantities needed for your target number of servings.

**Q: How do I see what ingredients I have left?**
The `get_pantry_summary` tool provides a categorized overview of your available ingredients.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pantry-meal-builder](https://vinkius.com/en/ai-agent-connect/pantry-meal-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pantry Meal Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pantry-meal-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pantry Meal Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pantry-meal-builder": {
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
