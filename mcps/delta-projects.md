# Delta Projects MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/delta-projects)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/delta-projects-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/delta-projects-mcp)
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


## Installation & Usage

To install and use the **Delta Projects** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/delta-projects](https://vinkius.com/mcp/delta-projects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
