# Cyberimpact MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cyberimpact)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cyberimpact-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cyberimpact-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage email subscribers, monitor campaigns, and track marketing metrics via the Cyberimpact API.

## Description
Integrate **Cyberimpact**, the Canadian email marketing platform, directly into your AI workflow. Manage your subscriber lists, monitor campaign performance, and track marketing automations using natural language.

### What you can do

- **Subscriber Management** — List, search, and retrieve profiles for your email subscribers.
- **Campaign Monitoring** — Track sent and scheduled email campaigns and their engagement metrics.
- **Automated Workflows** — Monitor active marketing automations and message templates.
- **Group Oversight** — Manage mailing lists and subscriber segments effectively via chat.

### How it works

1. Connect the Cyberimpact integration to your AI assistant.
2. Authorize using your Cyberimpact API Key (found in your account settings).
3. Orchestrate your email marketing strategy through intuitive conversation.

### Who is this for?

- **Email Marketers** — Quickly check campaign open rates and subscriber growth on the go.
- **Communications Teams** — Audit message templates and monitor scheduled broadcasts via chat.
- **Small Business Owners** — Manage their mailing lists and track engagement without complex workflows.


## Available Tools
- **add_subscriber**: Resolves the newly created subscriber ID. Mutates the subscriber database state.

Add a new subscriber to a specific group
- **get_account_details**: Resolves account identifiers and usage metrics. Interacts with the account and billing boundary.

Retrieve metadata and limits for your Cyberimpact account
- **get_campaign_details**: Resolves open rates, click rates, and bounce metrics. Interacts with the messaging analytics boundary.

Get performance metrics and settings for a specific campaign
- **get_subscriber_details**: Resolves custom fields, interaction history, and group memberships. Touches the granular subscriber profile boundary.

Get full profile and history for a specific subscriber
- **list_marketing_automations**: Resolves automation IDs and operational statuses. Interacts with the workflow automation engine.

List active automated marketing workflows
- **list_email_campaigns**: Resolves campaign IDs, titles, and delivery statuses. Touches the campaign management and messaging boundary.

List all sent and scheduled email campaigns
- **list_subscriber_groups**: Resolves group IDs, names, and member counts. Interacts with the audience segmentation boundary.

List all mailing lists and groups
- **list_subscribers**: Resolves subscriber IDs, email addresses, and subscription statuses. Interacts with the subscriber database boundary.

List all email subscribers in Cyberimpact
- **list_message_templates**: Resolves template identifiers and names. Touches the content management boundary.

List available email and automation templates
- **search_subscribers_by_email**: Resolves matching subscriber profiles. Touches the search and discovery boundary.

Search for a subscriber profile by email keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cyberimpact** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email subscriber groups."

**🤖 AI Agent:**
> I've found 4 groups in your account: 'General Newsletter', 'VIP Customers', 'Product Updates', and 'French Leads'. Would you like to see the subscriber count for any of these?

---

**👤 You:**
> "Show me the performance metrics for my last sent campaign."

**🤖 AI Agent:**
> Your latest campaign 'Monthly Digest - June' was sent to 1,200 recipients. It has a 28% open rate and a 4% click rate. No significant unsubscriptions were reported. Should I pull a detailed report?

---

**👤 You:**
> "Search for subscriber 'user@example.com'."

**🤖 AI Agent:**
> I found the profile for 'user@example.com'. They are currently 'Active' and a member of the 'General Newsletter' and 'VIP Customers' groups. Would you like to see their full interaction history?


## Installation & Usage

To install and use the **Cyberimpact** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cyberimpact](https://vinkius.com/mcp/cyberimpact)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
