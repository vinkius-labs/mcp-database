# Walmart Connect Ads MCP Server

Manage Walmart Sponsored Search campaigns, budgets, keywords, and performance reports with AI. Exclusive for Walmart Connect Partner Network members.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/walmart-connect-ads)

## Overview
**Category:** industry-titans
**Tools Count:** 8

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


## Installation & Usage

To install and use the **Walmart Connect Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/walmart-connect-ads](https://vinkius.com/mcp/walmart-connect-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
