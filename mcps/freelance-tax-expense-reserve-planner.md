# Freelance Tax & Expense Reserve Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/freelance-tax-expense-reserve-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise tax and expense reserves from your freelance invoices.

## Description
Manage your freelance cash flow by accurately calculating the funds needed for future liabilities. This MCP server provides tools to determine specific tax reserves per invoice using `get_tax_reserve_per_invoice`, forecast your savings growth with `calculate_projected_savings_timeline`, set monthly savings goals via `get_expense_reserve_requirement`, and verify your financial readiness with `analyze_reserve_sufficiency`.


## Available Tools (4)
- **analyze_reserve_sufficiency**: Checks if the current savings balance is enough to cover known upcoming tax liabilities and expense goals
- **calculate_projected_savings_timeline**: Forecasts how the savings balance will grow over a series of planned future payments
- **get_expense_reserve_requirement**: Calculates how much needs to be set aside from gross income to reach a specific expense funding goal
- **get_tax_reserve_per_invoice**: Determines the specific tax amount to set aside from a single incoming invoice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freelance Tax & Expense Reserve Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just received an invoice for $5000. My tax rate is 25% and my deductible share is 20%. How much tax should I set aside?"

**🤖 AI Agent:**
> You should set aside $1,000 for taxes. This is calculated from a taxable income of $4,000.

---

**👤 You:**
> "I need to save $1200 for new equipment in 4 months. My average monthly income is $3000. How much should I save each month?"

**🤖 AI Agent:**
> You need to set aside $300 per month to reach your $1200 goal in 4 months.

---

**👤 You:**
> "I have $2000 in savings. I have upcoming tax bills of $500 and $300, and I want to save $800 for expenses. Do I have enough?"

**🤖 AI Agent:**
> Yes, you have a surplus of $400.


## ❓ FAQ

**Q: How does the tax reserve calculation work?**
The `get_tax_reserve_per_invoice` tool calculates tax based on taxable income, which is your gross income minus the deductible business expenses.

**Q: Can I project my savings for the whole year?**
Yes, you can use `calculate_projected_savings_timeline` to see how your balance will grow based on your planned future invoices.

**Q: How do I know if I have enough money saved?**
You can use `analyze_reserve_sufficiency` to compare your current savings against your upcoming tax liabilities and expense goals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/freelance-tax-expense-reserve-planner](https://vinkius.com/en/ai-agent-connect/freelance-tax-expense-reserve-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freelance Tax & Expense Reserve Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freelance-tax-expense-reserve-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freelance Tax & Expense Reserve Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freelance-tax-expense-reserve-planner": {
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
