# Chatsistant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chatsistant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Deploy white-label AI assistants for your clients with custom branding, knowledge bases, and conversation analytics.

## Description
Connect your **Chatsistant** account to any AI agent and manage your AI chatbot ecosystem through natural conversation.

### What you can do

- **Bot Management** — List all configured chatbots and inspect individual bot profiles with knowledge base settings and status
- **Conversation Review** — Browse all chat sessions across bots and inspect full message histories for any conversation
- **Knowledge Training** — Review all data sources (URLs, text, files) training a bot and add new sources programmatically
- **Live Querying** — Send questions to any bot and receive AI-generated answers based on its trained knowledge base
- **Webhook Monitoring** — View all configured webhooks with event triggers and delivery settings

### How it works

1. Subscribe to this server
2. Enter your Chatsistant API Key from your dashboard settings
3. Start managing your chatbots from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Experience Teams** — review bot conversations, identify knowledge gaps, and improve response quality
- **Developers** — manage bot configurations and data sources through conversational AI instead of the dashboard
- **Operations Teams** — monitor webhook delivery and verify bot connectivity across all integrations


## Available Tools (8)
- **add_data_source**: Add a new data source to a bot
- **get_bot**: Get details for a specific bot
- **get_conversation**: Get details for a specific conversation
- **list_bots**: List Chatsistant bots
- **list_conversations**: Optionally filter by bot ID.

List bot conversations
- **list_data_sources**: List bot data sources
- **list_webhooks**: List configured webhooks
- **query_bot**: Query a bot knowledge base


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chatsistant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my bots and query the support bot about return policies."

**🤖 AI Agent:**
> You have 3 bots: 'Support Agent' (bot_101, active), 'Sales Helper' (bot_102, active), and 'Internal Wiki' (bot_103, paused). Querying 'Support Agent' about return policies... The bot responded: 'Our return policy allows returns within 30 days of purchase. Items must be in original packaging with proof of purchase. Refunds are processed within 5-7 business days.' Would you like to review the data sources training this bot?

---

**👤 You:**
> "Show recent conversations for the Sales Helper bot from this week."

**🤖 AI Agent:**
> Found 23 conversations for bot_102 this week. The most active topics were 'pricing plans' (8 conversations), 'integration setup' (6 conversations), and 'enterprise features' (4 conversations). The longest session was conv_8891 (12 messages, 8 minutes). 3 conversations ended with a demo booking request. Would you like to inspect a specific session?

---

**👤 You:**
> "Add our FAQ page and API documentation to the Internal Wiki bot."

**🤖 AI Agent:**
> Adding 2 data sources to 'Internal Wiki' (bot_103)... ✅ URL 'https://docs.example.com/faq' added successfully (type: url, status: processing). ✅ URL 'https://docs.example.com/api' added successfully (type: url, status: processing). The bot now has 9 data sources total: 5 URLs, 3 documents, 1 text snippet. Processing will complete within 3-5 minutes. Would you like to unpause the bot?


## ❓ FAQ

**Q: Can I send a question to a bot and get an AI-generated answer in real time?**
Yes! The `query_bot` tool accepts a Bot ID and a question string. It sends the query to the bot's AI engine and returns a response generated from its trained knowledge base — perfect for testing bot accuracy before deploying changes.

**Q: Can I review all the data sources currently training my bot?**
Yes. The `list_data_sources` tool returns all URLs, documents, and text snippets that have been added to a specific bot's knowledge base, including their processing status. Use `add_data_source` to programmatically add new URLs, text, or file content to expand the bot's training data.

**Q: Can I browse conversation histories across all my bots?**
Yes. Use `list_conversations` to retrieve all chat sessions — optionally filter by a specific Bot ID. Then use `get_conversation` with the Conversation ID to inspect the full message timeline, including user questions, bot responses, and timestamps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chatsistant](https://vinkius.com/mcp/chatsistant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chatsistant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chatsistant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chatsistant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chatsistant": {
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
