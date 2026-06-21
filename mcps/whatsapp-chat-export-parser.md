# WhatsApp Chat Export Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-chat-export-parser)
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


## ❓ FAQ

**Q: Are my private chats sent to the cloud?**
Never. The parsing is 100% local. Only the structured text representation is sent to the AI chat context during your session.

**Q: How do I export a WhatsApp chat?**
Open the chat in WhatsApp, tap the three dots > More > Export Chat > Without Media. Save the .txt file to your computer.

**Q: What if the chat has 50,000 messages?**
The engine uses a token-safe strategy: it sends only the first 100 and last 50 messages, plus full participant stats. Ask the AI to filter by sender or date for specific results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-chat-export-parser](https://vinkius.com/mcp/whatsapp-chat-export-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WhatsApp Chat Export Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `whatsapp-chat-export-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WhatsApp Chat Export Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "whatsapp-chat-export-parser": {
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
