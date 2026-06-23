# Criteo Marketing API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/criteo-marketing-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent to manage Criteo marketing campaigns, ad sets, and budgets directly via the Criteo API.

## Description
Integrate the **Criteo Marketing API** directly into your AI workflow. Manage your commerce marketing campaigns, monitor ad set performance, and track budgets and creatives across your advertiser accounts using natural language.

### What you can do

- **Campaign Management** — List and retrieve detailed settings for all your marketing campaigns.
- **Performance Monitoring** — Access real-time statistics and analytics for your ad sets and creatives.
- **Budget Tracking** — Monitor active budgets and spend across your advertiser portfolio.
- **Audience Insights** — Explore target audiences and available audience segments via chat.

### How it works

1. Connect the Criteo Marketing integration to your AI assistant.
2. Authorize using your Criteo Client ID and Client Secret (found in the Criteo Developer Portal).
3. Orchestrate your commerce marketing strategy through intuitive conversation.

### Who is this for?

- **Performance Marketers** — Quickly check campaign statuses and budget utilization on the go.
- **Digital Advertisers** — Audit ad creatives and monitor performance metrics via chat.
- **E-commerce Teams** — Track advertiser accounts and target audiences during project planning.


## Available Tools (10)
- **get_ad_set_details**: Get detailed configuration for an ad set
- **get_campaign_details**: Get detailed settings for a specific campaign
- **get_marketing_statistics**: Retrieve performance statistics for campaigns or ad sets
- **list_ad_sets**: List all ad sets (groups) within campaigns
- **list_advertisers**: List advertisers managed in your account
- **list_audiences**: List target audiences for your campaigns
- **list_marketing_budgets**: List active budgets and their spend
- **list_marketing_campaigns**: List all marketing campaigns in Criteo
- **list_ad_creatives**: List all ad creatives (banners, videos, etc.)
- **list_audience_segments**: List available audience segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Criteo Marketing API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns in my Criteo account."

**🤖 AI Agent:**
> I've found 5 active campaigns, including 'Spring Promotion 2024' and 'Retargeting Global'. Would you like to see the budget allocation for these?

---

**👤 You:**
> "Show me the performance statistics for ad set 's8s9df7' from last week."

**🤖 AI Agent:**
> For ad set 's8s9df7', you had 12,000 impressions, 450 clicks, and a conversion rate of 3.2% last week. The total spend was $1,250. Should I compare this to the previous week?

---

**👤 You:**
> "List all target audiences available for my advertisers."

**🤖 AI Agent:**
> I've retrieved 10 target audiences, including 'Frequent Shoppers', 'Cart Abandoners', and 'New Visitors'. Which audience would you like to target in your next campaign?


## ❓ FAQ

**Q: How do I get Criteo API credentials?**
Log in to the Criteo Developer Portal, create a new app, and you will be provided with a Client ID and Client Secret.

**Q: Which version of the API is used?**
This integration uses the 2024-04 version of the Criteo Marketing API, ensuring access to the latest features and data structures.

**Q: Can I retrieve reporting data?**
Yes, you can use the get_marketing_statistics tool to retrieve performance reports based on custom dimensions and metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/criteo-marketing-api](https://vinkius.com/mcp/criteo-marketing-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Criteo Marketing API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `criteo-marketing-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Criteo Marketing API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "criteo-marketing-api": {
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
