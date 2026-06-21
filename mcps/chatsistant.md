# Chatsistant MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chatsistant)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chatsistant-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chatsistant-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Chatsistant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chatsistant](https://vinkius.com/mcp/chatsistant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
