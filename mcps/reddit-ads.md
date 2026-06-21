# Reddit Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reddit-ads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/reddit-ads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/reddit-ads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage your Reddit Ads campaigns — audit accounts, ad groups, and reports via AI.

## Description
Empower your AI agent to orchestrate your entire advertising ecosystem on Reddit with **Reddit Ads**, the platform for reaching the most passionate communities on the internet. By connecting Reddit Ads to your agent, you transform complex campaign management into a natural conversation. Your agent can instantly list your ad accounts, audit campaign performance, and retrieve detailed reporting without you ever touching a dashboard. Whether you are running brand awareness or performance-driven ads, your agent acts as a real-time ad operator, ensuring your marketing is always optimized and data-backed.

### What you can do

- **Account Auditing** — List all ad accounts in your profile and retrieve detailed metadata for each, including status and IDs.
- **Campaign Oversight** — List all campaigns and ad groups to maintain a structured view of your advertising efforts.
- **Ad Management** — Query individual ads and creative assets to ensure your content is correctly published and active.
- **Performance Intelligence** — Retrieve detailed advertising reports with flexible dates and granularity to understand ROI.
- **Asset Governance** — List all creative assets in your account to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your Reddit Ads Access Token
3. Start managing your ad data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — monitor daily ad spend and campaign statuses straight from your workflow.
- **Ad Ops Specialists** — verify if new ad groups and creatives have been correctly configured and are live.
- **Growth Leads** — perform rapid audits of advertising performance and ROI without manual dashboard logins.
- **Business Owners** — automate ad querying to orchestrate your growth strategy smoothly.


## Available Tools
- **get_campaign**: Get details for a specific campaign
- **get_ad_account**: Get details for a specific ad account
- **get_ad_group**: Get details for a specific ad group
- **get_ad**: Get details for a specific ad
- **get_report**: Get an advertising report
- **list_ad_accounts**: List Reddit Ads accounts
- **list_ad_groups**: List Reddit Ads ad groups
- **list_ads**: List Reddit Ads
- **list_campaigns**: List Reddit Ads campaigns
- **list_creative_assets**: List creative assets for an account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reddit Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Reddit ad accounts."

**🤖 AI Agent:**
> I've retrieved your ad accounts. You have 2 accounts: 'Vinkius Main' and 'Test Account'. Which one would you like to audit for campaigns?

---

**👤 You:**
> "Show me my active campaigns for account ID t2_xxxx."

**🤖 AI Agent:**
> I've found 3 active campaigns in that account: 'Spring Launch', 'Community Outreach', and 'B2B Demo'. I can provide performance summaries for any of them.

---

**👤 You:**
> "Get an ads report for last week."

**🤖 AI Agent:**
> I've generated your report for last week. Your total spend was $450 with an average CPC of $0.85. Would you like a breakdown by ad group?


## Installation & Usage

To install and use the **Reddit Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reddit-ads](https://vinkius.com/mcp/reddit-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
