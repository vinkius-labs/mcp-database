# Notion V3 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/notion-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Notion V3 — Page styling (icon/cover), bulk database listing & page creation with children blocks.

## Description
Notion **V3 — Page Design Edition**. Unlike V1 (17 tools, full workspace CRUD + archive/delete) and V2 (13 tools, comments & bot identity), V3 is optimized for **page styling and bulk operations**.

### V3 Exclusive

- **Page Styling** — Update icon, cover and trash state via single `update_page` call (only V3 supports `icon`/`cover`/`in_trash`)
- **Bulk Database Listing** — `list_databases` returns all databases the integration can see without a search query (V1/V2 require search)
- **Creation with Content** — `create_page` accepts `parent` (page_id or database_id) + `properties` + `children` blocks in one atomic call
- **Advanced Search** — `search` with `query` + `filter` + `sorts` for precise discovery

### Shared (intentionally overlapping for compatibility)

- Retrieve page/database, query database, block children, users — same API as V1/V2 but with V3's styling focus

Use V1 for exhaustive workspace ops, V2 for collaboration/comments, V3 when you need page design and bulk listing.


## Available Tools (12)
- **list_users**: List workspace users
- **get_me**: Get bot user for this token
- **search**: Search pages/databases by title with optional filter/sorts
- **update_page**: Update page: properties, icon, cover, trash. V3 exclusive icon/cover
- **append_block_children**: Append blocks to page. V3 supports bulk via JSON array
- **list_databases**: List all databases (bulk, no search query needed). V3 exclusive
- **retrieve_database**: Get database schema (columns, types)
- **retrieve_page**: Get page metadata by ID
- **retrieve_user**: Get user by ID
- **create_page**: Create page with optional children blocks. Parent can be database or page
- **query_database**: Query database with filter/sorts
- **retrieve_block_children**: List child blocks of a page/block


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Notion V3** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Notion workspace for 'Q3 Roadmap'."

**🤖 AI Agent:**
> I found 2 pages mentioning 'Q3 Roadmap'. The primary document is at notion.so/q3-roadmap-xyz.

---

**👤 You:**
> "List all items in database 'DATABASE_ID' marked as 'In Progress'."

**🤖 AI Agent:**
> There are 4 tasks 'In Progress', including 'Redesign Header' and 'Optimize API calls'.

---

**👤 You:**
> "Create a new note titled 'Meeting Notes' under page 'PAGE_ID'."

**🤖 AI Agent:**
> Page 'Meeting Notes' created successfully.


## ❓ FAQ

**Q: Can the AI query specific rows in a Notion database?**
Yes! Supply the Database ID and you can filter rows by properties, check tags, and read text fields.

**Q: Does it support creating new pages?**
Absolutely. The agent can construct a new page as a child of an existing page or database.

**Q: How do I share my Notion pages with the integration?**
You must explicitly share specific databases or root pages with your 'Internal Integration' user via the Notion UI share menu.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/notion-alternative](https://vinkius.com/ai-agent-connect/notion-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Notion V3** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `notion-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Notion V3** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "notion-alternative": {
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
