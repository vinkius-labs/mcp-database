# Coffee Home Savings Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/coffee-home-savings-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Compare the cost of cafe coffee versus brewing at home.

## Description
This MCP server provides tools to analyze the financial impact of your coffee habits. You can use `calculate_ingredient_unit_costs` to find the cost per serving of your beans, `get_weekly_home_cost` to determine your weekly brewing expenses, and `calculate_savings_comparison` to see how much you save annually compared to cafe prices.


## Available Tools (4)
- **calculate_ingredient_unit_costs**: Helps users derive the per-serving cost of beans and milk from bulk purchase data
- **calculate_savings_comparison**: Compares cafe spending against home spending to determine savings
- **get_weekly_cafe_expenditure**: Calculates how much a user spends per week on cafe-bought coffee
- **get_weekly_home_cost**: Calculates how much a user spends per week to brew coffee at home


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coffee Home Savings Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does it cost to buy a 500g bag of beans for $15 if I use 20g per cup?"

**🤖 AI Agent:**
> The cost per serving is $0.60.

---

**👤 You:**
> "I spend $5 per cafe coffee and drink 7 a week. I brew at home for $0.70 per cup and drink 7 a week. How much do I save per year?"

**🤖 AI Agent:**
> You will save $1,222.00 per year.

---

**👤 You:**
> "If I spend $30 a week at cafes and $5 a week at home, and my machine cost $100, how many weeks until I break even?"

**🤖 AI Agent:**
> You will break even in 4 weeks.


## ❓ FAQ

**Q: How do I calculate the cost of my coffee beans?**
Use the `calculate_ingredient_unit_costs` tool. Provide the bulk price, the total weight, and your serving size to get the cost per cup.

**Q: Can I include the cost of my espresso machine?**
Yes, use `calculate_savings_comparison` and provide the equipment cost to find your break-even point.

**Q: Does this account for milk costs?**
Yes, `get_weekly_home_cost` allows you to include an optional milk cost per serving.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/coffee-home-savings-calculator](https://vinkius.com/en/ai-agent-connect/coffee-home-savings-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coffee Home Savings Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coffee-home-savings-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coffee Home Savings Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coffee-home-savings-calculator": {
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
