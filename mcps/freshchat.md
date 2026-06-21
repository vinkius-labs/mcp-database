# Freshchat MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshchat)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freshchat-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freshchat-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer conversations, track messages, and oversee agents via AI agents with Freshchat.

## Description
Connect your **Freshchat** account to any AI agent to automate your customer messaging and conversation management through the Model Context Protocol (MCP). Freshchat is a modern messaging software built for sales and support teams to engage with customers across web, mobile, and social channels. This MCP server enables you to track active chats, send real-time messages, and retrieve detailed user profiles directly through natural conversation.

### Key Features

- **Conversation Oversight** — List all active chats, fetch detailed conversation metadata, and monitor chat statuses (open, resolved) instantly.
- **Real-time Messaging** — Post new messages to existing conversations to keep your support workflows moving fast.
- **User & Customer Data** — Access detailed profile information for chat participants and search for users by email address.
- **Support Team Insights** — List all support agents and team members to maintain full context of who is online and available.
- **Channel & Group Management** — Access configured messaging channels and agent groups to understand your routing logic.
- **Message History** — Retrieve the full message history for any specific conversation ID for audit and reporting.
- **Multi-Region Support** — Seamlessly connect to your specific Freshchat data center (US, EU, IN, AU).

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshchat Region Domain and API Token (found in Settings > API Tokens)
3. Start managing your customer messaging from Claude, Cursor, or any MCP client

### Who is this for?

- **Support Leads** — quickly check for open conversations or list agent availability without leaving your primary workspace.
- **Customer Success Managers** — get a real-time overview of customer interactions and user profiles via simple AI commands.
- **Sales Engineers** — automate the sending of follow-up messages or verify chat history for lead qualification.


## Available Tools
- **check_account_status**: Verify account configuration
- **get_agent_profile**: Get agent metadata
- **get_conversation_details**: Get chat metadata
- **get_chat_user_details**: Get user metadata
- **list_support_agents**: List support agents
- **list_chat_channels**: List chat channels
- **list_conversations**: List active chats
- **list_agent_groups**: List agent groups
- **list_chat_messages**: List messages in a chat
- **list_chat_users**: List chat participants
- **search_chat_users**: Find user by email
- **send_chat_message**: Post a new message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshchat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open conversations in my Freshchat account."

**🤖 AI Agent:**
> Retrieving chats... I found 4 open conversations, including one with 'John Doe' regarding 'Billing' and another with 'Sarah' about 'API Integration'.

---

**👤 You:**
> "Find the Freshchat user with the email 'customer@example.com'."

**🤖 AI Agent:**
> Searching users... I found a record for 'Alice Smith' (ID: user_abc123) associated with that email. She has 2 past conversations in your account.

---

**👤 You:**
> "Send a message to conversation 'conv_987': 'I am looking into this for you'."

**🤖 AI Agent:**
> Message sent! Your update has been successfully posted to conversation 'conv_987'. The customer will see your reply in their chat widget.


## Installation & Usage

To install and use the **Freshchat** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshchat](https://vinkius.com/mcp/freshchat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
