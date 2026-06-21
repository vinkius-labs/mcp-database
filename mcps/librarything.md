# LibraryThing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/librarything)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Look up books by ISBN, explore works, and check library coverage — a bibliographic intelligence tool for AI agents.

## Description
Connect **LibraryThing** to your AI agent for instant book lookups, bibliographic data, and library coverage analysis.

### What you can do

- **ISBN Lookup** — Retrieve book details by ISBN including title, author, publication info, and ratings
- **Work Discovery** — Explore works and their editions, translations, and related metadata
- **Book Coverage** — Check which libraries hold a specific title for interlibrary research

### How it works

1. Subscribe to this server
2. Register for a [LibraryThing Developer Key](https://www.librarything.com/services/keys.php)
3. Start querying books from Claude, Cursor, or any MCP client


## Available Tools
- **get_book_coverage**: The coverage score (0-1) indicates how completely the book is cataloged on LibraryThing. Free, no API key required.

Get catalog coverage score for a book
- **get_work**: Returns title, author, coverage score (how well the work is cataloged), member count, review count and more. Free, no API key required. Use what_work to find the work ID first.

Get detailed info for a LibraryThing work
- **thing_isbn**: Useful for finding paperback, hardcover, audio, and international editions of a book. Free, no API key required.

Find all ISBNs for different editions of the same book
- **what_work**: The work ID is needed for other LibraryThing API calls. Free, no API key required.

Find the LibraryThing work ID for a book


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LibraryThing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Look up the book with ISBN 978-0-13-468599-1."

**🤖 AI Agent:**
> Found it! 'The Pragmatic Programmer' by David Thomas and Andrew Hunt. Publisher: Addison-Wesley (2019, 2nd edition). Community rating: 4.2/5 with 1,847 members. Tagged: programming, software-engineering, best-practices.


## ❓ FAQ

**Q: What information can I get from an ISBN lookup?**
An ISBN lookup returns the book title, author(s), publisher, publication date, page count, language, community ratings, and tags — all from the LibraryThing database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/librarything](https://vinkius.com/mcp/librarything)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LibraryThing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `librarything` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LibraryThing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "librarything": {
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
