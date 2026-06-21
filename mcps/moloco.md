# Moloco MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moloco)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage machine learning-powered advertising via Moloco — track campaigns and get analytics directly from your AI agent.

## Description
Connect your **Moloco Ads** account to your AI agent and manage your programmatic advertising campaigns through natural conversation.

### What you can do

- **AdAccount Overview** — List all advertising accounts and view their high-level status and balances.
- **Campaign Tracking** — Fetch all campaigns for an account, monitor active ones, and update statuses (ENABLED/PAUSED).
- **AdGroup & Creative Insights** — List ad groups and creative asset groups to understand your target segments and visuals.
- **Performance Reporting** — Generate analytics reports for specific time ranges to track ROI and engagement.
- **Conversion Tracking** — View recorded conversion events and monitor attribution tracking links.
- **Deep Inspection** — Retrieve detailed configuration and metadata for specific campaigns.

### How it works

1. Subscribe to this server
2. Enter your Moloco API Key
3. Start managing your ads from Claude, Cursor, or any MCP client

### Who is this for?

- **Ad Managers** — quickly check campaign performance or pause underperforming ads without opening the Moloco portal.
- **Marketing Analysts** — automate the retrieval of performance reports and conversion data for analysis.
- **Growth Teams** — monitor ad account health, budget balances, and campaign distribution in real-time.


## Available Tools (10)
- **get_account_balance**: Check AdAccount balance
- **get_analytics_report**: Get performance analytics report
- **get_campaign**: Get campaign details
- **list_ad_accounts**: List Moloco AdAccounts
- **list_ad_groups**: List ad groups in a campaign
- **list_campaigns**: List campaigns in an AdAccount
- **list_conversions**: List recorded conversion events
- **list_creative_groups**: List creative asset groups
- **list_tracking_links**: List attribution tracking links
- **update_campaign_status**: g., ENABLED, PAUSED).

Update campaign status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moloco** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in my primary AdAccount."

**🤖 AI Agent:**
> I've fetched the campaigns for AdAccount 'AC-12345'. You have 4 active campaigns: 'Summer Sale 2024', 'Brand Awareness - Global', and 2 others. Shall I retrieve the performance report for 'Summer Sale 2024'?

---

**👤 You:**
> "Pause the campaign with ID cp_98765."

**🤖 AI Agent:**
> Status update initiated... The campaign 'cp_98765' has been successfully PAUSED. I'll continue to monitor your account balance and other active campaigns.

---

**👤 You:**
> "Check the balance for AdAccount AC-12345."

**🤖 AI Agent:**
> Retrieving balance... Your AdAccount AC-12345 has a remaining balance of $2,450.00 with a daily budget threshold of $500.00. Based on your current spend, this should last for approximately 5 days.


## ❓ FAQ

**Q: How do I get a Moloco API Key?**
You can generate an API Key in the Moloco Ads Developer Portal. This key allows the server to authenticate requests on your behalf.

**Q: Can I pause a campaign using this server?**
Yes! Use the `update_campaign_status` tool and set the status to 'PAUSED'. You can also re-enable it by setting the status to 'ENABLED'.

**Q: What kind of analytics reports can I generate?**
The `get_analytics_report` tool allows you to retrieve performance metrics for an AdAccount within a specific date range, helping you track spend, impressions, and conversions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moloco](https://vinkius.com/mcp/moloco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moloco** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moloco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moloco** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moloco": {
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
