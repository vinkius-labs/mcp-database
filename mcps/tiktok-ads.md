# TikTok Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tiktok-ads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tiktok-ads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tiktok-ads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent with direct access to TikTok Ads — manage campaigns, track ad performance, and optimize spend without opening TikTok Ads Manager.

## Description
Connect **TikTok Ads** to your AI agent and manage your TikTok advertising campaigns conversationally.

### What you can do

- **Campaign Management** — List, create, update, and pause campaigns, ad groups, and individual ads.
- **Performance Analytics** — Pull impressions, clicks, CTR, CPC, CPM, conversions, and ROAS across date ranges.
- **Budget Optimization** — Adjust daily and lifetime budgets, bidding strategies, and targeting parameters.
- **Audience Insights** — Query audience demographics, interests, and engagement patterns.

### How it works

1. Subscribe to the TikTok Ads integration on the marketplace.
2. Create an app in the TikTok Developers portal and get your credentials (developers.tiktok.com → Manage Apps → Create App).
3. Ask your AI agent to manage campaigns, pull reports, or optimize budgets.

### Who is this for?

- **Performance Marketers** — Monitor and optimize TikTok ad spend with real-time conversational analytics.
- **Agencies** — Manage multiple client TikTok advertising accounts from one interface.
- **E-commerce Brands** — Track ROAS, conversion data, and product catalog performance.


## Available Tools
- **enable_campaign**: Enable a campaign
- **list_campaigns**: List all TikTok ad campaigns
- **list_adgroups**: List all TikTok ad groups
- **list_ads**: List all TikTok ads
- **get_campaign_reporting**: Get campaign performance
- **get_adgroup_reporting**: Get ad group performance
- **get_ad_reporting**: Get ad performance
- **pause_campaign**: Pause a campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TikTok Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's my TikTok ad spend this week?"

**🤖 AI Agent:**
> This week's TikTok Ads summary: Total spend: $3,420. Impressions: 1.2M. Clicks: 18,400. CTR: 1.53%. CPC: $0.19. Conversions: 245. ROAS: 4.2x. Top campaign: 'Summer Collection' ($1,800 spend, 5.1x ROAS).

---

**👤 You:**
> "Pause all ads with ROAS below 2x."

**🤖 AI Agent:**
> Found 3 ads with ROAS below 2x. Paused: 'Product Demo v2' (ROAS: 1.1x), 'Brand Awareness Fall' (ROAS: 0.8x), 'New Arrivals Teaser' (ROAS: 1.5x). Savings: ~$450/day.

---

**👤 You:**
> "Compare my campaign performance this month vs last month."

**🤖 AI Agent:**
> Month-over-month comparison: Spend: $12,400 (+8%). Impressions: 4.8M (+15%). CTR: 1.61% (+0.12pp). ROAS: 3.8x (-0.3x). Conversions: 890 (+12%). CPC dropped 5% — efficiency is improving but ROAS dipped slightly.


## Installation & Usage

To install and use the **TikTok Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tiktok-ads](https://vinkius.com/mcp/tiktok-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
