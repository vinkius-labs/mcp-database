# Cafe Daily Profit Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cafe-daily-profit-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate daily net profit by analyzing sales, ingredient costs, labor, waste, and overhead.

## Description
This MCP server provides cafe owners with a complete toolkit to monitor financial health. Use `get_sales_summary` to track revenue, `calculate_ingredient_costs` to monitor COGS and waste, `calculate_operational_overhead` for labor and rent, and `get_daily_profit_report` for a full net profit breakdown.


## Available Tools (4)
- **calculate_operational_overhead**: Calculates the daily fixed and variable expenses excluding food and ingredients
- **get_daily_profit_report**: Provides the final net profit calculation by aggregating sales, ingredients, labor, waste, rent, and fees
- **get_sales_summary**: Retrieves the total revenue and volume of items sold for a specific day
- **calculate_ingredient_costs**: Determines the total cost of ingredients used for items sold and the cost of wasted ingredients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cafe Daily Profit Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my total revenue for 2024-05-20?"

**🤖 AI Agent:**
> The total revenue for 2024-05-20 was $1,250.00 with 85 items sold.

---

**👤 You:**
> "How much did I lose to ingredient waste on 2024-05-20?"

**🤖 AI Agent:**
> The total waste cost for 2024-05-20 was $42.50.

---

**👤 You:**
> "Show me the profit report for 2024-05-20."

**🤖 AI Agent:**
> For 2024-05-20, the net profit was $315.00 with a profit margin of 25.2%.


## ❓ FAQ

**Q: How do I see my total revenue for yesterday?**
You can use the `get_sales_summary` tool by providing yesterday's date in YYYY-MM-DD format.

**Q: Does this tool account for ingredient waste?**
Yes, the `calculate_ingredient_costs` tool specifically returns both the cost of ingredients sold and the cost of wasted ingredients.

**Q: Can I get a full profit report?**
Yes, use `get_daily_profit_report` to get net profit, profit margin, and gross margin for any specific date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cafe-daily-profit-plan](https://vinkius.com/en/ai-agent-connect/cafe-daily-profit-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cafe Daily Profit Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cafe-daily-profit-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cafe Daily Profit Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cafe-daily-profit-plan": {
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
