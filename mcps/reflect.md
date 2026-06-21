# Reflect MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reflect)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI to read, write, and explore your networked thought graph in Reflect Notes securely via their API.

## Description
Connect your **Reflect** account securely to your AI agent via their developer API. This integration grants your AI the ability to directly explore your networked thought graph, lookup personal notes, manage book highlights, and append daily thoughts asynchronously from your conversation interface.

### What you can do

- **Explore Your Graph** — Direct your AI to investigate connected insights within your Reflect graphs (`list_graphs`). Request lists of your notes (`list_notes`) or retrieve the specific Markdown content of a single note (`get_note`).
- **Capture Ideas Instantly** — Ask the agent to establish new permanent notes (`create_note`) or quickly dump conversational insights, summaries, and tasks straight into your daily note (`append_daily_note`).
- **Analyze Connections** — Instruct the AI to map out your thoughts by retrieving all backlinks pointing to a specific subject (`get_backlinks`).
- **Save Links & Books** — Let your AI automatically bookmark URLs (`create_link`), browse your saved bookmarks (`list_links`), or explore your imported library of book highlights (`list_books`).

### How it works

1. Authorize the Reflect MCP plugin in your active extensions.
2. Obtain your personal OAuth Access Token from your Reflect application settings (reflect.app/developer/oauth) and embed it securely into the integration.
3. Chat naturally with your AI, prompting tasks like "Append a summary of this conversation to my daily note" or "List all notes connected to 'AI Strategy'."

### Who is this for?

- **Researchers & Writers** — Interactively synthesize information. Have your AI recall connected ideas from your graph while you brainstorm, without switching apps.
- **Founders & Execs** — Seamlessly capture action items. Simply ask your assistant to log decisions and links directly into today's daily note.
- **Knowledge Workers** — Transform your AI into a personalized knowledge broker that understands your private context and highlights instantly.


## Available Tools
- **append_daily_note**: Optionally specify a list/heading name.

Appends Markdown text to today's daily note
- **create_link**: Reflect will automatically attempt to extract metadata.

Saves a new web link/bookmark to a Reflect graph
- **create_note**: Specify subject and Markdown content.

Creates a new note in a Reflect graph
- **get_backlinks**: Retrieves all notes that link to a specific note
- **get_current_user**: Retrieves profile details for the authenticated Reflect user
- **get_note**: Retrieves the full content and metadata of a Reflect note
- **list_books**: Lists all books saved or imported into Reflect
- **list_graphs**: Lists all Reflect graphs (workspaces) accessible by the user
- **list_links**: Lists all saved links (bookmarks) in a graph
- **list_notes**: Lists all notes within a specific Reflect graph


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reflect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available graphs in my Reflect account."

**🤖 AI Agent:**
> Using `list_graphs`, I found 2 distinct workspaces: "Personal Brain" (ID: 6f...2c) and "Project Insights" (ID: 9a...11).

---

**👤 You:**
> "Create a permanent note titled 'Meeting 2024 Strategy' inside my 'Personal Brain' graph with summary bullet points."

**🤖 AI Agent:**
> Executing `create_note` on Graph ID '6f...2c'. I have successfully created 'Meeting 2024 Strategy' and piped the Markdown list of bullets into it.

---

**👤 You:**
> "Find notes linked by backlinks that point to my note 'React Learnings'."

**🤖 AI Agent:**
> I called `list_notes` to verify 'React Learnings', acquiring its note_id 'xx82', then ran `get_backlinks`. You have 3 other notes connecting to it: 'Frontend Architecture', 'Day 2 Journal', and 'Tech Stack Overview'.


## ❓ FAQ

**Q: Can the agent create new graphs from scratch?**
No. The AI via the MCP can fully manage notes, generate fresh links, and organize entries, but you must create top-level workspaces (Graphs) directly within the native Reflect desktop or web applications first.

**Q: Will `append_daily_note` overwrite my existing notes for today?**
No, `append_daily_note` strictly adds the provided Markdown blocks to the very bottom of today's Daily Note section in Reflect. It is a completely safe, non-destructive operation preserving your older notes intact.

**Q: Can I search notes by standard keywords instead of IDs?**
The underlying Reflect API largely focuses on ID-based lookups (`note_id`). You can request the AI to first `list_notes` which provides titles for semantic checking, and then it can dynamically chain the ID lookup to read your specific content immediately after.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reflect](https://vinkius.com/mcp/reflect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reflect** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `reflect` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reflect** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reflect": {
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
