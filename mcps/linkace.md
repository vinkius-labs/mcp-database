# LinkAce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkace)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your bookmarks, tags, and collections via the LinkAce REST API.

## Description
Connect your **LinkAce** instance to any AI agent to automate your personal knowledge base and link archiving. This MCP server enables your agent to add new bookmarks, organize them into lists and tags, and search your entire library directly from natural language interfaces.

### What you can do

- **Instant Archiving** — Quickly add new URLs to your LinkAce library with custom titles and descriptions
- **Deep Organization** — Create and manage tags and lists to keep your bookmarks categorized and easy to find
- **Semantic Discovery** — Search through your entire archived library using keywords via natural language commands
- **Library Maintenance** — Retrieve detailed metadata for specific links or permanently remove outdated bookmarks
- **Self-Hosted Support** — Works with any self-hosted LinkAce instance using your personal API token

### How it works

1. Subscribe to this server
2. Enter your LinkAce API Key (Bearer Token) and your Instance URL
3. Start managing your links from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — Automatically archive and tag useful resources while you work or browse
- **Developers** — Build a personal technical library and search for specific snippets or documentation links
- **Power Users** — Automate the curation of your personal bookmark manager directly from your productivity tools


## Available Tools
- **create_new_bookmark**: Requires at least a URL.

Add a new link to your archive
- **create_new_collection**: Add a new collection (list)
- **create_new_tag**: Add a new tag
- **delete_bookmark**: Remove a bookmark from your archive
- **get_bookmark_details**: Get details for a specific bookmark
- **list_all_bookmarks**: List all bookmarks (links) in your LinkAce account
- **list_all_collections**: List all bookmark collections (lists)
- **search_bookmarks**: Search for bookmarks by keyword
- **list_all_tags**: List all tags used for organizing bookmarks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkAce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add 'https://www.wikipedia.org' to my LinkAce bookmarks."

**🤖 AI Agent:**
> I've added Wikipedia to your LinkAce archive. The new bookmark ID is 'link-123' and it is currently marked as private.

---

**👤 You:**
> "Search my LinkAce library for 'Artificial Intelligence'."

**🤖 AI Agent:**
> I found 5 bookmarks matching 'Artificial Intelligence', including links to research papers and industry news. Would you like to see the full details for any of them?

---

**👤 You:**
> "List all my bookmark collections."

**🤖 AI Agent:**
> I've retrieved your collections. You have 3 active lists: 'Reading List', 'Technical Docs', and 'Work Projects'.


## ❓ FAQ

**Q: How do I find my LinkAce API Token?**
Log in to your LinkAce dashboard, navigate to User Settings, and generate a new API token from the API section.

**Q: What is the Instance URL?**
This is the full base URL where your LinkAce instance is hosted, for example: `https://links.yourdomain.com`.

**Q: Can I search for specific tags?**
While you can search for links by keyword, you can also list all tags to find the specific label IDs used for organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkace](https://vinkius.com/mcp/linkace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkAce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `linkace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkAce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkace": {
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
