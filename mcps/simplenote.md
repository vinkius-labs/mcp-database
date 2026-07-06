# Simplenote MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simplenote)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Simplenote notes directly from your AI assistant. Create, search, edit, and organize plain-text notes without leaving the conversation.

## Description
Connect your AI assistant to your Simplenote account for seamless note management. The **Simplenote MCP** enables your LLM to act as a personal note-taking assistant with full read and write access to your notes.

### What you can do

- **Browse & Search** — List all your notes with `list_notes` or find specific content using `search_notes`. Explore note history with `get_note_version` to review previous edits
- **Create & Edit** — Capture ideas instantly with `create_note` or update existing notes using `update_note`, all through natural conversation
- **Organize & Clean Up** — View your tag taxonomy with `list_tags` or permanently remove notes with `delete_note`

### How it works

1. Add this server to your MCP-compatible AI client
2. Configure your `SIMPLENOTE_APP_ID` and `SIMPLENOTE_TOKEN` in the credential settings
3. Start managing notes conversationally: "List my recent notes and search for anything mentioning 'project roadmap'"


## Available Tools (8)
- **search_notes**: Searches for notes containing specific text
- **update_note**: Requires the note key.

Updates an existing note
- **create_note**: Provide the full text content.

Creates a new note
- **delete_note**: This action is irreversible.

Permanently deletes a note
- **get_note_details**: Retrieves details for a specific note
- **get_note_version**: Requires note key and version number.

Retrieves a specific historical version of a note
- **list_notes**: Returns note keys and a preview of the content.

Lists all notes in Simplenote
- **list_tags**: Lists all tags used in your notes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Simplenote** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new note with my meeting minutes from today."

**🤖 AI Agent:**
> Done! I created a new note titled 'Meeting Minutes — April 4, 2026' with the key `abc123def`. You can ask me to update it anytime.

---

**👤 You:**
> "Search my notes for anything about 'tax_2023'."

**🤖 AI Agent:**
> I found 1 note containing 'tax_2023'. It was last modified on March 15. Would you like me to show the full content?

---

**👤 You:**
> "Delete the note with key f1b2c3d4."

**🤖 AI Agent:**
> The note f1b2c3d4 has been permanently deleted. This action cannot be undone.


## ❓ FAQ

**Q: Can the integration accidentally delete important notes?**
The `delete_note` tool performs a permanent deletion. We recommend instructing your AI agent to always confirm before executing any deletion. You can also use `get_note_version` to review note history before making changes.

**Q: Does it support shared or team notes?**
Simplenote is designed for personal note management. This integration accesses notes tied to the authenticated user's account only. Team collaboration features are not available through the Simperium API.

**Q: Does it support Markdown formatting?**
Yes. Simplenote stores plain text, so Markdown syntax is preserved as-is when you create or update notes. The Simplenote clients will render Markdown formatting natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplenote](https://vinkius.com/mcp/simplenote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Simplenote** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `simplenote` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Simplenote** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simplenote": {
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
