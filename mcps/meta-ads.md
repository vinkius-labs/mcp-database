# Meta Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meta-ads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/meta-ads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/meta-ads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent with direct access to Meta Ads — manage Facebook and Instagram campaigns, track ad performance, and optimize spend without opening Meta Ads Manager.

## Description
Connect **Meta Ads** to your AI agent and manage Facebook and Instagram advertising conversationally.

### What you can do

- **Campaign Management** — List, create, update, and pause campaigns, ad sets, and ads across Facebook and Instagram.
- **Performance Analytics** — Pull impressions, reach, clicks, CTR, CPC, CPM, conversions, ROAS, and frequency metrics.
- **Audience Management** — Create custom audiences, lookalikes, and saved audiences with demographic and interest targeting.
- **Creative Insights** — Compare ad creative performance, view thumbnail engagement, and identify winning variants.

### How it works

1. Subscribe to the Meta Ads integration on the marketplace.
2. Create an app in Meta for Developers (developers.facebook.com → My Apps → Create App → Business type).
3. Ask your AI agent to manage campaigns, pull reports, or optimize budgets.

### Who is this for?

- **Performance Marketers** — Monitor and optimize the world's largest ad network with conversational analytics.
- **E-commerce Brands** — Track ROAS, conversion events, and product catalog campaigns across Facebook and Instagram.
- **Agencies** — Manage multiple client ad accounts with unified campaign intelligence.


## Available Tools
- **list_campaigns**: List all Meta ad campaigns
- **get_account_info**: Get ad account details
- **get_campaign_insights**: Get campaign performance metrics
- **list_ad_sets**: List ad sets in a campaign
- **list_ads**: List ads in an ad set
- **get_account_insights**: Get account-level performance
- **list_audiences**: List custom audiences
- **list_creatives**: List ad creatives
- **pause_campaign**: Can be reactivated later.

Pause a campaign
- **activate_campaign**: Activate a paused campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meta Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's my Meta ad spend and ROAS this month?"

**🤖 AI Agent:**
> This month: Total spend: $15,400. Reach: 2.1M. Impressions: 5.8M. Clicks: 42,000. CTR: 0.72%. CPC: $0.37. Purchases: 620. ROAS: 4.8x. Best campaign: 'Product Catalog Retargeting' (8.2x ROAS).

---

**👤 You:**
> "Which ad creatives are performing best?"

**🤖 AI Agent:**
> Top 3 creatives by ROAS: 1) Video 'Product Unboxing' (6.5x ROAS, $2.1K spend), 2) Carousel 'Summer Collection' (5.8x, $3.4K), 3) Static 'Testimonial - Sarah' (5.2x, $1.8K). Worst: 'Brand Story v3' (0.9x ROAS — consider pausing).

---

**👤 You:**
> "Create a lookalike audience from my top 1000 customers."

**🤖 AI Agent:**
> Lookalike audience created: 'Top 1K Customers - 1% Lookalike' in US. Estimated reach: 2.5M people. Similarity: 1% (highest match). Ready to use in campaigns.


## Installation & Usage

To install and use the **Meta Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meta-ads](https://vinkius.com/mcp/meta-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
