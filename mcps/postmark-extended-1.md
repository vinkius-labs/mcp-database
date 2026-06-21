# Postmark MCP Server

Send transactional emails, manage templates, and track delivery status directly through Postmark's high-deliverability infrastructure.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/postmark-extended-1)

## Overview
**Category:** communication-messaging
**Tools Count:** 72

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


## Available Tools
- **activate_bounce**: Reactivate a bounced email address
- **add_domain**: Add a domain (Account level)
- **archive_message_stream**: Archive a message stream
- **bypass_inbound_message**: Bypass rules for a blocked inbound message
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


## Installation & Usage

To install and use the **Postmark** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postmark-extended-1](https://vinkius.com/mcp/postmark-extended-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
