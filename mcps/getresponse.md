# GetResponse MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getresponse)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/getresponse-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/getresponse-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing campaigns, track subscribers, and oversee newsletters via AI agents with GetResponse.

## Description
Connect your **GetResponse** account to any AI agent to automate your email marketing and audience engagement workflows through the Model Context Protocol (MCP). GetResponse is a scalable email marketing platform that helps businesses grow their lists and automate communication. This MCP server enables you to manage your mailing lists (campaigns), track subscriber profiles, and monitor newsletter performance directly through natural conversation.

### Key Features

- **Campaign & List Oversight** — List all mailing lists (campaigns) in your account and fetch detailed configuration metadata for each.
- **Subscriber Management** — Search and list contacts, retrieve detailed profile metadata, and programmatically add new subscribers to your lists.
- **Newsletter Tracking** — Access your history of sent and scheduled newsletters to monitor your broadcast strategy.
- **Performance Analytics** — Retrieve high-level statistics (opens, clicks, bounces) for your newsletters to measure engagement.
- **Automation Discovery** — List configured marketing automation workflows and signup forms to understand your lead acquisition funnel.
- **Webhook Monitoring** — List active webhooks to ensure your internal systems are receiving real-time campaign notifications.
- **Account Identity** — Fetch metadata for the authenticated GetResponse account to verify permissions and settings.
- **Real-time Synchronization** — Keep your marketing data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GetResponse API Key (found in Integrations and API)
3. Start managing your email marketing from Claude, Cursor, or any MCP client

### Who is this for?

- **Email Marketers** — quickly check newsletter performance or list recent subscribers without manual dashboard navigation.
- **Growth Engineers** — automate the synchronization of new leads and verify campaign settings via simple AI commands.
- **Account Managers** — get a real-time overview of client engagement and mailing list health seamlessly.


## Available Tools
- **verify_api_connection**: Check connection
- **add_new_subscriber**: Sync a contact
- **get_account_details**: Get account metadata
- **get_campaign_details**: Get campaign metadata
- **get_contact_details**: Get contact metadata
- **get_newsletter_analytics**: Get broadcast stats
- **list_marketing_campaigns**: List campaigns/lists
- **list_marketing_contacts**: List subscribers
- **list_marketing_forms**: List signup forms
- **list_marketing_newsletters**: List newsletters
- **list_marketing_webhooks**: List webhook configs
- **list_marketing_workflows**: List automation flows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GetResponse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email campaigns/lists in GetResponse."

**🤖 AI Agent:**
> Retrieving campaigns... I found 3 active lists: 'Main Newsletter' (ID: V), 'Product Updates' (ID: X), and 'Lead Magnets'. Which list would you like to see subscribers for?

---

**👤 You:**
> "Show me the performance stats for my last newsletter."

**🤖 AI Agent:**
> Fetching analytics... Your last newsletter 'October Update' had an Open Rate of 24.5% and a Click-Through Rate of 3.2% from 1,200 recipients.

---

**👤 You:**
> "Add 'John Doe' (john@example.com) to the 'Newsletter' list (ID: abc123)."

**🤖 AI Agent:**
> Subscriber added! I have successfully synchronized John Doe (john@example.com) to the 'Newsletter' list. He is now active in that campaign.


## Installation & Usage

To install and use the **GetResponse** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getresponse](https://vinkius.com/mcp/getresponse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
