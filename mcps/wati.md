# Wati MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wati)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wati-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wati-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Send WhatsApp template and session messages, and manage contacts on Wati — the leading WhatsApp Business API solution.

## Description
Connect your **Wati** account to any AI agent and power your customer communication on WhatsApp through natural conversation.

### What you can do

- **Unified Messaging** — Send approved WhatsApp template messages or free-text session replies to your customers
- **Contact Management** — List all WhatsApp contacts in your Wati CRM and retrieve full profile details by phone number
- **Chat History** — Retrieve the recent message history for any contact to provide personalized support or sales follow-ups
- **Template Discovery** — List all approved and pending WhatsApp message templates available for outbound messaging
- **Broadcast Campaigns** — Monitor previous and active WhatsApp broadcast campaigns and track their delivery status
- **Customer Roster** — Quickly browse your customer list and their associated phone numbers directly from your agent

### How it works

1. Subscribe to this server
2. Enter your Wati API URL and API Token
3. Start managing your WhatsApp business communication through Claude, Cursor, or any MCP-compatible client

No more manual logging into the Wati dashboard to reply to a single message. Your AI agent becomes your WhatsApp communication hub.

### Who is this for?

- **Customer Support Teams** — quickly reply to user messages and check chat history for better context
- **Sales Professionals** — send template messages to prospects and manage WhatsApp leads through chat
- **Marketing Managers** — monitor broadcast campaigns and verify template approval status
- **Account Managers** — lookup customer profiles and maintain active communication within the 24-hour window


## Available Tools
- **get_whatsapp_contact_details**: Retrieves profile details for a specific WhatsApp contact by phone number
- **get_whatsapp_chat_history**: Provide the contact’s phone number.

Retrieves the recent message history for a specific contact
- **list_broadcast_campaigns**: Lists previous and active WhatsApp broadcast campaigns
- **list_whatsapp_contacts**: Lists all WhatsApp contacts in the Wati CRM
- **list_whatsapp_templates**: Lists all approved and pending WhatsApp message templates
- **send_session_message**: Sends a free-text session message to a user
- **send_template_message**: Requires the template name and target phone number.

Sends an approved WhatsApp template message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wati** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my WhatsApp contacts in Wati."

**🤖 AI Agent:**
> I found 150 contacts. The most recent ones are 'John Doe' (+123456789), 'Jane Smith' (+987654321), and 'Robert Brown' (+112233445). Would you like the full profile details for any of them?

---

**👤 You:**
> "Send the 'order_confirmation' template to +123456789."

**🤖 AI Agent:**
> I've successfully sent the 'order_confirmation' template message to +123456789 via Wati. The message has been queued for delivery.

---

**👤 You:**
> "What was my last conversation with +123456789 about?"

**🤖 AI Agent:**
> Retrieving history for +123456789… The last 3 messages were: 1. Customer: 'Is my package arriving today?' 2. You: 'Yes, it's out for delivery.' 3. Customer: 'Thanks!'. Would you like me to pull more history?


## Installation & Usage

To install and use the **Wati** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wati](https://vinkius.com/mcp/wati)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
