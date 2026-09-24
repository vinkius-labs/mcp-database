# Ad Spend Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ad-spend-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Aggregate and analyze advertising expenditure across marketing channels.

## Description
This MCP server provides a specialized toolset for managing advertising budgets. It allows AI agents to calculate total expenditures using `get_total_spend`, break down costs by marketing channel with `get_spend_by_channel`, monitor specific campaign health via `get_campaign_performance_summary`, and track spending trends over time using `get_spend_over_time`.


## Available Tools (4)
- **get_campaign_performance_summary**: Provides a summary of spend and budget status for specific advertising campaigns
- **get_spend_by_channel**: You can filter by a specific channel name.

Breaks down total expenditure by the specific marketing channel used
- **get_spend_over_time**: Specify the start date, end date, and the granularity (daily, weekly, or monthly).

Analyzes how advertising costs fluctuate over a specific duration
- **get_total_spend**: Calculates the absolute total of all advertising expenses recorded in the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ad Spend Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my total ad spend in USD?"

**🤖 AI Agent:**
> Your total advertising expenditure is $12,450.00 USD.

---

**👤 You:**
> "Show me the spend breakdown by channel."

**🤖 AI Agent:**
> Social Media: $5,000, Search: $4,500, Display: $2,950.

---

**👤 You:**
> "How much did campaign CMP-99 spend compared to its budget?"

**🤖 AI Agent:**
> Campaign CMP-99 has spent $1,200 against a planned budget of $1,000, so it is currently Over Budget.


## ❓ FAQ

**Q: How can I see my total advertising costs?**
You can use the `get_total_spend` tool to retrieve the absolute total of all recorded advertising expenses.

**Q: Can I filter spending by a specific channel?**
Yes, the `get_spend_by_channel` tool allows you to view a breakdown of costs for all channels or filter for a specific one.

**Q: How do I check if a campaign is over budget?**
Use the `get_campaign_performance_summary` tool with the campaign ID to see the actual spend versus the planned budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ad-spend-total](https://vinkius.com/en/ai-agent-connect/ad-spend-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ad Spend Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ad-spend-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ad Spend Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ad-spend-total": {
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
