# WhatsApp Message Sender MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-message-sender)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/whatsapp-message-sender-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/whatsapp-message-sender-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it sends text messages using the official Meta WhatsApp Cloud API. That's its only function, and nothing else. Incredible for giving your AI agents direct access to customers.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WhatsApp Message Sender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message to 5511999999999 saying that their order is out for delivery."

**🤖 AI Agent:**
> I've successfully dispatched the WhatsApp message.


## Installation & Usage

To install and use the **WhatsApp Message Sender** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-message-sender](https://vinkius.com/mcp/whatsapp-message-sender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
