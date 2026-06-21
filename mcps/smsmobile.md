# Smsmobile MCP Server

Turn your smartphone into an SMS/WhatsApp gateway — send messages, read incoming texts, and track call logs directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/smsmobile)

## Overview
**Category:** communication-messaging
**Tools Count:** 26

## Description
Connect your **Smsmobile** account to any AI agent and turn your smartphone into a powerful communication gateway. Automate SMS and WhatsApp messaging directly through natural conversation.

### What you can do

- **SMS Messaging** — Send new messages with `send_sms` or resend failed ones using `resend_sms`.
- **WhatsApp Integration** — Dispatch WhatsApp messages from your own number using `send_whatsapp`.
- **Inbox Management** — Retrieve incoming texts with `get_received_sms` and mark them as read via `mark_sms_read`.
- **Conversation History** — Access full logs and grouped conversations using `get_sms_logs` and `list_sms_conversations`.
- **Device Control** — Manage your connected mobile gateways and SIM ports with `list_gateway_mobiles`.

### How it works

1. Subscribe to this server
2. Enter your Smsmobile API Key
3. Start messaging from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners** — Automate customer notifications and follow-ups directly from your business phone.
- **Developers** — Build SMS-based alerts and 2FA workflows without complex third-party carriers.
- **Support Agents** — Respond to SMS and WhatsApp inquiries within your existing AI-powered workspace.


## Available Tools
- **check_whatsapp_number**: Check if a number is registered on WhatsApp
- **delete_gateway_mobile**: Delete a mobile from SMS Gateway
- **delete_sms**: Delete SMS messages from the server log
- **get_emails**: Retrieve emails
- **get_received_sms**: Retrieve SMS messages received on the smartphone
- **get_sms_logs**: Retrieve logs of SMS messages sent through the API
- **get_unsubscribed_emails**: List unsubscribed email contacts
- **get_whatsapp_messages**: Retrieve WhatsApp messages
- **list_gateway_mobiles**: Manage mobiles connected to your SMS Gateway
- **list_incoming_calls**: List incoming calls
- **list_missed_calls**: List missed calls
- **list_mobile_sent_sms**: List SMS messages sent directly from the mobile device
- **list_notifications**: List notifications
- **list_outgoing_calls**: List outgoing calls
- **list_sms_conversations**: Retrieve grouped conversations (incoming and outgoing)
- **mark_sms_read**: Mark a received SMS as read in the API status
- **resend_sms**: Resend a previously unsent SMS (must be in error status)
- **resend_whatsapp**: Resend a WhatsApp message
- **send_email**: Send an email
- **send_notification**: Create a push notification for a target mobile device
- **send_sms**: Send an SMS from your mobile phone
- **send_whatsapp**: Send a WhatsApp message
- **set_whatsapp_active**: Activate or deactivate WhatsApp feature
- **sync_whatsapp**: Synchronize WhatsApp messages (Required before retrieval)
- **update_gateway_mobile**: Update mobile label in SMS Gateway
- **update_sms_alias**: Update the alias of a received SMS


## Installation & Usage

To install and use the **Smsmobile** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smsmobile](https://vinkius.com/mcp/smsmobile)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
