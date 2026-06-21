# Wallabag (Pocket Alternative) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wallabag-pocket-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your self-hosted read-it-later list — save URLs, organize with tags, and retrieve article content directly from your AI agent.

## Description
Connect your **Wallabag** instance to any AI agent and transform your read-it-later list into an interactive knowledge base. Wallabag is the leading open-source alternative to Pocket and Instapaper, allowing you to host your own articles.

### What you can do

- **Article Management** — List all saved entries, fetch full content for specific articles, and save new URLs instantly.
- **Organization** — Mark articles as read (archive) or favorite (star), and manage tags to keep your library structured.
- **Annotations & Highlights** — Retrieve existing annotations or create new highlights and notes directly on your saved articles.
- **Tagging System** — List all your existing tags and apply them to entries to categorize your research.
- **Clean Reading** — Access the extracted text of articles without ads or distractions, perfect for AI analysis.

### How it works

1. Subscribe to this server
2. Enter your Wallabag instance URL and API credentials (Client ID, Secret, Username, and Password)
3. Start managing your reading list from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — save sources and annotate them using AI to summarize key findings.
- **Knowledge Workers** — organize a massive backlog of articles and find exactly what you need via natural language.
- **Privacy Enthusiasts** — keep your reading data on your own server while still benefiting from AI-powered insights.


## Available Tools (11)
- **add_tags_to_entry**: Add tags to a specific entry
- **create_annotation**: Create an annotation on an entry
- **create_entry**: Save a new URL to Wallabag
- **delete_entry**: Delete an entry from Wallabag
- **get_entry**: Get a single entry by ID
- **list_annotations**: Get annotations for an entry
- **list_entries**: Get all entries (articles) from Wallabag
- **list_tags**: Get all tags from Wallabag
- **mark_entry_favorite**: Mark an entry as favorite (starred)
- **mark_entry_read**: Mark an entry as read (archive)
- **remove_tag_from_entry**: Remove a tag from an entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wallabag (Pocket Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my most recent articles from Wallabag."

**🤖 AI Agent:**
> I've retrieved your latest entries. You have articles like 'The Future of AI' (ID: 452) and 'Open Source Guide' (ID: 453). Would you like me to fetch the content for any of these?

---

**👤 You:**
> "Save this URL to my Wallabag: https://example.com/article"

**🤖 AI Agent:**
> Successfully saved! The article has been added to your Wallabag account with Entry ID 454. Would you like me to add any tags to it?

---

**👤 You:**
> "Mark article 452 as read and add the tag 'finished'."

**🤖 AI Agent:**
> Done. Article 452 has been archived and tagged as 'finished'.


## ❓ FAQ

**Q: Can I save a new article just by providing a URL?**
Yes! Use the `create_entry` tool with the URL you want to save. Your agent will add it to your Wallabag account immediately.

**Q: How do I archive an article once I've finished reading it?**
Simply ask the agent to mark the article as read using the `mark_entry_read` tool with the specific Entry ID.

**Q: Can I see the highlights and notes I've made on an article?**
Yes. The `list_annotations` tool retrieves all highlights and notes associated with a specific Entry ID, allowing the AI to reference your personal insights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wallabag-pocket-alternative](https://vinkius.com/mcp/wallabag-pocket-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wallabag (Pocket Alternative)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wallabag-pocket-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wallabag (Pocket Alternative)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wallabag-pocket-alternative": {
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
