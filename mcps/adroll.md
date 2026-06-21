# AdRoll MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adroll)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/adroll-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/adroll-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

E-commerce marketing and retargeting — manage campaigns, ads, and performance via AI.

## Description
Connect your **AdRoll (NextRoll)** account to your AI agent to unlock professional e-commerce marketing and retargeting orchestration. From auditing your advertisable accounts to monitoring real-time campaign performance and managing creative ad assets, your agent handles your advertising ecosystem through natural conversation.

### What you can do

- **Campaign Management** — List and retrieve details for active campaigns across multiple channels (Web, Facebook, etc.)
- **Account Auditing** — List your 'Advertisables' (advertiser accounts) and retrieve technical metadata for each
- **Performance Reporting** — Retrieve granular statistics on clicks, spend, and conversions to monitor your marketing ROI
- **Creative Asset Oversight** — List and audit your ad creatives (banners, videos) to ensure your visual content is optimized
- **Strategy Insights** — Quickly identify high-performing strategies and identify areas for budget optimization directly from chat

### How it works

1. Subscribe to this server
2. Enter your AdRoll API Key and Access Token
3. Start managing your e-commerce ads and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Marketers** — automate campaign audits and performance tracking effortlessly
- **Growth Managers** — monitor retargeting ROI and identify the most profitable ad strategies
- **Ad Ops Specialists** — audit creative assets and advertisable configurations instantly
- **Marketing Analysts** — retrieve granular performance data for ROI analysis and reporting


## Available Tools
- **list_ads**: List ad creatives
- **list_advertisables**: List advertiser accounts
- **list_campaigns**: List active campaigns
- **get_campaign_details**: Get campaign metadata
- **get_performance_report**: Filterable by EID and date.

Get performance statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AdRoll** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active advertisable accounts in my AdRoll organization."

**🤖 AI Agent:**
> I've retrieved your advertisable accounts. You have 3 active advertisers: 'Gourmet Coffee Shop', 'Travel Essentials', and 'Outdoor Gear'. Which one would you like to audit?

---

**👤 You:**
> "Show me the performance of my Web Retargeting campaign for the last 7 days."

**🤖 AI Agent:**
> I've retrieved the 7-day stats for your Web Retargeting campaign. It generated 50,000 impressions, 250 clicks (0.5% CTR), and 15 conversions with a total spend of $300. Would you like to check the creative performance?

---

**👤 You:**
> "List all ad creatives for advertisable EID 'AD1234567890'."

**🤖 AI Agent:**
> I've retrieved the creatives for EID 'AD1234567890'. You have 12 assets including 8 static banners and 4 video ads. Would you like to see the status or dimensions for any of them?


## Installation & Usage

To install and use the **AdRoll** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adroll](https://vinkius.com/mcp/adroll)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
