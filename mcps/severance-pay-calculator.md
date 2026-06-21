# Severance Pay Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/severance-pay-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise employee termination payouts, including salary balances and statutory penalties.

## Description
This MCP server provides a specialized engine for computing accurate employee severance packages. It automates the complex calculations required during contract termination, including salary balances for the final month, proportional 13th-month bonuses, and vacation entitlements (both expired and proportional) with the mandatory one-third constitutional supplement. Additionally, it determines statutory penalties like the FGTS multiplier based on the separation type using `calculate_statutory_penalties`. Whether you are calculating a `WITHOUT_CAUSE` termination, a `RESIGNATION`, or an `AGREEMENT`, this tool ensures mathematical precision for all legal obligations.


## Available Tools (3)
- **compute_salary_balance_and_bonuses**: Calculate the earned salary balance and proportional 13th month bonus
- **calculate_vacation_payout**: Calculate the total value for expired and proportional vacation time
- **calculate_statutory_penalties**: Determine the financial penalty owed based on termination type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Severance Pay Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much is my salary balance if I earned $3000 and worked 15 days in a 30-day month?"

**🤖 AI Agent:**
> $1,500.00

---

**👤 You:**
> "Calculate the vacation payout for a $2400 salary with 1 year of expired vacation and 6 months of proportional vacation."

**🤖 AI Agent:**
> Expired Vacation: $3,200.00 (including supplement), Proportional Vacation: $1,600.00 (including supplement).

---

**👤 You:**
> "What is the penalty for a termination without cause if my FGTS balance is $5,000?"

**🤖 AI Agent:**
> $2,000.00


## ❓ FAQ

**Q: How do I calculate the final month's salary balance?**
Use the `compute_salary_balance_and_bonuses` tool. You will need to provide the gross monthly salary, the number of days worked in the final month, and the total calendar days in that specific month.

**Q: Does the calculator include the one-third vacation bonus?**
Yes, the `calculate_vacation_payout` tool automatically includes the mandatory one-third constitutional supplement in both expired and proportional vacation calculations.

**Q: How are statutory penalties calculated?**
The `calculate_statutory_penalties` tool applies a 40% penalty for 'WITHOUT_CAUSE' terminations and a 20% penalty for 'AGREEMENT' scenarios, based on the provided severance fund balance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/severance-pay-calculator](https://vinkius.com/mcp/severance-pay-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Severance Pay Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `severance-pay-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Severance Pay Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "severance-pay-calculator": {
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
