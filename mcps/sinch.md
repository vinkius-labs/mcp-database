# Sinch MCP Server

Enable your AI agent to send SMS messages, monitor delivery reports, and manage contact groups via the Sinch API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sinch)

## Overview
**Category:** communication-messaging
**Tools Count:** 10

## Description
Connect your AI to **Sinch**, the global cloud communications platform for SMS messaging at scale.

### What you can do

- **Send Messages** — Dispatch individual or bulk SMS messages to any phone number or contact group.
- **Delivery Tracking** — Check delivery reports to see which messages were delivered, pending, or failed.
- **Batch Management** — List, update, or cancel SMS batches before they're delivered.
- **Contact Groups** — Create and manage contact groups for targeted campaign messaging.

### How it works

1. Add the Sinch integration to your AI toolset.
2. Provide your Service Plan ID and API Token.
3. Send and manage SMS campaigns via natural language.

### Who is this for?

- **Marketing Teams** — Launch SMS campaigns and track delivery rates from chat.
- **Customer Support** — Send transactional messages and verify delivery status instantly.
- **Developers** — Automate SMS workflows and integrate messaging into pipelines.


## Available Tools
- **cancel_sms_batch**: This action is irreversible for the remaining messages.

Cancels a pending SMS batch
- **create_sms_group**: Creates a new contact group
- **delete_sms_group**: This action is irreversible.

Permanently deletes a contact group
- **get_batch_details**: Retrieves details for a specific SMS batch
- **get_delivery_report**: Retrieves a delivery report for a specific batch
- **get_group_details**: Retrieves details for a specific contact group
- **list_sms_batches**: Lists recent SMS batches
- **list_sms_groups**: Lists all contact groups
- **send_sms**: You can provide multiple phone numbers in the "to" field. Ensure numbers are in international format (e.g., +1234567890).

Sends a text message (SMS) to one or more recipients
- **update_sms_batch**: Updates parameters of an existing SMS batch


## Installation & Usage

To install and use the **Sinch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sinch](https://vinkius.com/mcp/sinch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
