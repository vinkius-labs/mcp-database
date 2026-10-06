# Pantry Expiry & Use-First Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pantry-expiry-use-first-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Prioritize food usage to minimize waste with smart meal planning.

## Description
This MCP server helps you manage food waste by generating prioritized meal plans. It analyzes your inventory to identify items nearing expiration, especially those already opened, and schedules them into your planned meals. Use `generate_usage_plan` to create a daily schedule, `calculate_inventory_urgency` to see which items need immediate use, or `validate_plan_feasibility` to ensure you have enough ingredients for your upcoming meals.


## Available Tools (4)
- **get_item_availability**: Determines how many servings are remaining for a specific item
- **calculate_inventory_urgency**: Evaluates how critical it is to use specific items based on their current state
- **generate_usage_plan**: Generates a day-by-day meal schedule that utilizes inventory items in the most efficient order to prevent expiration
- **validate_plan_feasibility**: Checks if a proposed meal plan can actually be completed with the current inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pantry Expiry & Use-First Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a meal plan for tomorrow based on my inventory."

**🤖 AI Agent:**
> Your meal plan for tomorrow is: Breakfast: Oats with milk; Lunch: Chicken salad; Dinner: Pasta with tomato sauce.

---

**👤 You:**
> "How many servings of milk do I have left?"

**🤖 AI Agent:**
> You have 4 servings of milk remaining.

---

**👤 You:**
> "Is my plan to have steak and potatoes for dinner feasible?"

**🤖 AI Agent:**
> No, you are missing: steak.


## ❓ FAQ

**Q: How does the tool prioritize which food to use?**
The system prioritizes items that are already opened and those with the closest expiration dates using the `calculate_inventory_urgency` logic.

**Q: Can I check if I have enough food for my weekly plan?**
Yes, you can use the `validate_plan_feasibility` tool to check if your proposed meal plan can be completed with your current inventory.

**Q: How do I know which items are most urgent?**
You can run `calculate_inventory_urgency` to receive a list of items with urgency scores based on their expiry proximity and open status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pantry-expiry-use-first-planner](https://vinkius.com/en/ai-agent-connect/pantry-expiry-use-first-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pantry Expiry & Use-First Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pantry-expiry-use-first-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pantry Expiry & Use-First Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pantry-expiry-use-first-planner": {
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
