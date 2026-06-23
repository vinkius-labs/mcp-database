# Baremetrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baremetrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

SaaS financial analytics — audit MRR, churn, LTV, and customer subscriptions via AI.

## Description
Unlock the pulse of your subscription business with **Baremetrics**, the leading financial analytics platform for SaaS. By connecting Baremetrics to your AI agent, you transform complex revenue data into a natural conversation. Your agent can instantly retrieve high-level metrics like MRR (Monthly Recurring Revenue), LTV (Lifetime Value), and churn rates, or dive deep into specific customer subscription histories without you ever navigating through dense financial dashboards. Whether you're preparing a board report or auditing customer health, your agent acts as a real-time CFO, ensuring your growth data is always accessible and actionable.

### What you can do

- **Financial Auditing** — Retrieve instant summaries of core SaaS metrics including MRR, ARR, LTV, and active customer counts via natural language.
- **Customer Oversight** — List and search for specific customers, auditing their internal IDs, profile details, and subscription status.
- **Subscription Tracking** — Access detailed logs of user subscriptions to identify upgrade patterns or potential churn risks.
- **Source Management** — List all available data sources and defined plans to map your entire billing ecosystem.
- **Custom Timeframes** — Query financial metrics for specific date ranges to analyze growth trends and seasonal performance.

### How it works

1. Subscribe to this server
2. Enter your Baremetrics API Key (Bearer Token)
3. Start auditing your SaaS metrics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders & Executives** — get instant pulse checks on business health and growth metrics through natural conversation.
- **Customer Success Managers** — audit individual customer lifetime value and subscription history to prepare for renewals.
- **Financial Analysts** — extract raw metric data for reporting and modeling without manual dashboard data extraction.
- **Operations Leads** — verify data sources and plan configurations across the entire Baremetrics tenant.


## Available Tools (12)
- **get_account_check**: Verify Baremetrics connection
- **get_active_customers**: Convenience tool to get active customer count
- **get_churn_rate**: Convenience tool to get user churn rate
- **get_customer**: Get details for a specific customer
- **get_ltv**: Convenience tool to get Customer Lifetime Value (LTV)
- **get_metric**: Get specific data for a single metric type
- **get_mrr**: Convenience tool to get Monthly Recurring Revenue (MRR)
- **list_customers**: List all customers in Baremetrics
- **list_metrics**: List high-level financial metrics summary
- **list_plans**: List all defined plans
- **list_sources**: List all available data sources
- **list_subscriptions**: List all user subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baremetrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current Monthly Recurring Revenue (MRR)?"

**🤖 AI Agent:**
> Checking Baremetrics... Your current MRR is $45,200. This is a 3.5% increase compared to the same time last month.

---

**👤 You:**
> "Show me the top 5 customers by LTV."

**🤖 AI Agent:**
> I've retrieved your top customers. The top 5 by Lifetime Value are: Acme Corp ($12,500), Globex ($10,200), Soylent Corp ($9,800), Initech ($8,500), and Umbrella Corp ($7,200).

---

**👤 You:**
> "Search for a customer named 'John Smith' and show their active subscriptions."

**🤖 AI Agent:**
> I found John Smith (OID: `cus_123`). He currently has 1 active 'Pro Plan' subscription at $99/month, which started on Jan 15th, 2025.


## ❓ FAQ

**Q: Can I check my current MRR through the agent?**
Yes. Use the `get_mrr` tool to retrieve your current Monthly Recurring Revenue. Your agent will return the latest calculated value directly in the chat.

**Q: How do I find a specific customer's subscription history?**
First, use `list_customers` with a search term to find the customer's OID. Then, your agent can retrieve their detailed profile and subscription logs to summarize their journey.

**Q: Can the agent analyze churn rates for specific periods?**
Absolutely. Use the `get_churn_rate` tool and provide a `start_date` and `end_date` (as Unix timestamps) to see the churn metrics for that specific timeframe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baremetrics](https://vinkius.com/mcp/baremetrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baremetrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baremetrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baremetrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baremetrics": {
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
