# LinkedIn Ads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-ads-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/linkedin-ads-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/linkedin-ads-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent with direct access to LinkedIn Ads — manage campaigns, track B2B ad performance, and optimize LinkedIn marketing spend without opening Campaign Manager.

## Description
Connect **LinkedIn Ads** to your AI agent and manage your B2B advertising campaigns conversationally.

### What you can do

- **Campaign Management** — List, create, update, and pause campaigns, campaign groups, and creatives.
- **B2B Analytics** — Pull impressions, clicks, CTR, CPC, leads, and cost-per-lead metrics.
- **Audience Targeting** — Query targeting by job title, company, industry, seniority, and matched audiences.
- **Lead Gen Forms** — Access lead gen form submissions and sync leads to your CRM.

### How it works

1. Subscribe to the LinkedIn Ads integration on the marketplace.
2. Create an app in the LinkedIn Developer Portal (developer.linkedin.com → My Apps → Create App).
3. Ask your AI agent to manage campaigns, pull reports, or download leads.

### Who is this for?

- **B2B Marketers** — Monitor and optimize LinkedIn ad spend targeting professionals and decision-makers.
- **Demand Gen Teams** — Track lead gen form submissions and campaign ROI conversationally.
- **Agencies** — Manage multiple client LinkedIn advertising accounts from one interface.


## Available Tools
- **list_campaign_groups**: List campaign groups
- **list_campaigns**: List campaigns
- **list_creatives**: List ad creatives
- **get_campaign_analytics**: Get campaign analytics
- **get_account_info**: Get ad account info
- **pause_campaign**: Pause campaign
- **enable_campaign**: Enable campaign
- **get_account_analytics**: Get account analytics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How are my LinkedIn campaigns performing this month?"

**🤖 AI Agent:**
> This month: Total spend: $8,200. Impressions: 340K. Clicks: 2,100. CTR: 0.62%. CPC: $3.90. Leads: 145. CPL: $56.55. Top campaign: 'VP Sales Targeting' (42 leads, $48 CPL).

---

**👤 You:**
> "Download all leads from my 'CTO Retargeting' campaign."

**🤖 AI Agent:**
> Downloaded 67 leads from 'CTO Retargeting'. Fields: name, email, company, job title, company size. 89% have valid business emails. Ready for CRM sync.

---

**👤 You:**
> "Increase the daily budget on 'Brand Awareness' campaign to $200."

**🤖 AI Agent:**
> Budget updated: 'Brand Awareness' daily budget changed from $150 to $200 (+33%). Estimated new daily reach: ~2,800 impressions (up from ~2,100).


## Installation & Usage

To install and use the **LinkedIn Ads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-ads-1](https://vinkius.com/mcp/linkedin-ads-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
