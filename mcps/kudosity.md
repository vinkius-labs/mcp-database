# Kudosity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kudosity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate SMS & WhatsApp messaging via Kudosity — send and cancel SMS, send WhatsApp messages, manage contacts and lists, track delivery, and check account balance from any AI agent.

## Description
Connect your **Kudosity** account to any AI agent and take full control of your SMS and WhatsApp messaging workflows through natural conversation.

### What you can do

- **Send & Cancel SMS** — Send messages to individual recipients or entire contact lists, schedule sends, and cancel scheduled messages by message ID
- **Send WhatsApp Messages** — Send templated, text, or custom WhatsApp messages to single recipients with SMS fallback support
- **Number Formatting** — Sanitise phone numbers from your CRM into E.164 international format for reliable delivery
- **Delivery Tracking** — Retrieve delivery status, delivery statistics (delivered, bounced, pending), and reply responses for any message
- **Contact Management** — Create contact lists, add and remove contacts, and opt out subscribers for marketing compliance
- **Account Reporting** — Check your account balance, get SMS sent counts within timeframes, and retrieve campaign information

### How it works

1. Subscribe to this server
2. Enter your Kudosity API Key, API Secret, and V2 API Key (for WhatsApp)
3. Start sending and managing SMS and WhatsApp from Claude, Cursor, or any MCP-compatible client

No more switching between your messaging dashboard and your editor to check delivery status or add contacts. Your AI acts as a dedicated messaging operations assistant.

### Who is this for?

- **Marketing Teams** — send campaigns via SMS and WhatsApp, manage contact lists, and track delivery metrics without leaving the conversation
- **Engineering Teams** — integrate SMS and WhatsApp notifications into workflows with precise number formatting and delivery verification
- **Operations & Customer Support** — check delivery status, retrieve replies, and manage opt-outs directly from your AI agent


## Available Tools (17)
- **list_contact_lists**: Supports pagination.

List all contact lists in your account
- **remove_contact**: Number must be in E.164 format unless countrycode is provided.

Remove a contact from list(s)
- **add_contact_to_list**: If the contact already exists, it will be ignored (not updated). Number must be in E.164 format unless countrycode is provided.

Add a contact to a list
- **get_sms_responses**: Filter by message_id, keyword, keyword_id, or virtual number. Supports date range filtering.

Get SMS reply responses
- **get_sms_sent_count**: Start and end date must be within 7 days. If omitted, covers the last 24 hours.

Get total SMS sent count in a timeframe
- **get_sms_stats**: Get message/campaign delivery report
- **send_sms**: Numbers must be in E.164 international format unless countrycode is provided.

Send an SMS message
- **get_balance**: Get Kudosity account balance
- **cancel_sms**: Only messages that have been scheduled can be cancelled.

Cancel a scheduled SMS
- **format_number**: Useful for cleaning CRM data before sending SMS.

Format a phone number to E.164 international format
- **get_whatsapp**: Returns message content, delivery status, and metadata.

Get details of a sent WhatsApp message
- **list_whatsapp**: Messages returned in reverse chronological order (newest first). Supports cursor-based pagination with 1-100 messages per page. 

List WhatsApp messages for your account
- **opt_out_contact**: Required for marketing compliance — enables an unsubscribe method.

Unsubscribe a contact from list(s)
- **get_contact_list**: Get detailed information about a contact list
- **get_sms_delivery_status**: Get SMS delivery status for a specific recipient
- **get_sms_info**: Does not return individual messages with populated variables.

Get message/campaign information
- **send_whatsapp**: Supports text, template, and custom content types. Templates must be pre-approved by WhatsApp. Recipient must have an active WhatsApp account and have opted in.

Send a WhatsApp message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kudosity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS saying 'Your order has shipped!' to 61478038915."

**🤖 AI Agent:**
> Message sent successfully! Message ID: 339683245, 1 recipient, cost: $0.087 AUD. The message has been dispatched and delivery reports will be available shortly.

---

**👤 You:**
> "Check the delivery status of message 339683245 for recipient 61478038915."

**🤖 AI Agent:**
> Delivery confirmed! The message 'Your order has shipped!' was delivered to 61478038915 at 11:17 AM UTC on June 18th. Status: delivered. Sender: 61429720235.

---

**👤 You:**
> "What is my current Kudosity account balance?"

**🤖 AI Agent:**
> Your current account balance is $73.954 AUD. You have sufficient credit to continue sending messages.


## ❓ FAQ

**Q: Can my AI send an SMS to multiple recipients at once?**
Yes! Use the `send_sms` tool with up to 500 comma-separated recipient numbers in the `to` parameter, or send to an entire contact list by providing a `list_id`. Numbers must be in E.164 international format, or use the `countrycode` parameter to auto-format local numbers.

**Q: How do I check if my SMS was delivered successfully?**
Use `get_sms_stats` with the message ID to get aggregate delivery counts (delivered, bounced, pending), or use `get_sms_delivery_status` with both message ID and recipient number to get per-recipient delivery details including the full populated message content.

**Q: Can my AI manage contacts and opt-outs for marketing compliance?**
Absolutely. Use `add_contact_to_list` to add contacts, `remove_contact` to delete them from lists, and `opt_out_contact` to unsubscribe recipients. The opt-out tool is essential for marketing compliance — by law you must enable an unsubscribe method for marketing campaigns.

**Q: Can my AI send WhatsApp messages?**
Yes! Use the `send_whatsapp` tool to send text, template, or custom content messages. Templates must be pre-approved in your WhatsApp Business account. The recipient must have an active WhatsApp account and have opted in. You can also retrieve sent messages with `get_whatsapp` and list all messages with `list_whatsapp`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kudosity](https://vinkius.com/mcp/kudosity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kudosity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kudosity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kudosity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kudosity": {
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
