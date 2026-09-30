# Recipe Cost Breakdown MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recipe-cost-breakdown)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise recipe costs, serving prices, and ingredient waste impact.

## Description
This MCP server provides granular financial insights into food production. It bridges the gap between package purchasing and actual usage by accounting for ingredient waste. Use `get_recipe_cost_analysis` to see total costs and leftover values, or `calculate_ingredient_efficiency` to understand how waste affects your margins. It also supports `get_inventory_valuation` for stock monitoring and `compare_recipe_margins` for menu pricing decisions.


## Available Tools (4)
- **calculate_ingredient_efficiency**: Determines how much a specific ingredient's waste is driving up the cost of a recipe
- **compare_recipe_margins**: Compares the cost of different recipes to assist in menu pricing decisions
- **get_inventory_valuation**: Provides a summary of the total value of all ingredient packages currently held in stock
- **get_recipe_cost_analysis**: Calculates the total cost, cost per serving, and the value of remaining stock for a specific recipe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recipe Cost Breakdown** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost and cost per serving for recipe 'R123'?"

**🤖 AI Agent:**
> The total cost for the Signature Beef Stew (R123) is $45.50, with a cost per serving of $5.69 for 8 portions. The leftover value of unused ingredients is $12.20.

---

**👤 You:**
> "How much is my current inventory worth?"

**🤖 AI Agent:**
> The total value of all ingredient packages currently in stock is $1,240.50, across 45 unique items.

---

**👤 You:**
> "Compare the costs of recipe 'R101' and 'R102'."

**🤖 AI Agent:**
> The cost for Classic Tomato Soup (R101) is $12.00, while the cost for Roasted Garlic Bread (R102) is $8.50.


## ❓ FAQ

**Q: How does this tool account for ingredient waste?**
The tool calculates the effective cost by including both the amount used and the cost of the waste generated during preparation, ensuring your margins are accurate.

**Q: Can I check the value of my current stock?**
Yes, you can use `get_inventory_valuation` to get a summary of the total value of all ingredient packages currently held in stock.

**Q: What is the difference between recipe cost and leftover value?**
Recipe cost is the total expense for the ingredients used (including waste), while leftover value is the monetary value of the unused portions of the packages remaining in stock.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recipe-cost-breakdown](https://vinkius.com/en/ai-agent-connect/recipe-cost-breakdown)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recipe Cost Breakdown** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipe-cost-breakdown` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recipe Cost Breakdown** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipe-cost-breakdown": {
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
