# Ably MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ably)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ably-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ably-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage real-time messaging, presence, and push notifications via Ably — publish messages, track users, and monitor channels from your AI agent.

## Description
Connect your **Ably** account to any AI agent to orchestrate real-time communication infrastructure through natural language. This server provides full access to the Ably REST API for robust pub/sub messaging and presence management.

### What you can do

- **Messaging** — Publish messages to single or multiple channels, retrieve message history, and update or delete existing messages.
- **Presence Tracking** — Monitor real-time member status and history within specific channels to see who is online.
- **Push Notifications** — Send direct push notifications to devices or client IDs for mobile and web engagement.
- **Channel Management** — List active channels, fetch metadata, and monitor usage statistics across your application.
- **Security & Tokens** — Revoke tokens before expiry to maintain tight control over your real-time infrastructure access.

### How it works

1. Subscribe to this server
2. Enter your Ably API Key
3. Start managing your real-time streams from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — Debug real-time message flows and check channel states directly from the terminal or IDE.
- **DevOps Engineers** — Monitor application stats and manage API key security without leaving the command line.
- **Product Engineers** — Test push notification payloads and presence logic during feature development.


## Available Tools
- **batch_presence**: Get presence for multiple channels
- **batch_publish**: Publish messages to multiple channels at once
- **batch_push_publish**: Publish batch push notifications
- **get_channel_metadata**: Get metadata for a specific channel
- **get_message**: Get a specific message by serial
- **get_messages**: Retrieve message history for a channel
- **get_presence_history**: Get presence history for a channel
- **get_presence**: Get current presence members for a channel
- **get_stats**: Retrieve application usage statistics
- **list_channels**: Enumerate all active channels
- **publish_message**: Publish a message to a specific channel
- **push_publish**: Publish a direct push notification
- **revoke_tokens**: Requires revocableTokens: true on the API key.

Revoke Ably tokens before their expiry
- **update_message**: Update, delete, or append to a message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ably** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Publish a message to the 'orders' channel with the event name 'new_order' and data '{"id": 123}'"

**🤖 AI Agent:**
> I've published the message to the 'orders' channel. The message was successfully accepted by Ably.

---

**👤 You:**
> "Check who is currently online in the 'chat-room-1' channel."

**🤖 AI Agent:**
> I've retrieved the presence data for 'chat-room-1'. There are currently 3 active members: user_01, user_05, and admin_01.

---

**👤 You:**
> "Show me the usage statistics for my Ably application."

**🤖 AI Agent:**
> I've fetched your application stats. In the last period, you had 1,250 messages published and 45 peak concurrent connections.


## Installation & Usage

To install and use the **Ably** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ably](https://vinkius.com/mcp/ably)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
