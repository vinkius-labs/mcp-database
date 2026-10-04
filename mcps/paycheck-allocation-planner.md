# Paycheck Allocation Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paycheck-allocation-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Strategically distribute paychecks across bills, debt, savings, and spending.

## Description
The Paycheck Allocation Planner is a strategic financial tool designed to help you manage your income with precision. By connecting your AI agent to this MCP server via Vinkius Edge, you can automatically calculate how to split your paycheck among essential obligations and personal goals. Use `calculate_allocation` to determine exact distributions based on fixed-dollar amounts and percentage-based rules. You can also use `validate_rule_consistency` to ensure your financial plan is mathematically sound before committing, `get_category_summary` to view high-level spending totals, and `generate_transfer_plan` to receive clear, actionable instructions for moving your money.


## Available Tools (4)
- **generate_transfer_plan**: Format raw allocation data into human-readable, actionable transfer instructions
- **get_category_summary**: Aggregate individual allocations into higher-level spending categories
- **validate_rule_consistency**: Ensure a set of rules is mathematically possible before attempting an allocation
- **calculate_allocation**: Compute the precise distribution of a single paycheck based on a set of rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paycheck Allocation Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a paycheck of $3000. I need to pay $1200 for rent and $300 for utilities. I want to put 10% of the total paycheck into savings and 20% of the remaining balance into debt repayment. How should I allocate this?"

**🤖 AI Agent:**
> Your $3000 paycheck will be allocated as follows: $1200 for Rent, $300 for Utilities, $300 for Savings, and $300 for Debt Repayment. You will have $900 in residual cash.

---

**👤 You:**
> "Can you check if my rules are valid? I have $1000 total. Fixed rules: $500 for car loan. Percentage rules: 60% of total for groceries."

**🤖 AI Agent:**
> No, your rules are not valid. The total allocation ($500 fixed + $600 percentage) exceeds your $1000 paycheck.

---

**👤 You:**
> "Give me the transfer instructions for my $2000 paycheck where I have $500 for rent and 10% of the total for savings, with 'Buffer' as my residual account."

**🤖 AI Agent:**
> Transfer $500 to Rent, transfer $200 to Savings, and transfer $1300 to Buffer.


## ❓ FAQ

**Q: How do I ensure my budget is mathematically possible?**
You can use the `validate_rule_consistency` tool to check if your fixed obligations and percentage-based rules fit within your total paycheck amount.

**Q: Can I set specific amounts for my rent or mortgage?**
Yes, you can define these as fixed-dollar rules. The planner will prioritize these amounts before calculating any percentage-based distributions.

**Q: What happens to the money left over after all rules are applied?**
The remaining amount is identified as residual cash. You can use `generate_transfer_plan` to receive instructions on how to move this residual cash to a designated buffer account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paycheck-allocation-planner](https://vinkius.com/en/ai-agent-connect/paycheck-allocation-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paycheck Allocation Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paycheck-allocation-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paycheck Allocation Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paycheck-allocation-planner": {
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
