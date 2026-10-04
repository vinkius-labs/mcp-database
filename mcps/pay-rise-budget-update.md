# Pay Rise Budget Update MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pay-rise-budget-update)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Redistribute salary increases across savings, debt, goals, and spending.

## Description
This MCP server provides tools to help you plan how a salary increase affects your monthly budget. You can use `calculate_budget_reallocation` to see the before-and-after breakdown of your net income, `get_tax_impact` to see how much tax is deducted from your raise, and `summarize_allocation_shifts` to identify exactly how much extra money goes into each category like savings or debt repayment. It helps you make informed decisions about your financial future after a pay increase.


## Available Tools (4)
- **calculate_budget_reallocation**: Calculates the monthly distribution of funds before and after a pay rise is applied
- **get_tax_impact**: Determines how much of a gross increase is actually kept by the user after tax
- **summarize_allocation_shifts**: Provides a focused view of how much extra money is being funneled into each specific category due to the raise
- **validate_allocation_strategy**: 0).

Checks if a specific set of percentage allocations is mathematically sound and balanced


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pay Rise Budget Update** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I got a $500 monthly raise. My tax rate is 20%. How will this change my budget if I allocate 30% to savings, 20% to debt, 10% to goals, and 40% to spending?"

**🤖 AI Agent:**
> With a $500 gross raise and a 20% tax rate, your net increase is $400. Your new monthly allocations will increase by $120 for savings, $80 for debt, $40 for goals, and $160 for spending.

---

**👤 You:**
> "How much of my $1,000 raise will I actually keep if my tax rate is 25%?"

**🤖 AI Agent:**
> After a 25% tax deduction, you will keep $750 of your $1,000 raise.

---

**👤 You:**
> "Check if these percentages work: 40% savings, 30% debt, 20% goals, 10% spending."

**🤖 AI Agent:**
> Yes, those percentages are valid as they sum to exactly 100%.


## ❓ FAQ

**Q: How does the tool handle taxes?**
The tool uses the `get_tax_impact` logic to calculate the net increase by applying your specified tax rate to the gross raise amount.

**Q: Can I verify if my budget percentages are correct?**
Yes, you can use `validate_allocation_strategy` to ensure your savings, debt, goals, and spending percentages sum up to exactly 100%.

**Q: What information do I need to provide?**
To calculate a full reallocation, you will need your current gross income, the raise amount, your tax rate, and your desired allocation percentages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pay-rise-budget-update](https://vinkius.com/en/ai-agent-connect/pay-rise-budget-update)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pay Rise Budget Update** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pay-rise-budget-update` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pay Rise Budget Update** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pay-rise-budget-update": {
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
