# 1msg.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/1msgio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/1msgio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/1msgio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Official WhatsApp Business API automation — send messages, manage templates, and monitor channel status via AI.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **1msg.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message to +123456789 saying: Your order has been shipped!"

**🤖 AI Agent:**
> I've sent the WhatsApp message to +123456789. The message is now being processed by the official 1msg.io gateway.

---

**👤 You:**
> "Send the PDF invoice at https://example.com/inv123.pdf to +123456789 on WhatsApp."

**🤖 AI Agent:**
> I'm sending the PDF document from the provided URL to +123456789. The official 1msg.io gateway will handle the media delivery.

---

**👤 You:**
> "Is my WhatsApp channel connected and working?"

**🤖 AI Agent:**
> Checking your 1msg.io channel status... Your WhatsApp instance is currently 'connected' and ready to send/receive messages.


## Installation & Usage

To install and use the **1msg.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/1msgio](https://vinkius.com/mcp/1msgio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
