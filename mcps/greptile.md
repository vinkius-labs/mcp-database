# Greptile MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/greptile)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Search and understand any codebase instantly with AI that reads your repositories and answers technical questions accurately.

## Description
Connect your **Greptile** account to any AI agent and unlock AI-powered codebase understanding through natural conversation.

### What you can do

- **AI Codebase Q&A** — Ask natural language questions about one or more repositories and receive AI-generated answers with code references
- **Contextual Follow-ups** — Continue conversations with session context for multi-turn codebase exploration
- **Semantic Code Search** — Search across indexed repositories to find relevant files, functions, and code patterns
- **File-Specific Search** — Target searches within a specific file path for precise results
- **Repository Indexing** — Submit GitHub or GitLab repositories for indexing, check progress, and trigger re-indexing
- **Repository Management** — List all indexed repos, inspect file metadata, and remove outdated indexes
- **Usage Monitoring** — Track API consumption and rate limits

### How it works

1. Subscribe to this server
2. Enter your Greptile API Key from the developer dashboard
3. Start querying your codebase from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — understand unfamiliar codebases, find implementations, and navigate large repositories through conversation
- **Code Reviewers** — search for related patterns, understand code context, and trace dependencies
- **Engineering Managers** — get quick answers about architecture decisions, coding patterns, and technical debt


## Available Tools
- **delete_repository**: Delete indexed repository
- **get_file_info**: Get file info
- **get_repository_status**: Get repository status
- **get_greptile_usage**: Check API usage
- **index_repository**: Index a repository
- **list_repositories**: List indexed repositories
- **query_codebase**: Query codebase with AI
- **query_with_context**: Query with session context
- **reindex_repository**: Reindex a repository
- **search_by_filepath**: Search in specific file
- **search_codebase**: Search codebase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Greptile** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How does the authentication middleware work in our backend repository?"

**🤖 AI Agent:**
> Based on your indexed repository 'github:main:company/backend-api', the authentication middleware is implemented in `src/middleware/auth.ts` (lines 12-48). It uses a JWT-based flow: 1) Extracts the Bearer token from the Authorization header (line 18). 2) Verifies the token signature using the RS256 algorithm with a public key from `config/keys.ts` (line 24). 3) Attaches the decoded user payload to `req.user` (line 32). 4) Falls through to a 401 handler if verification fails (line 41). The middleware is applied globally in `src/app.ts` line 15 via `app.use(authMiddleware)`. Would you like to search for how specific routes use this middleware?

---

**👤 You:**
> "Search for all files that import the database connection module and show me the file info."

**🤖 AI Agent:**
> Semantic search for 'database connection import' found 8 files: 1) `src/services/user-service.ts` — imports `db` from `../config/database`, 42 functions. 2) `src/services/order-service.ts` — imports `db`, 28 functions. 3) `src/repositories/user-repo.ts` — imports `pool` from database config, 15 functions. 4) `src/migrations/001-initial.ts` — direct pg import for schema setup. 5-8) Four test files importing the test database mock. File info for `src/config/database.ts`: 89 lines, exports `db` (Knex instance) and `pool` (pg Pool), last indexed 2 hours ago. Would you like to query how the connection pooling is configured?

---

**👤 You:**
> "Index our new frontend repository and check the indexing status."

**🤖 AI Agent:**
> Repository submitted for indexing! Remote: github, Repository: company/frontend-app, Branch: main. Current status: 'processing' — 45% complete (scanning 1,247 files). Estimated time remaining: 3 minutes. Indexed repositories: 3 total. 1) 'company/backend-api' (main, completed, 892 files). 2) 'company/shared-lib' (main, completed, 234 files). 3) 'company/frontend-app' (main, processing, 45%). Once completed, you'll be able to query and search the frontend codebase. Would you like to check again in a few minutes?


## ❓ FAQ

**Q: Can I ask natural language questions about my codebase?**
Yes! The `query_codebase` tool sends a natural language question along with repository references and returns AI-generated answers with specific code references (file paths and line numbers). For follow-up questions, use `query_with_context` with the session ID from the previous response to maintain conversation continuity.

**Q: Do I need to index my repository before querying it?**
Yes. Use `index_repository` with the remote host (github or gitlab), repository path (owner/repo), and branch name. Check indexing progress with `get_repository_status`. Once indexed, you can query and search the repository. Use `reindex_repository` to refresh the index after significant code changes.

**Q: Can I search for specific code patterns across my repositories?**
Yes. The `search_codebase` tool performs semantic search across your indexed repositories to find relevant files and functions. For targeted results, use `search_by_filepath` to narrow the search to a specific file path. Use `get_file_info` to retrieve indexed metadata for any file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/greptile](https://vinkius.com/mcp/greptile)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Greptile** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `greptile` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Greptile** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "greptile": {
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
