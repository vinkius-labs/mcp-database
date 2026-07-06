# Plone MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plone)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage Plone CMS content, users, and workflows directly from your AI agent—search, create, and update resources effortlessly.

## Description
Connect your **Plone** CMS instance to any AI agent to manage your enterprise content through natural conversation.

### What you can do

- **Content Management** — Search, retrieve, create, update, and delete content objects using paths and metadata.
- **User & Group Administration** — List and manage users and groups, including profile updates and creation.
- **Workflow Transitions** — Inspect current workflow states and trigger transitions to move content through its lifecycle.
- **Advanced Search** — Use full-text search, type filtering, and path-based queries to find exactly what you need.

### How it works

1. Subscribe to this server
2. Enter your Plone Instance URL and Personal Access Token
3. Start managing your CMS from Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex CMS hierarchies. Your AI acts as a content editor and site administrator.

### Who is this for?

- **Content Managers** — quickly update pages, create news items, and manage publication workflows without the web UI
- **Site Administrators** — manage users and groups or perform bulk content searches via natural language
- **Developers** — inspect content structures and metadata directly from the code editor


## Available Tools (17)
- **update_user**: Update a user
- **delete_user**: Delete a user
- **create_content**: Create new content in Plone
- **create_group**: Create a new group
- **create_user**: Create a new user
- **delete_content**: Delete content from Plone
- **delete_group**: Delete a group
- **get_content**: Get a specific content object by path
- **get_group**: Get details for a specific group
- **get_user**: Get details for a specific user
- **get_workflow**: Get workflow status and history for content
- **list_groups**: List groups in Plone
- **list_users**: Requires Manager role.

List users in Plone
- **search_content**: Search for content in Plone
- **transition_workflow**: Trigger a workflow transition on content
- **update_content**: Supports partial updates.

Update existing content in Plone
- **update_group**: Update a group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plone** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all Documents containing 'roadmap' in the /news folder."

**🤖 AI Agent:**
> I've searched the /news path. I found 2 documents: 'Product Roadmap 2024' and 'Q3 Engineering Roadmap'. Would you like to see the details of either one?

---

**👤 You:**
> "Create a new Folder titled 'Marketing 2025' at the root path."

**🤖 AI Agent:**
> Successfully created the folder 'Marketing 2025' at path /marketing-2025. You can now start adding content to it.

---

**👤 You:**
> "Get the content of the page at /about-us and show its current workflow state."

**🤖 AI Agent:**
> I've retrieved the page. The title is 'About Our Company' and its current workflow state is 'private'. Would you like to transition it to 'published'?


## ❓ FAQ

**Q: Can I search for specific content types like Folders or Documents?**
Yes! Use the `search_content` tool and provide the `portal_type` parameter (e.g., 'Folder' or 'Document') to filter your results.

**Q: How do I update the title or description of an existing page?**
Use the `update_content` tool. Provide the `path` to the content and a `json_body` containing the fields you want to change, such as `{"title": "New Title"}`.

**Q: Is it possible to manage user accounts through this server?**
Yes, if your credentials have sufficient permissions, you can use `list_users`, `get_user`, and `create_user` to manage the site's membership.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plone](https://vinkius.com/mcp/plone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plone** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plone` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plone** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plone": {
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
