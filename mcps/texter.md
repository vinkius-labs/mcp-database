# Texter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/texter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/texter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/texter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send automated text messages and run SMS drip campaigns that engage leads and customers with timely follow-ups.

## Description
Connect your **Texter** account to any AI agent and simplify how you manage customer conversations across WhatsApp, Instagram, and more through natural conversation.

### What you can do

- **Chat Management** — List all active chats and retrieve detailed metadata and history for specific conversations.
- **Omichannel Messaging** — Send session messages to active chats or use pre-approved templates for new outreach.
- **Conversation Control** — Resolve or close chats and apply labels for better organization and tracking.
- **Workspace Oversight** — List departments, labels, and connected messaging channels (WhatsApp, Instagram, etc.).
- **Template Automation** — Send localized template messages with dynamic components directly via AI.
- **Team Coordination** — Monitor active threads and manage chat assignments across your unified inbox.

### How it works

1. Subscribe to this server
2. Enter your Texter API Token and Project ID (found in your workspace settings)
3. Start managing your unified messaging from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Support Teams** — quickly respond to inquiries and resolve chats via simple AI commands.
- **Sales & Marketing** — automate the sending of template-based notifications and manage lead conversations directly.
- **Operations Managers** — monitor chat volume and verify channel connectivity without leaving the workspace.


## Available Tools
- **add_label_to_texter_chat**: Assign a label to a chat
- **get_texter_chat_details**: Get chat details
- **list_texter_channels**: ).

List connected channels
- **list_texter_chats**: List all active chats
- **list_texter_departments**: List departments
- **list_texter_labels**: List chat labels
- **list_texter_messages**: List messages in a chat
- **resolve_texter_chat**: Resolve or close a chat
- **send_texter_message**: Send a message to an active chat
- **send_texter_template**: Send a WhatsApp/Messenger template message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Texter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active chats in my Texter account."

**🤖 AI Agent:**
> I've retrieved your active chats. You have 3 ongoing conversations including 'Inquiry from John Doe' (WhatsApp), 'Question about Pricing' (Instagram), and 1 other. Which one would you like to see the messages for?

---

**👤 You:**
> "Send the 'order_confirmed' template in 'pt_BR' to 5511999999999."

**🤖 AI Agent:**
> Template sent! I've triggered the 'order_confirmed' template in Portuguese to the recipient 5511999999999. The message ID is MSG-88231. Shall I track the delivery status?

---

**👤 You:**
> "Mark chat 'chat_10293' as resolved and add the label 'Support-Fixed'."

**🤖 AI Agent:**
> Chat updated! I've marked chat 10293 as resolved and assigned the 'Support-Fixed' label (ID: lb_552). The conversation is now organized and closed.


## Installation & Usage

To install and use the **Texter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/texter](https://vinkius.com/mcp/texter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
