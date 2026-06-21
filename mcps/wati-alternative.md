# Wati MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wati-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wati-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wati-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send WhatsApp messages at scale with official API access, chatbot automation, and shared team inbox for business conversations.

## Description
Connect your **Wati** WhatsApp Business account to any AI agent and simplify how you engage with your customers through natural conversation and automated messaging workflows.

### What you can do

- **Direct Messaging** — Send instant WhatsApp session messages to active contacts for real-time support and engagement.
- **Template Automation** — Send pre-approved WhatsApp templates to start conversations or send notifications with dynamic parameters.
- **Contact Management** — List and inspect your WhatsApp subscribers and contacts to keep your directory up-to-date.
- **Chat History** — Retrieve the complete message history for any specific contact to understand the conversation context.
- **Template Catalog** — List all available message templates to identify the best options for your communication strategy.

### How it works

1. Subscribe to this server
2. Enter your Wati API Key and API Endpoint (found in your Wati API dashboard)
3. Start managing your WhatsApp communication from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Support Teams** — quickly respond to inquiries and retrieve chat history via simple AI commands.
- **Sales & Marketing** — automate the sending of template-based notifications and manage lead contacts directly.
- **Operations Managers** — monitor communication flows and verify template availability without leaving the workspace.


## Available Tools
- **add_contact**: Add a contact
- **check_wati_status**: Verify connectivity
- **get_contact**: Get contact details
- **get_template**: Get template details
- **list_templates**: List message templates
- **list_broadcasts**: List broadcasts
- **list_contacts**: List contacts
- **list_messages**: List messages
- **list_tags**: List tags
- **send_media_message**: Send media message
- **send_session_message**: Send a session message
- **send_template_message**: Send a template message
- **update_contact**: Update contact attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wati** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my WhatsApp templates."

**🤖 AI Agent:**
> I've retrieved your message templates. You have 5 approved templates including 'Welcome Message', 'Order Confirmation', and 'Shipping Update'. Which one would you like to use?

---

**👤 You:**
> "Send the 'order_ready' template to 5511999999999."

**🤖 AI Agent:**
> Template message sent! I've triggered the 'order_ready' template to the recipient 5511999999999. The message ID is WATI_8823.

---

**👤 You:**
> "Show me the chat history for the number 5511888888888."

**🤖 AI Agent:**
> I've fetched the history. The last 3 messages show the customer asking about pricing, followed by your response and a confirmation of payment. Would you like to see the full transcript?


## Installation & Usage

To install and use the **Wati** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wati-alternative](https://vinkius.com/mcp/wati-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
