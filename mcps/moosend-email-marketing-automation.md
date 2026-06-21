# Moosend (Email Marketing & Automation) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moosend-email-marketing-automation)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moosend-email-marketing-automation-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moosend-email-marketing-automation-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing via Moosend — create campaigns, track mailing lists, and audit performance analytics.

## Description
Connect your **Moosend** account to any AI agent and take full control of your email marketing automation, audience management, and campaign performance through natural conversation.

### What you can do

- **Campaign Orchestration** — List, retrieve, and create new email campaigns directly from your agent, including subject lines and verified sender settings securely
- **Audience CRM** — Manage your mailing lists, retrieve detailed member profiles, and add or remove subscribers with precise status indicators natively
- **Live Execution** — Command your agent to send drafted campaigns immediately, triggering the physical outbound email pipeline with a single instruction
- **Performance Analytics** — Extract detailed performance logs for sent campaigns, tracking opens, clicks, bounces, and unsubscribes to understand engagement benchmarks
- **List Management** — Create new audience hubs and retrieve precise metadata mapping bounces and custom field boundaries across your organization
- **Subscriber Audit** — Query literal email lists to verify member statuses and iterate through audience chunks to maintain a clean and optimized subscriber directory

### How it works

1. Subscribe to this server
2. Enter your Moosend API Key
3. Start managing your marketing presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — audit campaign results and monitor audience growth through natural conversation without manual dashboard navigation
- **Growth Engineers** — automate the management of subscriber statuses and verify campaign tracking settings directly from your workspace
- **Business Owners** — get rapid summaries of newsletter performance and manage customer lists across multiple Moosend hubs efficiently


## Available Tools
- **add_subscriber**: Add a subscriber to a mailing list
- **create_campaign**: Create a new email campaign
- **create_mailing_list**: Create a new mailing list
- **get_campaign_stats**: Get performance metrics for a campaign
- **get_mailing_list**: Get details for a specific mailing list
- **list_campaigns**: List all email campaigns
- **list_mailing_lists**: List all mailing lists in Moosend
- **list_subscribers**: List subscribers in a mailing list
- **remove_subscriber**: Remove a subscriber from a mailing list
- **send_campaign**: Trigger the delivery of a campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moosend (Email Marketing & Automation)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Moosend mailing lists"

**🤖 AI Agent:**
> I've retrieved your mailing lists: 'Main Newsletter' (ID: 12345, 12,450 members), 'Product Beta' (ID: 67890, 450 members), and 'Event Leads' (ID: 13579). Which one would you like to add a subscriber to?

---

**👤 You:**
> "Show me the performance stats for campaign ID 'camp-98765'"

**🤖 AI Agent:**
> Retrieving stats for 'Spring Sale Update'… The campaign achieved a 22.5% open rate and a 4.2% click rate. There were 45 bounces and 12 unsubscribes. Engagement is trending 15% higher than last month. Would you like to see the click breakdown?

---

**👤 You:**
> "Send campaign ID 'camp-12345' now"

**🤖 AI Agent:**
> Triggering broadcast… I've successfully dispatched campaign 'camp-12345' to your 'Main Newsletter' list. The emails are now in the Moosend outbound queue. I'll notify you once the initial delivery metrics are available.


## Installation & Usage

To install and use the **Moosend (Email Marketing & Automation)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moosend-email-marketing-automation](https://vinkius.com/mcp/moosend-email-marketing-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
