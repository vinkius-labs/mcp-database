# Delta Projects MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/delta-projects)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage ad campaigns, monitor performance, and audit creatives via the Delta Projects API.

## Description
Integrate **Delta Projects**, the efficient programmatic advertising platform, directly into your AI workflow. Manage your digital ad campaigns, monitor real-time performance and budgets, and audit your ad creatives and placements using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed settings and performance metrics for all your ad campaigns.
- **Performance Reporting** — Retrieve custom reports on impressions, clicks, and conversions across various dimensions.
- **Creative Auditing** — List and review all ad creatives (banners, videos) uploaded to the platform.
- **Placement & Audience Insights** — Monitor media placements and explore target audiences available for your campaigns.

### How it works

1. Connect the Delta Projects integration to your AI assistant.
2. Authorize using your Delta Projects API Key (found in your account settings).
3. Optimize your programmatic advertising strategy through intuitive conversation.

### Who is this for?

- **Media Buyers & Planners** — Quickly check campaign delivery and budget pacing on the go.
- **Digital Marketers** — Audit creative assets and placement performance via chat.
- **Account Managers** — Gather structured campaign data and reports for client updates instantly.


## Available Tools
- **get_platform_metadata**: Retrieve metadata and configuration for your Delta Projects account
- **get_campaign_performance**: Get detailed settings and performance metrics for a specific campaign
- **get_custom_ad_report**: Retrieve a custom performance report based on specific dimensions
- **list_running_campaigns**: List only the ad campaigns that are currently active and serving
- **list_managed_advertisers**: List all advertisers configured in the platform
- **list_target_audiences**: List all first-party and third-party audiences available for targeting
- **list_ad_campaigns**: List all programmatic advertising campaigns in your Delta Projects account
- **list_ad_creatives**: List all creative assets (banners, videos) uploaded to the platform
- **list_media_placements**: List all configured ad placements and media sources
- **search_campaigns_by_name**: Search for an ad campaign using a keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Delta Projects** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active ad campaigns and their budgets."

**🤖 AI Agent:**
> I've found 4 active campaigns, including 'Summer Sale 2024' (Budget: $10,000) and 'Brand Awareness Q3' (Budget: $5,000). Would you like to see the current impression count for the largest one?

---

**👤 You:**
> "Show me the performance report for 'Summer Sale 2024' from yesterday."

**🤖 AI Agent:**
> Yesterday, 'Summer Sale 2024' generated 150,000 impressions and 1,200 clicks (CTR: 0.8%). Total spend for the day was $450. Should I pull a breakdown of performance by creative asset?

---

**👤 You:**
> "Search for ad creatives containing 'banner_300x250'."

**🤖 AI Agent:**
> I've found 3 creatives matching that term, including 'Summer_Sale_300x250.jpg' and 'Retargeting_Generic_300x250.html'. Would you like to see which campaigns are currently using these assets?


## ❓ FAQ

**Q: How do I get a Delta Projects API Key?**
Log in to your Delta Projects account and navigate to the API section in your settings to generate or retrieve your unique API Key.

**Q: Can the agent pause active campaigns?**
This integration currently focuses on listing and retrieving campaign performance and settings for monitoring purposes. Modifying campaign statuses should be handled via the Delta Projects dashboard.

**Q: Is real-time spending data included?**
Yes, when retrieving campaign details, the agent provides information on current budget usage and spent amounts as reported by the Delta Projects platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/delta-projects](https://vinkius.com/mcp/delta-projects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Delta Projects** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `delta-projects` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Delta Projects** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "delta-projects": {
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
