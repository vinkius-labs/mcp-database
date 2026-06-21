# BotPenguin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/botpenguin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage your chatbots and live chat via BotPenguin — list contacts, orchestrate chats, and send messages directly from any AI agent.

## Description
Connect your **BotPenguin** account to any AI agent and orchestrate your customer conversations, lead generation, and support workflows through natural language.

### What you can do

- **Contact Management** — List and search for contacts or leads collected by your chatbots across multiple channels.
- **Chat Oversight** — Retrieve active and historical chat sessions to monitor agent and bot performance.
- **Conversation Logging** — Access the full message history for specific chat sessions.
- **Message Automation** — Send messages directly into active chats to assist users programmatically.
- **Authentication Support** — Trigger OTP SMS messages to verify user phone numbers.
- **Team Coordination** — List all configured tags and human agents to ensure proper lead routing.

### How it works

1. Subscribe to this server
2. Enter your BotPenguin API Token
3. Start managing your conversational lead generation from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_chat_history**: Retrieve message history of a chat
- **get_contact**: Get details of a specific contact
- **list_agents**: List all human agents/operators
- **list_chats**: List active chat sessions
- **list_contacts**: Optional search text.

List all BotPenguin contacts/leads
- **list_tags**: List all contact tags
- **send_message**: Send a message in a specific chat
- **send_otp**: Send an OTP SMS to verify a phone number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BotPenguin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent contacts in BotPenguin."

**🤖 AI Agent:**
> I've retrieved your contacts. You have 3 recent leads: 'John Doe' (john@example.com), 'Jane Smith' (+15550199), and 'Alice Brown'.

---

**👤 You:**
> "Show the chat history for chat session chat_123."

**🤖 AI Agent:**
> Retrieving the history... The user asked for 'Pricing plans', the bot sent the 'Pricing Menu', and the user requested to speak to a human.

---

**👤 You:**
> "Send an OTP SMS to +1555998877."

**🤖 AI Agent:**
> OTP SMS successfully triggered for +1555998877. The user should receive their verification code momentarily.


## ❓ FAQ

**Q: Can I search for a specific lead or contact by name?**
Yes! Use the `list_contacts` tool and provide the `search_text` parameter with the name, email, or details you are looking for. The agent will return the matching profiles.

**Q: How do I review the chat history of a conversation?**
First, use `list_chats` to find the active or historical session. Then, use `get_chat_history` with the Chat ID to retrieve the full log of messages.

**Q: Can I send an OTP SMS to a user?**
Yes. Use the `send_otp` action and provide the user's phone number (with the country code). BotPenguin will handle the integration to send the verification code.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/botpenguin](https://vinkius.com/mcp/botpenguin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BotPenguin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `botpenguin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BotPenguin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "botpenguin": {
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
