# MailerSend MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailersend-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailersend-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailersend-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Send transactional and marketing emails with templates, analytics, and deliverability tools built for developers and businesses.

## Description
Connect your **MailerSend** account to any AI agent and manage transactional email through natural conversation.

### What you can do

- **Email Sending** — Send transactional and bulk emails with templates
- **Template Management** — Create and manage email templates with variables
- **Delivery Analytics** — Track opens, clicks, bounces, and delivery rates
- **Domain Management** — Configure sending domains and DNS records
- **Recipient Management** — Manage suppression lists and blocklists
- **Activity Logs** — Browse detailed email activity and event logs

### How it works

1. Subscribe to this server
2. Enter your MailerSend API Token
3. Start sending email from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate transactional email with rich analytics
- **Product Teams** — manage email templates and delivery
- **DevOps** — monitor domain health and deliverability


## Available Tools
- **get_date_analytics**: Check usage stats
- **get_domain_details**: Get domain info
- **get_message_info**: Get message status
- **get_account_limits**: Check plan quotas
- **get_template_details**: Get template info
- **list_email_activities**: ).

Check email logs
- **list_sending_domains**: List verified domains
- **list_sent_messages**: List specific messages
- **list_email_templates**: List saved templates
- **list_domain_webhooks**: Get notification configs
- **send_transactional_email**: Send custom email
- **send_templated_email**: Send with template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailerSend** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show sending analytics and domain health status."

**🤖 AI Agent:**
> Sending (7 days): 4,560 emails. Delivered: 4,468 (98% ✅). Opens: 1,824 (41%). Clicks: 456 (10%). Bounced: 68 (1.5%). Spam complaints: 4 (0.09%). Domains: 2. 'app.company.com' — Verified ✅, SPF ✅, DKIM ✅, DMARC ✅. 'notify.company.com' — Verified ✅, DMARC ⚠️ (policy: none).

---

**👤 You:**
> "List email templates and send a password reset email."

**🤖 AI Agent:**
> Templates: 6. 'Welcome' (used 1,200x), 'Password Reset' (890x), 'Invoice' (456x), 'Shipping Notification' (334x), 'Verification' (1,500x), 'Feedback Request' (220x). Email sent! ✅ Template: 'Password Reset'. To: sarah@company.com. Variables: {name: 'Sarah', reset_link: 'https://...'}. Delivered in 0.8s.

---

**👤 You:**
> "Show suppression list and recent bounce details."

**🤖 AI Agent:**
> Suppression list: 145 addresses. Hard bounces: 89. Spam complaints: 34. Manual: 22. Recent bounces (48h): 12. Hard: 'user@oldomain.com' (domain expired), 'test@fake.io' (mailbox not found). Soft: 'info@bigcorp.com' (mailbox full, retry in 4h). Bounce rate trend: 1.5% → 1.2% (improving ⬇️).


## Installation & Usage

To install and use the **MailerSend** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailersend-alternative](https://vinkius.com/mcp/mailersend-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
