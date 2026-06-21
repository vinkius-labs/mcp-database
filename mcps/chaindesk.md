# Chaindesk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chaindesk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chaindesk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chaindesk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Build no-code AI agents trained on your own data that handle customer support, lead qualification, and FAQ resolution.

## Description
Connect your **Chaindesk.ai** account to any AI agent and take full control of your custom LLM orchestration and automated knowledge retrieval workflows through natural conversation.

### What you can do

- **Agent Orchestration** — Create and manage multiple high-fidelity AI agent instances programmatically, including configuring system prompts and model selection
- **Knowledge Graph Ingestion** — Programmatically upsert data sources (website URLs, text, documents) into connected datastores to maintain a real-time knowledge base
- **Deep Semantic Querying** — Interact with your custom agents to retrieve context-aware AI responses based on your proprietary data and high-fidelity grounding
- **Conversation Intelligence** — Access complete session histories and message threads to provide perfectly coordinated context for support and research tasks
- **Datastore Monitoring** — Access and monitor your directory of knowledge collections (datastores) and their status directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Chaindesk dashboard (Settings > API Keys)
3. Start building and querying your custom AI assistants from Claude, Cursor, or any MCP client

No more manual copy-pasting of text for bot training. Your AI acts as your dedicated agent engineer and knowledge architect.

### Who is this for?

- **Developers & Ops** — integrate custom-trained AI models into internal tools and automate document ingestion using natural language commands
- **Support Teams** — monitor agent responses and update knowledge bases in real-time without leaving your workspace
- **Product Leads** — coordinate the deployment of specialized AI assistants for different business units through simple AI queries


## Available Tools
- **create_agent**: Provide name, datastoreId, and system prompt.

Create a new AI agent
- **delete_agent**: Delete an agent
- **get_agent**: Get details of a specific agent
- **get_datastore**: Get details of a datastore
- **get_messages**: Get messages from a conversation
- **list_agents**: List all AI agents
- **list_conversations**: Can be filtered by agentId.

List chat conversations
- **list_datastores**: List all datastores
- **query_agent**: Send a message to an agent
- **update_agent**: Update an existing agent
- **upsert_datasource**: Add or update a data source


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chaindesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available AI agents in Chaindesk."

**🤖 AI Agent:**
> I've retrieved your AI agents. You currently have 3 active bots: 'Support Bot' (ID: agent_1), 'Legal Analyst', and 'Product Research'. Which one would you like to query or update?

---

**👤 You:**
> "Ask my 'Support Bot' (ID: 'agent_1'): 'How do I reset my password?'."

**🤖 AI Agent:**
> Querying agent... Support Bot response: 'To reset your password, go to the login page and click Forgot Password. You will receive an email with instructions.' I've documented the session ID for context.

---

**👤 You:**
> "Add 'https://vinkius.com/faq' to datastore 'ds_123'."

**🤖 AI Agent:**
> Knowledge ingestion triggered! I've added the FAQ URL to datastore ds_123. Chaindesk is now processing the content to update your agents' knowledge base. Need any other sources added?


## Installation & Usage

To install and use the **Chaindesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chaindesk](https://vinkius.com/mcp/chaindesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
