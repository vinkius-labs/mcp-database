# Facebook Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/facebook-ads)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Facebook and Meta Ads via AI — list campaigns, track performance insights, and update ad status directly through your agent.

## Description
Connect your **Facebook Ads** (Meta Marketing) account to any AI agent and take full control of your advertising campaigns through natural conversation.

### What you can do

- **Campaign Management** — List all campaigns, fetch detailed settings, and update statuses (ACTIVE/PAUSED) directly from the cloud
- **Ad Set & Ad Inspection** — Drill down into specific ad sets and ads to review targeting, budgets, and creative details
- **Performance Insights** — Extract granular metrics like impressions, clicks, spend, reach, and CPC to analyze your ROI
- **Account Overview** — Retrieve ad account metadata including balance, currency, and overall account status
- **Identity Context** — Verify the authorized user and access level for the connected marketing token

### How it works

1. Subscribe to this server
2. Enter your Facebook Ads Access Token and Ad Account ID
3. Start managing your advertising from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Marketers** — monitor campaign performance and pause underperforming ads instantly
- **Business Owners** — check advertising spend and reach metrics through simple natural language questions
- **Growth Teams** — integrate ad management and insights directly into your AI-powered marketing workflow


## Available Tools (12)
- **get_ad_account_info**: Get basic info for the Facebook Ad Account
- **get_ad_details**: Get details for a specific ad
- **get_ad_set_details**: Get details for a specific ad set
- **get_campaign_details**: Get details for a specific campaign
- **get_insights**: Get performance insights for the Ad Account
- **get_me**: Get current token identity info
- **list_ad_sets**: List ad sets in the Ad Account
- **update_ad_status**: Update the status of an ad
- **update_campaign_status**: Update the status of a campaign
- **list_campaigns**: List campaigns in the Ad Account
- **update_ad_set_status**: Update the status of an ad set
- **list_ads**: List ads in the Ad Account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Facebook Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in my ad account."

**🤖 AI Agent:**
> Fetching active campaigns... You have 3 active campaigns: 'Spring Launch 2024' (ID: 123), 'Brand Awareness - Global' (ID: 456), and 'Retargeting - EU' (ID: 789). Would you like to see the daily spend for any of these?

---

**👤 You:**
> "Show me the performance insights for the last week."

**🤖 AI Agent:**
> Analyzing account insights... Over the last 7 days, your account generated 125,000 impressions and 2,400 clicks with a total spend of $1,250. Your average CPC is $0.52.

---

**👤 You:**
> "Pause campaign 123456789."

**🤖 AI Agent:**
> Updating campaign status... Campaign 123456789 ('Spring Launch') has been successfully PAUSED.


## ❓ FAQ

**Q: How do I find my Facebook Ad Account ID?**
You can find your Ad Account ID in the **Meta Ads Manager**. It's the numeric ID shown in the URL or account selector. Ensure you provide it without the 'act_' prefix.

**Q: Can I pause an underperforming campaign using this agent?**
Yes! Use the `update_campaign_status` tool and set the status to `PAUSED`. You can also resume it later by setting it back to `ACTIVE`.

**Q: Which performance metrics are available in the insights?**
The `get_insights` tool provides comprehensive data including impressions, clicks, total spend, reach, CPC (cost per click), CTR (click-through rate), and CPP (cost per purchase).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/facebook-ads](https://vinkius.com/mcp/facebook-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Facebook Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `facebook-ads` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Facebook Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "facebook-ads": {
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
