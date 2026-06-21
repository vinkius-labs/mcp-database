# Coze MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coze)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/coze-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/coze-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Coze bots — manage conversations, handle RAG datasets, and trigger bot actions directly from any AI agent.

## Description
Connect your AI agents to **Coze** (扣子), the advanced bot orchestration platform by ByteDance. This MCP provides 11 tools to manage the full lifecycle of your bots, from chat interactions to knowledge base document ingestion.

### What you can do

- **Bot Interaction** — Chat with published bots and handle multi-turn conversations with persistent history
- **Knowledge Engineering** — Upload, list, and delete documents in knowledge base datasets for RAG optimization
- **Workspace Management** — List available spaces and published bots to monitor your AI ecosystem
- **Action Handling** — Submit tool outputs when bots require human-in-the-loop or external plugin results

### How it works

1. Subscribe to this server
2. Sign up at [**Coze.com**](https://www.coze.com/) or [**Coze.cn**](https://www.coze.cn/)
3. Generate a **Personal Access Token (PAT)** from your profile settings
4. Identify your **Base URL** (e.g., `https://api.coze.com` for international or `https://api.coze.cn` for China)
5. Connect your account to Vurb to start automating your bot workflows.

### Who is this for?

- **Knowledge Engineers** — automate the ingestion of documentation across multiple datasets
- **RAG Developers** — debug semantic search results and optimize chunking strategies programmatically
- **System Integrators** — build complex AI workflows that require dynamic knowledge base management


## Available Tools
- **create_chat**: Send a message to a Coze bot and get a response
- **list_bots**: List published bots in a specific Coze Space
- **list_datasets**: List knowledge base datasets in a Coze Space
- **list_workspaces**: List available Coze workspaces/spaces
- **publish_bot**: Publish a Coze Bot draft
- **submit_tool_outputs**: Submit outputs for tools/plugins required by the bot
- **upload_document**: Upload a raw text document to a Knowledge Base
- **upload_file_url**: Upload an external file URL to Coze storage
- **clear_conversation**: Clear all messages from a conversation session
- **delete_document**: Delete documents from a dataset by ID
- **get_conversation_history**: Retrieve the message list from a conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Chat with bot 'bot_123' and ask 'Tell me about the history of Tokyo'."

**🤖 AI Agent:**
> Initializing Coze chat session... The bot responded: 'Tokyo, originally known as Edo, has a rich history dating back to the 12th century...' Would you like to continue the conversation?

---

**👤 You:**
> "List all active workspaces in my Coze account."

**🤖 AI Agent:**
> Fetching your Coze spaces... I found 2 active workspaces: 1. Main Project (ID: sp_1), 2. Sandbox (ID: sp_2). Which one would you like to explore?

---

**👤 You:**
> "Upload the content of 'manual.txt' to dataset 'ds_999'."

**🤖 AI Agent:**
> Reading 'manual.txt' and preparing for upload... Content successfully pushed to dataset 'ds_999'. The information is now being indexed for your RAG workflows.


## Installation & Usage

To install and use the **Coze** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coze](https://vinkius.com/mcp/coze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
