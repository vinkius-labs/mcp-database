# Aidbase MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aidbase)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aidbase-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aidbase-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deploy AI-powered customer support chatbots, manage knowledge bases, and resolve tickets faster with intelligent automation.

## Description
Connect your **Aidbase** account to any AI agent and take full control of your automated customer support and intelligent knowledge management workflows through natural conversation.

### What you can do

- **Chatbot Orchestration** — List and manage all configured AI chatbots programmatically, retrieving detailed high-fidelity metadata and configuration settings in real-time
- **Knowledge Graph Ingestion** — Programmatically update what your AI knows by pushing new website URLs or injecting specific Q&A items into existing FAQs dynamically
- **Conversational Intelligence** — Send messages and retrieve high-fidelity AI responses from specific chatbots to test performance or integrate chat into custom workflows
- **AI Email Inbox Management** — Access and monitor your automated email responders and their assigned knowledge bases to ensure perfectly coordinated context application
- **Operational Monitoring** — Verify API connectivity and retrieve account-level status directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Aidbase dashboard (Settings > API Keys)
3. Start orchestrating your customer service intelligence from Claude, Cursor, or any MCP client

No more manual logging into support portals to update FAQs or check bot logs. Your AI acts as your dedicated support engineer and knowledge architect.

### Who is this for?

- **Customer Support Leads** — instantly update AI knowledge bases with fresh documentation using natural language commands
- **Product Managers** — monitor chatbot interactions and verify responder accuracy without leaving your workspace
- **Developers** — integrate high-speed AI support intelligence into custom internal tools through simple AI queries


## Available Tools
- **add_aidbase_faq_item**: Add FAQ to knowledge base
- **add_aidbase_website_knowledge**: Add a website to knowledge base
- **check_aidbase_status**: Check API Status
- **get_aidbase_chatbot**: Get Chatbot details
- **get_aidbase_inbox**: Get AI Inbox details
- **list_aidbase_chatbot_knowledge**: List Chatbot knowledge items
- **list_aidbase_chatbots**: List all AI Chatbots
- **list_aidbase_inboxes**: List Email AI Inboxes
- **list_aidbase_inbox_knowledge**: List Inbox knowledge items
- **list_aidbase_knowledge**: List all Knowledge items
- **send_aidbase_reply**: Send a message to a Chatbot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aidbase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all configured chatbots in my Aidbase account."

**🤖 AI Agent:**
> I've retrieved your chatbots. You currently have 3 active bots, including 'Support Hero' (ID: bot_123) and 'Lead Qualifier'. Which one should we test or update with new knowledge?

---

**👤 You:**
> "Add 'https://docs.vinkius.com/faq' to my AI knowledge base."

**🤖 AI Agent:**
> Knowledge ingestion triggered! I've added the FAQ URL to your global knowledge base. Aidbase is now indexing the content. I'll notify you when your bots are updated with this high-fidelity data.

---

**👤 You:**
> "Send a message to chatbot 'bot_123': 'What is your refund policy?'."

**🤖 AI Agent:**
> Chatbot response received: 'Our refund policy allows for full returns within 30 days of purchase.' I've documented the session ID for your high-fidelity interaction logs.


## Installation & Usage

To install and use the **Aidbase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aidbase](https://vinkius.com/mcp/aidbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
