# ConnectAndSell MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/connectandsell)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Empower your conversational AI to interact with and review metrics from ConnectAndSell's B2B sales acceleration dialer.

## Description
Connect your conversational agent to the established **ConnectAndSell** platform. Efficiently monitor calling activities, track campaign success rates, and manage high-volume B2B cold calling campaigns effortlessly via text.

### What you can do

- **Track Campaigns** — Immediately instruct your agent to check live metrics for active dialing campaigns and list out agent statuses.
- **Review Activities** — Audit logs for specific sales reps to review connection rates, talk time, and disposition outcomes.
- **Extract Insights** — Identify which outreach lists are yielding the highest conversation ratios to optimize your CRM workflows.

### How it works

1. Append this integration securely to your AI application.
2. Authorize using active ConnectAndSell API credentials.
3. Chat seamlessly via natural language to audit your business-to-business calling cadence.

### Who is this for?

- **Sales Managers** — Daily assessment of representative activities without pulling reports manually from external dashboards.
- **SDR Leaders** — Quickly check active lists and prioritize campaign flows through continuous AI monitoring and reporting.
- **Operations Teams** — Combine calling stats natively into larger operational narratives reported within an AI environment.


## Available Tools
- **get_performance_summary**: Supports optional date range filtering.

Retrieve a summary of sales calling performance metrics
- **list_assigned_lists**: Returns the prospect lists assigned for outbound calling sessions.

Retrieve the calling lists assigned to a specific user
- **list_call_attempts**: Supports date filtering.

Retrieve history of all outbound call attempts
- **list_conversations**: Supports date filtering in YYYY-MM-DD format.

Retrieve history of successful connections and conversations
- **list_cas_users**: Retrieve all users in the ConnectAndSell account
- **sync_to_crm**: g. Salesforce, HubSpot). Requires the call ID and CRM type.

Manually trigger a sync of call data to your connected CRM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ConnectAndSell** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check the current statistics for our 'Q3 Outreach' ConnectAndSell dialer campaign?"

**🤖 AI Agent:**
> Certainly. The 'Q3 Outreach' campaign currently has 3 active reps logged in. So far today, they have completed 1,420 dials resulting in 43 live connections and 2 booked meetings. The average connect rate is tracking smoothly at approximately 3.03%.

---

**👤 You:**
> "Which SDR had the highest talk time ratio across outbound operations yesterday?"

**🤖 AI Agent:**
> Based on aggregate metrics from yesterday, SDR Jane Doe achieved the highest talk time ratio. She spent 38% of her logged-in time actively speaking with prospects, completing 312 dials and engaging in 15 conversations that exceeded 3 minutes each.

---

**👤 You:**
> "How many total connections were established today among all sales reps?"

**🤖 AI Agent:**
> Across all active reps today, there have been a total of 185 connections from 6,430 dials, giving an average connection rate of 2.87%.


## ❓ FAQ

**Q: How do I securely obtain ConnectAndSell API credentials?**
You typically need to contact your organization's ConnectAndSell technical administrator or reach out directly to the official support channel to provision API access. Once authorized, secure the credentials supplied and enter them safely in this integration's configuration context below.

**Q: Can the AI place active phone calls on behalf of the sales reps?**
No. This integration operates primarily in a reporting, querying, and monitoring capacity. It manages system metrics to retrieve data on usage, calling statistics, performance overviews and campaign metrics, rather than taking direct voice or real-time call control roles which structurally belong strictly within the dialer platform interface natively.

**Q: What exact statistics can be reviewed with this AI integration?**
You can effectively retrieve summary counts of dials made, connection and conversion ratios, active campaign performance statuses, agent-level tallies of successful meetings set, and various log insights correlating duration of talk to explicit disposition outcomes recorded internally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/connectandsell](https://vinkius.com/mcp/connectandsell)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ConnectAndSell** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `connectandsell` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ConnectAndSell** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "connectandsell": {
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
