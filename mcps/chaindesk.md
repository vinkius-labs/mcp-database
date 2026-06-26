# Chaindesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chaindesk)
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


## Available Tools (11)
- **list_agents**: List all AI agents
- **list_conversations**: Can be filtered by agentId.

List chat conversations
- **list_datastores**: List all datastores
- **get_datastore**: Get details of a datastore
- **query_agent**: Send a message to an agent
- **update_agent**: Update an existing agent
- **create_agent**: Provide name, datastoreId, and system prompt.

Create a new AI agent
- **delete_agent**: Delete an agent
- **get_agent**: Get details of a specific agent
- **get_messages**: Get messages from a conversation
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


## ❓ FAQ

**Q: How do I find my Chaindesk API Key?**
Log in to your Chaindesk.ai account, navigate to **Settings** > **API Keys**, and generate a new key for your integration.

**Q: What is a Datastore?**
A Datastore is a collection of documents and URLs that your AI agent uses as its knowledge base to answer queries accurately.

**Q: Can I maintain conversation context via AI?**
Yes! Provide a unique `conversationId` to the `query_agent` tool to maintain historical context across multiple turns with your custom bot.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chaindesk](https://vinkius.com/mcp/chaindesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chaindesk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chaindesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chaindesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chaindesk": {
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
