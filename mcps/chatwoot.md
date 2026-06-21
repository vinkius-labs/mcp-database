# Chatwoot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chatwoot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chatwoot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chatwoot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage customer engagement via Chatwoot — track conversations, reply to messages, and manage contacts directly from any AI agent.

## Description
Connect your **Chatwoot** account to any AI agent and take full control of your customer support and engagement through natural conversation. Streamline how you manage chats across Web, WhatsApp, Facebook, and more.

### What you can do

- **Conversation Oversight** — List and retrieve details for all active and resolved conversations natively
- **Live Replying** — Send messages to customers in active chat sessions flawlessly
- **Contact Management** — List and retrieve detailed customer contact information and history securely
- **Inbox Intelligence** — Monitor all configured inboxes, including Web widgets and social integrations flawlessly
- **Agent Tracking** — List all support agents and manage team availability in real-time
- **Message History** — Access complete chat histories to understand customer context directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chatwoot Access Token, Account ID, and Base URL
3. Start managing your customer support from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Managers** — monitor team performance and review chat histories using natural language
- **Customer Success Teams** — engage with customers and manage contact profiles without opening the dashboard
- **Small Business Owners** — quickly reply to customer inquiries across multiple channels straight from their chat interface
- **Developers** — automate message routing and contact synchronization


## Available Tools
- **get_contact_details**: Get detailed information for a specific customer contact
- **get_conversation_details**: Get detailed information for a specific conversation
- **list_support_agents**: List all support agents in the account
- **list_chatwoot_contacts**: List all customer contacts
- **list_woot_conversations**: List all conversations in the account
- **list_chatwoot_inboxes**: List all configured inboxes (Web, WhatsApp, etc)
- **get_chat_history**: Retrieve the message history for a specific conversation
- **send_chat_message**: Send a message to a customer in a specific conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chatwoot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active conversations in Chatwoot."

**🤖 AI Agent:**
> Retrieving your active conversations... I found 3 chats from 'John Doe' (Web), 'Sarah Smith' (WhatsApp), and 'Mike Miller' (Facebook). Which one would you like to open?

---

**👤 You:**
> "What did the customer in conversation ID 555 say last?"

**🤖 AI Agent:**
> Checking conversation 555... The last message from 'Sarah Smith' was: 'Hi, I haven't received my order confirmation email yet. Can you help?'

---

**👤 You:**
> "Reply to conversation 555: 'I'll look into this right now for you, Sarah.'"

**🤖 AI Agent:**
> Sending your reply to conversation 555... The message has been delivered to Sarah Smith via WhatsApp.


## Installation & Usage

To install and use the **Chatwoot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chatwoot](https://vinkius.com/mcp/chatwoot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
