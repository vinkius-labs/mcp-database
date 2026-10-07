# Complete Trip Budget MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/complete-trip-budget)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Comprehensive financial planning for travel expenses.

## Description
This MCP server provides a complete suite of financial tools for travelers. Use `get_total_trip_budget` to calculate grand totals including contingency and exchange losses, `get_category_breakdown` to see spending by category, `get_group_cost_distribution` to manage group liabilities, and `get_daily_spending_profile` to track daily spending rhythms.


## Available Tools (4)
- **get_daily_spending_profile**: 
- **get_category_breakdown**: 
- **get_group_cost_distribution**: 
- **get_total_trip_budget**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Complete Trip Budget** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my total budget for a trip with these expenses: [{"category":"Transport","amount":500,"people":1}, {"category":"Lodging","amount":1000,"people":1}] with a 10% contingency?"

**🤖 AI Agent:**
> Your total trip cost is $1,650.00, which includes a $150.00 contingency buffer.

---

**👤 You:**
> "Show me the breakdown of my expenses: [{"category":"Meals","amount":200,"people":1}, {"category":"Activities","amount":300,"people":1}]"

**🤖 AI Agent:**
> Your highest expense category is Activities at $300.00, and your lowest is Meals at $200.00.

---

**👤 You:**
> "How much is each group responsible for? Expenses: [{"category":"Transport","amount":100,"people":1,"groupName":"Family"}, {"category":"Transport","amount":50,"people":1,"groupName":"Friends"}]"

**🤖 AI Agent:**
> The Family group is responsible for $100.00, and the Friends group is responsible for $50.00.


## ❓ FAQ

**Q: How can I see my total trip cost?**
You can use the `get_total_trip_budget` tool to calculate the total cost, including any contingency buffers or exchange rate losses you specify.

**Q: Can I split costs between different groups?**
Yes, the `get_group_cost_distribution` tool allows you to see how costs are distributed among different subgroups of travelers.

**Q: How do I track daily spending?**
Use the `get_daily_spending_profile` tool to view a breakdown of expenses by date and identify your peak spending days.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/complete-trip-budget](https://vinkius.com/en/ai-agent-connect/complete-trip-budget)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Complete Trip Budget** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `complete-trip-budget` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Complete Trip Budget** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "complete-trip-budget": {
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
