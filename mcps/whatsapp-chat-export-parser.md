# WhatsApp Chat Export Parser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-chat-export-parser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/whatsapp-chat-export-parser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/whatsapp-chat-export-parser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Turn messy WhatsApp chat exports into clean, structured JSON instantly. Let your AI search years of conversations, find lost addresses, and summarize long threads local.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WhatsApp Chat Export Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse my WhatsApp chat with Maria and find the message where she sent me an address."

**🤖 AI Agent:**
> Found it! On 03/12/2024 at 14:23, Maria sent: 'The address is Rua Augusta 42, 3rd floor, Lisbon.'

---

**👤 You:**
> "Summarize my conversation with the landlord from last month."

**🤖 AI Agent:**
> Last month, you discussed 3 topics: 1) Rent payment date change (agreed to the 5th), 2) Plumbing issue (he'll send someone Friday), 3) Lease renewal (pending his response).

---

**👤 You:**
> "Who sends the most messages in my group chat? Show me the statistics."

**🤖 AI Agent:**
> Participant stats: João (1,204 messages), Ana (892), Pedro (456). João sends 42% of all messages.


## Installation & Usage

To install and use the **WhatsApp Chat Export Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-chat-export-parser](https://vinkius.com/mcp/whatsapp-chat-export-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
