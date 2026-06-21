# Digital Turbine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/digital-turbine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Equip your AI agent to manage mobile growth campaigns, track app monetization, and monitor performance via the Digital Turbine API.

## Description
Integrate **Digital Turbine**, the leading independent mobile growth platform, directly into your AI workflow. Manage your user acquisition campaigns, monitor app monetization performance, and track real-time revenue and install data using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed settings and performance metrics for all your growth and acquisition campaigns.
- **App Monetization Tracking** — Monitor your monetized mobile apps, including ad unit settings, floor prices, and active placements.
- **Performance Analytics** — Access high-level summaries of impressions, installs, and click-through rates (CTR).
- **Revenue Reporting** — Retrieve detailed financial telemetry for specific date ranges across your mobile portfolio.

### How it works

1. Connect the Digital Turbine integration to your AI assistant.
2. Authorize using your Digital Turbine API Key (found in your account settings).
3. Optimize your mobile growth and monetization strategy through intuitive conversation.

### Who is this for?

- **UA Managers** — Quickly check campaign delivery and acquisition costs on the go.
- **App Developers** — Monitor monetization performance and ad unit health via chat.
- **Growth Leads** — Audit overall performance metrics and revenue trends during strategy sessions.


## Available Tools
- **get_platform_metadata**: Retrieve metadata and limits for your Digital Turbine account
- **get_app_monetization_details**: Get detailed monetization settings and status for a specific app
- **get_campaign_analytics**: Get detailed settings and performance metrics for a specific campaign
- **get_performance_summary**: Retrieve high-level performance metrics including installs and CTR
- **get_revenue_report**: Retrieve a revenue report for a specific date range
- **list_monetized_apps**: List all mobile applications integrated for monetization
- **list_growth_campaigns**: List all mobile growth and acquisition campaigns in your Digital Turbine account
- **list_high_engagement_campaigns**: Identify campaigns with a CTR above a certain threshold (mock logic)
- **list_top_performing_apps**: Identify the apps with the highest revenue in your account (mock logic)
- **search_campaigns_by_name**: Search for a campaign using a name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Turbine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active UA campaigns."

**🤖 AI Agent:**
> I've found 4 active acquisition campaigns, including 'Global Android Launch' and 'US iOS Promo'. Would you like to see the current install count for the largest one?

---

**👤 You:**
> "Show me the revenue report for 'Game App X' from last week."

**🤖 AI Agent:**
> Last week, 'Game App X' generated $12,450 in ad revenue. The best performing placement was 'Rewarded Video - Main Menu'. Should I check the fill rate for this app?

---

**👤 You:**
> "What is the average CTR for our 'Summer Sale' campaign?"

**🤖 AI Agent:**
> The 'Summer Sale' campaign currently has an average CTR of 3.8%. Performance is highest on Android devices in the EU region. Would you like a breakdown by creative asset?


## ❓ FAQ

**Q: How do I get a Digital Turbine API Key?**
Log in to your Digital Turbine dashboard, navigate to the API section in your account settings, and you can generate or retrieve your unique API Key from there.

**Q: Can the agent show real-time install data?**
Yes, you can use the get_performance_summary tool to retrieve the latest reported install counts and engagement metrics for your campaigns.

**Q: Does the integration support revenue reporting?**
Yes, the get_revenue_report tool allows the agent to retrieve financial telemetry for specific date ranges, mapping earnings across your portolio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/digital-turbine](https://vinkius.com/mcp/digital-turbine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Turbine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `digital-turbine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Turbine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-turbine": {
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
