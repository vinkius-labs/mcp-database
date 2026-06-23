# Crafting Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crafting-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Analyze production costs, profit margins, and optimal ingredient sourcing strategies.

## Description
The Crafting Cost Calculator is an economic analysis tool designed to maximize profitability in crafting-based gameplay. By connecting your AI agent to real-time ingredient costs and market prices, it provides actionable insights through tools like `get_recipe_cost_analysis` for profit margin calculation, `optimize_ingredient_sourcing` for finding the cheapest mix of farming and buying, and `estimate_level_up_effort` to plan professional progression. It bridges the gap between raw data and strategic decision-making.


## Available Tools (3)
- **estimate_level_up_effort**: Calculate production volume required to reach a specific profession level
- **get_recipe_cost_analysis**: Calculate production cost and potential profit for a recipe
- **optimize_ingredient_sourcing**: Identify the most cost-effective way to acquire ingredients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crafting Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it profitable to craft 'Iron Sword' if the market price is 500 gold?"

**🤖 AI Agent:**
> The total production cost for an Iron Sword is 420 gold, resulting in a profit of 80 gold and a margin of 16%. It is currently profitable.

---

**👤 You:**
> "What is the best way to source ingredients for 'Health Potion'?"

**🤖 AI Agent:**
> The optimal strategy for Health Potion is a hybrid approach: farm Herbs and buy Glass Bottles to minimize your total cost to 15 gold.

---

**👤 You:**
> "How many 'Steel Plate' crafts do I need to reach level 20 from level 15?"

**🤖 AI Agent:**
> You will need to perform 45 more crafts of Steel Plate, which is estimated to take approximately 135 minutes.


## ❓ FAQ

**Q: How does the profit analysis work?**
Using `get_recipe_cost_analysis`, the tool compares the current market price you provide against the total cost of all ingredients, calculating your exact profit or loss and margin percentage.

**Q: Can I find the cheapest way to get materials?**
Yes. The `optimize_ingredient_sourcing` tool evaluates whether it is cheaper to farm or buy each ingredient in a recipe, providing you with the most cost-effective strategy.

**Q: How do I plan my profession leveling?**
The `estimate_level_up_effort` tool calculates exactly how many crafts you need to perform and the total time required to reach your target professional level based on experience gain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crafting-cost-calculator](https://vinkius.com/mcp/crafting-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crafting Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crafting-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crafting Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crafting-cost-calculator": {
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
