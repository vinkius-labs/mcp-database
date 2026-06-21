# 1msg.io MCP Server

Official WhatsApp Business API automation — send messages, manage templates, and monitor channel status via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/1msgio)

## Overview
**Category:** communication-messaging
**Tools Count:** 6

## Description
Transform your **1msg.io** instance into a conversational powerhouse for your AI agent. This integration bridges the gap between the official WhatsApp Business API and your AI workflows, allowing you to handle customer engagement, notifications, and channel health directly through natural language. Whether you are automating support or orchestrating marketing broadcasts, your agent acts as a direct bridge to your WhatsApp audience, ensuring every interaction follows official Meta standards.

### What you can do

- **Official Messaging** — Send text and media messages (images, PDF, video) to any WhatsApp number worldwide using official API standards
- **Template Management** — List and send pre-approved WhatsApp templates, essential for initiating conversations with customers
- **Channel Health** — Check your connection status (connected, connecting, disconnected) to ensure your automation is always live
- **Message History** — Retrieve and audit your recent incoming and outgoing message logs to maintain conversation context
- **Interactive Flows** — Handle complex WhatsApp interactions and broadcasts directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your 1msg.io JWT Token
3. Start communicating with your customers on WhatsApp through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Support Teams** — respond to inquiries and send helpful guides on WhatsApp instantly
- **Marketing & Growth** — automate notifications and broadcasts using official templates
- **Operations Managers** — monitor channel status and delivery rates to ensure reliable communications
- **SDRs & Sales** — follow up with leads on their preferred platform without leaving the CRM


## Available Tools
- **send_message**: Requires a recipient phone number and the message body. Do not use for media or templates.

Send a simple WhatsApp text message
- **send_file**: Optionally supports a caption or filename.

Send a media file (image, PDF, video) to a WhatsApp number
- **send_template**: Requires the template name.

Send a pre-approved WhatsApp template message
- **get_status**: g. connected, disconnected). Use this to debug communication failures.

Check the current connection status of the 1msg.io WhatsApp channel
- **list_messages**: Use this to check previous communications or audit chat history.

Retrieve recent incoming and outgoing WhatsApp message history
- **list_templates**: List all available and pre-approved WhatsApp templates


## Installation & Usage

To install and use the **1msg.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/1msgio](https://vinkius.com/mcp/1msgio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
