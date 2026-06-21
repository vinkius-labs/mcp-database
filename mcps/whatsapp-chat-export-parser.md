# WhatsApp Chat Export Parser MCP Server

Turn messy WhatsApp chat exports into clean, structured JSON instantly. Let your AI search years of conversations, find lost addresses, and summarize long threads local.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-chat-export-parser)

## Overview
**Category:** talk-to-me
**Tools Count:** 1

## Description
You know that address your landlord sent you 3 months ago in WhatsApp? Or that restaurant recommendation from Maria? Good luck scrolling through thousands of messages to find it.

This MCP solves the universal WhatsApp search problem. When you export any chat via WhatsApp's built-in 'Export Chat' feature, you get a `.txt` file. This engine parses it entirely local using dual-locale regex, extracting every message with its exact timestamp, sender, and content into a structured JSON. The AI can then instantly search, filter, and summarize your entire conversation history.

### The Superpowers

- **Dual-Locale Parsing:** Handles both US format `[1/15/23, 10:30 AM]` and EU format `15/01/2023, 10:30 -` automatically.
- **Token-Safe:** For massive chats, it sends only the first 100 and last 50 messages plus participant stats, preventing context crashes.
- **100% Air-Gapped Privacy:** Your private conversations are parsed locally. Zero cloud uploads.
- **2 Billion Potential Users:** Everyone with WhatsApp can use this instantly.


## Available Tools
- **parse_whatsapp_chat**: They can export any chat from WhatsApp > Chat > Export Chat.

Parse an exported WhatsApp chat .txt file offline. Extracts messages, senders, timestamps, and participant statistics


## Installation & Usage

To install and use the **WhatsApp Chat Export Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-chat-export-parser](https://vinkius.com/mcp/whatsapp-chat-export-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
