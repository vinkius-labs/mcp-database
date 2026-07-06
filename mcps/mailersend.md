# MailerSend MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailersend)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Send transactional emails and manage domains via the MailerSend REST API.

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


## Available Tools (10)
- **list_domain_activity**: List email activity for a specific domain
- **list_sender_domains**: List all verified and unverified sender domains
- **list_sent_messages**: List all sent email messages
- **list_email_recipients**: List all recipients in the account database
- **send_bulk_transactional_emails**: Send multiple transactional emails in one batch
- **send_transactional_email**: Requires a JSON body with sender, recipient, and content (text/html) or template ID.

Send a single transactional email
- **verify_sender_domain**: Trigger a DNS verification check for a domain
- **get_sender_domain_details**: Get details for a specific domain
- **get_sent_message_details**: Get details for a specific sent message
- **get_recipient_details**: Get details for a specific recipient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailerSend** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a transactional email to 'user@example.com' with subject 'Welcome' and body 'Hello!'."

**🤖 AI Agent:**
> I've sent the email to user@example.com. The message ID is '64f1abcde12345'. MailerSend has queued the delivery.

---

**👤 You:**
> "List all active sender domains in my account."

**🤖 AI Agent:**
> I've retrieved your domains. You have 2 verified domains: 'mail.example.com' and 'updates.myfirm.io'. Would you like to check the DNS settings for any of them?

---

**👤 You:**
> "Show recent opened events for domain ID '98765'."

**🤖 AI Agent:**
> I found 15 'opened' events for domain 98765 in the last 7 days. Most recent interactions were from 'customer@corp.com' and 'alice@test.io'.


## ❓ FAQ

**Q: Can I use templates with the send_transactional_email tool?**
Yes, you can specify a `template_id` within the `email_json` body to use pre-defined designs created in your MailerSend account.

**Q: How do I filter activity for a specific event like 'opened'?**
Use the `list_domain_activity` tool and provide the `params` string with the desired event types (e.g., `event[]=opened`).

**Q: Is there a limit to bulk email requests?**
The `send_bulk_transactional_emails` tool supports up to 500 email objects per single request as per MailerSend API limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailersend](https://vinkius.com/mcp/mailersend)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MailerSend** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailersend` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MailerSend** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailersend": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
