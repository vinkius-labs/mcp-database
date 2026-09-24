# Refund Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refund-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Aggregates and validates refund transactions by currency, status, and tier.

## Description
This MCP server provides tools to manage and analyze refund data. It allows AI agents to calculate total completed refunds using `get_total_refund_by_currency`, monitor pending requests with `get_pending_refund_count`, view status breakdowns via `get_refund_summary_by_status`, and generate volume reports by classification tier using `get_tier_volume_report`.


## Available Tools (4)
- **get_pending_refund_count**: You can optionally filter by currency.

Answers how many refund requests are currently awaiting processing
- **get_refund_summary_by_status**: You can optionally filter by currency.

Provides a breakdown of refund volumes across all possible statuses
- **get_tier_volume_report**: Aggregates refund totals based on the classification tier
- **get_total_refund_by_currency**: Calculates the sum of all completed refund amounts for a specific currency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refund Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total amount of completed refunds in EUR?"

**🤖 AI Agent:**
> The total amount of completed refunds in EUR is 1,250.50, consisting of 15 completed transactions.

---

**👤 You:**
> "How many refunds are pending right now?"

**🤖 AI Agent:**
> There are currently 8 pending refund requests.

---

**👤 You:**
> "Show me the refund breakdown by status for GBP."

**🤖 AI Agent:**
> For GBP, the status breakdown is: Completed: 500.00, Pending: 50.00, Failed: 10.00.


## ❓ FAQ

**Q: How do I check the total amount of completed refunds for USD?**
You can use the `get_total_refund_by_currency` tool and specify 'USD' as the currency.

**Q: Can I see how many refunds are currently pending?**
Yes, use the `get_pending_refund_count` tool to see the number of pending transactions.

**Q: What is a tier volume report?**
It is a report that groups completed refund amounts into Micro, Standard, and Bulk categories using `get_tier_volume_report`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refund-total](https://vinkius.com/en/ai-agent-connect/refund-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refund Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refund-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refund Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refund-total": {
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
