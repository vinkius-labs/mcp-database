# Pantry Expiry Meal Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pantry-expiry-meal-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Minimize food waste by generating meal plans that prioritize ingredients closest to their expiration date.

## Description
This MCP server connects your AI assistant to your kitchen inventory. It uses `query_pantry_inventory` to monitor ingredient freshness and `query_recipe_catalog` to find suitable meals. The core engine, `generate_meal_plan`, optimizes your schedule by selecting recipes that use up items nearing expiry, helping you reduce waste while meeting dietary needs. You can also use `check_ingredient_availability` to see if you have everything needed for a specific dish.


## Available Tools (4)
- **check_ingredient_availability**: Validates if a specific recipe can be made given the current pantry inventory
- **query_recipe_catalog**: Retrieves a list of available recipes and their requirements
- **generate_meal_plan**: Creates an optimized meal plan based on the user's needs and pantry state
- **query_pantry_inventory**: Retrieves the current state of the pantry to check what ingredients are available and when they expire


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pantry Expiry Meal Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a meal plan for 4 people that avoids dairy."

**🤖 AI Agent:**
> I have generated a meal plan for 4 people. You will make Spinach Pasta and Roasted Chicken. These recipes use your most urgent ingredients and respect your dairy-free requirement.

---

**👤 You:**
> "What ingredients in my pantry are expiring soon?"

**🤖 AI Agent:**
> Your Spinach and Chicken are expiring in 2 days, and your Milk expires in 3 days.

---

**👤 You:**
> "Can I make the Beef Stew recipe?"

**🤖 AI Agent:**
> Yes, you have all the necessary ingredients for the Beef Stew in your pantry.


## ❓ FAQ

**Q: How does the meal plan prioritize ingredients?**
The `generate_meal_plan` tool analyzes your pantry via `query_pantry_inventory` and selects recipes that include ingredients with the lowest number of days remaining until they expire.

**Q: Can I exclude specific ingredients from my meal plan?**
Yes. When using `generate_meal_plan`, you can provide a list of dietary exclusions to ensure no recipes containing those ingredients are selected.

**Q: How do I know if I have enough ingredients for a recipe?**
You can use the `check_ingredient_availability` tool with a specific recipe ID to receive a report on whether you can make the meal or which ingredients are missing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pantry-expiry-meal-plan](https://vinkius.com/en/ai-agent-connect/pantry-expiry-meal-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pantry Expiry Meal Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pantry-expiry-meal-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pantry Expiry Meal Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pantry-expiry-meal-plan": {
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
