# Job Relocation Budgeter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/job-relocation-budgeter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the total financial impact of moving for a new job.

## Description
This MCP server provides a suite of tools to calculate the true cost of relocating for a new position. It aggregates gross expenses like movers and travel, determines net out-of-pocket costs after employer reimbursements, and evaluates the long-term financial impact by factoring in salary changes and tax liabilities. Use `get_relocation_expenses` to sum up initial costs, `get_net_relocation_cost` to see what you actually pay, and `get_annual_financial_impact` to understand the yearly benefit of the move.


## Available Tools (4)
- **get_annual_financial_impact**: Calculates the yearly net benefit or loss by factoring in salary changes
- **get_net_relocation_cost**: Determines the actual out-of-pocket cost after employer assistance
- **get_relocation_expenses**: Calculates the total gross cost of all moving-related expenditures
- **get_tax_adjusted_reimbursement**: Estimates the real value of employer reimbursements after accounting for tax liabilities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Job Relocation Budgeter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my total moving costs if movers cost $3000, travel is $500, deposits are $1000, and temporary housing is $1500?"

**🤖 AI Agent:**
> Your total gross relocation cost is $6,000.

---

**👤 You:**
> "If my gross relocation costs are $5000 and my employer reimburses me $4000, what is my net cost?"

**🤖 AI Agent:**
> Your net out-of-pocket cost is $1,000, and your employer is covering 80% of the costs.

---

**👤 You:**
> "I am getting a $10,000 salary increase, but the move costs me $2,000 net. What is my first-year impact?"

**🤖 AI Agent:**
> Your first-year net impact is $8,000, and your subsequent year impact will be $10,000.


## ❓ FAQ

**Q: How do I calculate my total moving expenses?**
You can use the `get_relocation_expenses` tool by providing the costs for movers, travel, deposits, and temporary housing.

**Q: Does this tool account for taxes?**
Yes, the `get_tax_adjusted_reimbursement` tool helps estimate the net value of reimbursements after accounting for your estimated tax rate.

**Q: Can I see the impact of my new salary?**
Yes, use `get_annual_financial_impact` to see how your salary change affects your first-year and subsequent-year finances.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/job-relocation-budgeter](https://vinkius.com/en/ai-agent-connect/job-relocation-budgeter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Job Relocation Budgeter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `job-relocation-budgeter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Job Relocation Budgeter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "job-relocation-budgeter": {
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
