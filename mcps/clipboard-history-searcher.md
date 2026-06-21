# Clipboard History Searcher MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clipboard-history-searcher)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clipboard-history-searcher-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clipboard-history-searcher-mcp)
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


## Installation & Usage

To install and use the **Clipboard History Searcher** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clipboard-history-searcher](https://vinkius.com/mcp/clipboard-history-searcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
