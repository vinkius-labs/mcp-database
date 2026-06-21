# Voiceflow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/voiceflow)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/voiceflow-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/voiceflow-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Design, prototype, and launch conversational AI agents with a visual builder that handles complex dialog flows without code.

## Description
Connect your **Voiceflow** account to any AI agent and simplify how you build, test, and monitor your conversational assistants through natural language conversation.

### What you can do

- **Agent Interaction** — Send messages and trigger actions in your Voiceflow agents to test responses and flows instantly.
- **Knowledge Base (RAG) Control** — Query your agent's KB directly for answers and list uploaded documents and tags.
- **State Management** — Retrieve, update, or reset user conversation states and variables to debug complex logic.
- **Transcript Analysis** — List and fetch full conversation logs for any project to monitor user interactions.
- **Operational Monitoring** — Retrieve user feedback (upvotes/downvotes) and monitor project configurations in real-time.

### How it works

1. Subscribe to this server
2. Enter your Voiceflow API Key and Version ID
3. Start managing your conversational ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Conversation Designers** — quickly test agent responses and query the knowledge base via simple AI commands.
- **AI Developers** — debug user states and inspect transcripts during the development and testing cycle.
- **Product Managers** — monitor user feedback and conversation logs directly from the workspace.


## Available Tools
- **delete_state**: Reset user session
- **get_feedback**: Get user feedback
- **get_project**: Get project details
- **get_state**: Get user conversation state
- **get_transcript**: Get transcript details
- **interact**: Send message to Voiceflow agent
- **list_kb_docs**: List KB documents
- **list_kb_tags**: List KB document tags
- **list_projects**: List Voiceflow projects
- **list_transcripts**: List conversation transcripts
- **query_kb**: Ask the Knowledge Base
- **save_state**: Update user state/variables


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Voiceflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Voiceflow projects."

**🤖 AI Agent:**
> I've retrieved your projects. You have access to: 'Customer Support Bot', 'Sales Assistant v2', and 'Internal FAQ Bot'. Which one would you like to inspect?

---

**👤 You:**
> "Ask my KB: 'What is the return policy for international orders?'"

**🤖 AI Agent:**
> According to your Knowledge Base, international orders can be returned within 30 days, but the customer is responsible for shipping costs. Would you like the source document details?

---

**👤 You:**
> "Show me the last 3 transcripts for the 'Customer Support Bot'."

**🤖 AI Agent:**
> I've fetched the transcripts. Here are the 3 most recent sessions: User_8823 (Success), User_8824 (Dropped), and User_8825 (Handoff to Human). Shall I retrieve the dialogue for the dropped session?


## Installation & Usage

To install and use the **Voiceflow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/voiceflow](https://vinkius.com/mcp/voiceflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
