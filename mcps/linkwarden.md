# Linkwarden MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkwarden)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your bookmarks and web archives with Linkwarden — organize collections, preserve pages, and manage links directly from your AI agent.

## Description
Connect your **Linkwarden** instance to any AI agent and take full control of your personal knowledge base through natural conversation. Linkwarden is a self-hosted collaborative bookmark manager to collect, organize, and preserve webpages.

### What you can do

- **Collection Management** — List all your collections, create new ones, and organize your bookmarks into logical folders.
- **Web Archiving** — Retrieve preserved archive files for your links to ensure you never lose access to important information, even if the original site goes down.
- **Dashboard Insights** — Access your dashboard data (v1 and v2) to get a high-level overview of your saved content and activity.
- **Link Operations** — Create, update, and manage links and their associated metadata or highlights directly from the chat.
- **System Configuration** — Quickly retrieve public runtime configurations and user profile information.

### How it works

1. Subscribe to this server
2. Enter your Linkwarden Instance URL and Personal Access Token
3. Start managing your web archives from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — instantly organize sources and retrieve archived versions of papers or articles without leaving your research flow
- **Developers** — manage technical documentation links and code snippets directly from your IDE
- **Knowledge Workers** — maintain a clean, organized library of web resources using natural language commands


## Available Tools (32)
- **archive_link**: Archive a link (triggers an update of the link's archive files)
- **bulk_update_links**: Bulk update links (tags/collections)
- **create_collection**: Create a new collection
- **create_highlight**: Create or update a highlight
- **create_link**: Create a new link
- **delete_collection**: Delete a collection
- **delete_highlight**: Delete a highlight
- **auth_forgot_password**: Send password reset email
- **get_archive**: Retrieve an archive file by link ID
- **get_avatar**: Retrieve user avatar
- **get_collection**: Get collection by ID
- **get_config**: Retrieve public runtime configuration
- **get_dashboard_v1**: Get dashboard data (v1)
- **get_dashboard_v2**: Get dashboard data (v2)
- **get_link_highlights**: Get highlights for a link
- **get_link**: Get a link by ID
- **get_logins**: Get login configuration
- **get_migration**: Retrieve migration data (user info, collections, links for export)
- **get_preserved_token**: Create short-lived preserved format URL token
- **get_public_collection_links**: Retrieve links from a specific collection (public)
- **get_public_collection_tags**: Get tags for a collection (public)
- **import_migration**: Import data for migration
- **list_collections**: Get all collections
- **list_rss**: List RSS subscriptions
- **auth_reset_password**: Reset password with token
- **stream_preserved_view**: Stream archived format
- **update_collection**: Update a collection
- **update_dashboard_v2**: Update dashboard layout (v2)
- **update_link**: Update a link
- **upload_archive_for_link**: Upload or replace a client-side archive file for a specific link
- **upload_standalone_archive**: Upload an archive file, create a new link, and store it in the default collection
- **auth_verify_email**: Verify email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linkwarden** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Linkwarden collections."

**🤖 AI Agent:**
> I've retrieved your collections. You have 3 collections: 'Research' (ID: 1), 'Recipes' (ID: 2), and 'Tech News' (ID: 3).

---

**👤 You:**
> "Create a new collection called 'Project Alpha' with ID 'alpha-01'."

**🤖 AI Agent:**
> Successfully created the collection 'Project Alpha' with ID 'alpha-01'. You can now start adding links to it.

---

**👤 You:**
> "Show me my dashboard summary."

**🤖 AI Agent:**
> Fetching your dashboard data... You currently have 150 links across 5 collections, with 120 successfully archived.


## ❓ FAQ

**Q: How can I see a list of all my bookmark folders?**
You can use the `list_collections` tool. It will retrieve all your existing collections, allowing the AI to show you how your bookmarks are organized.

**Q: Is it possible to retrieve an archived version of a saved link?**
Yes! Use the `get_archive` tool with the specific Link ID. This will fetch the preserved archive file associated with that link.

**Q: Can I create a new collection directly through the AI?**
Absolutely. Use the `create_collection` tool by providing a unique ID and the collection details in the payload.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkwarden](https://vinkius.com/mcp/linkwarden)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Linkwarden** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkwarden` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Linkwarden** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkwarden": {
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
