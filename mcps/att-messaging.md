# AT&T Messaging MCP Server

CPaaS Messaging -- Send SMS/MMS, manage shortcodes, track delivery status, and run bulk campaigns via AT&T Messaging API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/att-messaging)

## Overview
**Category:** industry-titans
**Tools Count:** 9

## Description
Connect your **AT&T Messaging** account to any AI agent and take full control of your SMS/MMS communication workflows through natural conversation.

### What you can do

- **SMS Messaging** -- Send transactional alerts, OTPs, and customer notifications from registered shortcodes with delivery tracking
- **MMS Messaging** -- Attach images, videos, or audio to enrich marketing campaigns and visual alerts
- **Bulk Send** -- Broadcast the same message to hundreds of recipients in one request with per-recipient status tracking
- **Delivery Status** -- Check real-time delivery state (sent, delivered, failed, read) for any message by its ID
- **Message History** -- Query outbound and inbound message logs for auditing, compliance reporting, or reply tracking
- **Inbound Messages** -- Retrieve customer replies, opt-outs, and keyword-triggered auto-responses
- **Shortcode Management** -- Provision new shortcodes with keywords for campaign routing, or decommission retired numbers
- **Keyword Responses** -- Review configured auto-reply logic for shortcode keywords to verify opt-in/opt-out flows

### How it works

1. Subscribe to this server
2. Enter your AT&T Messaging API Key and API Secret
3. Start sending messages and managing campaigns from Claude, Cursor, or any MCP-compatible client

No more bouncing between the AT&T Messaging dashboard and your CRM. Your AI agent becomes your messaging command center.

### Who is this for?

- **Marketing Teams** -- launch SMS/MMS campaigns, monitor keyword engagement, and manage shortcodes for different brands
- **DevOps Engineers** -- trigger mass alert broadcasts, track delivery rates, and debug failed sends
- **Customer Support** -- review inbound customer messages, process STOP/START commands, and send order updates
- **Compliance Officers** -- audit full message history with timestamps, directions, and content snippets


## Available Tools
- **create_shortcode**: Returns provisioning status and activation timeline. Use for new marketing campaigns or service alerts.

Provision a new messaging shortcode with a keyword
- **delete_shortcode**: Use when retiring a campaign or transferring numbers.

Decommission a messaging shortcode
- **get_inbound_messages**: Returns sender number, keyword matched, message body, and timestamp. Use for monitoring customer engagement or processing STOP/START commands.

Retrieve recent inbound SMS/MMS from customers
- **get_keyword_responses**: Use to review campaign logic or verify opt-in/opt-out flows.

Get configured auto-replies for shortcode keywords
- **get_message_status**: Use to track campaign performance or debug failed sends.

Check delivery status of a specific message
- **list_messages**: Returns timestamps, sender, recipient, and content snippets. Use for auditing, compliance reporting, or reply tracking.

List outbound or inbound messaging history
- **send_bulk_sms**: 164 numbers. Returns job ID and per-recipient status array. Use for mass alerts, emergency broadcasts, or promotional campaigns.

Send SMS to multiple recipients in one request
- **send_mms**: Requires sender, recipient, message text, and media URL. Use for rich marketing campaigns, product images, or visual alerts.

Send an MMS message with media attachment
- **send_sms**: Requires sender ID, recipient E.164 number, and message body. Returns message ID and delivery status. Use this for transactional alerts, OTPs, or customer notifications.

Send a single SMS message to a phone number


## Installation & Usage

To install and use the **AT&T Messaging** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/att-messaging](https://vinkius.com/mcp/att-messaging)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
