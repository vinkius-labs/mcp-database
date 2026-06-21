# Wati MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wati-alternative-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate WhatsApp communication via Wati — send template messages, manage contacts, list chatbots, and assign operators directly from your AI agent.

## Description
Connect your **Wati** account to any AI agent to streamline your WhatsApp Business communication through natural conversation.

### What you can do

- **Template Messaging** — Send pre-approved WhatsApp templates with dynamic parameters to your customers using the `send_template_message` tool.
- **Contact Management** — Retrieve and filter your contact list with `get_contacts` to identify specific users or segments.
- **Chatbot Overview** — List all configured chatbots using `get_chatbots` to understand your automated flows.
- **Operator Assignment** — Route conversations to specific human agents or back to the bot for seamless handovers with `assign_operator`.

### How it works

1. Subscribe to this server
2. Enter your Wati API Endpoint and Access Token
3. Start managing your WhatsApp Business communication from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Teams** — instantly assign chats to operators or check contact details without leaving the chat interface
- **Marketing Managers** — trigger template broadcasts and monitor chatbot statuses directly through AI
- **Sales Ops** — automate lead follow-ups by sending structured templates to new contacts


## Available Tools (4)
- **assign_operator**: Assign a specific operator to a chat
- **get_chatbots**: Retrieve a list of existing chatbots
- **get_contacts**: Retrieve a list of contacts from Wati
- **send_template_message**: Send a pre-approved WhatsApp template message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wati** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the chatbots currently configured in Wati."

**🤖 AI Agent:**
> I've retrieved your chatbots. You have 3 active bots: 'Customer Support Bot', 'Sales Lead Bot', and 'After-Hours Assistant'.

---

**👤 You:**
> "Send the 'welcome_message' template to 85264318721."

**🤖 AI Agent:**
> Sending the template message... The 'welcome_message' has been successfully sent to 85264318721 via Wati.

---

**👤 You:**
> "Assign the chat with 85264318721 to support@company.com."

**🤖 AI Agent:**
> Processing assignment... The conversation with 85264318721 has been assigned to the operator support@company.com.


## ❓ FAQ

**Q: Can I send a WhatsApp message using a pre-approved template?**
Yes! Use the `send_template_message` tool. You'll need to provide the WhatsApp number, template name, and any dynamic parameters required by the template.

**Q: How do I find a specific contact in my Wati account?**
Use the `get_contacts` tool. You can filter by name, creation date, or specific attributes to locate the exact contact you need.

**Q: Is it possible to hand over a bot conversation to a human agent?**
Absolutely. Use the `assign_operator` tool with the contact's WhatsApp number and the email of the operator you wish to assign the chat to.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wati-alternative-1](https://vinkius.com/mcp/wati-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wati** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wati-alternative-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wati** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wati-alternative-1": {
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
