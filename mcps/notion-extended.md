# Notion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/notion-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Notion workspace, databases, and pages via AI.

## Description
Connect your Notion workspace to your AI agent. Search across databases, fetch page contents, update block properties, and create new knowledge entries directly from your chat without opening the Notion app.


## Available Tools
- **append_block_children**: Append child blocks to an existing block or page
- **create_page**: You must provide the parent object and properties (schema based on parent type).

Create a new page in Notion
- **get_me**: Get information about the current integration/bot
- **list_databases**: List all databases available to the integration
- **list_users**: List all users in the workspace
- **query_database**: Query a specific Notion database with filters and sorts
- **retrieve_block_children**: Retrieve child blocks of a specific block or page
- **retrieve_database**: Retrieve metadata for a specific database
- **retrieve_page**: Retrieve a specific Notion page by ID
- **retrieve_user**: Retrieve a specific user by ID
- **search**: Search for pages and databases by title
- **update_page**: Update properties of an existing Notion page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Notion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/notion-extended](https://vinkius.com/mcp/notion-extended)
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
3. Set Type to "SSE", enter `notion-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Notion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "notion-extended": {
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
