# CHATFLY MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chatfly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage AI chatbots and knowledge bases via CHATFLY — train bots on custom data and track conversations directly from any AI agent.

## Description
Connect your **CHATFLY** account to any AI agent and take full control of your custom chatbot workflows through natural conversation. Train and monitor your own AI agents using your business data.

### What you can do

- **Chatbot Oversight** — List and retrieve details for all custom AI chatbots in your account natively
- **Knowledge Logistics** — List all uploaded documents and data sources used for bot training flawlessly
- **Training Automation** — Trigger the training process for your chatbots to ingest new data securely
- **Conversation Intelligence** — Access recent chat conversations and full message history flawlessly
- **Live Messaging** — Send messages to your chatbots and receive AI-generated responses in real-time
- **System Monitoring** — Retrieve core account information and monitor your AI usage quotas directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ChatFly API Key (obtained from your dashboard)
3. Start managing your AI chatbots from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Managers** — monitor chatbot performance and review customer interactions using natural language
- **Content Strategists** — manage knowledge base documents and trigger bot retraining without opening the dashboard
- **Product Teams** — quickly test bot responses and verify training status straight from their chat interface
- **Business Owners** — audit total conversations and monitor AI resource usage


## Available Tools
- **list_uploaded_documents**: List all files uploaded to the knowledge base
- **get_chatbot_details**: Get detailed information for a specific chatbot
- **get_conversation_history**: Retrieve the message history for a specific conversation
- **get_chatfly_account_info**: Retrieve core account and quota information
- **list_chatfly_bots**: List all AI chatbots in your account
- **list_fly_conversations**: List recent chat conversations
- **send_bot_message**: Send a message to a chatbot and receive a response
- **trigger_bot_training**: Trigger the training process for a chatbot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CHATFLY** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active chatbots in CHATFLY."

**🤖 AI Agent:**
> Retrieving your chatbots... I found 3 active bots: 'Support Assistant', 'Sales Closer', and 'Internal FAQ Bot'. All are currently 'Ready' and trained.

---

**👤 You:**
> "Show me the last 5 conversations for bot 'Support Assistant'."

**🤖 AI Agent:**
> Retrieving conversations for 'Support Assistant'... I found 5 recent sessions. 3 users were asking about pricing, and 2 were asking about installation.

---

**👤 You:**
> "Send a test message to bot ID 123: 'How do I reset my password?'"

**🤖 AI Agent:**
> Sending message to bot 123... The AI responded: 'To reset your password, go to settings and click on Security. You will find the reset link there.'


## ❓ FAQ

**Q: Can I train my bot on a new PDF file through the agent?**
You can trigger the training process using the `trigger_bot_training` tool once you have added files via the ChatFly dashboard. Future updates will support direct file uploads.

**Q: How do I see the history of a specific conversation?**
Use the `get_conversation_history` tool with the unique conversation ID. Your agent will fetch the full transcript of messages between the user and the bot.

**Q: Where do I find my ChatFly API Key?**
Log in to your ChatFly dashboard and navigate to the 'API' or 'Integrations' section. You can generate and copy your API key from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chatfly](https://vinkius.com/mcp/chatfly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CHATFLY** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chatfly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CHATFLY** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chatfly": {
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
