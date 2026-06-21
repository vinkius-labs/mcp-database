# Rocket.Chat MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rocketchat)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rocketchat-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rocketchat-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Connect your AI assistant to Rocket.Chat to seamlessly send messages, explore channels, manage directories, and orchestrate chat operations directly.

## Description
Connect your conversational assistant directly to **Rocket.Chat**, the open-source team communication platform. This integration transforms your AI into an active participant capable of chatting, sending notifications to channels, identifying active users, and auditing chat room data organically within your workspace.

### What you can do

- **Communicate Actively** — Instruct your assistant to post messages into public channels or private direct messages (`chat_post_message`, `chat_send_message`). Need to fix a typo? The AI can seamlessly edit (`chat_update_message`) or delete previous messages (`chat_delete_message`).
- **Explore Channels & Groups** — Give your assistant vision over public discussions (`list_public_channels`) or private channels you belong to (`list_private_groups`). You can then extract deep information about specific rooms using `get_channel_info`.
- **Audit Users in the Network** — Scan the entire user directory (`list_users`) to locate team members and review their roles and connection status directly (`get_user_info`).

### How it works

1. Install this module in your MCP connectivity environment.
2. Visit your Rocket.Chat profile's 'Personal Access Tokens' panel online to configure and generate an Auth Token.
3. Securely enter your `Rocket.Chat URL`, your associated `Rocket.Chat User ID`, and the `Auth Token` in the form below.
4. Interact naturally with your AI: "Send a welcome message to #general thanking the new members, and then list all of my active direct messages."

### Who is this for?

- **Team Leaders** — Orchestrate team-wide announcements asynchronously or ask the AI to summarize active channels without navigating through clunky chat apps.
- **Support Staff** — Instantly ping specific users or lookup a colleague's profile and roles using natural language.
- **Operations & IT** — Empower your conversational agent to act as a responsive chatbot directly inside Rocket.Chat, running commands and pushing logs directly to specific channels.


## Available Tools
- **chat_delete_message**: You must provide both room ID and message ID.

Deletes a message from a room
- **chat_post_message**: Sends a message to a channel or user by name
- **chat_send_message**: Sends a message to a specific room by ID
- **chat_update_message**: Updates the text of an existing message
- **get_channel_info**: Retrieves details for a specific channel
- **get_user_info**: Retrieves detailed information for a specific user
- **list_direct_messages**: Lists all active direct message rooms
- **list_private_groups**: Lists all private groups (channels) the user is a member of
- **list_public_channels**: Lists all public channels in the workspace
- **list_users**: Lists all users in the workspace directory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rocket.Chat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all of my active direct messages."

**🤖 AI Agent:**
> I checked your direct communications using `list_direct_messages` and retrieved 4 active room IDs. These IDs represent ongoing 1-on-1 private channels. Let me know if you would like me to list public channels or drop a message into one of these direct rooms.

---

**👤 You:**
> "Send a welcome message to #general thanking the new members."

**🤖 AI Agent:**
> Done. I invoked the `chat_post_message` tool assigning `#general` as the destination. The room successfully received the message: 'Welcome to all the new members! Glad to have you here.' Let me know if you would like me to modify or erase it.

---

**👤 You:**
> "Find and get the user info for the ID abCD123."

**🤖 AI Agent:**
> I utilized the `get_user_info` tool passing the specific ID. The resulting payload revealed this belongs to user 'Richard', logged as active, carrying an 'Admin' organizational role within your servers. I can list their joined groups next if you want.


## Installation & Usage

To install and use the **Rocket.Chat** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rocketchat](https://vinkius.com/mcp/rocketchat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
