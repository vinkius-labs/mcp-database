# Notion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/notion-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Notion pages, databases and blocks via API — search content, query databases, create rows and append blocks from any AI agent.

## Description
Connect your **Notion** workspace to any AI agent and take full control of your pages, databases and content through natural conversation.

### What you can do

- **Global Search** — Search all pages and databases the integration has access to by title
- **Database Operations** — Get database schemas, query rows with filters and sorts, and create new entries
- **Page Management** — Retrieve page metadata, update properties and read page content
- **Block Operations** — Read block children (paragraphs, headings, lists, code, images) and append new blocks
- **User Discovery** — List workspace users, get user details and verify the bot identity
- **Comments** — Read comment threads on pages and add new comments

### How it works

1. Subscribe to this server
2. Enter your Notion Internal Integration Token
3. Start managing your workspace from Claude, Cursor, or any MCP-compatible client

No more navigating through the Notion app to find a database or update page properties. Your AI acts as a dedicated knowledge ops assistant.

### Who is this for?

- **Knowledge Managers** — quickly search pages, query databases and review content without opening the Notion app
- **Developers** — create database rows programmatically, append blocks and update page properties from chat
- **Team Leads** — audit workspace users, review comments and track page changes via conversation


## Available Tools
- **append_block**: Requires the parent block/page ID and a JSON array of block objects. Each block must follow Notion's block schema: {"object":"block","type":"paragraph","paragraph":{"rich_text":[{"type":"text","text":{"content":"Hello"}}]}}. Common types: paragraph, heading_1, heading_2, heading_3, bulleted_list_item, numbered_list_item, to_do, toggle, code.

Append blocks to a Notion page
- **create_comment**: Requires the page ID and rich text content. Rich text follows Notion's format: [{"type":"text","text":{"content":"This looks great!"}}]. The comment will appear in the page's comment thread.

Add a comment to a Notion page
- **create_database_row**: Requires the database ID and a properties JSON object matching the database schema. Use get_database to see the property types and keys. Properties must follow Notion's format: {"Name":{"title":[{"text":{"content":"My Page"}}]},"Status":{"select":{"name":"Done"}}}.

Create a new row (page) in a Notion database
- **get_database**: ), parent page and creation date. Provide the database ID (32-character hex or UUID format).

Get details for a specific Notion database
- **get_me**: Returns the bot name, ID and type. Use this to verify your integration token is working correctly and to see which bot identity the API calls will appear as.

Get the authenticated Notion bot user
- **get_page**: Does NOT return block content — use get_page_blocks for that. Provide the page ID.

Get details for a specific Notion page
- **get_page_blocks**: Each block has a type (paragraph, heading_1, heading_2, heading_3, bulleted_list_item, numbered_list_item, to_do, toggle, code, image, etc.) and content. Use this to read the actual text and media content of a page. Provide the page or block ID.

Get blocks (content) of a Notion page
- **get_user**: Provide the user ID from list_users.

Get details for a specific Notion user
- **list_comments**: Each comment includes the rich text content, author, creation date and parent reference. Useful for reviewing discussion threads and feedback on pages.

List comments on a Notion page or block
- **list_database_rows**: Returns pages matching the database schema with their property values. Optionally provide a filter object to narrow results (e.g. {"property":"Status","select":{"equals":"Done"}}) and sorts to order results. Use get_database first to understand the property schema.

Query rows in a Notion database
- **list_users**: Each user has an ID, name, avatar URL, email (if available) and type (person or bot). Useful for identifying who has access and who created content.

List users in your Notion workspace
- **search**: Optionally filter by text query (matches page titles and database names). Returns pages and databases with their properties, titles and parent info. Use this to discover content before querying or editing specific pages.

Search pages and databases in Notion
- **update_page**: Requires the page ID and a properties JSON object with the fields to change. Only provided properties will be updated. Follow Notion's property format: {"Status":{"select":{"name":"Done"}},"Priority":{"select":{"name":"High"}}}.

Update properties of a Notion page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Notion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all pages related to 'Q4 planning'."

**🤖 AI Agent:**
> I found 3 pages matching 'Q4 planning': 'Q4 OKRs' (database), 'Q4 Budget Review' (page, last edited 2 days ago) and 'Q4 Team Retrospective' (page, last edited last week). Would you like to see the content of any of these?

---

**👤 You:**
> "Query my Task Tracker database and show me all items with status 'In Progress'."

**🤖 AI Agent:**
> I found 12 tasks with status 'In Progress' in your Task Tracker database. The highest priority items are 'Implement OAuth flow' (due tomorrow), 'Fix checkout bug' (due today) and 'Update API documentation' (no due date). Want me to show all 12?

---

**👤 You:**
> "Add a new task to my Task Tracker called 'Review PR #234' with status 'To Do'."

**🤖 AI Agent:**
> Done! I've created a new page 'Review PR #234' in your Task Tracker database with status set to 'To Do'. The page URL is notion.so/your-workspace/... You can add more properties or blocks to it anytime.


## ❓ FAQ

**Q: How do I create a Notion Internal Integration Token?**
Go to [**Notion Integrations**](https://www.notion.so/my-integrations), click **+ New integration**, give it a name, select the workspace and click **Submit**. Copy the **Internal Integration Secret** (starts with `ntn_`). Then, open any page or database in Notion, click **...** > **Add connections** and select your integration to grant access.

**Q: Why can't the integration see my pages?**
Notion integrations only have access to pages and databases you explicitly share with them. Open any page, click **...** (top-right) > **Add connections**, and select your integration. The integration will then have access to that page and all its children. Use the `search` tool to discover accessible content.

**Q: Can I create new pages in a database?**
Yes! Use `create_database_row` with the database ID and a properties JSON object. First use `get_database` to see the property schema (column names and types). Properties follow Notion's format: {"Name":{"title":[{"text":{"content":"My Page"}}]},"Status":{"select":{"name":"Done"}}}.

**Q: Can I read and append page content?**
Yes! Use `get_page_blocks` with a page ID to read all block children (paragraphs, headings, lists, etc.). Use `append_block` to add new blocks — provide the page ID and a JSON array of block objects following Notion's block schema.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/notion-alternative](https://vinkius.com/mcp/notion-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Notion** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `notion-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Notion** tools.

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
