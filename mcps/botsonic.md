# Botsonic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/botsonic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Train custom AI chatbots on your own data to deliver instant, accurate support that learns from your knowledge base.

## Description
Connect your **Botsonic** (by Writesonic) account to any AI agent and manage your AI chatbot fleet through natural conversation.

### What you can do

- **Bot Management** — Create, update, list, and inspect AI chatbots with personality, instructions, and knowledge base configuration
- **Knowledge Base Training** — Add web page URLs to a bot's knowledge base and review all training sources (URLs, documents, files)
- **Conversation History** — Browse all chat sessions per bot and inspect the full message history of any conversation
- **Live Querying** — Send messages to a bot and receive AI-generated responses in real time
- **Lead Capture** — Retrieve all leads collected by the chatbot during customer conversations
- **Performance Analytics** — Track usage metrics including conversation volume, message count, resolution rate, and customer satisfaction

### How it works

1. Subscribe to this server
2. Enter your Botsonic API Token from your Writesonic dashboard
3. Start managing your chatbot fleet from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Support Teams** — monitor bot conversations, review resolution rates, and capture leads without switching dashboards
- **Product Managers** — train bots with new knowledge sources and test responses through conversational AI
- **Growth Teams** — analyze chatbot engagement metrics and lead capture performance across all bots


## Available Tools (12)
- **add_knowledge_url**: Add knowledge URL
- **check_botsonic_status**: Verify connectivity
- **create_bot**: Create a bot
- **get_bot_analytics**: Get bot analytics
- **get_bot**: Get bot details
- **get_conversation**: Get conversation
- **list_bots**: List all bots
- **list_conversations**: List conversations
- **list_knowledge_base**: List knowledge base
- **list_leads**: List captured leads
- **send_message**: Send message to bot
- **update_bot**: Update a bot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Botsonic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my bots and show the analytics for the one with the most conversations."

**🤖 AI Agent:**
> You have 4 bots configured. 'Customer Support Bot' (bot_301) leads with 1,284 conversations this month. Running analytics... Resolution rate: 78%, average satisfaction: 4.2/5, total messages: 8,921. The second most active is 'Sales Assistant' (bot_302) with 456 conversations. Would you like to inspect specific conversations or review the knowledge base?

---

**👤 You:**
> "Add our pricing page and help center to the 'Sales Assistant' bot's knowledge base."

**🤖 AI Agent:**
> Adding 2 URLs to bot 'Sales Assistant' (bot_302)... ✅ https://example.com/pricing — crawled successfully, 3 pages indexed. ✅ https://help.example.com — crawled successfully, 28 articles indexed. The bot's knowledge base now has 14 sources total (8 URLs, 4 documents, 2 text snippets). The new content will be available in responses within 2-3 minutes.

---

**👤 You:**
> "Show me all leads captured by the 'Customer Support Bot' this week."

**🤖 AI Agent:**
> Found 18 leads captured by bot_301 this week. Top 5 by engagement: 1) Sarah Chen (sarah@techcorp.io) — asked about enterprise pricing, 4 messages. 2) James Miller (james@startupxyz.com) — demo request, 3 messages. 3) Lisa Park (lisa@retailco.com) — integration question, 6 messages. Average lead quality score: 7.2/10. Would you like to export these leads or view specific conversation transcripts?


## ❓ FAQ

**Q: Can I train a bot by adding web pages to its knowledge base?**
Yes! The `add_knowledge_url` action accepts a Bot ID and a URL. Botsonic will crawl the page and add its content to the bot's training data. Use `list_knowledge_base` to review all sources (URLs, documents, files) currently training a specific bot.

**Q: Can I retrieve leads captured by my chatbot during customer interactions?**
Yes. The `list_leads` tool retrieves all leads collected by a specific bot during conversations, including contact details, conversation context, and capture timestamp. This is ideal for syncing chatbot-qualified leads into your CRM.

**Q: How can I measure the performance of my chatbots?**
Use `get_bot_analytics` with the Bot ID. It returns conversation count, total messages, resolution rate (percentage of conversations resolved without human handoff), and customer satisfaction scores. Compare across bots to identify which ones need KB improvements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/botsonic](https://vinkius.com/mcp/botsonic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Botsonic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `botsonic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Botsonic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "botsonic": {
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
