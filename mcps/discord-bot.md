# Discord Bot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/discord-bot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/discord-bot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/discord-bot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Control and manage your Discord bots — audit guilds, channels, and messages via AI.

## Description
Empower your AI agent to orchestrate your entire community ecosystem on **Discord**, the leading platform for real-time communication. By connecting your Discord bot to your agent, you transform complex server management into a natural conversation. Your agent can instantly list your guilds, audit channel structures, and send messages without you ever touching a terminal or dashboard. Whether you are a community manager or a bot developer, your agent acts as a real-time moderator, ensuring your community is always healthy and your bot's interactions are precise.

### What you can do

- **Guild Auditing** — List all servers your bot belongs to and retrieve detailed metadata, including roles and member counts.
- **Channel Oversight** — Browse guild channels to maintain a clear view of your community organization and structure.
- **Messaging Intelligence** — Send and delete messages in any channel, and audit recent message history for real-time monitoring.
- **Member Administration** — Query guild member lists to stay on top of your community growth and participant profiles.
- **Bot Governance** — Retrieve detailed bot user information to ensure organizational alignment and control.

### How it works

1. Subscribe to this server
2. Enter your Discord Bot Token
3. Start managing your Discord interactions through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — monitor server activity and audit channel structures straight from your workflow.
- **Bot Developers** — test message delivery and retrieve guild metadata without manual API calls.
- **Support Teams** — perform rapid audits of member lists and send announcements directly from chat.
- **Operations Leads** — automate Discord data querying to orchestrate cross-functional outreach teams smoothly.


## Available Tools
- **delete_message**: Delete a message from a channel
- **get_channel**: Get details for a specific channel
- **get_guild_roles**: Get roles for a guild
- **get_guild**: Get details for a specific guild
- **get_me**: Get authenticated Discord bot info
- **list_channels**: List channels in a guild
- **list_guild_members**: List members of a guild
- **list_guilds**: List guilds the bot is in
- **list_messages**: List recent messages in a channel
- **send_message**: Send a message to a channel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Discord Bot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Discord servers my bot is in."

**🤖 AI Agent:**
> I've retrieved your guilds. Your bot is currently active in 3 servers: 'Vinkius Community', 'Dev Lounge', and 'Support Hub'. Which one would you like to explore?

---

**👤 You:**
> "Send 'Maintenance starting in 10 minutes' to channel ID 12345678."

**🤖 AI Agent:**
> Message delivered! I've sent the maintenance notice to channel 12345678. The message ID is 987654321 and it is now visible to members.

---

**👤 You:**
> "Get the roles for guild ID xxxx."

**🤖 AI Agent:**
> I've found 5 roles in that server: '@everyone', 'Admin', 'Moderator', 'VIP', and 'New Member'. I can provide the permission bits for any of them if you like.


## Installation & Usage

To install and use the **Discord Bot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/discord-bot](https://vinkius.com/mcp/discord-bot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
