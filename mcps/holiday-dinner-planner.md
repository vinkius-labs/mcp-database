# Holiday Dinner Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/holiday-dinner-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform guest lists and recipes into complete cooking schedules, shopping lists, and budget estimates.

## Description
The Holiday Dinner Planner is a comprehensive planning engine designed to handle the logistics of hosting a large meal. By connecting your recipes and guest counts to AI agents via Vinkius Edge, you can automatically generate precise ingredient quantities, chronological cooking timelines, and consolidated shopping lists. Use `plan_menu_quantities` to scale ingredients for any number of guests, `generate_cooking_timeline` to work backward from your target serving time, and `calculate_table_settings` to ensure you have enough plates and cutlery for a formal or casual setting. It even provides a full budget overview to keep your holiday planning on track.


## Available Tools (5)
- **calculate_table_settings**: Determines the inventory of physical items needed for the dining arrangement
- **plan_menu_quantities**: Calculates the total amount of each ingredient needed to serve the entire guest list based on provided recipes
- **create_shopping_list**: Generates a consolidated and categorized list of items to purchase
- **estimate_total_budget**: Provides a high-level financial overview of the planned dinner
- **generate_cooking_timeline**: Creates a chronological schedule of tasks to ensure the meal is ready at the desired time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Holiday Dinner Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 12 guests and a recipe for Roast Turkey that serves 8. How much turkey and seasoning do I need?"

**🤖 AI Agent:**
> To serve 12 guests, you will need 1.5 times the original recipe quantities. This includes 15kg of turkey and 45g of seasoning.

---

**👤 You:**
> "What items do I need to buy for a formal dinner for 6 people?"

**🤖 AI Agent:**
> For a formal dinner for 6, you will need 6 plates, 6 dessert spoons, 6 forks, 6 knives, 6 spoons, and 12 pieces of glassware.

---

**👤 You:**
> "I want to serve dinner at 7:00 PM. When should I start preparing my recipes?"

**🤖 AI Agent:**
> Based on your recipes, you should begin preparation at 3:30 PM to account for all cooking and resting durations before the 7:00 PM serving time.


## ❓ FAQ

**Q: How does the tool handle ingredient scaling?**
The `plan_menu_quantities` tool scales all ingredients proportionally based on your total guest count relative to the original recipe servings.

**Q: Can I plan for different dining styles?**
Yes, using `calculate_table_settings`, you can specify either a 'formal' or 'casual' style to determine the required inventory of plates, cutlery, and glassware.

**Q: How do I ensure my food is ready on time?**
You can use `generate_cooking_timeline` by providing your target serving time. The tool calculates a backward schedule including prep, cooking, and resting times.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/holiday-dinner-planner](https://vinkius.com/en/ai-agent-connect/holiday-dinner-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Holiday Dinner Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `holiday-dinner-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Holiday Dinner Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "holiday-dinner-planner": {
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
