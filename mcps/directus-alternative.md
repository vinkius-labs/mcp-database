# Directus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/directus-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Turn any SQL database into a powerful headless CMS with instant REST and GraphQL APIs for your custom content models.

## Description
Connect your **Directus** instance to any AI agent and manage your content database through natural conversation.

### What you can do

- **Collection Management** — List all data collections with field counts and inspect individual collection schemas
- **Content CRUD** — Create, read, update, and delete items in any collection using JSON payloads
- **Search & Query** — Search items within collections by keyword to find specific content quickly
- **Schema Inspection** — List all fields and their data types for any collection to understand your data model
- **File Management** — Browse uploaded files and retrieve metadata for specific assets
- **User & Role Management** — List all users with roles and status, view role configurations, and check your own profile
- **Audit Trail** — Access the activity log of recent database operations for compliance and debugging

### How it works

1. Subscribe to this server
2. Enter your Directus Static Token from your user profile in the Data Studio
3. Start managing your content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Teams** — create, update, and search content items across collections without opening the Directus dashboard
- **Developers** — inspect collection schemas, manage fields, and debug data issues through conversational AI
- **Administrators** — audit user activity, manage roles, and monitor database operations


## Available Tools (16)
- **check_directus_status**: Verify connectivity
- **create_item**: Create an item
- **delete_item**: Delete an item
- **get_collection**: Get collection details
- **get_file**: Get file details
- **get_item**: Get item details
- **get_me**: Get current user
- **list_activity**: List recent activity
- **list_collections**: List collections
- **list_fields**: List fields
- **list_files**: List files
- **list_items**: List items
- **list_roles**: List roles
- **list_users**: List users
- **search_items**: Search items
- **update_item**: Update an item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Directus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all collections in my Directus instance and the fields for the 'articles' collection."

**🤖 AI Agent:**
> Your Directus instance has 8 collections: 'articles' (24 fields), 'categories' (6 fields), 'authors' (12 fields), 'media' (8 fields), 'pages' (15 fields), 'settings' (10 fields), 'comments' (9 fields), and 'tags' (4 fields). Fields for 'articles': id (uuid), title (string), slug (string), body (text), status (string: draft/published/archived), featured_image (file), author (m2o → authors), category (m2o → categories), tags (m2m → tags), date_published (datetime), sort (integer). Would you like to list items or create a new article?

---

**👤 You:**
> "Create a new article titled 'AI in Healthcare 2025' with status 'draft' and search for existing articles about AI."

**🤖 AI Agent:**
> Article created! ID: a3f8c291, Title: 'AI in Healthcare 2025', Status: draft, Slug: ai-in-healthcare-2025. Searching existing articles for 'AI'... Found 3 matches: 1) 'AI-Driven Drug Discovery' (published, 2024-11-15). 2) 'Machine Learning in Diagnostics' (published, 2024-09-22). 3) 'AI Ethics Framework' (draft, 2025-01-08). Would you like to update the new article's body or assign it to an author?

---

**👤 You:**
> "Show me the recent activity log and list all users with their roles."

**🤖 AI Agent:**
> Recent activity (last 24h): 14 operations. Top actions: 8 item updates (articles, pages), 3 item creates (articles, media), 2 logins, 1 role change. Most active user: 'editor@example.com' (9 operations). Users: 1) Admin User (admin role, active). 2) Sarah Editor (editor role, active). 3) Mike Writer (writer role, active). 4) API Bot (api-readonly role, active). 3 roles configured: admin (full access), editor (content CRUD), writer (create/read only). Would you like to inspect a specific user or see more activity?


## ❓ FAQ

**Q: Can I create, update, and delete content items in any collection?**
Yes! Use `create_item` with a collection name and JSON payload to add new items. Use `update_item` with the collection, item ID, and updated fields to modify existing items. Use `delete_item` to remove items. All operations respect the permissions assigned to your Static Token's user role.

**Q: How does Directus authentication work with a Static Token?**
Directus uses a non-expiring Static Token associated with a specific user account. Generate it from your **User Profile** in the Data Studio. The token is sent as a `Bearer` token in the Authorization header. Its permissions match the role assigned to that user — use an admin role for full access or a restricted role for read-only operations.

**Q: Can I audit what changes have been made to my database?**
Yes. The `list_activity` tool retrieves the audit log of recent database operations, showing who made changes, which collections were affected, timestamps, and the type of operation (create, update, delete). Combine with `list_users` and `list_roles` for full accountability tracking.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/directus-alternative](https://vinkius.com/mcp/directus-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Directus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `directus-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Directus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "directus-alternative": {
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
