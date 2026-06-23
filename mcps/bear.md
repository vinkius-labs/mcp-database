# Bear MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bear)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Bear notes via AI — search, create, and organize your markdown knowledge base autonomously.

## Description
Connect your **Bear App** database to any AI agent and manage your entire localized knowledge base through natural conversation.

### O que você pode fazer

- **Note Operations** — Search globally, read explicit full-markdown note content, and orchestrate the creation of rich hierarchical docs
- **Content Mutation** — Inject new blocks into existing resources (`add_text`), avoiding constant manual copy-pasting
- **Lifecycle Control** — Move outdated research aggressively to the Archive or permanently isolate abandoned drafts in the Trash
- **Taxonomy & Tags** — List tags, explore bounded nested hierarchies, or completely rename structural tags across thousands of items

### Como funciona

1. Subscribe to this server
2. Enter your Bear API Token (interfacing directly with your private local instance)
3. Take absolute control of your linked-thinking graph via Claude or Cursor natively

Say goodbye to breaking focus. Your autonomous agent fetches the precise code snippets or creative writing you saved months ago without breaking context.

### Para quem é?

- **Developers** — inject raw saved configuration blocks directly into your active coding environment
- **Writers & Researchers** — let the AI read your fragmented thoughts, organize your nested active tags, and assemble pristine drafts
- **Productivity Enthusiasts** — search the "@todo" tag instantly summarizing all pending personal action items


## Available Tools (10)
- **search_notes**: g. @todo @today).

Search across all Bear app notes
- **open_note**: Retrieve explicit complete Markdown content of a Bear note
- **create_note**: Create a new native Bear note
- **add_text**: Append or prepend Markdown chunks to a Bear note
- **trash_note**: Move an explicit Bear Note to the Trash
- **archive_note**: Archive an explicit Bear Note
- **list_tags**: g. parent/child).

Retrieve the exact Tags taxonomy nesting globally
- **open_tag**: List all explicit Bear notes matching a specific tag
- **rename_tag**: Rename globally an entire tag across all mapped Notes
- **delete_tag**: Destroy entirely a Tag constraint globally


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bear** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Bear notes for anything mentioning 'Database Migration 2026'."

**🤖 AI Agent:**
> The query returned 3 explicit note UUIDs. The highly relevant document is titled 'Q1 Migration Plan' (UUID: FE12...). Should I open this full exact note fetching its entire underlying Markdown syntax?

---

**👤 You:**
> "Rename the tag '#project/legacy' to '#archive/legacy_projects' across all my notes."

**🤖 AI Agent:**
> Globally executed target mutation. The tag '#project/legacy' has been fully reconstructed into '#archive/legacy_projects'. Bear natively propagated changes eliminating any obsolete string traces successfully.

---

**👤 You:**
> "Create a new note with the title 'Meeting Notes - App V2' and tag it 'work/meetings/vurb'."

**🤖 AI Agent:**
> The note 'Meeting Notes - App V2' has been initialized via API injection and synced instantly. Its explicitly nested taxonomy tag 'work/meetings/vurb' binds correctly inside the local knowledge cache.


## ❓ FAQ

**Q: Can the AI precisely update a note without overwriting its entire content?**
Yes. It uses the `add_text` mutation tool, seamlessly attaching blocks of text to either the absolute bottom (append) or the explicit top (prepend) of the given UUID note, leaving the core intact.

**Q: Does it understand nested tags (like #work/design/logo)?**
Bear relies heavily on tagging workflows. The agent natively queries and navigates explicit sub-tag pathways exactly like the application UI, mapping out your distinct taxonomy rules efficiently.

**Q: Can it search for uncompleted action items across many notes?**
Simply ask the agent to search for the specialized string '@todo'. Bear exposes these native markers directly via the API, returning every unique UUID containing a matching string checklist efficiently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bear](https://vinkius.com/mcp/bear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bear** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bear` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bear** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bear": {
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
