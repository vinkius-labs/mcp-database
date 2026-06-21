# TikTok Full Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tiktok-full-ads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tiktok-full-ads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tiktok-full-ads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Complete TikTok Ads management � create campaigns, control budgets, analyze performance, track conversions, and manage creative assets via AI.

## Description
Empower your AI agent to orchestrate your entire advertising ecosystem on TikTok with the **TikTok Business API**, the platform for reaching the most engaged audience in short-form video. By connecting TikTok Ads to your agent, you transform complex campaign management into a natural conversation. Your agent can instantly list your advertiser accounts, audit ad group performance, and retrieve detailed analytics without you ever touching a dashboard. Whether you are scaling e-commerce sales or building brand presence, your agent acts as a real-time ad strategist, ensuring your marketing is always creative and data-driven.

### What you can do

- **Advertiser Auditing** — List all advertiser accounts associated with your app and retrieve detailed metadata for each.
- **Campaign Oversight** — List and audit campaigns, ad groups, and individual ads to maintain a structured view of your efforts.
- **Creative Intelligence** — Query creative assets and metadata to ensure your video content is correctly published and active.
- **Integrated Reporting** — Retrieve performance reports with flexible dates and dimensions to understand conversion and ROI.
- **Audience Management** — List custom audiences to ensure your targeting strategy is correctly implemented.

### How it works

1. Subscribe to this server
2. Enter your TikTok Ads Access Token
3. Start managing your ad data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Buyers** — monitor daily spend and ad group status straight from your workflow.
- **Growth Engineers** — verify if tracking and custom audiences are correctly configured and active.
- **Marketing Managers** — perform rapid audits of campaign performance and creative assets without manual logins.
- **Business Owners** — automate ad querying to orchestrate your TikTok-driven growth strategy smoothly.


## Available Tools
- **get_advertiser_balance**: Get the current balance and spending of an advertiser
- **list_ads**: List all ads for an advertiser
- **list_audiences**: List custom audiences for retargeting
- **create_campaign**: Objective types: TRAFFIC, CONVERSIONS, APP_INSTALL, REACH, VIDEO_VIEWS, LEAD_GENERATION, CATALOG_SALES.

Create a new TikTok Ads campaign
- **get_ad_group_details**: Get details for specific ad groups
- **get_advertiser_info**: Get TikTok advertiser account details
- **get_campaign_details**: Get full details of specific campaigns by ID
- **update_ad_status**: Enable, disable, or delete ads
- **get_performance_report**: ) and dimensions (campaign_id, adgroup_id, ad_id, stat_time_day) for granular analysis.

Get advanced performance reports with custom metrics
- **list_ad_groups**: List all ad groups for an advertiser
- **list_campaigns**: Supports pagination.

List all campaigns for an advertiser
- **list_ad_images**: List uploaded image assets for an advertiser
- **list_ad_videos**: List uploaded video assets for an advertiser
- **track_pixel_event**: g., CompletePayment, AddToCart, ViewContent, SubmitForm) via server-to-server tracking.

Send a server-side pixel event to TikTok
- **update_ad_group_status**: Enable, disable, or delete ad groups
- **update_campaign_budget**: Update budget for an existing campaign
- **update_campaign_status**: Enable, disable, or delete campaigns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TikTok Full Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my TikTok advertiser accounts."

**🤖 AI Agent:**
> I've retrieved your advertiser accounts associated with App ID '12345'. You have 2 accounts: 'Vinkius Global' and 'Vinkius BR'. Which one would you like to audit?

---

**👤 You:**
> "Show me my active campaigns for advertiser ID 67890."

**🤖 AI Agent:**
> I've found 3 active campaigns in that account: 'Summer Promo', 'App Install Drive', and 'Brand Reveal'. I can provide budget and performance info for each.

---

**👤 You:**
> "Get a performance report for advertiser 67890 for last month."

**🤖 AI Agent:**
> I've generated the integrated report. Your total spend was $1,500 with 250,000 impressions and a CTR of 1.2%. Would you like a breakdown by ad group?


## Installation & Usage

To install and use the **TikTok Full Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tiktok-full-ads](https://vinkius.com/mcp/tiktok-full-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
