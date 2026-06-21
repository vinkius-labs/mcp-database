# Discord MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/discord-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/discord-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/discord-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Manage Discord servers, post messages, organize channels, and moderate communities with full bot-level API access.

## Description
Connect your **Discord Bot** account to any AI agent and take full control of your community interactions and server operations through natural conversation.

### What you can do

- **Server & Guild Orchestration** — List and monitor the servers (guilds) your bot is in and retrieve detailed metadata about server configurations
- **Channel Architecture** — Manage text, voice, and category channels programmatically to organize your community structure in real-time
- **Messaging & Engagement** — Programmatically send and retrieve messages from channels and Direct Messages (DMs) to coordinate community discussions
- **Member Lifecycle** — Access complete directories of server members and monitor user profiles to maintain high-fidelity community oversight
- **Private Communication** — Programmatically create DM channels with specific users to coordinate private support or internal notifications

### How it works

1. Subscribe to this server
2. Retrieve your **Bot Token** from the Discord Developer Portal
3. Enable **Message Content Intent** and **Server Members Intent** in your Bot settings
4. Start managing your communities from Claude, Cursor, or any MCP client

No more manual toggling between servers or missed messages in busy channels. Your AI acts as your dedicated community moderator and server coordinator.

### Who is this for?

- **Community Managers** — instantly respond to common queries and moderate server discussions using natural language commands
- **Developers & Bot Operators** — automate server structural changes and monitor bot activity without leaving your terminal
- **Support Teams** — coordinate customer assistance via Discord DMs and track user issues across multiple channels


## Available Tools
- **get_bot_info**: Get current Discord bot information
- **send_message**: Send a message to a channel
- **create_dm_channel**: Returns the DM channel ID.

Create a DM channel with a user
- **get_channel**: Get details for a specific channel
- **get_guild**: Get details for a specific server
- **get_user**: Get details for a specific user
- **list_channels**: List channels in a server
- **list_guilds**: List Discord servers (guilds)
- **list_guild_members**: List members in a server
- **list_messages**: List recent messages in a channel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Discord** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Discord servers the bot is currently in."

**🤖 AI Agent:**
> I've retrieved the list of servers. Your bot is active in 3 guilds: 'Vinkius Community' (ID: 123), 'Internal Testing', and 'Product Feedback'. Which one should we explore for channels?

---

**👤 You:**
> "Show the last 10 messages from channel ID '456'."

**🤖 AI Agent:**
> Scanning channel 456... I found 10 recent messages. Highlights include a feature request from @user1 and a question about deployment. Would you like the full text of any of these?

---

**👤 You:**
> "Send a welcome message to channel '456': 'Welcome to the server!'."

**🤖 AI Agent:**
> Message sent! I've posted your welcome note to the specified channel (ID: 456). The message ID is 'msg_789'. I'll monitor for any immediate reactions.


## Installation & Usage

To install and use the **Discord** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/discord-alternative](https://vinkius.com/mcp/discord-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
