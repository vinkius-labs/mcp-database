# Zoho Notebook MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-notebook)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage notebooks, capture notes, and organize your ideas on Zoho Notebook — the secure and beautiful note-taking app.

## Description
Connect your **Zoho Notebook** account to any AI agent and take control of your personal and professional knowledge base through natural conversation.

### What you can do

- **Notebook Organization** — List all your notebooks, create new ones for specific projects, or delete obsolete collections directly from your agent
- **Notecard Discovery** — Browse and list all notecards within any notebook to find relevant information and retrieve unique card IDs
- **Content Capture** — Create new text or checklist notecards instantly by providing a title and body content through simple commands
- **Rich Notecards** — Retrieve full metadata and content for specific cards, including support for different types (text, checklist, etc.)
- **Global Search** — Search across all your notebooks and cards by keyword to find specific ideas or data points instantly
- **Idea Management** — Update existing notecards with new information or permanently delete obsolete items through conversation
- **Workspace Auditing** — Verify your notebook hierarchy and retrieve unique IDs required for automated knowledge workflows

### How it works

1. Subscribe to this server
2. Enter your Zoho Notebook Access Token
3. Start managing your ideas through Claude, Cursor, or any MCP-compatible client

No more manual digging through cards to find a meeting note. Your AI agent becomes your personal knowledge assistant.

### Who is this for?

- **Productivity Seekers** — quickly capture ideas and organize project notes through simple chat commands
- **Content Creators** — manage research notebooks and search across multiple draft cards without manual filtering
- **Project Leads** — organize team knowledge into specific notebooks and retrieve card details through conversation
- **Students & Researchers** — search through massive collections of study notes and update existing entries efficiently


## Available Tools (10)
- **list_notecards**: Notebook ID is required.

List notecards in notebook
- **create_notecard**: Create notecard
- **create_notebook**: Useful for organizing notecards.

Create notebook
- **delete_notecard**: Delete notecard
- **delete_notebook**: Delete notebook
- **get_notecard**: Get notecard details
- **get_notebook**: Get notebook details
- **list_notebooks**: Returns notebook IDs which are needed to fetch notecards.

List all notebooks
- **search_notecards**: Search notecards
- **update_notecard**: Update notecard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Notebook** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my notebooks in Zoho Notebook."

**🤖 AI Agent:**
> I found 3 notebooks: 1. 'Personal Ideas' (ID: nb-101), 2. 'Project Roadmap' (ID: nb-102), and 3. 'Meeting Notes' (ID: nb-103). Which one would you like to browse?

---

**👤 You:**
> "Create a new text note in 'nb-101' called 'Gift Ideas' with content 'Buy a watch for John'."

**🤖 AI Agent:**
> Success! I've created the notecard 'Gift Ideas' (ID: card-999) inside your 'Personal Ideas' notebook. Is there anything else you'd like to capture?

---

**👤 You:**
> "Search for notes about 'React navigation'."

**🤖 AI Agent:**
> Searching notebooks... I found 2 cards: 1. 'Frontend Best Practices' (in nb-102) and 2. 'Library Wishlist' (in nb-101). Would you like the full content for either of these?


## ❓ FAQ

**Q: Can I search for specific keywords across all my notebooks?**
Yes. The `search_notecards` tool allows your AI agent to perform a global search across your entire Zoho Notebook account, returning all cards that match your query string instantly.

**Q: How do I add a new checklist or note to a specific notebook?**
You can use the `create_notecard` tool. Provide the parent `notebook_id`, a title, and the content. You can also specify the type as 'text' or 'checklist' to match your organizational needs.

**Q: Is it possible to see the full content of a card via chat?**
Absolutely. Use the `get_notecard_details` tool and provide the notebook and card IDs. Your agent will retrieve the full body content and metadata for that specific note.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-notebook](https://vinkius.com/mcp/zoho-notebook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Notebook** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-notebook` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Notebook** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-notebook": {
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
