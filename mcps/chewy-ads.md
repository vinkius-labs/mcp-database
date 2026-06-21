# Chewy Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chewy-ads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chewy-ads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chewy-ads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage retail media and sponsored products via Chewy Ads — track campaigns, monitor performance, and audit keywords directly from any AI agent.

## Description
Connect your **Chewy Ads (PromoteIQ)** account to any AI agent and take full control of your retail media operations through natural conversation. Streamline how you manage sponsored products and advertising performance on Chewy.

### What you can do

- **Campaign Oversight** — List and retrieve details for all active and inactive ad campaigns natively
- **Performance Intelligence** — Access detailed performance reports, including impressions, clicks, and spend flawlessly
- **Ad Group Logistics** — Monitor specific ad groups and individual product ads to optimize your reach securely
- **Keyword Management** — List and audit keywords and their associated performance metrics flawlessly
- **Budget Tracking** — Retrieve current account balance and budget statuses in real-time
- **Catalog Synchronization** — Access product catalogs synced with your ad account directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chewy Ads API Key and Client ID (obtained from your PromoteIQ dashboard)
3. Start managing your pet product advertising from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor ad performance and ROI for pet brands using natural language
- **Marketing Specialists** — audit keyword success and campaign statuses without opening the dashboard
- **Brand Owners** — quickly verify account balances and budget utilization straight from their chat interface
- **Retail Media Teams** — verify product synchronization and catalog health for advertising


## Available Tools
- **get_chewy_account_balance**: Retrieve the current account balance and budget status
- **get_campaign_details**: Get detailed information for a specific campaign
- **get_performance_report**: Retrieve a performance report for a specific period
- **list_campaign_adgroups**: List ad groups within a specific campaign
- **list_adgroup_ads**: List specific ads within an ad group
- **list_chewy_campaigns**: List all ad campaigns in the account
- **list_chewy_catalogs**: List product catalogs synced with the ad account
- **list_adgroup_keywords**: List keywords and their performance for an ad group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chewy Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active campaigns in Chewy Ads."

**🤖 AI Agent:**
> Retrieving your active campaigns... I found 3: 'Puppy Food Launch', 'Cat Litter Promo', and 'Summer Treats'. Would you like to see the performance for any of these?

---

**👤 You:**
> "What is my current account balance?"

**🤖 AI Agent:**
> Checking your account balance... Your current remaining budget is $1,250.00, and your daily cap is set to $100.00 across all active campaigns.

---

**👤 You:**
> "Show me the top 5 keywords for the 'Cat Litter' ad group."

**🤖 AI Agent:**
> Retrieving keywords for 'Cat Litter'... The top 5 by impressions are: 'clumping litter', 'dust free litter', 'cat sand', 'unscented litter', and 'odor control'.


## Installation & Usage

To install and use the **Chewy Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chewy-ads](https://vinkius.com/mcp/chewy-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
