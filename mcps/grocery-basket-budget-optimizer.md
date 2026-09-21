# Grocery Basket Budget Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grocery-basket-budget-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes grocery shopping by selecting items to meet dietary, meal, and household needs within a strict budget.

## Description
This MCP server provides a mathematical optimization engine to manage grocery shopping efficiently. It calculates the best combination of items to satisfy meal requirements, serving needs, and household inventory while strictly adhering to a budget. The engine accounts for package sizes and waste rates to ensure accurate planning. You can use `optimize_grocery_basket` to solve for the entire basket, `validate_dietary_compliance` to check for allergens or dietary restrictions, `calculate_effective_yield` to predict usable food amounts, and `find_best_substitutions` to identify cost-effective alternatives.


## Available Tools (4)
- **find_best_substitutions**: Identifies the most cost-effective alternatives for a required item based on user preferences
- **optimize_grocery_basket**: Selects quantities from supplied grocery items to satisfy meal, serving, dietary, and household needs under a budget
- **validate_dietary_compliance**: Checks if a specific item or a collection of items adheres to the provided dietary rules
- **calculate_effective_yield**: Determines how much usable material remains from a purchase after accounting for waste and usage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grocery Basket Budget Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Optimize a grocery basket for a $50 budget including milk, eggs, and bread for 3 people."

**🤖 AI Agent:**
> Selected items: 1x Milk (2L), 1x Eggs (12pk), 1x Bread (500g). Total cost: $12.50. All requirements satisfied.

---

**👤 You:**
> "Check if this item is compliant with a vegan diet: Organic Almond Milk."

**🤖 AI Agent:**
> The item is compliant with the vegan dietary constraint.

---

**👤 You:**
> "Find the best substitute for Butter if it is too expensive."

**🤖 AI Agent:**
> The best alternative is Margarine, which costs $3.00.


## ❓ FAQ

**Q: How does the optimizer handle food waste?**
The engine uses the `calculate_effective_yield` logic to account for the waste rate of each item, ensuring that the usable amount meets your requirements.

**Q: Can I suggest alternative items if my primary choice is too expensive?**
Yes, you can define substitution preferences. The `find_best_substitutions` tool helps identify the most cost-effective alternatives available in your catalog.

**Q: How are dietary restrictions enforced?**
Dietary constraints are prioritized. The `validate_dietary_compliance` tool ensures that selected items adhere to your specific rules, such as vegan or gluten-free requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grocery-basket-budget-optimizer](https://vinkius.com/en/ai-agent-connect/grocery-basket-budget-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grocery Basket Budget Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grocery-basket-budget-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grocery Basket Budget Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grocery-basket-budget-optimizer": {
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
