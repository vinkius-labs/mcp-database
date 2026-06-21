# Amplitude MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplitude)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Analyze product data via Amplitude — get user activity, calculate retention, analyze funnels, and track revenue directly from any AI agent.

## Description
Connect your **Amplitude** account to your AI agent and seamlessly query behavioral data and product analytics using natural language.

### What you can do

- **User Activity & Search** — Search for specific users and track their detailed event stream to diagnose individual journeys
- **Funnels & Conversions** — Request step-by-step conversion funnels to identify where users drop off
- **Retention** — Generate day-over-day retention curves to understand how well features keep users engaged
- **Segmentation** — Query event counts and uniques over time to see clear adoption trends
- **Cohorts** — List your behavioral cohorts, view sizes, and request exports for further targeted analysis
- **Active Users & Revenue** — Instantly pull DAU/WAU/MAU and daily revenue metrics right into your workflow

### How it works

1. Subscribe to this server
2. Enter your Amplitude Project API Key and Secret Key
3. Start answering product questions directly via Claude, Cursor, or any MCP-compatible client

Never break your context to build dashboards. Ask your agent, get real-time data.

### Who is this for?

- **Product Managers** — rapidly test hypotheses by asking for funnel conversions or feature retention without coding
- **Data Analysts** — export raw events, find out user activity, and cross-reference cohorts easily
- **Customer Success** — debug specific user sessions by pulling their exact event activity stream
- **Growth Teams** — monitor daily revenue and active users instantly from your workspace


## Available Tools
- **export_events**: Amplitude is a product analytics platform. Pass start/end as YYYYMMDDTHH (e.g. 2026010100).

Export raw Amplitude event data for a time range
- **get_user_activity**: Useful for diagnosing individual user journeys.

Get Amplitude user activity stream
- **event_segmentation**: Pass event name, start/end as YYYYMMDD.

Query Amplitude event segmentation
- **search_users**: Useful to find specific users before checking their activity.

Search Amplitude users by user ID, device ID, or email
- **get_retention**: Pass start_event (acquisition), return_event, start/end dates. Start/End should be YYYYMMDD.

Query Amplitude retention
- **get_funnel**: Pass comma-separated event names, start/end as YYYYMMDD.

Query Amplitude funnel conversion
- **list_cohorts**: Cohorts group users by behavior.

List Amplitude behavioral cohorts
- **get_cohort**: Depending on the backend this may require polling until ready.

Request an Amplitude cohort download
- **revenue_analysis**: Start/End as YYYYMMDD.

Get Amplitude revenue analysis by day
- **active_users**: Start/End as YYYYMMDD.

Get Amplitude daily/weekly/monthly active users (DAU/WAU/MAU)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplitude** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's our funnel conversion from 'Landing_Page_View' to 'Sign_Up_Success' for the last 3 days?"

**🤖 AI Agent:**
> I checked the conversion funnel. Over the last 3 days, 14,200 users triggered 'Landing_Page_View'. Of those, 2,840 completed 'Sign_Up_Success'. This represents an overall conversion rate of 20%, which is slightly above our weekly average.

---

**👤 You:**
> "Show the recent user activity for customer email@example.com"

**🤖 AI Agent:**
> I've pulled the activity stream for email@example.com. In the last 2 hours, they logged in, triggered 'Payment_Initiated', but then hit an error on 'Payment_Gateway_Failed'. You might want to review the exact property payload.

---

**👤 You:**
> "What is our Daily Active Users (DAU) count since start of the month?"

**🤖 AI Agent:**
> I fetched the DAU data. Since the 1st of the month, DAU has ranged from 45,000 to 52,000. Yesterday hit a peak at 52,104, reflecting our recent campaign launch. Would you like a breakdown of revenue from this period?


## ❓ FAQ

**Q: Can my AI agent debug a specific user dropping out of our onboarding?**
Yes. Search for the user by their email or ID using `search_users`, completely avoiding the manual lookup. Then, ask your agent to pull their raw activity stream via `get_user_activity`. The agent will retrieve all events triggered by this user, making it simple to spot exactly where they failed or stopped interacting.

**Q: Can I request funnel conversions without building a dashboard manually?**
Absolutely. You can provide a sequence of events (e.g., 'Homepage Viewed', 'Sign Up Clicked', 'Account Created') and ask for the funnel conversion for the last 7 days. Your AI agent queries Amplitude and parses the exact drop-off rates at each step right into your prompt window.

**Q: How does the cohort fetching work for custom targeted segments?**
Your agent can list all available cohorts associated with your project. Once you find the target cohort's ID, you can use the `get_cohort` tool to request its download URL. This is incredibly useful for instantly moving targeted lists of power-users or churned-users into your other workflows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplitude](https://vinkius.com/mcp/amplitude)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amplitude** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amplitude` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amplitude** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amplitude": {
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
