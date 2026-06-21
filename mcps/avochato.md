# Avochato MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/avochato)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/avochato-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/avochato-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage business messaging, contacts, and broadcasts via Avochato — orchestrate SMS and MMS directly via AI.

## Description
Connect your **Avochato** account to any AI agent and manage your business messaging workflows through natural conversation.

### What you can do

- **Business Messaging** — Send and receive SMS/MMS messages with full delivery status tracking and conversation history
- **Contact Organization** — Create, update, and search for contacts and manage tags to segment your audience
- **Broadcast Management** — Coordinate and audit mass messaging campaigns and broadcasts across your target inboxes
- **Inbox Auditing** — Monitor specific subdomains and verify current API user details for secure communication

### How it works

1. Subscribe to this server
2. Enter your Avochato Auth ID and Auth Secret
3. Start managing your business messaging from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support & Sales Teams** — instantly respond to customer messages and update contact details without leaving the workspace
- **Marketing Leads** — coordinate SMS broadcasts and monitor campaign results through natural language
- **Operations Teams** — automate localized messaging workflows and audit conversation logs directly from the IDE


## Available Tools
- **create_broadcast**: Schedule or send a message broadcast
- **create_contact**: Add a new contact to Avochato
- **get_account_check**: Verify Avochato account connection
- **get_contact**: Get details for a specific contact
- **list_broadcasts**: List message broadcasts
- **list_contacts**: List and search contacts
- **list_messages**: List message history in Avochato
- **send_message**: Send an SMS/MMS message
- **update_contact**: Update an existing contact
- **who_am_i**: Get current API user and inbox information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Avochato** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a message to '555-0199': 'Hi there, your order is ready for pickup!'"

**🤖 AI Agent:**
> Sending message to 555-0199... Success! The SMS has been transmitted. The current status is 'sent'. Would you like me to notify you when it's delivered?

---

**👤 You:**
> "List the last 10 messages from today."

**🤖 AI Agent:**
> I've retrieved your recent message history. I found 10 messages from today, including 4 outgoing SMS and 6 incoming responses. Most are related to 'Pickup Notifications'. Shall I summarize the incoming replies for you?

---

**👤 You:**
> "Find all contacts with the tag 'High-Value'."

**🤖 AI Agent:**
> Searching contacts... I found 5 contacts matching the 'High-Value' tag: John D., Sarah M., Robert P., Emily W., and Kevin S. Would you like to schedule a broadcast message for this group?


## Installation & Usage

To install and use the **Avochato** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/avochato](https://vinkius.com/mcp/avochato)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
