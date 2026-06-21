# Postmark MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postmark-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/postmark-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/postmark-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate transactional email delivery via Postmark — manage servers, templates, and bounces directly from any AI agent.

## Description
Connect your **Postmark** account to any AI agent and simplify your transactional email management, deliverability tracking, and template orchestration through natural conversation.

### What you can do

- **Email Delivery** — Send single or bulk transactional emails programmatically directly from your agent using verified signatures
- **Template Management** — Query and manage your catalog of email templates to ensure consistent messaging across your server
- **Bounce Tracking** — Access a history of bounced emails and monitor deliverability issues in real-time
- **Server & Account Control** — List and manage your Postmark servers and account settings programmatically
- **Engagement Insights** — Access aggregate performance analytics, including sent and open metrics

### How it works

1. Subscribe to this server
2. Enter your Postmark Server Token (and optional Account Token) from your settings
3. Start managing your transactional emails from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_delivery_stats**: Get email delivery statistics
- **get_outbound_stats**: Get outbound delivery stats
- **get_template**: Get details for a specific email template
- **list_bounces**: List recent email bounces
- **list_domains**: List all verified sending domains
- **list_outbound_messages**: List sent messages
- **list_account_servers**: List account servers
- **list_email_templates**: List email templates
- **send_batch_email**: Send emails in batch
- **send_email**: Send a single email
- **get_server_info**: Get Postmark server configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postmark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a transactional email from support@example.com to john@doe.com with subject 'Reset Password'."

**🤖 AI Agent:**
> I've sent the email. The message ID is '123-abc-456' and it was successfully accepted by Postmark.

---

**👤 You:**
> "Show me all email bounces from the last 7 days and identify the main failure patterns."

**🤖 AI Agent:**
> 47 bounces in the last 7 days (1.2% bounce rate). Hard bounces: 28 (invalid addresses), Soft bounces: 14 (mailbox full), Spam complaints: 5. Top offending domain: outlook.com with 12 bounces. 8 addresses were auto-suppressed after repeated failures. Your sender reputation score remains healthy at 97/100. Recommendation: clean 28 invalid addresses from your mailing list to maintain deliverability.

---

**👤 You:**
> "Send a transactional welcome email to new user sarah@meridian.io using the onboarding template."

**🤖 AI Agent:**
> Welcome email sent successfully via Postmark. Recipient: sarah@meridian.io. Template: "Onboarding Welcome v3" (ID: tpl_2847). Subject: "Welcome to the platform, Sarah!". Message ID: msg_9f3a2b. Delivery confirmed in 0.8 seconds. The template automatically personalized the greeting, included the quickstart guide link, and set the first follow-up email to trigger in 24 hours.


## Installation & Usage

To install and use the **Postmark** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postmark-extended](https://vinkius.com/mcp/postmark-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
