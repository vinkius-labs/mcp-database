# GaggleAMP MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gaggleamp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gaggleamp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gaggleamp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Amplify your brand reach through employee advocacy with curated social sharing activities that boost organic engagement.

## Description
Connect your **GaggleAMP** manager account to any AI agent and take full control of your employee advocacy and B2B social marketing workflows through natural conversation.

### What you can do

- **Activity Orchestration** — List and manage social sharing tasks (LinkedIn, Twitter) and retrieve detailed engagement metrics programmatically
- **Advocate CRM** — Manage your complete directory of members and retrieve detailed profiles, including point balances and impact scores
- **Gamification Control** — Access global and Gaggle-specific leaderboards to identify top performers and monitor your program's social footprint
- **Reward Automation** — List redeemable items and process reward claims for members using their earned points directly through your agent
- **Team Onboarding** — Programmatically invite new advocates to your Gaggle and manage team structures to scale your social reach

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your GaggleAMP Manager Dashboard (Settings > Integrations)
3. Start managing your employee advocacy program from Claude, Cursor, or any MCP client

No more manual status checking or complex activity creation through slow web dashboards. Your AI acts as your dedicated advocacy program manager.

### Who is this for?

- **Marketing Managers** — instantly launch new sharing activities and track campaign reach using natural language
- **Social Media Leads** — monitor top advocate performance and identify content that resonates best with the team
- **HR & Culture Teams** — manage employee recognition and reward redemptions without leaving your workspace


## Available Tools
- **create_activity**: Add new task for members
- **get_activity_engagement**: Get stats for activity
- **get_top_advocates**: Get rankings
- **get_account_details**: Get user profile
- **get_member_points**: Check point balance
- **invite_new_advocate**: Invite to Gaggle
- **list_activities**: List available activities
- **list_all_gaggles**: List accessible Gaggles
- **list_gaggle_members**: List all advocates
- **list_reward_history**: Get claimed rewards
- **list_available_rewards**: List redeemable items
- **redeem_reward_item**: Process reward claim


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GaggleAMP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active social activities in my Gaggle."

**🤖 AI Agent:**
> I've retrieved your activities. You have 5 active tasks, including a LinkedIn share for the 'Q3 Product Update' and a Twitter like request. Would you like the engagement stats for any of these?

---

**👤 You:**
> "Who are the top 3 performers in the leaderboard right now?"

**🤖 AI Agent:**
> Retrieving rankings... Currently, the top performers are 'John Smith' (1,200 points), 'Sarah Jane' (950 points), and 'Michael Scott' (880 points). John has the highest social reach this month.

---

**👤 You:**
> "Show me all available rewards and their point costs."

**🤖 AI Agent:**
> Scanning reward catalog... You have 4 items available: 'Gift Card' (500 pts), 'Company Swag' (300 pts), 'Extra Day Off' (2,000 pts), and 'Charity Donation' (100 pts). Should I check the redemption history?


## Installation & Usage

To install and use the **GaggleAMP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gaggleamp](https://vinkius.com/mcp/gaggleamp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
