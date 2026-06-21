# Gupshup Messaging MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gupshup-messaging)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Send WhatsApp messages, templates, media, and reactions via Gupshup API.

## Description
Connect **Gupshup** to any AI agent and automate your WhatsApp Business communications — send template messages, media, interactive buttons, and reactions through natural conversation.

### What you can do
- **Template Messages** — Send pre-approved WhatsApp templates for notifications and alerts
- **Free Text** — Send quick text messages within the 24-hour session window
- **Media Sharing** -- Share images, videos, audio, and documents via public URLs
- **Interactive Buttons** -- Send quick reply buttons to engage users
- **Reactions** -- React to specific messages with emojis

### How it works
1. Subscribe to this server
2. Enter your Gupshup API Key
3. Start messaging from Claude, Cursor, or any MCP-compatible client

Gupshup is a leading conversational messaging platform used by enterprises to communicate with customers on WhatsApp, SMS, and RCS.

### Who is this for?
- **Marketing Teams** -- Send template messages and interactive polls to customers
- **Support Agents** -- React to customer messages and share media (images/docs)
- **Developers** -- Automate WhatsApp notifications and alerts via AI


## Available Tools
- **get_template_info**: Get information about a specific template
- **send_interactive_message**: Provide up to 3 buttons in a JSON array.

Send an interactive message with buttons
- **send_media_message**: Type can be image, video, audio, or document.

Send a media message (Image, Video, Document, Audio)
- **send_reaction**: React to a message with an emoji
- **send_template_message**: Provide recipient phone number, template name, language code (e.g., en_US), and an array of string parameters to fill the template.

Send a WhatsApp template message
- **send_text_message**: Send a free-form text message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gupshup Messaging** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a template 'order_confirmation' in en_US to 5511999999999 with params ['12345']."

**🤖 AI Agent:**
> Template message sent successfully! Status: 200 OK.

---

**👤 You:**
> "Send an interactive message to 5511999999999 asking 'Did you receive your order?' with buttons 'Yes' and 'No'."

**🤖 AI Agent:**
> Interactive message sent successfully! Status: 200 OK.

---

**👤 You:**
> "React with a thumbs up emoji to message ID msg_123 for user 5511999999999."

**🤖 AI Agent:**
> Reaction sent successfully! Status: 200 OK.


## ❓ FAQ

**Q: How do I get my Gupshup API Key?**
Log in to your Gupshup Console, navigate to Apps > Your App > Settings, and copy your API Key.

**Q: Can I send free text messages?**
Yes, but only within the 24-hour session window after the user messages you first.

**Q: Do I need to pre-approve templates?**
Yes, template messages must be approved by Meta before they can be sent via the send_template_message tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gupshup-messaging](https://vinkius.com/mcp/gupshup-messaging)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gupshup Messaging** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gupshup-messaging` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gupshup Messaging** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gupshup-messaging": {
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
