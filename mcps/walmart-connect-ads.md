# Walmart Connect Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/walmart-connect-ads)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Walmart Sponsored Search campaigns, budgets, keywords, and performance reports with AI. Exclusive for Walmart Connect Partner Network members.

## Description
### What you can do

Take complete control of your Walmart Connect Advertising campaigns with full Sponsored Search API access:

- **Track Ad Campaigns:** Monitor campaign performance with real-time CPC, ROAS, and conversion metrics.
- **Execute Budgets & CPCs:** Set and adjust daily budgets per campaign to maintain profitable ROAS targets.
- **Handle Keyword Auctions:** Optimize keyword bids and discover high-performing search terms within Walmart Connect.

### How it works

1. **Hybrid WCPN Authentication:** Combines OAuth 2.0 token generation with RSA-SHA256 request signing, matching the exact security model required by the Walmart Connect Partner Network.
2. **Isolated Ad Access:** Exclusively targets advertising endpoints — your product catalog and inventory remain untouched.

### Who is this for?

Built for **Advertising Agencies**, **Growth Managers**, and **E-Commerce Advertisers** managing Sponsored Search campaigns.

> **Prerequisite:** You must be an approved Walmart Connect Partner Network (WCPN) partner with valid API credentials (Consumer ID, Private Key) issued during onboarding.


## Available Tools
- **ads_add_keywords**: Each keyword needs a text, match type (exact, phrase, or broad), and a bid amount in dollars. Send keywords as a JSON array string, e.g. [{"keyword":"laptop stand","matchType":"broad","bid":1.50}].

Add new keywords to a Sponsored Search ad group
- **ads_get_cpc_metrics**: Data lag is approximately 1-3 hours. Optionally filter by a single campaign ID.

Retrieve near real-time spend, impression, and click metrics for active campaigns
- **ads_get_keyword_performance**: Optionally filter by campaign ID or ad group ID to narrow results.

List keywords and their performance data for the advertiser account
- **ads_get_item_health_report**: Supported report types: adGroup, adItem, keyword, itemHealth, placement, platform, category, brand, pageType, attributedPurchases, searchImpression, videoCampaigns, videoKeywords, outOfBudgetRecommendations, itemKeyword. A reportDate (yyyy-MM-dd) is optional for most types but required for date-bound reports.

Generate a performance snapshot report for the advertiser account
- **ads_create_ad_group**: Create a new ad group within a Sponsored Search campaign
- **ads_list_campaigns**: Supports optional filtering by campaign ID or campaign name.

List all Sponsored Search advertising campaigns for the authorized advertiser account
- **ads_pause_campaign**: Pause an active Sponsored Search campaign
- **ads_update_daily_budget**: Budget is in dollars.

Update the daily budget for a specific Sponsored Search campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Walmart Connect Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze active Walmart Connect campaigns and list their current daily budgets."

**🤖 AI Agent:**
> Successfully queried Connect Ads. Found 3 campaigns active bounding daily constraints correctly.

---

**👤 You:**
> "Increase the bid on the exact keyword 'laptop stand' from $0.50 to $0.75 in Campaign A."

**🤖 AI Agent:**
> Operation successful. The bid for keyword 'laptop stand' has been updated to $0.75 in the targeted ad group.

---

**👤 You:**
> "Generate a performance report for all Sponsored Products over the last 30 days."

**🤖 AI Agent:**
> Report generation initiated. Extracting Cost-Per-Click statistics and total ROAS metrics for the requested 30-day window.


## ❓ FAQ

**Q: Can the LLM alter my product images using this MCP?**
No. This MCP server targets Advertising endpoints only. To alter catalog media, use the general `walmart-marketplace-mcp`.

**Q: Can I adjust Cost-Per-Click bids dynamically?**
Yes, you can monitor auction performance and instruct the agent to increase or decrease bids on specific converting keywords or ad groups natively.

**Q: Does this tool extract long-term advertising performance reports?**
Absolutely. It runs async snapshot reports downloading dense ROI, ROAS, and conversion metrics directly from Walmart's ad exchange.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/walmart-connect-ads](https://vinkius.com/mcp/walmart-connect-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Walmart Connect Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `walmart-connect-ads` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Walmart Connect Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "walmart-connect-ads": {
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
