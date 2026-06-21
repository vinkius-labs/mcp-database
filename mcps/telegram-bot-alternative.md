# Telegram Bot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telegram-bot-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/telegram-bot-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/telegram-bot-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Control and manage your Telegram bots — send messages, photos, and audit chats via AI.

## Description
Empower your AI agent to orchestrate your messaging workflows with the **Telegram Bot API**, the high-speed platform for real-time communication. By connecting your bot to your agent, you transform bot administration into a natural conversation. Your agent can instantly send rich media, audit group memberships, and manage webhooks without you ever touching a terminal or code. Whether you are running a customer support bot or a large community broadcast, your agent acts as a real-time bot operator, ensuring your messages are always delivered and your chats are healthy.

### What you can do

- **Rich Messaging** — Send text and photos to users or groups instantly with full control over formatting.
- **Chat Auditing** — List chat administrators, check member counts, and retrieve detailed chat metadata.
- **Bot Administration** — Set, delete, and inspect webhooks or fetch recent updates via polling in real-time.
- **File Management** — Retrieve information for media files shared with your bot to keep your content organized.
- **Group Management** — Autonomously leave groups or supergroups when they no longer meet your bot's criteria.

### How it works

1. Subscribe to this server
2. Enter your Telegram Bot Token (from @BotFather)
3. Start managing your bot interactions through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Bot Developers** — monitor bot health and test message delivery straight from your workspace.
- **Community Managers** — audit group members and send announcements without manual bot commands.
- **Support Teams** — send quick photo instructions or text updates to users directly from chat.
- **Operations Leads** — automate bot webhook configurations to orchestrate messaging pipelines smoothly.


## Available Tools
- **delete_webhook**: Delete Telegram webhook
- **get_chat_administrators**: Get chat admins
- **get_chat_member_count**: Get chat member count
- **get_chat**: Get chat details
- **get_file**: Get file info
- **get_me**: Get Telegram bot details
- **get_updates**: Get recent Telegram updates
- **get_webhook_info**: Get webhook status
- **leave_chat**: Leave a chat
- **send_message**: Send a message via Telegram
- **send_photo**: Send a photo via Telegram
- **set_webhook**: Set Telegram webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telegram Bot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send 'Hello from Vinkius!' to chat ID 12345678."

**🤖 AI Agent:**
> Message delivered! I've sent your greeting to chat 12345678. The message ID is 42 and it was delivered instantly.

---

**👤 You:**
> "Get my Telegram bot details."

**🤖 AI Agent:**
> I've retrieved your bot info. Your bot name is 'VinkiusHelperBot' (@vinkius_bot). It has access to groups and is currently online.

---

**👤 You:**
> "Who are the admins in chat -100123456789?"

**🤖 AI Agent:**
> I've found 3 administrators in that chat: 'Marcus R.' (Owner), 'Jane Doe', and 'BotAssistant'. Would you like their specific permission sets?


## Installation & Usage

To install and use the **Telegram Bot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telegram-bot-alternative](https://vinkius.com/mcp/telegram-bot-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
