# AT&T Messaging MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/att-messaging)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/att-messaging-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/att-messaging-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

CPaaS Messaging -- Send SMS/MMS, manage shortcodes, track delivery status, and run bulk campaigns via AT&T Messaging API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AT&T Messaging** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS from shortcode 12345 to +12125551234 saying 'Your order #48291 has shipped! Track it at example.com/track'."

**🤖 AI Agent:**
> SMS sent successfully from 12345 to +12125551234. Message ID: msg-8x4k2p. Status: delivered. The shipping notification reached the recipient's device.

---

**👤 You:**
> "Send a bulk SMS to all these numbers: +12125551001, +12125551002, +12125551003 with the message 'Flash Sale: 50% off everything for the next 2 hours!'."

**🤖 AI Agent:**
> Bulk SMS campaign launched. Job ID: bulk-7n3m. Results: 3/3 messages queued. +12125551001 (delivered), +12125551002 (delivered), +12125551003 (sent). All recipients will receive the Flash Sale alert momentarily.

---

**👤 You:**
> "Show me all inbound messages from the last 24 hours and check if anyone sent STOP."

**🤖 AI Agent:**
> Retrieved 12 inbound messages in the last 24 hours. Found 1 opt-out: +13105554567 sent 'STOP' to shortcode 12345 at 14:32 UTC. This number has been added to your suppression list and will not receive further messages. The remaining 11 messages are keyword responses and customer replies.


## Installation & Usage

To install and use the **AT&T Messaging** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/att-messaging](https://vinkius.com/mcp/att-messaging)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
