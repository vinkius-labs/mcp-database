# Amazon Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-ads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amazon-ads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amazon-ads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Advertising management — manage Sponsored Products, brands, and performance reports via AI.

## Description
Connect your **Amazon Ads** account to your AI agent to unlock professional campaign orchestration and performance tracking. From auditing Sponsored Products and Sponsored Brands to generating asynchronous performance reports and managing keyword bids, your agent handles your e-commerce advertising strategy through natural conversation.

### What you can do

- **Profile Oversight** — Retrieve Amazon Ads profiles to manage campaigns across different global marketplaces
- **Campaign Orchestration** — List and audit Sponsored Products and Sponsored Brands campaigns to monitor active budgets
- **Ad Group & Keyword Management** — List ad groups and targeted keywords to ensure your products appear in the right search results
- **Performance Reporting** — Request and retrieve asynchronous reports to analyze clicks, impressions, and ad spend
- **Advertising Insights** — Quickly identify underperforming keywords or out-of-budget campaigns directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Amazon Ads Client ID, Client Secret, Refresh Token, and Region
3. Start managing your Amazon campaigns and monitoring ROAS through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Sellers** — automate campaign audits and monitor ad spend across global Amazon marketplaces
- **Performance Marketers** — retrieve granular keyword reports to optimize bidding strategies and maximize ROAS
- **Brand Managers** — audit Sponsored Brands campaigns and ensure brand visibility on critical search terms
- **Data Analysts** — generate and fetch asynchronous performance reports for external data visualization


## Available Tools
- **list_sb_keywords**: List SB keywords
- **list_sp_campaigns**: List Sponsored Products campaigns
- **list_sp_keywords**: List SP keywords
- **list_profiles**: List advertiser profiles
- **list_sp_ad_groups**: List SP ad groups
- **list_sb_campaigns**: List Sponsored Brands campaigns
- **request_sp_report**: Request performance report
- **get_report_status**: Check report status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my Amazon Ads profiles."

**🤖 AI Agent:**
> I've retrieved your advertising profiles. You have 2 profiles active: 'US Marketplace' (ID: 123456) and 'Canada Marketplace' (ID: 789012). Which profile's campaigns would you like to review?

---

**👤 You:**
> "Show me the active Sponsored Products campaigns for profile ID '123456'."

**🤖 AI Agent:**
> I've listed the active Sponsored Products campaigns for that profile. There are 5 running campaigns, including 'Holiday Promo' with a daily budget of $50.00 and 'Brand Defense' with a budget of $25.00.

---

**👤 You:**
> "Request a campaign performance report for yesterday (Profile ID '123456')."

**🤖 AI Agent:**
> I have successfully requested the Sponsored Products campaign report for yesterday. The Report ID is 'rep-abc-123'. Because Amazon generates reports asynchronously, it is currently processing. Would you like me to check its status and download the data now?


## Installation & Usage

To install and use the **Amazon Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-ads](https://vinkius.com/mcp/amazon-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
