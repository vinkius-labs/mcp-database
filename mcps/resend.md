# Resend MCP Server

Automate transactional and broadcast email delivery via Resend — send messages, manage domains, audiences, and contacts directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/resend)

## Overview
**Category:** developer-tools
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Resend** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/resend](https://vinkius.com/mcp/resend)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
