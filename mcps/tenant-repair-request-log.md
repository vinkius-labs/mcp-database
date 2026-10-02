# Tenant Repair Request Log MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tenant-repair-request-log)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [property-management](../categories/property-management.md)

Track and manage tenant repair requests, landlord response deadlines, and repair costs.

## Description
This MCP server provides a specialized logging and tracking system for managing tenant-submitted repair requests. It allows AI agents to monitor landlord responsiveness, audit service costs, and evaluate completion timelines. Use `get_open_requests` to find active issues, `get_overdue_responses` to identify landlords missing deadlines, `get_repair_timeline` to audit specific request histories, and `get_cost_summary` to aggregate financial impacts of completed repairs.


## Available Tools (4)
- **get_cost_summary**: Aggregates the financial impact of repairs over a specific period
- **get_open_requests**: Retrieves all repair requests that have not yet been finalized
- **get_overdue_responses**: Identifies requests where the landlord has failed to meet the mandatory response deadline
- **get_repair_timeline**: Provides a chronological audit trail for a specific repair request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tenant Repair Request Log** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all open plumbing repair requests."

**🤖 AI Agent:**
> There are currently 2 open plumbing requests: Request #102 (Leaking faucet) and Request #105 (Clogged drain).

---

**👤 You:**
> "Which repair requests are overdue?"

**🤖 AI Agent:**
> Request #98 is overdue by 3 days, and Request #101 is overdue by 5 days.

---

**👤 You:**
> "What was the total repair cost between 2024-01-01 and 2024-03-31?"

**🤖 AI Agent:**
> The total cost for completed repairs in that period was $1,250.00 across 5 requests, with an average cost of $250.00 per request.


## ❓ FAQ

**Q: How can I see which repairs are currently active?**
You can use the `get_open_requests` tool to retrieve a list of all repair requests that have not yet been finalized.

**Q: How do I identify landlords who are slow to respond?**
Use the `get_overdue_responses` tool to find requests where the landlord has failed to meet the mandatory response deadline.

**Q: Can I calculate the total cost of repairs for a specific month?**
Yes, the `get_cost_summary` tool allows you to aggregate total costs, request counts, and average costs for completed repairs within a specified date range.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tenant-repair-request-log](https://vinkius.com/en/ai-agent-connect/tenant-repair-request-log)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tenant Repair Request Log** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tenant-repair-request-log` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tenant Repair Request Log** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tenant-repair-request-log": {
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
