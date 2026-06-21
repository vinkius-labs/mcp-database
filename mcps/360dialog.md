# 360dialog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/360dialog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send WhatsApp messages at scale, manage templates, and track delivery with the official 360dialog Business API integration.

## Description
Connect your **360dialog** WhatsApp Business API to any AI agent and manage your entire messaging workflow through natural conversation.

### What you can do

- **Text Messaging** — Send individual WhatsApp messages to any phone number in international format
- **Template Messages** — Send pre-approved template messages with language targeting for marketing and transactional flows
- **Media Messages** — Send images, videos, documents, and audio files directly to WhatsApp contacts
- **Template Management** — List all approved message templates and inspect individual template details and components
- **Contact Verification** — Check whether phone numbers are registered on WhatsApp before sending campaigns
- **Media Uploads** — Upload media files to the WhatsApp cloud for reuse across multiple messages
- **Webhook Configuration** — Set the callback URL where incoming messages and delivery status updates are received
- **Health Monitoring** — Verify API connectivity and account health in real time

### How it works

1. Subscribe to this server
2. Enter your **API Key** from the 360dialog Client Hub
3. Start messaging from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Support** — respond to inquiries and verify WhatsApp availability via simple AI commands
- **Marketing Teams** — send template campaigns and check delivery readiness before launch
- **Sales Operations** — verify lead phone numbers and automate first-touch outreach


## Available Tools
- **check_contacts**: Check WhatsApp contacts
- **check_360dialog_status**: Verify API connectivity
- **get_media**: Get media file details
- **get_template**: Get template details
- **list_templates**: List all message templates
- **send_media_message**: Provide the media type and URL.

Send a media message
- **send_message**: Provide the recipient number in international format.

Send a WhatsApp text message
- **send_template_message**: Requires the template name and language code.

Send a template message
- **set_webhook**: Configure webhook URL
- **upload_media**: Upload media for messaging


## 💬 Prompt Examples

Here are some examples of how you can interact with the **360dialog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message to +5511999999999 saying 'Your order has been shipped'."

**🤖 AI Agent:**
> Done! I sent the message to +5511999999999 through your 360dialog account. The delivery was queued and the message ID is wa_msg_4821. Would you like to send a follow-up?

---

**👤 You:**
> "List all my approved WhatsApp message templates."

**🤖 AI Agent:**
> I found 7 approved templates in your account: 'order_confirmation' (en, pt), 'appointment_reminder' (en), 'welcome_message' (en, es, fr), and 4 more. Would you like to inspect the components of any specific template?

---

**👤 You:**
> "Check if these numbers have WhatsApp: +5511988888888, +5511977777777."

**🤖 AI Agent:**
> Verified! +5511988888888 is a valid WhatsApp account. +5511977777777 is not currently registered on the platform. Would you like me to send a message to the valid number?


## ❓ FAQ

**Q: Can my AI verify if phone numbers are registered on WhatsApp?**
Yes. Use the `check_contacts` tool with a comma-separated list of phone numbers. The agent returns the WhatsApp registration status for each number instantly.

**Q: How do I send a pre-approved template message?**
Use the `send_template_message` tool. Provide the recipient phone number, the template name, and the language code (e.g., en_US). The agent delivers the template through the 360dialog API.

**Q: Can I send images and documents through WhatsApp via AI?**
Yes. The `send_media_message` tool supports image, video, document, and audio types. Provide the media URL and type, and the agent delivers it directly to the WhatsApp contact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/360dialog](https://vinkius.com/mcp/360dialog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **360dialog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `360dialog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **360dialog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "360dialog": {
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
