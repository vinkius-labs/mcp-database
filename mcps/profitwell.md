# ProfitWell MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/profitwell)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate subscription metrics via ProfitWell (Paddle) — track churn, MRR, and customer history directly with AI.

## Description
Connect your **ProfitWell** (Paddle Metrics) account to any AI agent and take full control of your subscription revenue orchestration through natural conversation. ProfitWell provides a world-class platform for subscription intelligence, and this integration allows you to retrieve real-time metrics (MRR, Churn, LTV), manage customer history, and update subscription data directly from your chat interface.

### What you can do

- **Metric & Revenue Orchestration** — Retrieve monthly and daily subscription metrics programmatically to maintain a clear overview of your business growth.
- **Customer Lifecycle Intelligence** — Access and monitor detailed customer history, including subscription changes and churn events directly from the AI interface.
- **Subscription & Manual Data Control** — Create, update, and 'un-churn' subscriptions via natural language to keep your revenue data synchronized.
- **Retention & LTV Monitoring** — Retrieve retention metrics and customer lifetime value (LTV) metadata to ensure your unit economics are always optimized.
- **Operational Monitoring** — Track system health and manage plan metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your ProfitWell Private API Token from your integration settings
3. Start managing your subscription metrics from Claude, Cursor, or any MCP-compatible client

No more manual exporting of CSV results for basic churn checks. Your AI acts as a dedicated revenue analyst or growth coordinator.

### Who is this for?

- **Founders & Growth Leads** — quickly retrieve revenue summaries and monitor churn trends without switching apps.
- **Finance Operations Teams** — automate the retrieval of subscription metadata and track retention metrics via natural conversation.
- **Customer Success Managers** — streamline the retrieval of customer history and monitor account health directly within the chat.


## Available Tools
- **churn_subscription**: Mark churn event
- **create_subscription**: Add new subscriber
- **get_customer_history**: Get billing history
- **get_daily_metrics**: Get daily growth stats
- **exclude_customer**: g. test accounts).

Exclude from metrics
- **get_account_status**: Get API status
- **list_subscription_plans**: List product plans
- **get_customer_ltv**: Get Lifetime Value
- **get_monthly_metrics**: Get monthly financial stats
- **get_retention_stats**: Get churn metrics
- **unchurn_subscription**: Reverse a cancellation
- **update_subscription**: Update subscription


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProfitWell** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all monthly metrics for my account."

**🤖 AI Agent:**
> I've retrieved your metrics. For this month, your MRR is $15,200 with a 2.5% churn rate. Would you like to see the daily breakdown?

---

**👤 You:**
> "Show me our MRR trend for the last 6 months with churn and expansion breakdown."

**🤖 AI Agent:**
> MRR trend (Dec-May): $124K, $131K, $138K, $142K, $149K, $156K (current). Net growth: $32K (+25.8%). Monthly breakdown for May: New MRR $12,400, Expansion $4,800, Contraction -$2,100, Churn -$8,100. Net new MRR: $7,000. Gross churn rate: 5.2% (down from 6.1% in Dec). Your LTV/CAC ratio improved to 4.2x. Customer count grew from 847 to 1,023.

---

**👤 You:**
> "Identify the top 10 customers at risk of churning based on engagement and usage patterns."

**🤖 AI Agent:**
> Top 10 at-risk customers identified by ProfitWell Retain analysis. #1: DataFlow Inc ($2,400/mo MRR) has not logged in for 18 days and usage dropped 78%. #2: CloudBridge ($1,800/mo) downgraded payment method. #3: TechVentures ($1,500/mo) submitted 3 support tickets about limitations. #4: ScaleUp ($1,200/mo) has declining API calls. Combined at-risk MRR: $14,200. Recommended actions: schedule check-in calls for top 5, send personalized feature discovery emails to the remaining 5.


## ❓ FAQ

**Q: Can my AI automatically find the MRR and churn metrics for the current month?**
Yes! Use the `get_monthly_metrics` tool. Your agent will respond with complete metadata for all key metrics, including MRR, churned revenue, and active customers in seconds.

**Q: How do I find my ProfitWell Private API Token?**
Log in to your ProfitWell/Paddle account, navigate to **Account Settings** > **Integrations**, and look for the **ProfitWell API** card to find your Private Token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/profitwell](https://vinkius.com/mcp/profitwell)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ProfitWell** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `profitwell` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ProfitWell** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "profitwell": {
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
