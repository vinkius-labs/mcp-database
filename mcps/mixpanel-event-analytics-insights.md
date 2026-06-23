# Mixpanel (Event Analytics & Insights) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mixpanel-event-analytics-insights)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage product analytics via Mixpanel — query event trends, track conversion funnels, and audit user cohorts.

## Description
Connect your **Mixpanel** account to any AI agent and take full control of your product analytics, user behavior tracking, and conversion insights through natural conversation.

### What you can do

- **Event Orchestration** — Query aggregate event occurrences and unique user trends over specific date intervals to understand high-level feature engagement directly from your agent
- **Conversion Analysis** — Calculate step-by-step conversion rates and drop-offs for saved 'Funnels' to identify bottlenecks in your user journey securely
- **Retention Monitoring** — Compute user retention curves and recurring action return rates to understand long-term product stickiness and cohort behavior natively
- **Deep Segmentation** — Execute property-based breakdowns to split any event by specific attributes (e.g., plan type, region, device) for granular analytical insights
- **User Profile Audit** — Query distinct user profiles using proprietary JQL expression variables to retrieve detailed company metadata and user traits instantly
- **Behavioral Cohorts** — List and retrieve size metrics for saved user segments (Cohorts) to identify high-value audiences or risky churn segments securely
- **Raw Data Export** — Extract atomic event logs for deep-dive investigations or external reporting pipelines, maintaining literal chronological event fidelity

### How it works

1. Subscribe to this server
2. Enter your Mixpanel Service Account (User/Secret) and Project ID
3. Start exploring your product data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — audit feature adoption and monitor conversion funnels through natural conversation without manual report generation
- **Growth Leads** — track retention trends and experiment with property-based segmentation to optimize user acquisition directly from your workspace
- **Data Analysts** — retrieve raw event logs and query user profiles via JQL for rapid diagnostic investigations efficiently


## Available Tools (10)
- **list_cohorts**: List saved behavioral cohorts
- **list_funnels**: List all saved funnel configurations
- **query_retention**: Calculate user retention curves
- **query_top_events**: Get the top 20 events by volume
- **query_events**: Query aggregate Mixpanel event counts over time
- **export_events**: Note: This API is rate-limited to 60 requests per hour.

Export raw event data logs
- **query_funnel**: Get conversion data for a specific funnel
- **query_insights**: Query complex dashboard insights
- **query_profiles**: g., properties["plan"]=="pro").

Search for specific user profiles
- **query_segmentation**: g., device or region).

Break down an event by specific properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mixpanel (Event Analytics & Insights)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 5 events by volume in my project for the last 7 days"

**🤖 AI Agent:**
> Retrieving top events… I've identified the highest volume triggers: 1) 'Session Start' (45k), 2) 'Page View' (38k), 3) 'Button Click' (12k), 4) 'Search Query' (8k), and 5) 'Checkout Success' (2k). Would you like to segment 'Checkout Success' by region?

---

**👤 You:**
> "Query retention from 'User Signup' to 'App Open' for Feb 2026"

**🤖 AI Agent:**
> Computing retention curve… For the February cohort, Day 1 retention was 45%, dropping to 18% by Day 7 and stabilizing at 12% by Day 30. This is 5% higher than your January cohort. Would you like me to check the retention for 'Pro' users specifically?

---

**👤 You:**
> "List all active user cohorts in my project"

**🤖 AI Agent:**
> I've retrieved 4 behavioral cohorts: 'Power Users' (Size: 1,250), 'Trial Expired' (Size: 4,500), 'Recent Churn' (Size: 890), and 'iOS Users' (Size: 12,450). Which cohort would you like to query profile traits for?


## ❓ FAQ

**Q: Can I query my conversion funnels through my agent?**
Yes. Use the `query_funnel` tool with a specific Funnel ID and date range. Your agent will retrieve the step-by-step conversion percentages and drop-off counts, allowing you to identify exactly where users are leaving your flow.

**Q: How do I filter user profiles using specific properties through a conversation?**
The `query_profiles` tool allows your agent to execute JQL expressions. You can ask your agent to find users matching literal conditions like `properties['plan'] == 'pro'`, and it will retrieve the corresponding profiles and metadata securely.

**Q: Can my agent check user retention for my application?**
Absolutely. Use the `query_retention` tool by providing a 'born' event (first action) and a recurring 'return' event. Your agent will compute the N-Day retention curve, showing you how sticky your product is for specific user cohorts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mixpanel-event-analytics-insights](https://vinkius.com/mcp/mixpanel-event-analytics-insights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mixpanel (Event Analytics & Insights)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mixpanel-event-analytics-insights` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mixpanel (Event Analytics & Insights)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mixpanel-event-analytics-insights": {
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
