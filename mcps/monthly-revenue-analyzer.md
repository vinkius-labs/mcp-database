# Monthly Revenue Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/monthly-revenue-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Aggregate and analyze transaction data to calculate monthly revenue totals and growth trends.

## Description
This MCP server provides a suite of tools for financial analysis. It allows AI agents to access transaction data to calculate monthly revenue totals, identify top-performing months, and track month-over-month growth rates. Use `get_revenue_summary` for high-level lifetime statistics or `get_monthly_totals` to break down revenue by specific timeframes.


## Available Tools (4)
- **get_monthly_totals**: Get monthly revenue totals within a timeframe
- **get_revenue_growth**: Get month-over-month revenue growth
- **get_revenue_summary**: Get high-level revenue statistics
- **get_top_performing_months**: Get the top performing months by revenue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monthly Revenue Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my total revenue for the first half of 2023?"

**🤖 AI Agent:**
> The total revenue for the period from 2023-01-01 to 2023-06-30 was $45,250.00.

---

**👤 You:**
> "Which were my top 3 performing months?"

**🤖 AI Agent:**
> Your top 3 performing months were: March 2023 ($12,000), May 2023 ($11,500), and January 2023 ($10,200).

---

**👤 You:**
> "Show me the revenue growth for Q4 2023."

**🤖 AI Agent:**
> In Q4 2023, revenue grew by 5.2% in October compared to September, and by 3.1% in November compared to October.


## ❓ FAQ

**Q: How can I see my total revenue for a specific period?**
You can use the `get_monthly_totals` tool by providing a start and end date in ISO 8601 format.

**Q: How do I calculate month-over-month growth?**
Use the `get_revenue_growth` tool with your desired analysis period to see the percentage change between consecutive months.

**Q: Can I get a summary of all lifetime revenue?**
Yes, the `get_revenue_summary` tool provides lifetime revenue, average monthly revenue, and extreme values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/monthly-revenue-analyzer](https://vinkius.com/en/ai-agent-connect/monthly-revenue-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Monthly Revenue Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `monthly-revenue-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Monthly Revenue Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "monthly-revenue-analyzer": {
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
