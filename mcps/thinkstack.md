# ThinkStack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thinkstack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/thinkstack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/thinkstack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage AI chatbots via ThinkStack u2014 query bots, manage knowledge sources, review conversations, and configure actions from your AI agent.

## Description
Connect your **ThinkStack** account to any AI agent and manage your chatbots, knowledge bases, and conversations through natural language.

### What you can do

- **Chatbot Management** u2014 List and configure all AI chatbots in your account
- **Knowledge Base** u2014 Add, list, and remove knowledge sources (URLs, documents) for any chatbot
- **Live Queries** u2014 Send messages to your chatbots and receive AI-generated responses in real time
- **Conversation History** u2014 Review all chat sessions with full message history and user metadata
- **Actions & Webhooks** u2014 View all configured REST API actions for your chatbots

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the ThinkStack dashboard
3. Start managing chatbots from Claude, Cursor, or any MCP client

### Who is this for?

- **Support Teams** u2014 monitor chatbot conversations and optimize knowledge base accuracy
- **Product Managers** u2014 review chatbot usage patterns and refine AI responses
- **Developers** u2014 manage knowledge sources and test chatbot queries programmatically


## Available Tools
- **add_source**: The content will be crawled and indexed automatically.

Add a knowledge source
- **check_thinkstack_status**: Verify ThinkStack API connectivity
- **delete_source**: Remove a knowledge source
- **get_bot**: Get chatbot details
- **get_conversation**: Get conversation details
- **list_actions**: List bot actions
- **list_bots**: List all chatbots
- **list_conversations**: List conversations
- **list_sources**: List knowledge sources
- **send_query**: Query a chatbot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ThinkStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my chatbots in ThinkStack."

**🤖 AI Agent:**
> You have 3 chatbots: 'Support Bot' (24 sources, 1,250 conversations), 'Sales Assistant' (8 sources), and 'Onboarding Guide' (12 sources). Which one would you like to query?

---

**👤 You:**
> "Ask my Support Bot: 'How do I reset my password?'"

**🤖 AI Agent:**
> Support Bot says: 'To reset your password, go to Settings > Security > Change Password. If you forgot your password, click Forgot Password on the login page.' Want to ask another question?

---

**👤 You:**
> "Add docs.example.com as a knowledge source for my Sales bot."

**🤖 AI Agent:**
> URL added successfully. ThinkStack is now crawling docs.example.com — 42 pages detected. The bot's knowledge base will be updated within minutes. Would you like to test a query?


## Installation & Usage

To install and use the **ThinkStack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thinkstack](https://vinkius.com/mcp/thinkstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
