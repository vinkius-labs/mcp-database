# Slite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/slite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage your Slite knowledge base, notes, and AI insights with AI agents.

## Description
### What you can do
- List, create, and update notes in your workspace knowledge base.
- Search for documents using keywords and nested hierarchies.
- Ask Slite AI questions to derive answers directly from your documentation.
- Manage document quality by verifying docs or flagging outdated content.

### How it works
1. Obtain your API Key from your Slite workspace settings under Developer.
2. Enter your credentials in Vinkius platform.
3. Start chatting with your Slite agent to manage your team's knowledge.

### Who is it for?
- Teams needing automated documentation management.
- Product managers tracking specifications and meeting notes.
- Operations teams keeping the internal knowledge base verified and up-to-date.


## Available Tools (12)
- **ask_slite_ai**: Ask a question to Slite AI
- **create_note**: Create a new note in Slite
- **flag_outdated**: Flag a document as needing review
- **get_me**: Get current user profile
- **get_note**: Get details and content of a specific note
- **list_note_children**: List sub-notes of a parent
- **list_collections**: List all structured collections
- **list_notes**: List all notes in Slite
- **list_users**: List organization users
- **search_notes**: Search for notes in your workspace
- **update_note**: Update an existing note
- **verify_note**: Mark a document as verified


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for notes about the 'Marketing Plan' in Slite."

**🤖 AI Agent:**
> I've found 2 notes: 1. Marketing Plan 2026 (ID: n1), 2. Q3 Ad Strategy (ID: n2).

---

**👤 You:**
> "Show me the most active knowledge base documents this month with view counts and contributors."

**🤖 AI Agent:**
> Top 10 documents by activity. #1: "API Documentation v3" (456 views, 12 edits, 5 contributors). #2: "Onboarding Guide 2025" (345 views, 8 edits). #3: "Architecture Decision Records" (234 views, 15 edits, most collaborative). #4: "Sprint Planning Template" (198 views). #5: "Security Policies" (167 views, 3 edits). Total docs: 234. New this month: 18. Updated: 45. Stale (90+ days no edit): 67. Search queries: 890. Most searched: "API authentication" (34 searches). Knowledge coverage score: 78%.

---

**👤 You:**
> "Search the knowledge base for all documents related to API authentication and rate limiting."

**🤖 AI Agent:**
> Found 8 documents matching "API authentication" and "rate limiting". Most relevant: "API Authentication Guide" (last updated 3 days ago, OAuth 2.0, API keys, JWT tokens covered). "Rate Limiting Policy" (updated last week, 1000 req/min default, burst handling). "API Security Best Practices" (comprehensive, 2,340 words). "Developer Quickstart" (getting started with auth). "Troubleshooting Auth Errors" (common 401/403 fixes). 3 additional related docs. Combined reading time: 45 minutes. 2 documents flagged as needing review.


## ❓ FAQ

**Q: Can I ask questions to Slite AI?**
Yes, use the ask_slite_ai tool to get answers sourced directly from your documents.

**Q: How do I create a nested note?**
When using create_note, provide the note_id of the parent in the parent_note_id parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slite](https://vinkius.com/mcp/slite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Slite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `slite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slite": {
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
