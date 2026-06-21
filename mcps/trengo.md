# Trengo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trengo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/trengo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/trengo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage customer conversations across WhatsApp, email, chat, and social from one shared inbox your whole team can use.

## Description
Connect your **Trengo** omnichannel inbox to any AI agent and simplify how you manage customer conversations, team collaboration, and support tickets through natural conversation.

### What you can do

- **Unified Inbox Management** — List all tickets and conversations across WhatsApp, Email, and Chat in one place.
- **Ticket Control** — Create new support tickets, update statuses (OPEN, CLOSED, ASSIGNED), and manage assignments via AI.
- **Omichannel Messaging** — Send messages to customers or add internal team notes to any conversation.
- **Contact & Channel Directory** — List your customer database and verify all configured communication channels.
- **Team Coordination** — Query team member lists to understand availability and workload.
- **Event Monitoring** — List and create webhooks to track conversation events in real-time.

### How it works

1. Subscribe to this server
2. Enter your Trengo API Token (found in your account profile or settings)
3. Start managing your unified inbox from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Managers** — quickly retrieve ticket histories and monitor team activity via simple AI commands.
- **Customer Success Teams** — respond to inquiries and update ticket statuses directly from the workspace.
- **Operations Leads** — coordinate communication channels and monitor webhook events via the AI assistant.


## Available Tools
- **create_ticket**: Create a new ticket
- **create_webhook**: Create a new webhook
- **get_account_profile**: Get current user profile
- **get_ticket**: Get ticket details
- **list_channels**: ).

List communication channels
- **list_contacts**: List all contacts
- **list_messages**: List ticket messages
- **list_tickets**: List all support tickets
- **list_team_members**: List team users
- **list_webhooks**: List configured webhooks
- **send_message**: Send a message
- **update_ticket**: Update ticket status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trengo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all currently open support tickets."

**🤖 AI Agent:**
> I've retrieved your open tickets. You have 4 active conversations including 'Billing issue' from John Doe, 'Login error' from Smith, and 2 others. Which one would you like to see the messages for?

---

**👤 You:**
> "Show me the last 3 messages for ticket #88231."

**🤖 AI Agent:**
> I've fetched the history. The last 3 messages include: a customer query about shipping, your team's response, and an internal note regarding the tracking number. Shall I reply to the customer?

---

**👤 You:**
> "Close ticket #10293 as 'CLOSED' and add a note 'Resolved via AI'."

**🤖 AI Agent:**
> Ticket updated! I've set the status of ticket 10293 to 'CLOSED' and added your internal note. The conversation has been archived successfully.


## Installation & Usage

To install and use the **Trengo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trengo](https://vinkius.com/mcp/trengo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
