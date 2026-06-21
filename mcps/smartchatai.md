# SmartChatAI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smartchatai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage AI bots, knowledge bases, and messaging on SmartChatAI with AI agents.

## Description
Connect your **SmartChatAI** account to any AI agent to automate your intelligent chatbot orchestration and lead collection. SmartChatAI provides a premier platform for building custom AI bots, and this integration allows you to retrieve chatbot metadata, manage knowledge bases via URL or PDF, and track conversational history through natural conversation.

### What you can do

- **Chatbot Orchestration** — List all managed AI bots and retrieve detailed profile metadata, including status and configuration programmatically.
- **Knowledge Base Lifecycle Management** — Add new data sources (URL, PDF, Text) to your bots' knowledge base directly from the AI interface to ensure they are always informed.
- **Message & Reply Control** — Send automated replies and retrieve detailed chat history to maintain high-quality customer interactions via natural language.
- **Web Scraper Automation** — Trigger website scraping to ingest content into your AI models and ensure your bots have the latest information.
- **Operational Monitoring** — Track system health, manage webhooks, and monitor bot activity to ensure your conversational platform is always optimized.

### How it works

1. Subscribe to this server
2. Enter your SmartChatAI API Key from your dashboard settings
3. Start managing your AI bots from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Bot Developers** — quickly update knowledge bases and test bot responses without switching tabs.
- **Marketing Operations** — automate the retrieval of lead data from chats and monitor bot engagement results via natural conversation.
- **Customer Success Teams** — streamline the retrieval of conversational logs and monitor user satisfaction directly within the chat.


## Available Tools (12)
- **add_pdf_to_knowledge_base**: Train bot using a PDF
- **add_text_to_knowledge_base**: Train bot using raw text
- **add_website_to_knowledge_base**: Train bot using a URL
- **check_api_health**: Verify SmartChatAI API status
- **create_new_ai_bot**: Requires a name and optional initial prompt.

Provision a new AI agent
- **get_chatbot_details**: Get configuration for a specific bot
- **get_bot_chat_history**: Retrieve conversation transcripts
- **get_authenticated_user_profile**: Get account profile
- **list_ai_chatbots**: List all AI chatbots
- **list_configured_webhooks**: List active webhooks
- **scrape_domain_links**: Discover and index domain links
- **message_ai_chatbot**: Send a message and get AI reply


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SmartChatAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active AI bots in my SmartChatAI account."

**🤖 AI Agent:**
> I've retrieved your bots. You have 3 active bots online: 'Customer Support Lead', 'Sales Assistant', and 'FAQ Guide'. Which one would you like to update?

---

**👤 You:**
> "Show me all active chatbot conversations with their resolution rates and average response times."

**🤖 AI Agent:**
> 45 active conversations across 3 chatbot flows. "Customer Support" (28 active): Resolution rate 84%, avg response 1.2s, 23 resolved without agent handoff. "Sales Assistant" (12 active): 67% lead qualification rate, avg 1.8s. "FAQ Bot" (5 active): 92% answer accuracy. Today's totals: 234 conversations completed, 12 escalated to human agents (5.1%), customer satisfaction: 4.6/5. Peak hour: 2-3 PM (45 concurrent chats). Most asked topic: "pricing plans" (34 times).

---

**👤 You:**
> "Train the chatbot with 10 new FAQ entries about our refund and return policies."

**🤖 AI Agent:**
> 10 FAQ entries added to knowledge base. Topics: refund eligibility (30-day window), return shipping process, exchange policy, digital product refunds, partial refund scenarios, international returns, defective item procedure, refund processing time (5-7 business days), gift return policy, subscription cancellation refunds. Training status: complete. Confidence score improvement: FAQ accuracy expected to increase from 89% to 95% on refund topics. 234 existing intents re-evaluated. No conflicts detected.


## ❓ FAQ

**Q: How do I find my SmartChatAI API Key?**
Log in to your SmartChatAI dashboard and you will find your unique secret API Key in the Settings or account management section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smartchatai](https://vinkius.com/mcp/smartchatai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SmartChatAI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smartchatai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SmartChatAI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smartchatai": {
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
