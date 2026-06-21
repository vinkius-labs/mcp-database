# Google Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-ads-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-ads-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-ads-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent with direct access to Google Ads — manage search, display, and shopping campaigns, track conversions, and optimize ad spend without opening the Google Ads console.

## Description
Connect **Google Ads** to your AI agent and manage the world's largest advertising platform conversationally.

### What you can do

- **Campaign Management** — List, create, update, and pause search, display, shopping, video, and performance max campaigns.
- **Performance Analytics** — Pull impressions, clicks, CTR, CPC, conversions, conversion value, ROAS, quality score, and search impression share.
- **Keyword Management** — Add, pause, and optimize keywords with bid adjustments, negative keywords, and match type changes.
- **Audience & Targeting** — Manage audience segments, location targeting, demographic adjustments, and remarketing lists.

### How it works

1. Subscribe to the Google Ads integration on the marketplace.
2. Create OAuth credentials in Google Cloud Console (console.cloud.google.com → APIs & Services → Credentials → Create OAuth Client ID).
3. Get your Google Ads Developer Token from your Manager account.
4. Ask your AI agent to manage campaigns, pull reports, or optimize bids.

### Who is this for?

- **PPC Managers** — Monitor and optimize Google Ads campaigns with real-time conversational analytics.
- **E-commerce Brands** — Track shopping campaign ROAS, product group performance, and conversion attribution.
- **Agencies** — Manage multiple client Google Ads accounts from one unified interface.


## Available Tools
- **list_campaigns**: List all Google Ads campaigns
- **get_campaign**: Get campaign performance details
- **list_ad_groups**: List ad groups in a campaign
- **list_ads**: List ads in an ad group
- **list_keywords**: List keywords in a campaign
- **get_account_budget**: Get account budget info
- **get_performance_report**: Get daily performance report
- **list_conversion_actions**: List conversion tracking actions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's my Google Ads spend and ROAS this month?"

**🤖 AI Agent:**
> This month: Total spend: $24,800. Clicks: 38,200. CTR: 4.2%. Avg CPC: $0.65. Conversions: 1,420. Conv value: $98,400. ROAS: 3.97x. Top campaign: 'Brand Search' (12.4x ROAS). Worst: 'Broad Match Discovery' (1.1x).

---

**👤 You:**
> "Which keywords have the lowest quality score?"

**🤖 AI Agent:**
> 5 keywords with quality score below 5: 'cheap software' (QS: 3, CPC: $2.40), 'buy online tool' (QS: 4, CPC: $1.90), 'best app' (QS: 3, CPC: $3.10), 'platform pricing' (QS: 4, CPC: $2.20), 'tool comparison' (QS: 4, CPC: $1.75). Recommendation: improve landing page relevance or pause.

---

**👤 You:**
> "Pause all shopping campaigns with ROAS below 2x."

**🤖 AI Agent:**
> Found 2 shopping campaigns below 2x ROAS. Paused: 'Electronics Clearance' (ROAS: 1.3x, $4,200 spend) and 'Accessories Broad' (ROAS: 1.7x, $1,800 spend). Estimated daily savings: ~$450.


## Installation & Usage

To install and use the **Google Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-ads-1](https://vinkius.com/mcp/google-ads-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
