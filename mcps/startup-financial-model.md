# Startup Financial Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/startup-financial-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate 12, 24, or 36-month financial projections including P&L, Cash Flow, and Break-even analysis.

## Description
This MCP server provides a specialized engine for startup financial modeling. Use `query_revenue_growth` to forecast monthly revenue, `query_cost_structure` to calculate COGS and operating expenses, or `generate_comprehensive_projection` to produce a full P&L statement, cash flow projection, and identify your break-even month based on growth rates and cost margins.


## Available Tools (3)
- **generate_comprehensive_projection**: Generates a complete financial report
- **query_cost_structure**: Calculate monthly COGS and Operating Expenses
- **query_revenue_growth**: Calculate monthly revenue breakdown based on growth assumptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Startup Financial Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 12-month projection starting with $10,000 revenue and 5% monthly growth."

**🤖 AI Agent:**
> I will use `generate_comprehensive_projection` with initialRevenue: 10000, growthRate: 0.05, and periodMonths: 12 to calculate your P&L and cash flow.

---

**👤 You:**
> "What are my monthly revenues for the next 24 months if I grow at 10% MoM?"

**🤖 AI Agent:**
> I'll use `query_revenue_growth` with a growthRate of 0.10 and periodMonths of 24 to provide the breakdown.

---

**👤 You:**
> "Calculate costs for a revenue stream of [5000, 6000, 7000] with 30% COGS and $1000 fixed expenses."

**🤖 AI Agent:**
> I will use `query_cost_structure` with the provided revenue array, cogsPercentage: 0.3, and fixedExpenses: 1000.


## ❓ FAQ

**Q: What time horizons can I model?**
The engine supports projections for 12, 24, or 36 months.

**Q: How do I calculate the break-even month?**
Use the `generate_comprehensive_projection` tool. It automatically identifies the first month where net income becomes non-negative.

**Q: Can I input custom growth rates?**
Yes, you can specify any monthly percentage increase as a decimal (e.g., 0.05 for 5%) in the tool parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/startup-financial-model](https://vinkius.com/mcp/startup-financial-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Startup Financial Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startup-financial-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Startup Financial Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startup-financial-model": {
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
