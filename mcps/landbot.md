# Landbot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/landbot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Empower your AI to generate, route, and interact with conversational chatbots and customers naturally.

## Description
Engage your conversational pipelines through **Landbot** instantly using your AI assistant. Route leads, send custom programmatic messages to open channels, or check active interactions without checking external software tools.

### What you can do

- **Bot Management:** Oversee and pull active bot matrices.
- **Customer Operations:** Send automated text messages securely to connected accounts.
- **Lead Routing:** Reassign critical pipeline threads directly to live agents programmatically.

### How it works

1. Authorize the plugin connection
2. Provide your Landbot API Token in Vinkius credentials
3. Engage conversational commands locally or through llm interfaces

### Who is this for?

- **DevOps Support** — manage conversational states from your terminal
- **Sales Marketers** — view chat history of high value funnels
- **Product Teams** — examine customer journeys natively


## Available Tools (8)
- **assign_agent**: Route conversation from bot to live agent status
- **get_bot**: Get a single bot details by ID
- **get_customer**: Retrieve specific metadata of one customer
- **get_messages**: Fetch the chat sequence messages for a given customer context
- **list_bots**: List all accessible bots in Landbot
- **list_customers**: List recent customers interacting with bots
- **search_customers**: Search for a particular customer by email
- **send_text_message**: Send a message programmatically to a customer conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Landbot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List standard bots running active pipelines right now."

**🤖 AI Agent:**
> Loading Landbot configurations. There are currently 3 standard matrix bots running active logic mapping sequences.

---

**👤 You:**
> "Fetch the entire transcription log for customer ID 98453."

**🤖 AI Agent:**
> Extracted session log for 98453. The prospect answered 4 initial screening questions mentioning 'Price points'.

---

**👤 You:**
> "Force assign the highest severity angry customer ticket to Agent Sarah."

**🤖 AI Agent:**
> Operation complete. I've intercepted the live interaction and injected the routing update pointing to Agent Sarah gracefully.


## ❓ FAQ

**Q: How do I authenticate?**
Grab the main API Access Integration token located centrally in settings inside Landbot App context.

**Q: Can I route chats to human agents?**
Yes, standard endpoints enable you to extract active sessions and invoke assignment APIs gracefully.

**Q: Do bots answer incoming queries automatically?**
No interruption occurs. Read functionalities passively pull context without disconnecting current funnels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/landbot](https://vinkius.com/mcp/landbot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Landbot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `landbot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Landbot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "landbot": {
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
