# Bot9 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bot9)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bot9-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bot9-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage your AI agents via Bot9 — orchestrate bots, train them, and automate conversations directly from any AI agent.

## Description
Connect your **Bot9** account to any AI agent and orchestrate your customer support and conversational automation workflows through natural language.

### What you can do

- **Bot Management** — List all configured AI bots, retrieve specific configurations, and create new bots on the fly.
- **Training & Data Sources** — List existing knowledge base sources and dynamically add new URLs for your bots to learn from.
- **Conversation Oversight** — Retrieve active conversation lists and export historical chat logs for analysis.
- **Message Automation** — Send messages to your bots programmatically to test responses or simulate user interactions.

### How it works

1. Subscribe to this server
2. Enter your Bot9 API Key
3. Start managing your conversational AI fleet from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **add_data_source**: Add a URL to train the bot
- **create_bot**: Create a new AI chatbot
- **get_bot**: Get details of a specific bot
- **get_conversation_history**: Retrieve message history of a conversation
- **list_bots**: List all AI bots
- **list_conversations**: List active conversations for a bot
- **list_data_sources**: List knowledge base sources for a bot
- **send_message**: Send a message to a bot and get a response


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bot9** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all bots in my Bot9 account."

**🤖 AI Agent:**
> I've retrieved your bots. You currently have 'Support Assistant' (ID: bot_123) and 'Sales Lead Gen' (ID: bot_456).

---

**👤 You:**
> "Add the URL https://example.com/pricing to bot_123's knowledge base."

**🤖 AI Agent:**
> The URL has been successfully added to bot_123. The bot is now training on the new pricing data.

---

**👤 You:**
> "Get the chat history for conversation conv_789 on bot_123."

**🤖 AI Agent:**
> Retrieving the history... The user asked 'What are your operating hours?' and the bot replied 'We are open 9AM to 5PM EST'.


## Installation & Usage

To install and use the **Bot9** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bot9](https://vinkius.com/mcp/bot9)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
