# Mem0 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mem0)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Give your AI agent persistent memory — store, search, and recall facts, preferences, and context across sessions using the leading agent memory platform.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mem0** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Remember that I prefer dark mode, use VS Code, and my favorite language is TypeScript."

**🤖 AI Agent:**
> Stored 3 new memories for your profile:
1. 'User prefers dark mode for UI'
2. 'User's primary IDE is VS Code'
3. 'User's favorite programming language is TypeScript'
These will be automatically recalled in future conversations.

---

**👤 You:**
> "What do you remember about my coding preferences?"

**🤖 AI Agent:**
> Found 3 relevant memories (ranked by relevance):
🧠 'User's favorite programming language is TypeScript' (relevance: 0.95)
🧠 'User's primary IDE is VS Code' (relevance: 0.89)
🧠 'User prefers dark mode for UI' (relevance: 0.72)

---

**👤 You:**
> "Show me all the memories you have stored for my user profile."

**🤖 AI Agent:**
> Found 5 memories for user_123:
🧠 'User prefers dark mode'
🧠 'User's primary IDE is VS Code'
🧠 'Favorite language is TypeScript'
🧠 'Works best in the morning'
🧠 'Prefers functional programming patterns'
Created between 2026-01-15 and 2026-04-01.


## ❓ FAQ

**Q: Is Mem0 free to use?**
Yes! Mem0 offers a free Hobby tier with 10,000 memories and 1,000 search calls per month — no credit card required. Paid plans start at $19/month for higher limits. An open-source version (Apache 2.0) is also available for self-hosting.

**Q: How does Mem0 extract and store memories?**
When you send content to Mem0, its AI automatically extracts key facts and structured information. For example, if you send 'I prefer Python over JavaScript and work best in the morning', Mem0 creates two separate memories: one about language preference and one about work schedule. These are stored in a hybrid architecture (key-value + vector + graph) for fast semantic retrieval.

**Q: Can I organize memories by user or agent?**
Yes! Every memory operation supports scoping by user_id, agent_id, or run_id. This means you can maintain separate memory banks for different users, different agents, or even different conversation runs — keeping context perfectly isolated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mem0](https://vinkius.com/mcp/mem0)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mem0** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mem0` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mem0** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mem0": {
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
