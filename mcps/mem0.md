# Mem0 MCP Server

Give your AI agent persistent memory — store, search, and recall facts, preferences, and context across sessions using the leading agent memory platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mem0)

## Overview
**Category:** ai-frontier
**Tools Count:** 4

## Description
Connect your AI agent to **Mem0** — the industry-standard memory layer that enables agents to remember, learn, and personalize across conversations.

### What you can do

- **Add Memories** — Store facts, preferences, and context from conversations. Mem0 AI automatically extracts key information and structures it as searchable memories
- **Semantic Search** — Find relevant memories using natural language queries. Ask 'What does the user prefer?' and get ranked results by relevance
- **List Memories** — View all stored memories for a user to build comprehensive profiles and understand accumulated context
- **Delete Memories** — Remove outdated or incorrect memories to keep the knowledge base clean

### How it works

1. Subscribe to this server
2. Enter your Mem0 API key (free tier available — 10K memories/month)
3. Your agent can now remember everything across sessions

### Who is this for?

- **AI Agent Developers** — build agents that remember user preferences, past decisions, and accumulated context without re-asking
- **Chatbot Builders** — create conversational experiences that feel truly personal by recalling past interactions
- **SaaS Teams** — add persistent memory to any AI feature so users feel understood and valued


## Available Tools
- **delete_memory**: Use with caution — this action cannot be undone.

Delete a specific memory by its ID
- **get_memories**: Useful for reviewing what the agent knows about a user or for building a user profile.

List all stored memories for a specific user
- **search_memories**: Returns results ranked by relevance score, enabling the agent to recall past preferences, facts, and context.

Semantically search stored memories for a specific user. Returns the most relevant memories matching your query
- **add_memory**: The system automatically extracts structured facts from the provided content and stores them as searchable, persistent memories associated with the given user ID.

Store a new memory for a user. The AI extracts key facts and preferences from the content and stores them as persistent memories


## Installation & Usage

To install and use the **Mem0** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mem0](https://vinkius.com/mcp/mem0)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
