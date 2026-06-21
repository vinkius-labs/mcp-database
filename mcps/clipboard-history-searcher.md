# Clipboard History Searcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clipboard-history-searcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search through your exported clipboard history (Ditto, CopyQ, Maccy) with AI. Find that URL, phone number, or code snippet you copied days ago.

## Description
You copied something important 3 days ago — a phone number, a URL, a code snippet — and now you need it. If you use a clipboard manager like Ditto, CopyQ, or Maccy, you can export your history. This MCP makes it instantly searchable by your AI.

### The Superpowers

- **Universal Format Support:** Reads JSON exports (CopyQ, Maccy) and plain text (Ditto).
- **Zero Dependencies:** Pure native parsing.
- **Token-Safe:** Shows up to 200 clips to prevent context overflow.


## Available Tools
- **search_clipboard_history**: Supports both JSON and plain text formats.

Parse an exported clipboard history file (JSON or TXT from Ditto, CopyQ, Maccy) and make it searchable by your AI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clipboard History Searcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the URL I copied yesterday that had 'github' in it."

**🤖 AI Agent:**
> Found it: 'https://github.com/vinkius/awesome-project' — copied at entry #142.

---

**👤 You:**
> "Search my clipboard for any phone numbers."

**🤖 AI Agent:**
> Found 3 entries with phone numbers: +1 555-0199, +351 912 345 678, (11) 99999-0000.

---

**👤 You:**
> "Show me all code snippets in my clipboard history."

**🤖 AI Agent:**
> Found 8 entries that appear to be code: Python (3), JavaScript (4), SQL (1).


## ❓ FAQ

**Q: Which clipboard managers are supported?**
Any manager that exports as JSON or plain text: Ditto (Windows), CopyQ (cross-platform), Maccy (macOS), Clipy (macOS).

**Q: Does it capture images from clipboard?**
No, this parser focuses on textual clipboard entries to save AI context tokens.

**Q: Is my clipboard data sent to the cloud?**
No. Parsed locally. Only text entries are sent to AI context during your session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clipboard-history-searcher](https://vinkius.com/mcp/clipboard-history-searcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clipboard History Searcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clipboard-history-searcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clipboard History Searcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clipboard-history-searcher": {
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
