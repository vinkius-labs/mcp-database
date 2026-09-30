# Note Archive Structure Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/note-archive-structure-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize user notes into structured directories using metadata, tags, and project status.

## Description
This MCP server provides a logic engine to categorize user notes into a structured directory system. It uses note metadata, user-defined tags, and project lifecycles to map notes to a provided folder taxonomy. Use `get_folder_assignments` to map notes to folders, `identify_unclassified_notes` to find notes that don't fit the structure, `find_archive_candidates` to identify stale notes, and `validate_taxonomy_structure` to ensure your folder hierarchy is valid.


## Available Tools (4)
- **find_archive_candidates**: Identifies notes that are no longer relevant for active work
- **get_folder_assignments**: Maps a collection of notes to the provided folder taxonomy
- **identify_unclassified_notes**: Isolates notes that do not fit into the existing folder structure
- **validate_taxonomy_structure**: Ensures the user-supplied folder hierarchy is logical and non-conflicting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Note Archive Structure Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you assign these notes to my folder structure?"

**🤖 AI Agent:**
> I have mapped the notes. Note ID 123 is assigned to /projects/active, and Note ID 456 is unclassified.

---

**👤 You:**
> "Which notes should I archive?"

**🤖 AI Agent:**
> The following notes are candidates for archiving: Note ID 789 and Note ID 101.

---

**👤 You:**
> "Is my folder taxonomy valid?"

**🤖 AI Agent:**
> Yes, the folder hierarchy is valid and contains no conflicting paths.


## ❓ FAQ

**Q: How does the tool decide where a note goes?**
The assignment logic prioritizes tag matches to taxonomy names first, followed by project status alignment, and finally date-based placement.

**Q: What is an archive candidate?**
A note is an archive candidate if it is not part of an Active project and its creation or last edit date exceeds the specified staleness threshold.

**Q: Can I validate my folder structure?**
Yes, you can use `validate_taxonomy_structure` to ensure your folder hierarchy is a valid directed tree structure without conflicts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/note-archive-structure-plan](https://vinkius.com/en/ai-agent-connect/note-archive-structure-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Note Archive Structure Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `note-archive-structure-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Note Archive Structure Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "note-archive-structure-plan": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
