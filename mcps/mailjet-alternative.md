# Mailjet MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailjet-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailjet-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailjet-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Deliver emails at scale with collaborative template editing, real-time monitoring, and deliverability analytics in one platform.

## Description
Connect your **Mailjet** account to any AI agent and manage email operations through natural conversation.

### What you can do

- **Email Sending** — Send transactional and marketing emails at scale
- **Contact Management** — Manage contact lists with properties and segmentation
- **Template Management** — Browse, create, and manage email templates
- **Delivery Analytics** — Track opens, clicks, bounces, and spam reports
- **Campaign Management** — Create and monitor email campaigns
- **Statistics** — Access detailed sending statistics and trends

### How it works

1. Subscribe to this server
2. Enter your Mailjet API Key and Secret Key
3. Start managing email from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate email sending with rich APIs
- **Marketers** — manage campaigns and contact lists
- **Operations** — monitor deliverability and sender reputation


## Available Tools
- **subscribe_to_list**: Add contact to list
- **create_new_contact**: Add email to contacts
- **get_campaign_performance**: ) for a specific campaign ID.

Check campaign stats
- **get_account_analytics**: Check account stats
- **get_template_details**: Get template content
- **list_sent_campaigns**: List past campaigns
- **list_contact_groups**: List contact lists
- **list_all_contacts**: List audience contacts
- **list_sender_domains**: Check sending domains
- **list_email_templates**: List saved templates
- **send_plain_email**: Send transactional email
- **send_template_email**: Send using template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailjet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show sending statistics and contact list summary."

**🤖 AI Agent:**
> Sending (7 days): 18,400 emails. Delivered: 18,032 (98% ✅). Opens: 6,624 (36%). Clicks: 1,472 (8%). Bounced: 184 (1%). Blocked: 92 (0.5%). Spam: 12 (0.07%). Contact lists: 5. 'Newsletter' (8,200), 'Customers' (3,400), 'Leads' (2,100), 'Partners' (450), 'Beta' (340). Total: 14,490.

---

**👤 You:**
> "List email templates and send a transactional email."

**🤖 AI Agent:**
> Templates: 8. 'Welcome Email' (ID: 1234, used 5.2K times). 'Order Confirmation' (ID: 1235, 3.8K). 'Password Reset' (ID: 1236, 2.1K). 'Invoice' (ID: 1237, 1.2K). 4 others. Email sent! ✅ Template: 'Welcome Email'. To: sarah@company.com. Variables: {name: 'Sarah', plan: 'Pro'}. Status: Queued → Sent (0.3s).

---

**👤 You:**
> "Show campaign performance and bounce analysis."

**🤖 AI Agent:**
> Campaigns (last 5): 'April Newsletter' (8,200 sent, 38% open, 9% click ⭐). 'Product Launch' (3,400, 42% open, 12% click ⭐). 'Webinar Invite' (2,100, 35% open). 2 others. Bounce analysis: Total: 184 (1%). Hard: 45 (mailbox not found). Soft: 139 (temp issues). Top domains: gmail.com (8 bounces), outlook.com (12).


## Installation & Usage

To install and use the **Mailjet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailjet-alternative](https://vinkius.com/mcp/mailjet-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
