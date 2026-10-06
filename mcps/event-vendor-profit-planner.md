# Event Vendor Profit Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/event-vendor-profit-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Project net profits by calculating sales, inventory, labor, and commissions.

## Description
This MCP server provides a suite of financial tools for event vendors to accurately project their profitability. By using tools like `calculate_revenue_projection` and `calculate_profit_summary`, vendors can model the impact of sales volume, inventory costs, labor, booth fees, and travel expenses on their bottom line. It also accounts for commission structures to ensure a realistic net profit estimation.


## Available Tools (4)
- **inventory_expense**: Calculates the total cost of goods to be sold
- **operational_costs**: Aggregates all non-inventory expenses including labor, fees, and travel
- **profit_summary**: Provides a complete financial overview including net profit and commission obligations
- **revenue_projection**: Determines the expected gross income based on sales targets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Event Vendor Profit Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will my gross revenue be if I sell 500 units at $25 each?"

**🤖 AI Agent:**
> Your gross revenue will be $12,500.

---

**👤 You:**
> "Calculate my operational costs for 40 hours of labor at $20/hour, $500 booth fee, and $300 travel."

**🤖 AI Agent:**
> Your total operational costs are $1,600.

---

**👤 You:**
> "If I have $10,000 revenue, $3,000 inventory cost, $1,000 operational costs, and a 10% commission, what is my net profit?"

**🤖 AI Agent:**
> Your net profit is $5,000.


## ❓ FAQ

**Q: How do I calculate my total expected income?**
You can use the `calculate_revenue_projection` tool by providing your unit price and the number of units you expect to sell.

**Q: Can I include travel and booth fees in my planning?**
Yes, the `calculate_operational_costs` tool allows you to aggregate labor, booth fees, and travel expenses into a single total.

**Q: How is net profit determined?**
The `calculate_profit_summary` tool calculates net profit by subtracting inventory costs, operational costs, and organizer commissions from your gross revenue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/event-vendor-profit-planner](https://vinkius.com/en/ai-agent-connect/event-vendor-profit-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Event Vendor Profit Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `event-vendor-profit-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Event Vendor Profit Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "event-vendor-profit-planner": {
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
