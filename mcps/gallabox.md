# Gallabox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gallabox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate WhatsApp Business communication, send templates, and manage chats via AI agents with Gallabox.

## Description
Connect your **Gallabox** account to any AI agent to automate your WhatsApp Business messaging and customer engagement through the Model Context Protocol (MCP). Gallabox is a leading WhatsApp automation platform that enables teams to handle shared inboxes, deploy bots, and send transactional notifications at scale. This MCP server enables you to send real-time messages, track chat histories, and manage your contact database directly through natural conversation.

### Key Features

- **WhatsApp Messaging** — Send standard text messages or pre-approved rich media templates to your customers instantly.
- **Chat Oversight** — List all active WhatsApp conversations, check their current status, and monitor recent engagement.
- **Message Threading** — Fetch the complete message history for any specific conversation ID to maintain context before replying.
- **Contact Management** — Access your WhatsApp contact database, retrieve detailed profiles, and verify phone numbers.
- **Template Discovery** — List all approved message templates available in your account to ensure compliant outreach.
- **Channel Management** — Access configured WhatsApp Business channels and identify unique Channel IDs for routing.
- **Workforce Collaboration** — List support teams and verify your own profile metadata to optimize chat assignments.
- **Real-time Synchronization** — Keep your WhatsApp communication accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gallabox API Key and API Secret (found in Settings > API Keys)
3. Start managing your WhatsApp Business workflows from Claude, Cursor, or any MCP client

### Who is this for?

- **Support Leads** — quickly check missed messages or list active chats without manual dashboard navigation.
- **Marketing Teams** — automate the sending of follow-up templates or verify campaign engagement via simple AI commands.
- **Customer Success Ops** — monitor conversation histories and verify contact metadata seamlessly.


## Available Tools
- **verify_api_connection**: Check connection
- **get_contact_details**: Get contact metadata
- **get_chat_details**: Get thread metadata
- **get_my_profile**: Get account profile
- **list_whatsapp_channels**: List active channels
- **list_whatsapp_contacts**: List chat contacts
- **list_active_chats**: List chat threads
- **list_thread_messages**: List message history
- **list_support_teams**: List Gallabox teams
- **list_message_templates**: List WhatsApp templates
- **send_whatsapp_template**: Send template message
- **send_whatsapp_text**: Send WhatsApp message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gallabox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message to '+1234567890' saying 'Hello from AI!'."

**🤖 AI Agent:**
> Message sent! I've successfully queued your WhatsApp message to +1234567890 via Gallabox. The message will appear in your open conversations inbox.

---

**👤 You:**
> "List all my approved WhatsApp templates."

**🤖 AI Agent:**
> Retrieving templates... I found 5 approved templates, including 'Order Confirmation', 'Welcome Message', and 'Appointment Reminder'. Which one would you like to use?

---

**👤 You:**
> "Show the message history for conversation 'conv_987'."

**🤖 AI Agent:**
> Fetching thread... For conversation conv_987, I found 3 recent messages. The customer asked about 'shipping times' and the bot replied with the standard '2-4 days' policy.


## ❓ FAQ

**Q: How do I get an API Key and Secret for Gallabox?**
Log in to Gallabox, navigate to Settings > API Keys, and click on 'Generate Key' to retrieve your credentials.

**Q: What is a 'Channel ID' and where do I find it?**
The Channel ID is the unique identifier for your WhatsApp Business number. You can find it in Settings > Connect > WhatsApp Channel, or by using the 'list_whatsapp_channels' tool.

**Q: Can I send interactive buttons via this agent?**
Currently, the 'send_whatsapp_template' tool supports pre-approved templates which can include interactive buttons configured in your WhatsApp dashboard.

**Q: Are templates required for all messages?**
No. You can send standard text messages to customers who have messaged you in the last 24 hours using 'send_whatsapp_text'. Templates are required for business-initiated outreach outside this window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gallabox](https://vinkius.com/mcp/gallabox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gallabox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gallabox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gallabox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gallabox": {
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
