# Side-Gig Profit Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/side-gig-profit-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate net take-home pay by accounting for fees, expenses, and taxes.

## Description
This MCP server provides essential financial tools for gig workers to understand their true earnings. Use `get_job_profit_summary` to calculate a complete breakdown of gross revenue, platform fees, operational expenses, and net profit. You can also use `get_tax_reserve_estimate` to determine how much to set aside for taxes, `get_expense_impact` to analyze material and travel costs, or `compare_gig_efficiency` to decide between two different job opportunities based on their effective hourly rate.


## Available Tools (4)
- **compare_gig_efficiency**: Compares two different gig opportunities to see which offers a better return on time
- **get_expense_impact**: Evaluates how specific operational costs (materials and travel) reduce the total profit
- **get_job_profit_summary**: Calculates the complete financial breakdown for a single completed gig
- **get_tax_reserve_estimate**: Determines how much money a user should set aside from a specific revenue amount to cover tax liabilities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Side-Gig Profit Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I earned $500 on a delivery job. The platform takes 20%, I spent $30 on supplies, drove 15 miles at $0.60 per mile, and it took me 4 hours total (including travel). My tax rate is 15%. What is my net profit and hourly rate?"

**🤖 AI Agent:**
> Your net profit is $311.10, and your effective hourly rate is $77.78 per hour.

---

**👤 You:**
> "How much should I set aside for taxes if I made $1,200 and my tax rate is 22%?"

**🤖 AI Agent:**
> You should set aside $264.00 for taxes, leaving you with $936.00.

---

**👤 You:**
> "Which is better: a job paying $100 with 10% fees and 2 hours of work, or a job paying $150 with 25% fees and 3 hours of work?"

**🤖 AI Agent:**
> The first job is better. It offers an effective hourly rate of $45.00, while the second job only offers $40.00.


## ❓ FAQ

**Q: How do I calculate my actual take-home pay?**
You can use the `get_job_profit_summary` tool. Provide your gross revenue, platform fee percentage, material costs, mileage, tax rate, and hours worked to see your net profit and effective hourly rate.

**Q: Can I compare two different jobs?**
Yes, use the `compare_gig_efficiency` tool. It compares the effective hourly rate of two different gig scenarios to show you which one is more profitable for your time.

**Q: How much should I save for taxes?**
The `get_tax_reserve_estimate` tool helps you determine the exact amount to set aside based on your anticipated tax rate and income amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/side-gig-profit-planner](https://vinkius.com/en/ai-agent-connect/side-gig-profit-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Side-Gig Profit Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `side-gig-profit-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Side-Gig Profit Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "side-gig-profit-planner": {
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
