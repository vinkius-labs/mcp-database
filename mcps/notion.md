# Notion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/notion)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Unified AI interface for your Notion workspace — search pages, query databases, and manage blocks via AI.

## Description
Unlock the full potential of your connected workspace by linking **Notion** to your AI agent. This integration transforms Notion from a static documentation hub into a dynamic, queryable engine for your AI workflows. Your agent can now perform global fuzzy searches to locate misplaced documents, query structured databases to extract tabular data, and even read deep into nested block hierarchies to summarize project specs or meeting notes. Whether you're automating task creation or retrieving team knowledge, your agent acts as an intelligent librarian for your entire Notion domain.

### What you can do

- **Global Search** — Rapidly find pages and databases across your workspace by title or content using fuzzy text matching.
- **Database Orchestration** — Query databases to read structured data rows or fetch the exact schema defining your trackers.
- **Deep Content Reading** — Access metadata and dive into nested paragraphs, lists, and images using advanced block retrieval.
- **Record Creation** — Programmatically create new pages or insert data rows directly inside specific Notion containers.
- **Identity Mapping** — Enumerate all workspace users and bots to accurately map assignee tags to team members.

### How it works

1. Subscribe to this server
2. Enter your Notion Internal Integration Secret
3. Start querying your company wiki and project trackers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Productivity Experts** — quickly search the internal wiki, read deep project specs, and append notes to central databases.
- **Software Teams** — query central sprint trackers and create new tasks without ever leaving your development environment.
- **Ops Managers** — build automated AI reporting flows by safely reading the real-time state of active rows and users.
- **Knowledge Workers** — retrieve specific documentation fragments instantly through natural language conversation.


## Available Tools
- **create_database**: Properties define columns. Minimum: provide a title property with type "title".

Create a new Notion database inside a page
- **append_block_children**: ) to the end of a page or nested block. Provide blocks as a JSON array of Notion block objects. Example for a paragraph: [{"type":"paragraph","paragraph":{"rich_text":[{"type":"text","text":{"content":"Hello world"}}]}}]

Append content blocks to a Notion page or block
- **archive_page**: Archive/Delete a Notion Page
- **get_blocks**: Read hierarchical textual content under a Page
- **create_page**: Insert a new row/page inside a Database
- **delete_block**: ) from a page. This action is irreversible — the block and all nested children are permanently deleted.

Permanently delete a Notion block
- **get_database**: ) defining rows within a Database.

Retrieve the schema definition of a Database
- **get_page**: Does NOT fetch body text.

Retrieve metadata properties for a single Notion Page
- **list_users**: Enumerate workspace members and bots
- **query_database**: Read structured data rows from a Notion Database
- **search_databases**: Essential for tracking down Database UUIDs.

Fuzzy text search globally across Notion workspace Databases
- **search_pages**: Necessary to locate Page UUIDs rapidly.

Fuzzy text search globally across Notion workspace pages
- **update_page_properties**: ) using the Notion properties schema. Provide the properties as a JSON object matching the Notion API property format.

Update arbitrary properties on a Notion page
- **update_page_title**: Update the title of a Notion Page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Notion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Notion workspace for any pages containing 'Q4 Marketing Strategy'."

**🤖 AI Agent:**
> I searched your Notion workspace and found the page 'Q4 Marketing Strategy (Final)' with ID `abc-123`. Let me know if you would like me to read the contents of its blocks.

---

**👤 You:**
> "Create a new row in my Project Tasks database marking the title as 'Update API Docs'."

**🤖 AI Agent:**
> I've successfully created a new active row 'Update API Docs' within the Project Tasks database. The new record has been initialized and is ready for further updates.

---

**👤 You:**
> "List all team members currently registered in my Notion."

**🤖 AI Agent:**
> Here are the users active within your Notion domain: Jane Doe (`jane@domain.com`), John Smith (`john@domain.com`), and 3 active Bot integrations.


## ❓ FAQ

**Q: Can my AI automatically create task assignments?**
Yes. Your agent can pull the exact schema of your tracker database, retrieve the user UUIDs via `list_users`, and seamlessly insert a new row assigning the task—all within seconds.

**Q: How do I extract long notes from a page?**
While `get_page` gives you raw page metadata, your agent will use `get_blocks` to traverse paragraphs, lists, and images to stream the entire document context back into your chat workflow.

**Q: Does it support deep searches?**
Absolutely. It leverages multiple endpoints like `search_pages` and `search_databases` globally so your agent can track down any missing document UUID using just a textual query snippet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/notion](https://vinkius.com/mcp/notion)
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
3. Set Type to "SSE", enter `notion` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Notion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "notion": {
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
