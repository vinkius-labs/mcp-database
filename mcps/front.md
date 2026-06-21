# Front MCP Server

Manage shared inboxes, track conversations, and collaborate on emails via AI agents with Front.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/front)

## Overview
**Category:** communication-messaging
**Tools Count:** 12

## Description
Connect your **Front** account to any AI agent to automate your customer communication and shared inbox workflows through the Model Context Protocol (MCP). Front is a customer operations platform that enables teams to manage shared emails, SMS, and chats collaboratively. This MCP server enables you to track active conversations, assign messages, and fetch thread histories directly through natural conversation.

### Key Features

- **Shared Inbox Management** — List all accessible shared inboxes and retrieve the specific conversations routed to them.
- **Conversation Tracking** — Search and list all customer conversations, checking their current status (open, archived) and assigned owners.
- **Message Threading** — Fetch the complete message history for any specific conversation to maintain context before replying.
- **Collaborative Replies** — Draft and send replies to active conversations directly from your chat interface on behalf of a teammate.
- **Status Automation** — Programmatically update conversation statuses (e.g., archiving resolved issues) to keep inboxes clean.
- **Team & Contact Discovery** — List all workspace teammates and customer contacts to ensure accurate routing and messaging.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Front API Token (found in your Developer Settings)
3. Start managing your shared inboxes from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Support** — quickly check open conversations in the support inbox and fetch message history without leaving your agent.
- **Operations Teams** — automate the archiving of specific conversation types or verify teammate assignments.
- **Account Managers** — get a real-time overview of client communications and send quick follow-ups via simple AI commands.


## Available Tools
- **verify_api_status**: Verify connection
- **get_conversation_details**: Get conversation metadata
- **get_inbox_details**: Get inbox metadata
- **list_address_book**: List contacts
- **list_all_conversations**: List all conversations
- **list_inbox_threads**: List inbox conversations
- **list_shared_inboxes**: List shared inboxes
- **list_conversation_messages**: List thread messages
- **list_inbox_teammates**: List Front teammates
- **search_conversations**: g. "inbox:inb_123 is:open").

Search all conversations
- **send_inbox_reply**: Send a reply
- **update_conversation_status**: g., archived, open) or assignee of a conversation.

Update conversation


## Installation & Usage

To install and use the **Front** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/front](https://vinkius.com/mcp/front)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
