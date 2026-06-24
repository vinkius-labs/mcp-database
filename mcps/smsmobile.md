# Smsmobile MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smsmobile)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Turn your smartphone into an SMS/WhatsApp gateway — send messages, read incoming texts, and track call logs directly from any AI agent.

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


## Available Tools (26)
- **delete_gateway_mobile**: Delete a mobile from SMS Gateway
- **delete_sms**: Delete SMS messages from the server log
- **get_received_sms**: Retrieve SMS messages received on the smartphone
- **get_sms_logs**: Retrieve logs of SMS messages sent through the API
- **get_unsubscribed_emails**: List unsubscribed email contacts
- **get_whatsapp_messages**: Retrieve WhatsApp messages
- **sync_whatsapp**: Synchronize WhatsApp messages (Required before retrieval)
- **update_gateway_mobile**: Update mobile label in SMS Gateway
- **list_gateway_mobiles**: Manage mobiles connected to your SMS Gateway
- **list_incoming_calls**: List incoming calls
- **list_missed_calls**: List missed calls
- **list_mobile_sent_sms**: List SMS messages sent directly from the mobile device
- **list_notifications**: List notifications
- **list_outgoing_calls**: List outgoing calls
- **list_sms_conversations**: Retrieve grouped conversations (incoming and outgoing)
- **mark_sms_read**: Mark a received SMS as read in the API status
- **resend_sms**: Resend a previously unsent SMS (must be in error status)
- **send_notification**: Create a push notification for a target mobile device
- **send_sms**: Send an SMS from your mobile phone
- **send_whatsapp**: Send a WhatsApp message
- **set_whatsapp_active**: Activate or deactivate WhatsApp feature
- **update_sms_alias**: Update the alias of a received SMS
- **check_whatsapp_number**: Check if a number is registered on WhatsApp
- **get_emails**: Retrieve emails
- **resend_whatsapp**: Resend a WhatsApp message
- **send_email**: Send an email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smsmobile** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +1234567890 saying 'Your appointment is confirmed for tomorrow at 10 AM'."

**🤖 AI Agent:**
> I've sent the SMS via `send_sms`. The message is now queued on your mobile device with GUID: sms_98765.

---

**👤 You:**
> "Check for any unread SMS messages received in the last hour."

**🤖 AI Agent:**
> I'm checking `get_received_sms`... I found 2 unread messages. One from 'John' regarding 'Project Update' and another from an unknown number.

---

**👤 You:**
> "Show me the logs for all SMS messages sent today that resulted in an error."

**🤖 AI Agent:**
> Querying `get_sms_logs` for today's errors... I found 1 failed delivery to +1987654321 due to a mobile network timeout. Would you like me to try `resend_sms`?


## ❓ FAQ

**Q: Can I send a message via WhatsApp instead of standard SMS?**
Yes! You can use the `send_whatsapp` tool directly, or use `send_sms` and set the `sendwa` parameter to 1 to route it through WhatsApp on your connected device.

**Q: How do I check for new incoming messages on my phone?**
Use the `get_received_sms` tool. You can filter for only unread messages by setting `onlyunread` to 'yes', allowing your AI to process new inquiries automatically.

**Q: Can I see the history of a specific conversation?**
Absolutely. Use `list_sms_conversations` with a specific phone number (`numero`) to retrieve the grouped history of incoming and outgoing messages for that contact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smsmobile](https://vinkius.com/mcp/smsmobile)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smsmobile** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smsmobile` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smsmobile** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smsmobile": {
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
