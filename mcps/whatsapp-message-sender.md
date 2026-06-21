# WhatsApp Message Sender MCP Server

This MCP does exactly one thing: it sends text messages using the official Meta WhatsApp Cloud API. That's its only function, and nothing else. Incredible for giving your AI agents direct access to customers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-message-sender)

## Overview
**Category:** industry-titans
**Tools Count:** 1

## Description
We refused to build a complex conversational chatbot system that forces you into a specific workflow. Instead, this MCP server provides a surgical, zero-trust bridge: **just sending text messages via WhatsApp.**

Your AI agent gains the immediate, zero-friction ability to drop status updates, payment confirmations, or emergency alerts straight to any WhatsApp user, bridging the gap between your systems and the most popular messaging app in the world.

### The Superpowers

- **Direct Customer Reach:** When an agent finishes a task (like processing an order or analyzing a report), it can immediately ping the user directly on WhatsApp.
- **Zero-Bloat Integration:** No massive SDKs. It uses the direct REST API endpoint (`/messages`). You only need your Meta Phone Number ID and Access Token.
- **Absolute Containment:** Because this is strictly a sending tool using the official Meta Cloud API, the agent cannot read your WhatsApp inbox, cannot snoop on replies, and cannot alter your Business Manager settings. It is a secure, pure one-way megaphone.


## Available Tools
- **send_whatsapp_message**: Provide the destination phone number in E.164 format WITHOUT the plus sign (e.g., 5511999999999 for Brazil) in the "to" parameter, and the text in the "body" parameter. Note: Sending to users outside of the 24-hour service window requires pre-approved templates on the Meta API, otherwise it may fail.

Send a text message directly to a WhatsApp number using the Meta Cloud API


## Installation & Usage

To install and use the **WhatsApp Message Sender** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-message-sender](https://vinkius.com/mcp/whatsapp-message-sender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
