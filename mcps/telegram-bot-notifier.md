# Telegram Bot Notifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telegram-bot-notifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

This MCP does exactly one thing: it sends messages to your Telegram chats. That's its only function, and nothing else. Incredible for giving your AI agents a voice on mobile.

## Description
We refused to build a bloated Telegram integration that requires complex long-polling daemons or scary webhook ingress setups. Instead, this MCP server provides a surgical, zero-trust bridge: **a simple Bot Token and a Chat ID.**

Your AI agent gains the immediate, zero-friction ability to drop critical alerts, status updates, and direct notifications straight into your pocket (or a designated group chat) via Telegram.

### The Superpowers

- **Zero-Bloat Deployment:** No servers to host, no webhooks to expose. You just provide the Bot token and the Chat ID, and your AI can speak.
- **Native Formatting:** The agent isn't limited to boring plain text. It can programmatically generate formatted messages using HTML or MarkdownV2—complete with bold text, italics, inline links, and code blocks.
- **Absolute Containment:** The agent can only *push* messages. It doesn't poll your chat history, it doesn't read your private DMs, and it cannot spy on your groups. It is the purest, safest way to give your AI a megaphone directly to your phone.


## Available Tools
- **send_telegram_message**: Provide the text in the "text" parameter. You can optionally format the text using HTML or MarkdownV2 by specifying the "parseMode" parameter.

Send a notification or message to a Telegram chat, group, or channel via a Bot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telegram Bot Notifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a Telegram message saying the nightly build failed."

**🤖 AI Agent:**
> I've successfully sent the failure notification to your Telegram chat.

---

**👤 You:**
> "Send an alert to Telegram. Format it in HTML with bold text for 'CRITICAL'."

**🤖 AI Agent:**
> The HTML formatted alert has been delivered to your Telegram chat.


## ❓ FAQ

**Q: Can the agent read my Telegram messages with this?**
No. This MCP only utilizes the 'sendMessage' API endpoint. It does not use `getUpdates` or webhooks, meaning it acts strictly as a one-way notification megaphone. It cannot see your replies.

**Q: How do I get a Telegram Bot Token and Chat ID?**
1. Message @BotFather on Telegram to create a bot and get the Token.
2. Send a message to your new bot.
3. Visit `https://api.telegram.org/bot<YourBotToken>/getUpdates` in your browser to find your Chat ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telegram-bot-notifier](https://vinkius.com/mcp/telegram-bot-notifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Telegram Bot Notifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `telegram-bot-notifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Telegram Bot Notifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "telegram-bot-notifier": {
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
