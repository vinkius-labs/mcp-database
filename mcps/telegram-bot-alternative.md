# Telegram Bot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telegram-bot-alternative)
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


## Available Tools (12)
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


## ❓ FAQ

**Q: How do I get my Telegram Bot Token?**
Message [**@BotFather**](https://t.me/botfather) on Telegram and follow the simple steps to create a new bot. He will provide a token string which you should paste here.

**Q: Can the agent send images to a group?**
Yes. Use the `send_photo` tool providing the target Chat ID and a public image URL. Your agent will confirm the delivery and provide the message metadata.

**Q: Is it possible to check who are the administrators of a chat?**
Yes. The `get_chat_administrators` tool retrieves a list of all users with admin privileges in a specific group or channel, including their custom titles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telegram-bot-alternative](https://vinkius.com/mcp/telegram-bot-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Telegram Bot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `telegram-bot-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Telegram Bot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "telegram-bot-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
