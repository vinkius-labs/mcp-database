# Resend MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/resend)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/resend-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/resend-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate transactional and broadcast email delivery via Resend — send messages, manage domains, audiences, and contacts directly from any AI agent.

## Description
Connect your **Resend** account to any AI agent and take full control of your email infrastructure through natural conversation.

### What you can do

- **Send Emails** — Dispatch transactional emails with HTML content, attachments, and reply-to headers instantly from your agent
- **Track Delivery** — Retrieve complete delivery metadata, bounce information, and open/click analytics for any sent email
- **Domain Management** — List verified sending domains, inspect DNS records (SPF/DKIM), and trigger verification checks
- **Audience & Contact Management** — Browse audiences, list subscribers, and add new contacts programmatically for broadcast campaigns
- **Broadcast Campaigns** — Monitor active broadcast campaigns, check delivery statuses, and audit mass email operations
- **API Key Auditing** — List active API keys and their permission scopes to maintain security hygiene

### How it works

1. Subscribe to this server
2. Enter your Resend API Key (starts with `re_`)
3. Start managing your email infrastructure from Claude, Cursor, or any MCP-compatible client

Your AI becomes a dedicated email operations center. No more switching between dashboard tabs to check if a critical transactional email was delivered.

### Who is this for?

- **Developers** — send test emails, verify domain DNS, and debug delivery issues without leaving the code editor
- **Marketing Teams** — inspect broadcast campaign statuses and audience lists through conversational queries
- **DevOps Engineers** — audit API keys, monitor domain verification, and automate email infrastructure checks


## Available Tools
- **send_email**: Returns email ID for tracking delivery status.

Send a transactional email
- **create_contact**: Add a contact to an audience
- **get_email**: Get email delivery status
- **send_batch_emails**: Each email needs from, to, subject, and html fields.

Send batch of emails
- **list_domains**: List verified sending domains
- **get_domain**: Get domain details
- **add_domain**: Returns DNS records to configure.

Add a new sending domain
- **list_api_keys**: List all API keys
- **list_audiences**: List email audiences
- **list_contacts**: List contacts in an audience


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resend** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a welcome email to john@example.com from our onboarding address."

**🤖 AI Agent:**
> Done! I sent the welcome email from 'Onboarding <welcome@yourdomain.com>' to john@example.com. The email ID is `49a3999c-0ce1-4ea6-ab68-afcd6dc2e794`. Would you like me to check its delivery status?

---

**👤 You:**
> "Show me all our verified sending domains and their DNS status."

**🤖 AI Agent:**
> You have 2 domains configured:

1. **notifications.acme.com** — Status: `verified` (Region: us-east-1)
2. **marketing.acme.com** — Status: `pending` (Region: eu-west-1)

Would you like me to trigger DNS verification for the pending domain?

---

**👤 You:**
> "List all contacts in our newsletter audience."

**🤖 AI Agent:**
> I found 3 audiences. The 'Newsletter' audience (ID: `78b36e1b-...`) contains 1,247 contacts. Here are the first entries:

- john@acme.com (John Smith)
- sarah@startup.io (Sarah Chen)
- dev@company.com (Marcus R.)

Would you like to add a new contact or inspect a specific subscriber?


## Installation & Usage

To install and use the **Resend** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/resend](https://vinkius.com/mcp/resend)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
