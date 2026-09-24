# Weekly Revenue Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weekly-revenue-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Aggregate and analyze weekly transaction volumes for financial visibility.

## Description
This MCP server provides tools to calculate and compare weekly transaction totals. Use `get_weekly_total` to find revenue for a specific date range, `compare_weekly_revenue` to identify growth or loss between periods, `get_revenue_by_category` to see distribution across business sectors, and `get_revenue_trend` to visualize historical revenue patterns over time.


## Available Tools (4)
- **compare_weekly_revenue**: Compares the revenue of one week against another
- **get_weekly_total**: Calculates the total revenue for a specific week
- **get_revenue_by_category**: Breaks down the total revenue of a specific week into different transaction categories
- **get_revenue_trend**: Provides a sequence of total revenues over a series of weeks to visualize trends


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekly Revenue Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the total revenue for the first week of January 2024?"

**🤖 AI Agent:**
> The total revenue for the period between 2024-01-01 and 2024-01-07 was $12,450.00 across 45 transactions.

---

**👤 You:**
> "Compare the revenue from the week of May 1st to the week of April 24th, 2024."

**🤖 AI Agent:**
> Revenue increased by $1,200.00, representing a 10.5% growth compared to the previous week.

---

**👤 You:**
> "Show me the revenue trend for the last 4 weeks."

**🤖 AI Agent:**
> The revenue trend for the last 4 weeks shows a steady increase, starting from $8,000 in week 1 to $10,500 in week 4.


## ❓ FAQ

**Q: How can I see if my revenue grew compared to last week?**
You can use the `compare_weekly_revenue` tool by providing the start and end dates for both the current week and the previous week.

**Q: Can I see which categories are generating the most money?**
Yes, the `get_revenue_by_category` tool breaks down total revenue into specific transaction categories for a given period.

**Q: How do I view revenue trends over several weeks?**
Use the `get_revenue_trend` tool. You specify how many weeks of data you want to retrieve and the end date for the look-up.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weekly-revenue-analyzer](https://vinkius.com/en/ai-agent-connect/weekly-revenue-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekly Revenue Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekly-revenue-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekly Revenue Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekly-revenue-analyzer": {
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
