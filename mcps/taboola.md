# Taboola MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/taboola)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/taboola-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/taboola-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage Taboola advertising campaigns, ads, and performance reports directly from any AI agent.

## Description
Connect your **Taboola Backstage** account to any AI agent and take full control of your native advertising workflows through natural conversation.

### What you can do

- **Account Management** — List all allowed accounts and retrieve current user profile details
- **Campaign Control** — List, fetch, create, and update campaigns including budgets, CPC, and active status
- **Ad Management** — Manage campaign items (ads) by listing existing creatives or adding new URLs and thumbnails
- **Performance Reporting** — Run detailed campaign summary reports by dimension (day, week, month) or identify top-performing content

### How it works

1. Subscribe to this server
2. Enter your Taboola Client ID and Client Secret
3. Start optimizing your native ads from Claude, Cursor, or any MCP-compatible client

No more jumping between tabs to check CTR or adjust daily caps. Your AI acts as a dedicated Ad Ops specialist.

### Who is this for?

- **Digital Marketers** — instantly retrieve performance metrics and adjust campaign settings without opening Backstage
- **Ad Ops Teams** — automate the creation of campaign items and monitor account access across multiple clients
- **Growth Engineers** — integrate real-time ad performance data into development workflows for faster iteration


## Available Tools
- **list_allowed_accounts**: List allowed Taboola accounts
- **list_campaign_items**: List items (ads) in a campaign
- **create_campaign**: Create a new Taboola campaign
- **get_current_user**: Get current Taboola user details
- **get_campaign**: Get details for a specific campaign
- **get_top_campaign_content_report**: Get top campaign content report
- **update_campaign**: Update an existing Taboola campaign
- **get_campaign_summary_report**: Get campaign summary report
- **list_campaigns**: List campaigns for an account
- **create_campaign_item**: Create a new campaign item (ad)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Taboola** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Taboola accounts."

**🤖 AI Agent:**
> I've retrieved your accounts. You have access to: 'Global_Marketing_US' (ID: act-9821) and 'EMEA_Expansion' (ID: act-4432). Which one would you like to manage?

---

**👤 You:**
> "Get a summary report for account 'act-9821' grouped by day."

**🤖 AI Agent:**
> Fetching the daily summary for 'act-9821'... For the last period, you had 1.2M impressions, 4.5k clicks (0.37% CTR), and a total spend of $2,140. Would you like to see the top-performing items for this account?

---

**👤 You:**
> "Update campaign 'camp-556' in account 'act-9821' to change the CPC to '0.45'."

**🤖 AI Agent:**
> Updating campaign settings... The CPC for 'camp-556' has been successfully updated to 0.45. The campaign remains active with its current daily cap.


## Installation & Usage

To install and use the **Taboola** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taboola](https://vinkius.com/mcp/taboola)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
