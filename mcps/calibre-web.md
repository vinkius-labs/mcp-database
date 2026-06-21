# Calibre-Web MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calibre-web)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Browse and manage your Calibre-Web library via OPDS and Kobo sync — access catalogs, specific shelves, and device metadata directly.

## Description
Connect your **Calibre-Web** instance to any AI agent and interact with your digital book collection using natural language. This server provides tools to navigate your library structure and prepare books for e-reader synchronization.

### What you can do

- **OPDS Catalog Access** — Retrieve the main OPDS XML feed to browse your entire library structure, categories, and recent additions.
- **Shelf Browsing** — Query specific shelf IDs to list books within curated collections or user-defined categories.
- **Kobo Synchronization** — Fetch structured metadata and secure download links optimized for Kobo devices using your dedicated sync token.
- **Library Inspection** — Use the AI to find specific book entries and metadata within your self-hosted instance.

### How it works

1. Subscribe to this server
2. Enter your Calibre-Web instance URL and optional credentials
3. Start exploring your library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Avid Readers** — quickly find books in large collections without manual searching
- **Digital Librarians** — verify shelf contents and catalog structures via chat
- **Kobo Users** — automate the retrieval of sync metadata for your e-reader devices


## Available Tools
- **sync_kobo_library**: Requires Kobo Token.

Sync Kobo library
- **get_opds_catalog**: Useful for browsing the library structure.

Get the main OPDS catalog feed
- **get_opds_shelf**: Get the OPDS feed for a specific shelf


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calibre-Web** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the main OPDS catalog from my library."

**🤖 AI Agent:**
> I've accessed your Calibre-Web OPDS feed. I can see categories for 'Newest', 'Authors', 'Series', and 'Hot'. Which section would you like to explore?

---

**👤 You:**
> "Show me the books available on shelf ID 5."

**🤖 AI Agent:**
> Fetching shelf 5... I found 3 books: 'The Great Gatsby', '1984', and 'Brave New World'. Would you like the metadata for any of these?

---

**👤 You:**
> "Sync my Kobo library and provide the download links."

**🤖 AI Agent:**
> Syncing with Kobo... I've generated the metadata for your library. You have 12 books ready for sync, including direct download links for your device.


## ❓ FAQ

**Q: Can I browse my entire library structure through the AI?**
Yes. By using the `get_opds_catalog` tool, the agent retrieves the root XML feed of your Calibre-Web instance, allowing it to see categories, authors, and series as defined in your OPDS settings.

**Q: How do I list books from a specific custom shelf?**
You can use the `get_opds_shelf` tool by providing the specific `shelf_id`. The AI will then return the list of books and metadata associated with that particular shelf.

**Q: Does this support syncing my Kobo e-reader?**
Yes. If you provide your `CALIBRE_WEB_KOBO_TOKEN`, you can use the `sync_kobo_library` tool to get structured metadata and download links specifically formatted for Kobo device synchronization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calibre-web](https://vinkius.com/mcp/calibre-web)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calibre-Web** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `calibre-web` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calibre-Web** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calibre-web": {
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
