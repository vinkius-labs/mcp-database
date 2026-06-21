# MailerSend MCP Server

Send transactional emails and manage domains via the MailerSend REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mailersend)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **MailerSend** account to any AI agent to automate your transactional messaging and domain management. This MCP server enables your agent to send single or bulk emails, monitor domain verification, and track email activity directly from natural language interfaces.

### What you can do

- **Email Delivery** — Send transactional emails instantly with support for HTML, text, and templates
- **Bulk Operations** — Send up to 500 emails in a single batch request for high-volume communications
- **Domain Oversight** — List sender domains, retrieve DNS settings, and trigger ownership verification checks
- **Recipient Management** — List and query recipients from your account database to track engagement
- **Activity Auditing** — Access real-time logs of email events (sent, delivered, opened, clicked) for any domain
- **Message Insight** — Retrieve complete metadata and lifecycle history for individual sent messages

### How it works

1. Subscribe to this server
2. Enter your MailerSend API Token
3. Start managing your transactional emails from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Quickly test email sending and verify domain configurations from your IDE
- **Operations Teams** — Monitor email delivery performance and audit activities via natural language commands
- **Marketing Engineers** — Automate the synchronization of recipient data and track campaign-level interactions


## Available Tools
- **get_sender_domain_details**: Get details for a specific domain
- **get_sent_message_details**: Get details for a specific sent message
- **get_recipient_details**: Get details for a specific recipient
- **list_domain_activity**: List email activity for a specific domain
- **list_sender_domains**: List all verified and unverified sender domains
- **list_sent_messages**: List all sent email messages
- **list_email_recipients**: List all recipients in the account database
- **send_bulk_transactional_emails**: Send multiple transactional emails in one batch
- **send_transactional_email**: Requires a JSON body with sender, recipient, and content (text/html) or template ID.

Send a single transactional email
- **verify_sender_domain**: Trigger a DNS verification check for a domain


## Installation & Usage

To install and use the **MailerSend** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailersend](https://vinkius.com/mcp/mailersend)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
