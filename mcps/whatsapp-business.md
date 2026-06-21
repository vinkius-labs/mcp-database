# WhatsApp Business MCP Server

Send text, media, and interactive messages on WhatsApp — the world's most popular messaging platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-business)

## Overview
**Category:** talk-to-me
**Tools Count:** 9

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


## Installation & Usage

To install and use the **WhatsApp Business** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-business](https://vinkius.com/mcp/whatsapp-business)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
