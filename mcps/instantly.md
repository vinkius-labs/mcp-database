# Instantly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/instantly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/instantly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/instantly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Equip your AI agent with direct access to Instantly — manage cold email campaigns, track deliverability, and scale outreach across unlimited sending accounts.

## Description
Connect **Instantly** to your AI agent and manage your high-volume cold email platform conversationally.

### What you can do

- **Campaign Management** — Create, pause, resume, and monitor email campaigns with engagement metrics.
- **Lead Management** — Add, update, and search leads across campaigns with custom variables.
- **Account Warm-up** — Monitor email warm-up progress and deliverability scores across sending accounts.
- **Analytics** — Track opens, replies, bounces, and campaign-level performance in real time.

### How it works

1. Subscribe to the Instantly integration on the marketplace.
2. Generate an API key from your Instantly dashboard (Settings → API → Create API Key).
3. Ask your AI agent to manage campaigns, add leads, or check deliverability.

### Who is this for?

- **Cold Email Agencies** — Manage dozens of client campaigns and sending accounts from one interface.
- **SDR Teams** — Scale outreach across multiple email accounts while monitoring deliverability health.
- **Growth Hackers** — Automate high-volume cold outreach with AI-driven campaign management.


## Available Tools
- **add_leads**: Add leads to a campaign
- **get_account_stats**: Get account summary stats
- **get_campaign**: Get campaign details
- **get_campaign_analytics**: Get campaign analytics
- **list_accounts**: List sending accounts
- **list_campaigns**: List all campaigns
- **list_leads**: List leads in a campaign
- **list_subsequences**: List campaign subsequences
- **pause_campaign**: Pause a campaign
- **resume_campaign**: Resume a campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Instantly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the open rate on my 'SaaS Founders Q2' campaign?"

**🤖 AI Agent:**
> Campaign 'SaaS Founders Q2': 1,200 leads enrolled. Open rate: 62%, Reply rate: 9%, Bounce rate: 1.8%. Sent from 8 accounts. Top performing variant: Subject line B (71% open rate).

---

**👤 You:**
> "Check warm-up status on all my sending accounts."

**🤖 AI Agent:**
> You have 12 sending accounts. 8 are fully warmed (score 90+), 3 in progress (scores 45-70, ETA 2 weeks), and 1 just started (score 15, ETA 4 weeks). All accounts showing healthy inbox placement rates above 85%.

---

**👤 You:**
> "Add 50 leads to the 'Enterprise Outreach' campaign."

**🤖 AI Agent:**
> 50 leads added to 'Enterprise Outreach'. 48 accepted, 2 skipped (duplicates already in campaign). They'll start receiving emails based on your campaign schedule and sending account rotation.


## Installation & Usage

To install and use the **Instantly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/instantly](https://vinkius.com/mcp/instantly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
