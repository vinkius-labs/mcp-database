# 360dialog MCP Server

Send WhatsApp messages at scale, manage templates, and track delivery with the official 360dialog Business API integration.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/360dialog)

## Overview
**Category:** communication-messaging
**Tools Count:** 10

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


## Installation & Usage

To install and use the **360dialog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/360dialog](https://vinkius.com/mcp/360dialog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
