# BotGenuity MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/botgenuity)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/botgenuity-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/botgenuity-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Create and manage AI chatbots with custom knowledge bases that answer customer questions accurately around the clock.

## Description
Connect your **BotGenuity** account to any AI agent and take full control of your automated customer engagement and chatbot operations through natural conversation.

### What you can do

- **Bot Orchestration** — List and manage all your AI chatbot instances programmatically, retrieving detailed configuration and high-fidelity operational status in real-time
- **Lead Capture Intelligence** — Access complete directories of leads captured during bot interactions, including high-fidelity contact metadata and conversation context
- **Conversation Discovery** — Retrieve detailed chat histories and individual message threads to maintain a perfectly coordinated overview of customer needs
- **Real-Time Interaction** — Programmatically send messages to your chatbots to test performance or integrate bot responses into custom business workflows
- **Platform Monitoring** — Access chatbot configuration details and monitor account-level connectivity directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** (Bearer Token) from your BotGenuity dashboard (Settings > Security)
3. Start managing your conversational AI pipeline from Claude, Cursor, or any MCP client

No more manual toggling between chatbot portals or digging through individual lead tables. Your AI acts as your dedicated bot engineer and lead coordinator.

### Who is this for?

- **Customer Support Teams** — instantly retrieve chat histories and monitor bot performance using natural language commands
- **Marketing Managers** — track lead generation trends and verify bot engagement without leaving your workspace
- **Product Teams** — integrate custom-trained chatbot responses into internal tools through simple AI queries


## Available Tools
- **get_chatbot_details**: Get details of a specific chatbot
- **get_conversation_history**: Get full history for a conversation
- **list_chatbots**: List all chatbots in your BotGenuity account
- **list_chatbot_conversations**: List conversations for a chatbot
- **list_captured_leads**: List leads captured by a chatbot
- **chat_with_bot**: Send a message to a chatbot and get a response


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BotGenuity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my chatbots in BotGenuity."

**🤖 AI Agent:**
> I've retrieved your chatbots. You currently have 3 active bots, including 'Customer Hero' (ID: B123) and 'Sales Assistant'. Which one should we check for lead activity?

---

**👤 You:**
> "Show the captured leads for chatbot ID 'B123'."

**🤖 AI Agent:**
> Fetching leads... Chatbot B123 has captured 12 new leads today, including @user1 and @user2. I've retrieved their contact metadata and high-fidelity interest tags for you.

---

**👤 You:**
> "Ask my 'Customer Hero' bot: 'What are our shipping rates?'."

**🤖 AI Agent:**
> Bot response received: 'Our standard shipping is $5.99, or free for orders over $50.' Shall I check the session logs for this interaction?


## Installation & Usage

To install and use the **BotGenuity** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/botgenuity](https://vinkius.com/mcp/botgenuity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
