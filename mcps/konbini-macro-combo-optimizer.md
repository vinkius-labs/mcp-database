# Konbini Macro Combo Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/konbini-macro-combo-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Optimize Japanese convenience store meals to hit specific calorie and protein targets.

## Description
This MCP server provides a deterministic optimization engine for planning meals from Japanese convenience stores like 7-Eleven, Lawson, and FamilyMart. By using the `find_optimal_meal_combo` tool, you can input specific caloric and protein goals to receive the best combination of up to four items. You can also use `search_available_items` to browse the product catalog or `get_item_nutrition_details` to inspect the macro profile of individual products. The optimizer calculates total calories, protein, carbs, fat, and cost in JPY, ensuring the selection stays within a 15% tolerance of your targets.


## Available Tools (3)
- **find_optimal_meal_combo**: Finds the best combination of up to 4 items to meet target calories and protein
- **get_item_nutrition_details**: Get detailed nutritional information for a specific item
- **search_available_items**: Browse the catalog of available convenience store items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Konbini Macro Combo Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to eat around 500 calories and get 30g of protein from a konbini. What should I pick?"

**🤖 AI Agent:**
> Your optimal meal is: 1x Chicken Bento (600kcal, 25g protein) and 1x Protein Drink (150kcal, 15g protein). Total: 750kcal, 40g protein. Note: This is outside the 15% tolerance for your 500kcal target.

---

**👤 You:**
> "Find me a snack combo near 200 calories and 10g of protein."

**🤖 AI Agent:**
> Your optimal snack is: 1x Salmon Onigiri (180kcal, 7g protein) and 1x Boiled Egg (70kcal, 6g protein). Total: 250kcal, 13g protein.

---

**👤 You:**
> "What items are available in the onigiri category?"

**🤖 AI Agent:**
> The available onigiri items are: Salmon Onigiri, Tuna Mayo Onigiri, and Pickled Plum Onigiri.


## ❓ FAQ

**Q: How many items can be in a meal combo?**
A single meal combo is limited to a maximum of four items to maintain the nature of a single meal or snack.

**Q: What happens if a combination doesn't meet my targets?**
The optimizer will still provide the best mathematical match, but it will flag the result if the totals fall outside a 15% tolerance window of your requested calories or protein.

**Q: Can I see the full nutrition facts for a specific item?**
Yes, you can use the `get_item_nutrition_details` tool to retrieve the full macro profile, including calories, protein, carbs, fat, and cost for any item in the catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/konbini-macro-combo-optimizer](https://vinkius.com/ai-agent-connect/konbini-macro-combo-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Konbini Macro Combo Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `konbini-macro-combo-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Konbini Macro Combo Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "konbini-macro-combo-optimizer": {
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
