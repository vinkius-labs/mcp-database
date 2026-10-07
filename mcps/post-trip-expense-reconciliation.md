# Post-Trip Expense Reconciliation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/post-trip-expense-reconciliation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Reconcile planned vs. actual trip spending by category, traveler, and currency.

## Description
This MCP server provides tools to compare budgeted amounts against real-world spending. It helps identify budget variances by analyzing expenses through several dimensions: category-based breakdowns, individual traveler spending, currency conversions, and the impact of refunds or shared charges. Use `get_trip_summary` for a high-level overview, `reconcile_by_category` to see specific expense types, or `reconcile_by_traveler` to track individual budget adherence.


## Available Tools (5)
- **reconcile_by_category**: Compares planned vs. actual spending broken down by specific expense types
- **get_currency_reconciliation**: Validates spending across different currencies to ensure accurate base-currency reporting
- **get_refund_and_shared_impact**: Specifically isolates the impact of refunds and shared cost distributions on the total budget
- **get_trip_summary**: Provides a high-level overview of the financial health of a trip
- **reconcile_by_traveler**: Analyzes spending per person to identify who stayed within budget or overspent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Post-Trip Expense Reconciliation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of the financial health for trip ID trip_123."

**🤖 AI Agent:**
> Trip trip_123 has a total planned budget of $1,500 and total actual spending of $1,450, resulting in a positive variance of $50.

---

**👤 You:**
> "How much did each person spend on trip trip_456?"

**🤖 AI Agent:**
> For trip trip_456, Alice spent $450, Bob spent $300, and Charlie spent $250.

---

**👤 You:**
> "Show me the spending breakdown by category for trip trip_789."

**🤖 AI Agent:**
> In trip trip_789, Lodging was $800, Transport was $200, and Meals were $150.


## ❓ FAQ

**Q: How can I see if my trip is over budget?**
You can use the `get_trip_summary` tool to view the total planned amount versus the total actual spending and the resulting variance.

**Q: Can I track spending for specific people?**
Yes, the `reconcile_by_traveler` tool provides a breakdown of planned and actual spending for each individual traveler.

**Q: How are shared costs handled?**
The `get_refund_and_shared_impact` tool allows you to isolate the impact of shared charges and refunds on your total budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/post-trip-expense-reconciliation](https://vinkius.com/en/ai-agent-connect/post-trip-expense-reconciliation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Post-Trip Expense Reconciliation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `post-trip-expense-reconciliation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Post-Trip Expense Reconciliation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "post-trip-expense-reconciliation": {
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
