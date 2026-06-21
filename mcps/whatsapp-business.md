# WhatsApp Business MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-business)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/whatsapp-business-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/whatsapp-business-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Send text, media, and interactive messages on WhatsApp — the world's most popular messaging platform.

## Description
Connect your **WhatsApp Business API** account to any AI agent and power your customer engagement through natural conversation.

### What you can do

- **Conversational Messaging** — Send free-form text messages to users within the 24-hour customer service window
- **Rich Media Support** — Distribute images, videos, documents, and audio files with captions directly from your agent
- **Template Messages** — Use Meta-approved templates to initiate or resume conversations outside the 24-hour window
- **Interactive Buttons** — Send quick-reply buttons (up to 3) to help users navigate choices and workflows easily
- **Location Pinning** — Share physical business addresses or meeting points by sending map pins with custom names
- **Emoji Reactions** — Acknowledge and react to specific incoming messages using any standard emoji character
- **Scalable Engagement** — Automate outbound communication using professional WhatsApp Business infrastructure

### How it works

1. Subscribe to this server
2. Enter your WhatsApp Access Token and Phone Number ID
3. Start dispatching messages and media through Claude, Cursor, or any MCP-compatible client

No more manual typing into phone apps. Your AI agent becomes your WhatsApp communication engine.

### Who is this for?

- **Customer Support Teams** — quickly reply to user inquiries and send helpful documents or location pins
- **Sales Professionals** — use approved templates to follow up with leads and provide product media via chat
- **Marketing Managers** — automate notification broadcasts and verify template delivery status
- **Operations Teams** — share logistics information and use interactive buttons for rapid user confirmations


## Available Tools
- **send_quick_reply_buttons**: Provide the explanation text and a comma-separated list of button labels (max 3).

Sends up to 3 quick-reply buttons with a message block
- **get_business_profile**: Get the WhatsApp Business Profile for this phone number
- **mark_as_read**: Provide the raw wamid message ID.

Mark a WhatsApp message as read
- **send_contact_card**: Provide contacts as a JSON array with name and phone fields.

Send a contact card via WhatsApp
- **send_location_pin**: Provide recipient number and lat/lng coordinates.

Sends a physical location pin on the map
- **send_media_message**: Provide the recipient number, absolute file URL, and media type.

Sends an image, video, document, or audio file via a public URL
- **send_emoji_reaction**: Provide the recipient number, the target message_id (starting with wamid...), and an emoji.

Reacts to a specific WhatsApp message with an emoji
- **send_template_message**: Requires the exact template name and language code.

Sends a Meta-approved Template message to initiate or resume a conversation
- **send_text_message**: Provide the E.164 phone number and the message text.

Sends a free-form conversational text message to a user on WhatsApp


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WhatsApp Business** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message to +123456789 saying 'Hi, your appointment is confirmed for 3 PM!'."

**🤖 AI Agent:**
> I've sent the message to +123456789 via WhatsApp. The message ID is 'wamid.HBgMMTIzNDU2Nzg5...' and it has been successfully queued for delivery.

---

**👤 You:**
> "Send the 'welcome_offer' template to +123456789 in en_US."

**🤖 AI Agent:**
> Success! I've initiated contact with +123456789 using the 'welcome_offer' template in English (US). The conversation has been resumed.

---

**👤 You:**
> "Send a quick reply message to +123456789: 'How would you like to proceed?' with buttons 'Yes', 'No', 'Maybe'."

**🤖 AI Agent:**
> I've dispatched the interactive message block to +123456789. The user will see 'How would you like to proceed?' followed by your 3 custom buttons.


## Installation & Usage

To install and use the **WhatsApp Business** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-business](https://vinkius.com/mcp/whatsapp-business)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
