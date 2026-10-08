# Hourly Rate After Expenses MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hourly-rate-after-expenses)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate your true net hourly earnings by accounting for taxes and business overhead.

## Description
This MCP server provides precision tools for freelancers and contractors to determine their actual take-home pay. By accounting for gross revenue, tax liabilities, and various operating expenses like software, equipment, travel, and insurance, you can find your true net hourly rate. Use `calculate_net_hourly_rate` to see your final earnings, `summarize_expense_distribution` to analyze your cost breakdown, `calculate_break_even_hours` to plan your workload, or `compare_rate_scenarios` to simulate how changes in taxes or expenses impact your income.


## Available Tools (4)
- **calculate_break_even_hours**: Calculates the number of hours required to cover fixed expenses and taxes
- **calculate_net_hourly_rate**: Calculates the actual net hourly pay after all costs and taxes are deducted
- **compare_rate_scenarios**: Compares how changes in tax rate or expenses affect take-home pay
- **summarize_expense_distribution**: Analyzes how income is consumed by different types of business costs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hourly Rate After Expenses** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my actual hourly pay if I invoice $5000, have a 25% tax rate, $200 in software costs, and worked 40 hours?"

**🤖 AI Agent:**
> Your net hourly rate is $90.00. This is calculated from a net revenue of $3,750 after taxes and $3,550 after all expenses.

---

**👤 You:**
> "How many hours do I need to work to earn a net rate of $60/hour if my total expenses and taxes are $1200 and my target revenue is $3000?"

**🤖 AI Agent:**
> You need to work 70 hours to cover your $1,200 in costs and reach your target.

---

**👤 You:**
> "Show me the breakdown of my $5000 revenue with a 20% tax rate and $500 in total expenses."

**🤖 AI Agent:**
> Your tax amount is $1,000 and your total operating expenses are $500, resulting in total deductions of $1,500.


## ❓ FAQ

**Q: What is the difference between gross and net hourly rate?**
Gross hourly rate is the total amount you bill before any deductions. Net hourly rate is what you actually keep after paying taxes and business expenses.

**Q: How can I see how much my software costs affect my pay?**
You can use the `compare_rate_scenarios` tool to simulate how adjusting your total expenses impacts your final net hourly rate.

**Q: Can I calculate how many hours I need to work to cover my costs?**
Yes, the `calculate_break_even_hours` tool allows you to determine the exact number of hours required to cover your fixed expenses and taxes based on a target rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hourly-rate-after-expenses](https://vinkius.com/en/ai-agent-connect/hourly-rate-after-expenses)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hourly Rate After Expenses** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hourly-rate-after-expenses` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hourly Rate After Expenses** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hourly-rate-after-expenses": {
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
