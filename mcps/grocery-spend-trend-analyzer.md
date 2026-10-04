# Grocery Spend Trend Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grocery-spend-trend-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze grocery spending patterns, weekly summaries, and budget compliance.

## Description
This MCP server provides deep insights into grocery transaction data. Use `get_weekly_summary` to see how much you spend each week across different categories or stores. You can also track monthly trends against historical baselines, calculate your average basket size, and monitor budget compliance using `check_category_budget_compliance` to ensure you stay within your spending limits.


## Available Tools (1)
- **get_weekly_summary**: You can filter by store or category.

Summarizes grocery spending by week, store, and category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grocery Spend Trend Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much did I spend on groceries last week?"

**🤖 AI Agent:**
> Last week, you spent a total of $145.50, with the largest portion being Produce at $42.00.

---

**👤 You:**
> "Am I over budget on Dairy?"

**🤖 AI Agent:**
> No, your current spending for Dairy is $25.00, which is below your $30.00 limit.

---

**👤 You:**
> "What was my average basket size in January?"

**🤖 AI Agent:**
> Your average basket size in January was $62.30.


## ❓ FAQ

**Q: How can I see my weekly spending breakdown?**
You can use the `get_weekly_summary` tool by providing a start and end date to see totals for categories and stores.

**Q: Can I check if I am exceeding my budget for specific items?**
Yes, the `check_category_budget_compliance` tool checks your spending against predefined category caps.

**Q: How do I compare my current spending to previous months?**
Use the `get_monthly_trend_vs_baseline` tool to compare current monthly spending against a historical baseline period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grocery-spend-trend-analyzer](https://vinkius.com/en/ai-agent-connect/grocery-spend-trend-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grocery Spend Trend Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grocery-spend-trend-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grocery Spend Trend Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grocery-spend-trend-analyzer": {
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
