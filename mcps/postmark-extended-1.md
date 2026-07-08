# Postmark MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postmark-extended-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send transactional emails, manage templates, and track delivery status directly through Postmark's high-deliverability infrastructure.

## Description
Connect your **Postmark** account to any AI agent to automate your transactional email workflows and template management with ease.

### What you can do

- **Email Delivery** — Send single, batch (up to 500), or bulk emails with full control over HTML/Text bodies, attachments, and metadata.
- **Template Management** — List, create, edit, and delete email templates directly. Use the validation tool to ensure your syntax is perfect before sending.
- **Dynamic Content** — Send emails using existing templates by injecting variables through the TemplateModel.
- **Tracking & Analytics** — Enable open tracking and link tracking to monitor how recipients interact with your messages.
- **Bulk Operations** — Handle large-scale distributions and check the status of bulk requests asynchronously.

### How it works

1. Subscribe to this server
2. Enter your Postmark Server Token (and optionally your Account Token)
3. Start sending emails and managing templates from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Send test emails and manage templates directly from your IDE without switching to the Postmark dashboard.
- **Marketing Ops** — Quickly update email copy or validate template structures using natural language.
- **Support Teams** — Automate personalized follow-ups or notification emails through AI-driven workflows.


## Available Tools (72)
- **create_message_stream**: Create a message stream
- **create_sender_signature**: Create a sender signature (Account level)
- **create_server**: Create a new server (Account level)
- **create_suppressions**: Create suppressions for a message stream (max 50)
- **create_template**: Create a new email template
- **create_webhook**: Create a webhook
- **delete_domain**: Remove a domain (Account level)
- **delete_sender_signature**: Delete a sender signature (Account level)
- **delete_server**: Delete a server (Account level)
- **delete_suppressions**: Remove suppressions (reactivate) for a message stream
- **delete_template**: Delete a template
- **delete_webhook**: Delete a webhook
- **edit_current_server**: Edit current server configuration (Server level)
- **edit_domain**: Edit a domain (Account level)
- **edit_message_stream**: Edit a message stream
- **edit_sender_signature**: Edit a sender signature (Account level)
- **edit_server**: Edit server settings (Account level)
- **edit_template**: Edit an existing template
- **edit_webhook**: Edit a webhook
- **get_bounce_dump**: Get raw SMTP dump for a bounce
- **get_bounce**: Get details for a specific bounce
- **get_bulk_request_status**: Get bulk email request status
- **get_current_server**: Get current server configuration (Server level)
- **get_data_removal_status**: Check data removal request status
- **get_delivery_stats**: Get delivery and bounce statistics
- **get_domain**: Get domain details (Account level)
- **get_inbound_message_details**: Get details for an inbound message
- **get_message_stream**: Get message stream details
- **get_outbound_bounces_stats**: Get bounce counts for outbound messages
- **get_outbound_clicks_stats**: Get click counts for outbound messages
- **get_outbound_message_details**: Get full details and events for an outbound message
- **get_outbound_message_dump**: Get raw source for an outbound message
- **get_outbound_opens_clients_stats**: Get open usage by email client for outbound messages
- **get_outbound_opens_platforms_stats**: Get open usage by platform for outbound messages
- **get_outbound_opens_stats**: Get open counts for outbound messages
- **get_outbound_sends_stats**: Get sent counts for outbound messages
- **get_outbound_spam_stats**: Get spam complaint counts for outbound messages
- **get_outbound_stats**: Get overview stats for outbound messages
- **get_outbound_tracked_stats**: Get tracked email counts for outbound messages
- **get_sender_signature**: Get sender signature details (Account level)
- **get_server**: Get server details (Account level)
- **get_template**: Get details for a specific template
- **get_webhook**: Get webhook details
- **list_domains**: List domains (Account level)
- **list_message_streams**: List message streams
- **list_sender_signatures**: List sender signatures (Account level)
- **list_servers**: List all servers (Account level)
- **list_suppressions**: List suppressions for a message stream
- **list_templates**: List all templates on the server
- **list_webhooks**: List webhooks for a stream
- **push_templates**: Push templates from one server to another
- **request_data_removal**: Request removal of recipient data (GDPR/CCPA)
- **resend_sender_signature**: Resend confirmation email for a sender signature
- **retry_inbound_message**: Retry failed processing for an inbound message
- **rotate_domain_dkim**: Rotate DKIM keys for a domain
- **search_bounces**: Search bounces
- **search_inbound_messages**: Search received inbound messages
- **search_outbound_clicks**: Search click events for outbound messages
- **search_outbound_messages**: Search sent outbound messages
- **search_outbound_opens**: Search open events for outbound messages
- **send_batch_emails**: Send batch emails via Postmark
- **send_bulk_emails**: Send bulk emails via Postmark
- **send_email**: Send a single email via Postmark
- **send_email_with_template**: Send an email using a Postmark template
- **unarchive_message_stream**: Restore an archived message stream
- **validate_template**: Validate template syntax
- **verify_domain_dkim**: Trigger DKIM verification for a domain
- **verify_domain_return_path**: Trigger Return-Path verification for a domain
- **activate_bounce**: Reactivate a bounced email address
- **add_domain**: Add a domain (Account level)
- **archive_message_stream**: Archive a message stream
- **bypass_inbound_message**: Bypass rules for a blocked inbound message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postmark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an email from 'sales@company.com' to 'client@example.com' with the subject 'Meeting Follow-up' and a simple thank you message."

**🤖 AI Agent:**
> I've sent the email using `send_email`. The Message ID is 'abc-123' and the status is 'Submitted'.

---

**👤 You:**
> "List all the email templates available on my Postmark server."

**🤖 AI Agent:**
> I found 3 templates: 'Welcome Email' (Alias: welcome), 'Password Reset' (Alias: reset), and 'Invoice' (Alias: invoice).

---

**👤 You:**
> "Send a welcome email to 'newuser@gmail.com' using the template alias 'welcome-pack' and set the 'name' variable to 'John'."

**🤖 AI Agent:**
> Processing `send_email_with_template`... The email has been successfully queued for delivery to John.


## ❓ FAQ

**Q: Can I send multiple emails in a single request?**
Yes! You can use `send_batch_emails` to send up to 500 messages at once, or `send_bulk_emails` for larger distributions using templates and recipient variables.

**Q: How do I use my existing Postmark templates?**
Use the `send_email_with_template` tool. You just need to provide the `TemplateId` or `TemplateAlias` and the `TemplateModel` containing your dynamic variables.

**Q: Can I manage my templates without leaving the chat?**
Absolutely. You can use `list_templates`, `create_template`, `edit_template`, and `delete_template` to perform full CRUD operations on your Postmark server templates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postmark-extended-1](https://vinkius.com/mcp/postmark-extended-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postmark** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `postmark-extended-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postmark** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postmark-extended-1": {
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
