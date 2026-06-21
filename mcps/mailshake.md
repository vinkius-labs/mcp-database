# Mailshake MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailshake)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailshake-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailshake-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm-sales](../categories/crm-sales.md)

Manage cold outreach campaigns, leads, and prospects via the Mailshake REST API.

## Description
Connect your **Mailshake** account to any AI agent to automate your cold outreach and sales engagement workflows. This MCP server enables your agent to manage campaigns, promote prospects to lead status, and track email interactions directly from natural language interfaces.

### What you can do

- **Campaign Management** — List all outreach campaigns, retrieve detailed sequences, and pause or unpause sending
- **Lead Tracking** — Monitor qualified leads, retrieve interaction histories, and update prospect statuses
- **Prospect Ingestion** — Programmatically add new recipients to existing campaigns to keep your pipeline full
- **Message Insights** — List sent and received messages and retrieve full content for automated sentiment analysis or follow-up planning
- **Audience Oversight** — List all recipients in a campaign and monitor their individual engagement stages (Sent, Opened, Replied)

### How it works

1. Subscribe to this server
2. Enter your Mailshake API Key
3. Start managing your sales outreach from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — Quickly check campaign statuses and lead updates without opening the dashboard
- **Growth Marketers** — Automate the process of adding new prospects from research tools into active campaigns
- **Sales Operations** — Monitor outreach performance and audit message sequences via natural language commands


## Available Tools
- **add_prospects_to_campaign**: Requires a JSON body with recipient details.

Add new prospects to an existing campaign
- **list_outreach_campaigns**: List all outreach campaigns
- **get_campaign_details**: Get details for a specific campaign
- **get_lead_history**: Get history for a specific lead
- **get_message_content**: Get content for a specific email message
- **list_campaign_leads**: List qualified leads
- **list_outreach_messages**: List sent and received messages
- **pause_outreach_campaign**: Pause a running campaign
- **list_campaign_recipients**: List all recipients in a campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailshake** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active outreach campaigns in Mailshake."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active campaigns: 'Q3 SaaS Outreach (ID: 123)', 'Webinar Follow-up', and 'Partnership Requests'.

---

**👤 You:**
> "Show recent leads for the 'Partnership' campaign."

**🤖 AI Agent:**
> I found 5 recent leads for the Partnership campaign. Notable responses from 'John Smith' (Acme Corp) and 'Jane Doe' (Global Tech) are awaiting your follow-up.

---

**👤 You:**
> "Pause the campaign with ID '12345'."

**🤖 AI Agent:**
> Successfully paused campaign 12345. No more messages will be sent until you unpause the campaign.


## Installation & Usage

To install and use the **Mailshake** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailshake](https://vinkius.com/mcp/mailshake)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
