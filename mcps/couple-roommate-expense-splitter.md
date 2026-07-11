# Couple & Roommate Expense Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/couple-roommate-expense-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Fairly split household expenses based on income proportions or assigned categories.

## Description
An essential tool for partners and roommates to manage shared finances equitably. This MCP server provides specialized tools like `compute_income_weights` to calculate proportional contributions based on relative earnings, and `calculate_assignment_obligation` for when specific bills are assigned to certain individuals. It also handles complex scenarios such as `calculate_amortized_installment` for spreading large one-off purchases over several months and `generate_monthly_reconciliation` to determine the final settlement amount between parties.


## Available Tools (5)
- **calculate_assignment_obligation**: Calculates individual responsibilities when partners are assigned specific categories of bills
- **calculate_amortized_installment**: Calculates the monthly cost for a one-off large purchase to be spread across multiple months
- **generate_monthly_reconciliation**: Determines exactly how much money must be transferred between partners to settle the month's expenses
- **calculate_proportional_split_amount**: Determines the specific currency amount each person is responsible for based on their calculated income weights
- **compute_income_weights**: Calculates the percentage share of total household income for each partner


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Couple & Roommate Expense Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Person A earns $5000 and Person B earns $3000. What are our income weights?"

**🤖 AI Agent:**
> Person A's weight is 0.625 (62.5%) and Person B's weight is 0.375 (37.5%).

---

**👤 You:**
> "We have $2000 in shared bills. Based on our weights of 0.6 and 0.4, how much should each pay?"

**🤖 AI Agent:**
> Person A is responsible for $1,200 and Person B is responsible for $800.

---

**👤 You:**
> "I bought a new sofa for $600. How much should we add to our monthly shared expenses if we split it over 6 months?"

**🤖 AI Agent:**
> The monthly installment amount is $100.


## ❓ FAQ

**Q: How does the proportional split work?**
The tool uses `compute_income_weights` to determine each person's share of total household income. Then, `calculate_proportional_split_amount` applies those weights to your shared bills.

**Q: Can I handle large one-time purchases?**
Yes, use `calculate_amortized_installment` to break down a single high-cost item into manageable monthly payments.

**Q: How do we settle up at the end of the month?**
Use `generate_monthly_reconciliation` by providing what each person actually paid versus their calculated obligation to find the exact transfer amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/couple-roommate-expense-splitter](https://vinkius.com/mcp/couple-roommate-expense-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Couple & Roommate Expense Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `couple-roommate-expense-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Couple & Roommate Expense Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "couple-roommate-expense-splitter": {
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
