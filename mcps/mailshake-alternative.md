# Mailshake MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailshake-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailshake-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailshake-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Run cold email outreach campaigns with personalization, automated follow-ups, and reply detection that fills your sales pipeline.

## Description
Connect your **Mailshake** account to any AI agent and manage sales outreach through natural conversation.

### What you can do

- **Campaign Management** — Create and manage outreach campaigns
- **Lead Tracking** — Browse leads with engagement status and activity
- **Sequence Management** — Configure multi-step email sequences
- **Reply Monitoring** — Track replies, opens, and click activity
- **Team Performance** — Monitor team outreach metrics and quotas
- **Lead Lists** — Import and manage prospect lists

### How it works

1. Subscribe to this server
2. Enter your Mailshake API Key
3. Start managing outreach from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SDRs** — manage outbound campaigns and track engagement
- **Sales Teams** — monitor reply rates and lead quality
- **Growth** — scale cold outreach with analytics


## Available Tools
- **add_prospects**: Add new prospects
- **get_campaign_details**: Get campaign info
- **get_user_profile**: Get profile info
- **get_team_details**: Get account team
- **list_engagement_activity**: Get open/click activity
- **list_campaigns**: List cold email campaigns
- **list_sales_leads**: List qualified leads
- **list_campaign_recipients**: List recipients
- **pause_campaign**: Stop campaign sending
- **pause_prospect**: Stop outreach for user
- **resume_campaign**: Resume campaign sending
- **update_lead_status**: g., Reply, Won, Lost, Ignored).

Set lead stage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailshake** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all campaigns and reply rates."

**🤖 AI Agent:**
> Campaigns: 5 active. 'Q2 Outbound' (450 leads, 42% open, 8% reply ⭐). 'Product Demo' (200, 38% open, 12% reply ⭐). 'Follow-up Series' (150, 35% open, 6% reply). 'Partner Outreach' (80, 45% open, 10%). 'Re-engagement' (120, 28% open, 4%). Total sent: 3,200. Avg reply: 7.8%. Interested: 89 leads.

---

**👤 You:**
> "Show leads from Q2 Outbound and their engagement."

**🤖 AI Agent:**
> Q2 Outbound: 450 leads. Replied: 36 (8%). Interested: 18 (4%). Meeting booked: 8 (1.8%). Not interested: 12. No reply: 414. Step breakdown: Step 1 (450 sent, 42% open), Step 2 (380, 35%), Step 3 (320, 30%). Top engaged: sarah@acme.com (opened 3x, clicked 2x, replied ✅).

---

**👤 You:**
> "Show team performance and daily sending quotas."

**🤖 AI Agent:**
> Team: 3 reps. Sarah — 180 leads, 12% reply ⭐, 6 meetings. Mike — 150 leads, 8% reply, 4 meetings. Lisa — 120 leads, 6% reply, 2 meetings. Daily quota: 200/rep (600 total). Used today: 145 (24%). Best day: Tuesday (highest open rates). Best time: 9-10 AM EST.


## Installation & Usage

To install and use the **Mailshake** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailshake-alternative](https://vinkius.com/mcp/mailshake-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
