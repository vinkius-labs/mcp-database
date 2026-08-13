# Claude Session Memory Indexer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/claude-session-memory-indexer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Preserves and retrieves cross-session learnings using deterministic hashing and Jaccard similarity.

## Description
This MCP server solves the problem of lost context in AI coding sessions. It indexes and retrieves cross-session learnings by mapping developer insights to specific project contexts using deterministic hashing. By using `get_project_context`, the system ensures that insights are isolated to the correct project. You can use `index_learning` to save new patterns or commands, and `query_memories` to retrieve them using keyword matching and Jaccard similarity. This allows your AI assistant to remember build commands, debugging patterns, and project conventions across different sessions.


## Available Tools (3)
- **get_project_context**: Provides the current project's unique identity to the caller
- **index_learning**: Persists a new insight or learning into the long-term memory store
- **query_memories**: Searches for relevant past learnings based on a user's current context or question


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claude Session Memory Indexer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How do I run the build for this project?"

**🤖 AI Agent:**
> To run the build, use the command `npm run build` as specified in your project's build commands.

---

**👤 You:**
> "What are the project conventions for naming files?"

**🤖 AI Agent:**
> The project follows kebab-case for all file names.

---

**👤 You:**
> "I'm seeing a recurring error with the database connection. Have we seen this before?"

**🤖 AI Agent:**
> Yes, a similar issue was recorded. It usually occurs when the environment variable `DB_URL` is missing from the local configuration.


## ❓ FAQ

**Q: How does the system ensure memories don't leak between projects?**
The system uses a unique project hash generated from your `CLAUDE.md` and directory structure. This ensures that `index_learning` only stores and retrieves memories belonging to the specific project context.

**Q: Can I filter my search by specific categories?**
Yes, when using `query_memories`, you can provide a `categoryFilter` to narrow down results to specific groups like `build_commands` or `project_conventions`.

**Q: What happens if I save a duplicate learning?**
The system automatically detects near-duplicates. If a new learning has a Jaccard similarity greater than 0.9 with an existing one, it updates the existing entry instead of creating a new one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/claude-session-memory-indexer](https://vinkius.com/mcp/claude-session-memory-indexer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claude Session Memory Indexer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-session-memory-indexer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claude Session Memory Indexer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-session-memory-indexer": {
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
