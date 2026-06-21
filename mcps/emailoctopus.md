# EmailOctopus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emailoctopus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/emailoctopus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/emailoctopus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage email campaigns, track contact lists, and monitor reports via the EmailOctopus API.

## Description
Integrate **EmailOctopus**, the affordable and powerful email marketing platform, directly into your AI workflow. Manage your marketing lists and subscriber profiles, track email campaigns and their real-time statuses, monitor detailed performance reports, and oversee your entire marketing operation using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed information and status for all your email marketing campaigns.
- **Contact Intelligence** — Monitor contact address lists, individual profile details, and subscription statuses across your organization.
- **Performance Monitoring** — Access real-time campaign performance summaries, resolving sent, open, and click-through counts via chat.
- **Marketing Auditing** — Retrieve high-level summaries of list volumes, campaign activity, and organizational marketing health instantly.

### How it works

1. Connect the EmailOctopus integration to your AI assistant.
2. Authorize using your EmailOctopus API Key (found in your account settings).
3. Orchestrate your email marketing and subscriber management through intuitive conversation.

### Who is this for?

- **Email Marketers** — Quickly check campaign performance and list subscriber counts on the go.
- **CRM Managers** — Research contact profiles and list memberships via chat during segmentation.
- **Operations Teams** — Monitor marketing volumes and organizational campaign metadata instantly.


## Available Tools
- **get_campaign_performance_summary**: Get a summary of performance metrics for a specific campaign
- **get_campaign_details**: Get detailed settings for a specific email campaign
- **get_contact_profile**: Get full profile and history for a specific contact
- **get_list_details**: unsubscribed counts and organizational markers.

Get detailed settings and subscriber counts for a specific list
- **quick_marketing_volume_audit**: Retrieve a high-level summary of list and campaign activity
- **list_marketing_lists**: List all contact lists in your EmailOctopus account
- **list_email_campaigns**: List all email marketing campaigns in your account
- **list_list_contacts**: List all contacts within a specific marketing list
- **list_successfully_sent_campaigns**: Identify campaigns that have already been sent to subscribers
- **search_contacts_by_email**: Search for a contact within a list using their email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EmailOctopus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my marketing lists."

**🤖 AI Agent:**
> I've found 3 lists, including 'Product Updates' (1,200 subscribers) and 'Weekly Newsletter' (5,500 subscribers). Would you like to see the details for the Weekly Newsletter?

---

**👤 You:**
> "Show me the performance report for campaign 'Q1 Promo'."

**🤖 AI Agent:**
> Campaign 'Q1 Promo' was sent to 5,450 recipients. It has 1,230 opens (22.5%) and 450 clicks (8.2%). Status is 'Sent'. Should I check which links were clicked the most?

---

**👤 You:**
> "Search for contact 'jane@example.com' in the Weekly Newsletter list."

**🤖 AI Agent:**
> Jane is a member of 'Weekly Newsletter' and is currently 'Subscribed'. They joined on February 10th. Should I pull their complete field data?


## Installation & Usage

To install and use the **EmailOctopus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emailoctopus](https://vinkius.com/mcp/emailoctopus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
