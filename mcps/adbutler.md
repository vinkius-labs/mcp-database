# AdButler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adbutler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Ad serving and reporting — manage publishers, zones, campaigns, and ad performance via AI.

## Description
Connect your **AdButler** account to your AI agent to unlock professional ad serving management and real-time reporting. From auditing publisher inventory to monitoring campaign delivery and analyzing click-through rates (CTR), your agent handles your ad operations through natural conversation.

### What you can do

- **Inventory Management** — List publishers and ad zones to maintain full control over where your advertisements are displayed
- **Campaign Oversight** — List and retrieve details for self-serve campaigns, including statuses and targeting rules
- **Performance Reporting** — Retrieve instant statistics on impressions, clicks, and revenue across your entire network
- **Creative Auditing** — List and manage ad creative assets to ensure your visual content is always up-to-date
- **Revenue Optimization** — Quickly identify top-performing zones or underdelivering campaigns directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your AdButler Secret API Key
3. Start managing your ad serving and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Ad Ops Managers** — automate campaign audits and inventory checks without manual dashboard diving
- **Digital Publishers** — monitor zone performance and publisher earnings on the fly
- **Marketing Analysts** — retrieve ad performance data for ROI analysis and reporting
- **Ad Network Administrators** — manage multiple publishers and zones using simple natural language commands


## Available Tools
- **list_campaigns**: Retrieve a list of active and pending self-serve advertising campaigns in AdButler
- **list_publishers**: Retrieve the full list of publishers managing ad inventory in your AdButler network
- **list_zones**: Requires Publisher ID.

Retrieve the active ad zones (placements) linked to a specific AdButler publisher
- **list_creatives**: Retrieve the library of ad assets (banners, videos) stored in your AdButler account
- **get_performance_report**: Provide a specific metric type and optional dates.

Retrieve aggregated ad performance metrics (impressions, clicks, CTR) across zones and campaigns in AdButler


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AdButler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all publishers in my AdButler network."

**🤖 AI Agent:**
> I've retrieved the list of publishers. You have 10 active publishers, including 'Tech Daily', 'News Corp', and 'Gaming Hub'. Would you like to see the zones for any of them?

---

**👤 You:**
> "Show me the performance report for the last 7 days."

**🤖 AI Agent:**
> I've retrieved your 7-day performance report. Your network served 1.2M impressions with 5,400 clicks (CTR: 0.45%) and generated $3,200 in revenue. Which metric would you like to dive deeper into?

---

**👤 You:**
> "List all active zones for publisher ID 12345."

**🤖 AI Agent:**
> I've found 5 active zones for publisher 12345: 'Sidebar Banner', 'Top Leaderboard', 'Interstitial', and others. Would you like to check the current fill rate for these zones?


## ❓ FAQ

**Q: Where do I find my AdButler API Key?**
Log in to your AdButler dashboard, go to **Settings** > **API Settings**. You can generate your Secret API Key there. Note that API access requires the API add-on to be enabled.

**Q: Can I see real-time impressions and clicks?**
Yes! Use the `get_report` tool to retrieve up-to-the-minute statistics for your campaigns, zones, or entire network.

**Q: Does this server support creative management?**
Yes, you can use the `list_creatives` tool to audit and manage the ad assets associated with your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adbutler](https://vinkius.com/mcp/adbutler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AdButler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `adbutler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AdButler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adbutler": {
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
