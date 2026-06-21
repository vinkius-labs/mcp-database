# Snapchat Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snapchat-ads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/snapchat-ads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/snapchat-ads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent with direct access to Snapchat Ads — manage campaigns, track ad performance, and optimize spend without opening Snapchat Ads Manager.

## Description
Connect **Snapchat Ads** to your AI agent and manage your Snapchat advertising conversationally.

### What you can do

- **Campaign Management** — List, create, update, and pause campaigns, ad squads, and individual ads.
- **Performance Analytics** — Pull impressions, swipe-ups, story views, conversions, and ROAS metrics.
- **Audience Management** — Create and manage custom audiences, lookalikes, and Snap Audience Match lists.
- **Creative Insights** — Track performance per creative variant and identify top-performing stories and lenses.

### How it works

1. Subscribe to the Snapchat Ads integration on the marketplace.
2. Create an app in the Snap Developer Portal (kit.snapchat.com → Manage Apps → Create App).
3. Ask your AI agent to manage campaigns, pull analytics, or manage audiences.

### Who is this for?

- **Performance Marketers** — Optimize Snapchat ad spend targeting Gen Z and Millennial demographics.
- **Agencies** — Manage multiple client Snapchat ad accounts from one conversational interface.
- **D2C Brands** — Track story ad engagement, AR lens performance, and shopping conversion attribution.


## Available Tools
- **list_campaigns**: List campaigns
- **list_adsquads**: List ad squads
- **list_ads**: List ads
- **get_campaign_stats**: Get campaign statistics
- **get_account_stats**: Get account statistics
- **pause_campaign**: Pause a campaign
- **enable_campaign**: Enable a campaign
- **get_ad_account**: Get ad account info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snapchat Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How are my Snapchat campaigns performing this week?"

**🤖 AI Agent:**
> This week: Total spend: $1,850. Impressions: 820K. Swipe-ups: 3,400. Swipe-up rate: 0.41%. eCPSU: $0.54. Conversions: 89. ROAS: 3.1x. Top: 'Back to School Story' (1.8x ROAS).

---

**👤 You:**
> "Create a lookalike audience based on my best customers."

**🤖 AI Agent:**
> Lookalike audience created: 'Top Customers Lookalike' based on 2,400 seed users. Estimated reach: 1.2M users in US (18-34). Ready to assign to campaigns.

---

**👤 You:**
> "Pause any ad squads with spend over $500 and ROAS below 1.5x."

**🤖 AI Agent:**
> Found 2 ad squads matching criteria. Paused: 'Broad Awareness 18-24' ($620 spend, 0.9x ROAS) and 'Interest - Gaming' ($540 spend, 1.2x ROAS). Estimated daily savings: ~$165.


## Installation & Usage

To install and use the **Snapchat Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snapchat-ads](https://vinkius.com/mcp/snapchat-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
