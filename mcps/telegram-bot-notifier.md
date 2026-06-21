# Telegram Bot Notifier MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telegram-bot-notifier)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/telegram-bot-notifier-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/telegram-bot-notifier-mcp)
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


## Installation & Usage

To install and use the **Telegram Bot Notifier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telegram-bot-notifier](https://vinkius.com/mcp/telegram-bot-notifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
