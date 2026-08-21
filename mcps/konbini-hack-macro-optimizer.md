# Konbini Hack Macro Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/konbini-hack-macro-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Find the most cost-effective nutritional hacks in Japanese convenience stores.

## Description
This MCP server provides a deterministic optimization engine for Japanese convenience store enthusiasts. It calculates the most efficient nutritional 'hacks' by combining base items with various add-ons to maximize a specific target macro like protein, carbs, or calories relative to price. Use `calculate_macro_efficiency` to find the best combinations, `get_item_nutrition` to look up specific item profiles, or `validate_combination_feasibility` to check if a combination fits your budget or calorie limits.


## Available Tools (3)
- **calculate_macro_efficiency**: Evaluates potential food combinations to find the most efficient hacks for a specific nutritional goal
- **get_item_nutrition**: Retrieves the nutritional data for a single item
- **validate_combination_feasibility**: Checks if a proposed combination of items meets specific user-defined constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Konbini Hack Macro Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best way to get protein using a Famichiki as a base?"

**🤖 AI Agent:**
> The most efficient protein hack is combining Famichiki with a Protein Drink and a Boiled Egg, yielding a macro efficiency of 0.15 protein/JPY.

---

**👤 You:**
> "Check if a combination of Onigiri and a Protein Bar is under 300 Yen."

**🤖 AI Agent:**
> The combination is feasible and costs 280 Yen.

---

**👤 You:**
> "Get the nutrition facts for a specific item named 'Salad Chicken'."

**🤖 AI Agent:**
> Salad Chicken: 120 calories, 25g protein, 2g carbs, 1g fat, and 180 JPY.


## ❓ FAQ

**Q: How do I find the best protein hack?**
You can use the `calculate_macro_efficiency` tool. Provide your base item and a list of add-on items, then set the target macro to 'protein' to see the most efficient combinations.

**Q: Can I check if a combination is within my budget?**
Yes, use the `validate_combination_feasibility` tool. You can specify a `maxBudgetJpy` to ensure the total price of your items stays within your limit.

**Q: Where does the nutritional data come from?**
Nutritional data is retrieved from a local item catalog containing verified convenience store products.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/konbini-hack-macro-optimizer](https://vinkius.com/ai-agent-connect/konbini-hack-macro-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Konbini Hack Macro Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `konbini-hack-macro-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Konbini Hack Macro Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "konbini-hack-macro-optimizer": {
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
