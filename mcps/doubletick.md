# DoubleTick MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doubletick)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/doubletick-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/doubletick-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Equip your AI agent to manage WhatsApp conversations, track contacts, and monitor message delivery via the DoubleTick API.

## Description
Integrate **DoubleTick**, the official WhatsApp Business API-powered marketing and CRM platform, directly into your AI workflow. Manage your customer conversations, track contacts and opt-in statuses, monitor message delivery and templates, and oversee your team activity using natural language.

### What you can do

- **Conversation Oversight** — List and retrieve detailed information and status for all your WhatsApp customer conversations.
- **Contact Intelligence** — Monitor contact profiles, phone numbers, and opt-in statuses across your organization.
- **Messaging Intelligence** — Monitor real-time message delivery statuses, approved templates, and interaction history via chat.
- **Fulfillment Auditing** — Retrieve high-level summaries of messaging activity, success rates, and active in-progress communications.

### How it works

1. Connect the DoubleTick integration to your AI assistant.
2. Authorize using your DoubleTick API Key (found in your platform settings).
3. Orchestrate your WhatsApp marketing and customer engagement through intuitive conversation.

### Who is this for?

- **Sales Managers** — Quickly check customer response rates and conversation history on the go.
- **Marketing Teams** — Monitor template performance and contact opt-in volumes via chat.
- **Customer Support** — Research specific contact details and previous message history to assist customers instantly.


## Available Tools
- **get_doubletick_account_metadata**: Retrieve metadata and limits for your DoubleTick account
- **get_contact_details**: Get detailed profile and conversation status for a specific contact
- **quick_whatsapp_volume_audit**: Retrieve a high-level summary of messaging activity and success rates
- **list_whatsapp_contacts**: List all contacts registered in your DoubleTick account
- **list_conversation_messages**: List messages from a specific conversation
- **list_opted_in_contacts**: Identify contacts that have explicitly opted in for WhatsApp communications
- **list_latest_whatsapp_messages**: Identify the most recently received or sent messages across all conversations
- **list_approved_templates**: List all approved WhatsApp message templates in your account
- **search_contacts_by_keyword**: Search for contacts using a name keyword or phone number
- **send_whatsapp_template**: Send a pre-approved WhatsApp template message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DoubleTick** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our WhatsApp contacts."

**🤖 AI Agent:**
> I've found several contacts, including 'John Doe' (+1 555-0123) and 'Jane Smith' (+1 555-9876). Would you like to see the last message for any of these?

---

**👤 You:**
> "Show me the approved WhatsApp templates."

**🤖 AI Agent:**
> I've retrieved your approved templates, including 'welcome_message', 'order_update', and 'appointment_reminder'. Would you like the full JSON structure for 'order_update' to send a message?

---

**👤 You:**
> "Search for contact with phone number '+1 555-4444'."

**🤖 AI Agent:**
> I've found a contact matching that number: 'Robert Brown'. He is currently 'Opted In' and his last interaction was yesterday. Should I pull his full conversation history?


## Installation & Usage

To install and use the **DoubleTick** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doubletick](https://vinkius.com/mcp/doubletick)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
