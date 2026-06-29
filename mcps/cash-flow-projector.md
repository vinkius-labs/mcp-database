# Cash Flow Projector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cash-flow-projector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Project monthly cash flow, identify liquidity gaps, and calculate working capital requirements.

## Description
The Cash Flow Projector is a financial forecasting tool that helps businesses plan for the future. By providing monthly inflows and outflows, you can use `generate_cash_flow_projection` to see your cumulative cash balance over time. The server also includes tools like `analyze_liquidity_gaps` to pinpoint months where your cash position might fall below critical thresholds and `calculate_working_ amounts` to determine the exact funding needed to maintain a safety buffer.


## Available Tools (3)
- **analyze_liquidity_gaps**: Analyzes liquidity gaps in a projection
- **generate_cash_flow_projection**: Generates a month-by-month cash flow projection
- **calculate_working_capital_metrics**: Calculates working capital metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cash Flow Projector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have $10,000 starting balance. For month 0, I have $2,000 inflow and $3,000 outflow. What is my projected cumulative balance?"

**🤖 AI Agent:**
> Your cumulative cash balance at the end of month 0 will be $9,000.

---

**👤 You:**
> "Based on my projection, are there any months where my balance drops below $500?"

**🤖 AI Agent:**
> Yes, month 3 is identified as a liquidity gap because the cumulative balance falls below $500.

---

**👤 You:**
> "How much safety margin should I maintain?"

**🤖 AI Agent:**
> Based on your projection, you should maintain a recommended safety balance of $1,500 to cover potential deficits.


## ❓ FAQ

**Q: How do I start a projection?**
Use the `generate_cash_flow_projection` tool by providing your starting balance and an array of monthly data containing inflows and outflows.

**Q: How can I identify months with negative cash flow?**
After generating a projection, pass the resulting series to the `analyze_liquidity_gaps` tool to find any months where the balance falls below your threshold.

**Q: What is the working capital requirement?**
It is the maximum deficit found in your projection. You can calculate this using `calculate_working_capital_metrics` to understand how much extra funding you might need.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cash-flow-projector](https://vinkius.com/mcp/cash-flow-projector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cash Flow Projector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cash-flow-projector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cash Flow Projector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cash-flow-projector": {
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
