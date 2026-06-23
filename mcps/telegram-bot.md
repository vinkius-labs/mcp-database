# Telegram Bot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telegram-bot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Control Telegram bots programmatically — send messages, photos, documents, and manage chats via AI.

## Description
Connect any **Telegram Bot** to your AI agent and automate messaging, broadcasting, and chat management through natural language commands.

### What you can do

- **Bot Information** — Retrieve your bot's profile details, username, and configuration
- **Message Handling** — Send text messages with Markdown or HTML formatting to any chat or channel
- **Media Delivery** — Send photos, documents, videos, and audio files via URL or file_id
- **Chat Management** — Get detailed info about groups, channels, and private chats including member counts and admin lists
- **Message Operations** — Forward and delete messages programmatically in any chat

### How it works

1. Subscribe to this server
2. Enter your Telegram Bot Token from BotFather
3. Start controlling your Telegram bot from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — broadcast announcements to channels and groups without manual Telegram app access
- **Automation Engineers** — integrate Telegram messaging into AI workflows for alerting and notifications
- **Support Teams** — manage customer chats and forward important messages between departments


## Available Tools (13)
- **delete_message**: Delete a message from Telegram
- **forward_message**: Forward a message in Telegram
- **get_chat_admins**: Get list of chat administrators
- **get_chat_members_count**: Get the number of chat members
- **get_chat_info**: Get information about a Telegram chat
- **get_bot_info**: Get information about the Telegram bot
- **get_updates**: Useful for seeing what users have sent.

Get updates for the Telegram bot
- **get_user_profile_photos**: Returns a list of photo sizes.

Get user profile photos
- **send_audio**: Send an audio file to a Telegram chat
- **send_document**: Send a document to a Telegram chat
- **send_message**: Supports Markdown and HTML parse modes for formatting.

Send a text message to a Telegram chat
- **send_photo**: Optionally includes a caption.

Send a photo to a Telegram chat
- **send_video**: Send a video to a Telegram chat


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telegram Bot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get information about my Telegram bot."

**🤖 AI Agent:**
> Your bot 'MyAssistantBot' (@my_assistant_bot) is active. Bot ID: 123456789. It's currently configured to handle messages and commands.

---

**👤 You:**
> "Send a message to my channel @mychannel saying 'Hello everyone!'"

**🤖 AI Agent:**
> Message sent successfully to @mychannel. The message ID is 456 and was delivered at 2024-01-01 10:00:00 UTC.

---

**👤 You:**
> "How many members are in my group -1001234567890?"

**🤖 AI Agent:**
> Your group 'Tech Community' currently has 1,247 members. It's a supergroup with public visibility.


## ❓ FAQ

**Q: How do I get a Telegram Bot Token?**
Open Telegram, search for **@BotFather**, send `/newbot`, follow the prompts to name your bot, and copy the token provided (format: `123456:ABC-DEF...`).

**Q: Can I send messages to specific groups or channels?**
Yes! Use the `send_message` tool with the chat_id of your target group, channel, or user. The bot must already be added to the group/channel as a member.

**Q: What media types can the bot send?**
The bot supports sending photos, documents, videos, and audio files. Simply provide a public URL or a file_id from Telegram's servers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telegram-bot](https://vinkius.com/mcp/telegram-bot)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `telegram-bot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Telegram Bot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "telegram-bot": {
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
