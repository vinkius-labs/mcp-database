# String Alternative MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/string-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Engage mobile app users with targeted push notifications, in-app messages, and behavioral triggers that improve retention.

## Description
Connect your **String** account to any AI agent and manage business messaging.

### What you can do

- **Contact Management** — List, view, and create contacts
- **Messaging** — Send SMS and MMS messages to any phone number
- **Conversation Tracking** — View message history and active threads
- **Campaign Management** — List SMS marketing campaigns
- **Tag Organization** — View contact tags for segmentation
- **Health Check** — Verify API connectivity


## Available Tools (10)
- **list_string_tags**: List all tags
- **create_string_contact**: Create a contact
- **get_string_contact**: Get contact details
- **list_string_campaigns**: List campaigns
- **list_string_contacts**: List all contacts
- **list_string_conversations**: List conversations
- **list_string_messages**: List messages
- **send_string_message**: Send a text message
- **check_string_status**: Verify API connectivity
- **get_string_message**: Get message details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **String Alternative** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a text to +14155551234 saying 'Your order is ready for pickup'."

**🤖 AI Agent:**
> Message sent! ID: msg_4921 delivered to +14155551234 via String.

---

**👤 You:**
> "List all my contacts."

**🤖 AI Agent:**
> You have 234 contacts. Top recent: 'Sarah K.' (+1415...), 'Mike R.' (+1650...), 'Lisa T.' (+1212...).

---

**👤 You:**
> "Show all active conversations."

**🤖 AI Agent:**
> 12 active conversations. Most recent: Sarah K. (last message 5 min ago), Mike R. (2 hours ago).


## ❓ FAQ

**Q: Can my AI send text messages?**
Yes. Use `send_string_message` with the recipient phone number and message text. The agent delivers it via String.

**Q: Can I view conversation history?**
Yes. `list_string_conversations` shows all active threads, and `list_string_messages` returns full message history.

**Q: Can I create contacts through the AI?**
Yes. `create_string_contact` adds a new contact with name and phone number to your String directory.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/string-alternative](https://vinkius.com/ai-agent-connect/string-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **String Alternative** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `string-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **String Alternative** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "string-alternative": {
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
