# Apple Search Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apple-search-ads)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage and optimize your Apple Search Ads campaigns — track performance, keywords, and search terms via AI.

## Description
The **Apple Search Ads MCP Server** empowers your AI agent to directly manage your advertising campaigns on the App Store. Gain deep insights into your marketing performance, optimize keyword targeting, and monitor search term trends using natural language.

### Key Features

- **Campaign Management** — List all campaigns, view detailed settings, and monitor budget allocation.
- **Ad Group Oversight** — Drill down into ad groups within your campaigns to see granular configurations.
- **Performance Reporting** — Generate comprehensive reports at the campaign, ad group, keyword, and search term levels.
- **Keyword Intelligence** — Retrieve keyword-level metrics to understand what drives conversions and high ROI.
- **Search Term Discovery** — Identify the exact terms users are typing to find your app and adjust your bidding strategy accordingly.
- **Real-time Analytics** — Monitor impressions, clicks, and conversions across different granularities (hourly, daily, monthly).

### Benefits for Teams

- **UA Managers** — Quickly audit campaign performance and budget status without manually exporting reports.
- **Growth Marketers** — Use AI to discover high-performing search terms and identify negative keyword opportunities.
- **Product Teams** — Understand user intent by analyzing the search queries that lead to app installs.


## Available Tools
- **get_account_check**: Verify Apple Search Ads account connection
- **get_campaign_report**: Get performance report at the campaign level
- **get_campaign**: Get details for a specific campaign
- **get_keyword_report**: Get performance report for keywords
- **get_me**: Retrieve information about the authenticated user and organization
- **get_search_term_report**: Get performance report for search terms
- **get_ad_group_report**: Get performance report for ad groups
- **list_ad_groups**: List ad groups within a campaign
- **list_campaigns**: List all search ads campaigns
- **list_keywords**: List all keywords in a campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apple Search Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Apple Search Ads campaigns."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 4 active campaigns, including 'USA - Brand', 'UK - Generic', and 'Canada - Competitors'.

---

**👤 You:**
> "Show me the performance report for campaign ID '987654321' for last week."

**🤖 AI Agent:**
> For campaign '987654321', you had 12,500 impressions, 1,200 clicks, and 450 conversions last week, with a CPT of $0.85.

---

**👤 You:**
> "What were the top 5 search terms for campaign ID '123456789' yesterday?"

**🤖 AI Agent:**
> The top 5 search terms yesterday were: 'fitness app', 'workout tracker', 'home workout', 'gym guide', and 'health monitor'.


## ❓ FAQ

**Q: How do I get my Apple Search Ads API credentials?**
Log in to Apple Search Ads, navigate to **Settings > API**, and generate a public/private key pair. Upload the public key to receive your Client ID, Team ID, and Key ID.

**Q: What is the 'orgId'?**
The `orgId` identifies your specific organization or account within Apple Search Ads. You can find it in your account settings or in the URL when logged into the dashboard.

**Q: Is there a limit on search term reports?**
Yes, Apple enforces a privacy threshold. Search term reports only return data for terms that have at least 10 impressions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apple-search-ads](https://vinkius.com/mcp/apple-search-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apple Search Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apple-search-ads` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apple Search Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apple-search-ads": {
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
