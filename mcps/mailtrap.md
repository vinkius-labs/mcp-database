# Mailtrap MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailtrap)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailtrap-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailtrap-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Test, debug, and preview emails in a sandbox before sending to production with analytics that catch rendering issues early.

## Description
Connect your **Mailtrap** account to any AI agent and manage email testing and delivery through natural conversation.

### What you can do

- **Email Sending** — Send transactional emails via the Mailtrap API
- **Inbox Testing** — Browse testing inboxes and inspect captured emails
- **Message Analysis** — Analyze email HTML, spam scores, and headers
- **Delivery Analytics** — Track opens, clicks, bounces, and delivery rates
- **Project Management** — Manage testing projects and inboxes
- **Account Management** — Switch between connected accounts and domains

### How it works

1. Subscribe to this server
2. Enter your Mailtrap API Key and Account ID
3. Start testing and sending email from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — test email flows safely in staging
- **QA Engineers** — verify email rendering and spam scores
- **Operations** — monitor production transactional delivery


## Available Tools
- **clear_sandbox_inbox**: Delete all emails in inbox
- **delete_sandbox_message**: Delete captured email
- **get_domain_status**: Get domain details
- **get_message_html**: Get email HTML body
- **get_message_details**: Get message metadata
- **list_accessible_accounts**: Get user accounts
- **list_verified_domains**: List sending domains
- **list_sandboxes**: List virtual inboxes
- **list_sandbox_messages**: List messages in inbox
- **list_mailtrap_projects**: List account projects
- **send_production_email**: Send email in production
- **send_test_email**: Send test email to sandbox


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailtrap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show testing inboxes and recent captured emails."

**🤖 AI Agent:**
> Inboxes: 3 active. 'Staging Env' (45 messages), 'QA Pipeline' (12), 'Dev Local' (0). Staging Latest: 'Welcome User' (to: test@user.com). Received: 2 min ago. Spam Score: 0.1 (Excellent ✅). HTML size: 45 KB. B2B Client Support: 98% compatibility.

---

**👤 You:**
> "Show transactional sending analytics for this week."

**🤖 AI Agent:**
> Sending (7 days): 12,500 emails. Delivered: 12,250 (98% ✅). Bounces: 150 (1.2%). Hard: 45, Soft: 105. Open rate: 45%. Click rate: 12%. Spam complaints: 2 (0.01%). Top template: 'Password Reset' (3,400 sent, 100% delivered). Delivery speed: avg 1.2s.

---

**👤 You:**
> "Analyze the spam score for the last captured email."

**🤖 AI Agent:**
> Analysis for message 'Invoice #890': Overall Spam Score: 2.4 (Good ✅, threshold is 5.0). SpamAssassin checks: 0.0 HTML_MESSAGE, 0.1 MIME_HTML_ONLY. Blacklists: Not listed on 18/18 checks ✅. Authentication: SPF pass, DKIM pass. Recommendation: Improve text-to-image ratio.


## Installation & Usage

To install and use the **Mailtrap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailtrap](https://vinkius.com/mcp/mailtrap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
