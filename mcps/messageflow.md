# MessageFlow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/messageflow)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/messageflow-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/messageflow-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Omnichannel communication via MessageFlow — send SMS, WhatsApp, and Email messages.

## Description
Connect your **MessageFlow** account to any AI agent and take full control of your cross-channel communications through natural conversation.

### What you can do

- **Omnichannel Dispatch** — Send messages across SMS, WhatsApp, and Email using a unified set of tools
- **Delivery Auditing** — Retrieve real-time status updates and delivery reports for every message sent
- **Template Management** — List and inspect saved message templates for consistent communication
- **Channel Orchestration** — Enumerate available communication channels and their specific configurations
- **Account Visibility** — Monitor your financial balance and limits to ensure continuous operation

### How it works

1. Subscribe to this server
2. Enter your MessageFlow API Key
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_account_balance**: Get account balance
- **get_delivery_status**: Get message delivery status
- **get_template**: Get template details
- **list_channels**: ).

List all communication channels
- **list_messages**: List sent messages
- **list_templates**: List message templates
- **send_email**: Send an email message
- **send_generic_message**: Send a message through any channel
- **send_sms**: Send an SMS message
- **send_whatsapp**: Send a WhatsApp message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MessageFlow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message to '+1234567890' saying 'Your order is on the way!'"

**🤖 AI Agent:**
> Dispatching WhatsApp message... Sent! The Message ID is 'mf-98765'. I'll monitor the status for you.

---

**👤 You:**
> "Check the delivery status for message ID 'mf-12345'."

**🤖 AI Agent:**
> Checking status... Message 'mf-12345' was successfully delivered to the recipient at 10:30 AM.

---

**👤 You:**
> "What is my current MessageFlow account balance?"

**🤖 AI Agent:**
> Retrieving balance... You have $150.00 available in your account.


## Installation & Usage

To install and use the **MessageFlow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/messageflow](https://vinkius.com/mcp/messageflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
