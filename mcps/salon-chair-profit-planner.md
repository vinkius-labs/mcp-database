# Salon Chair Profit Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/salon-chair-profit-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate net profitability for salon chairs based on revenue, splits, and overhead.

## Description
This MCP server provides financial modeling tools for salon owners and stylists to track chair profitability. Use `get_revenue_summary` to view total income, `calculate_stylist_earnings` to determine commissions, `calculate_chair_overhead` to aggregate costs like rent and transaction fees, and `get_net_profitability_report` for a complete financial breakdown.


## Available Tools (4)
- **calculate_chair_overhead**: Aggregates all fixed and variable costs associated with maintaining the chair
- **calculate_stylist_earnings**: Determines how much a stylist earns based on their specific commission or split agreement
- **get_net_profitability_report**: Produces a complete breakdown of the profit remaining for the salon or stylist after all splits and expenses
- **get_revenue_summary**: Provides a high-level overview of total service and product revenue for a specific period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salon Chair Profit Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my total revenue for the month?"

**🤖 AI Agent:**
> Your total service revenue was $5,000 and your total product revenue was $800, resulting in a gross revenue of $5,800.

---

**👤 You:**
> "How much will I earn if I have $2,000 in service revenue with a 50% split?"

**🤖 AI Agent:**
> With a 50% split on $2,000 of service revenue, your service earnings are $1,000.

---

**👤 You:**
> "Calculate my net profit for $3,000 revenue, $500 rent, and 3% transaction fees."

**🤖 AI Agent:**
> After subtracting the $500 rent and $90 in transaction fees, your net profit is $2,410.


## ❓ FAQ

**Q: How do I calculate my total earnings?**
You can use the `calculate_stylist_earnings` tool by providing your service revenue, split percentage, and product commission details.

**Q: Can I see a full breakdown of my profits?**
Yes, the `get_net_profitability_report` tool generates a complete breakdown including service profit, product profit, and overhead deductions.

**Q: Does this tool account for rent and transaction fees?**
Yes, the `calculate_chair_overhead` tool specifically aggregates fixed rent and variable transaction fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/salon-chair-profit-planner](https://vinkius.com/en/ai-agent-connect/salon-chair-profit-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salon Chair Profit Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salon-chair-profit-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salon Chair Profit Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salon-chair-profit-planner": {
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
