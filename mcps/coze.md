# Coze MCP Server

Orchestrate Coze bots — manage conversations, handle RAG datasets, and trigger bot actions directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coze)

## Overview
**Category:** industry-titans
**Tools Count:** 11

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


## Installation & Usage

To install and use the **Coze** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coze](https://vinkius.com/mcp/coze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
