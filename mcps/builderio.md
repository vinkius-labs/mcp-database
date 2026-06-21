# Builder.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/builderio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your visual CMS via Builder.io — track content entries, models, and symbols directly from any AI agent.

## Description
Connect your **Builder.io** account to any AI agent and orchestrate your visual CMS, content management, and digital experience workflows through natural conversation.

### What you can do

- **Content Oversight** — List and retrieve detailed metadata for all your content entries across different models (Pages, Blog Posts, etc.).
- **Model Management** — List all content models in your space and retrieve detailed schema metadata.
- **Visual Automation** — Create and update content entries programmatically using the Write API directly from your workspace.
- **Infrastructure Coordination** — Access and monitor your spaces, organization settings, and reusable symbols.
- **Performance Tracking** — Retrieve real-time API usage statistics to monitor your CMS performance.
- **Entry Deep Dives** — Get detailed data for specific content or model IDs straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Builder.io Public and Private API Keys
3. Start managing your digital experiences from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers & Engineers** — quickly check content structures or update entries without manual dashboard work.
- **Content Managers & Editors** — retrieve published content and monitor model schemas straight from their workflow tools.
- **Digital Teams** — orchestrate cross-space content and monitor usage using natural language.


## Available Tools
- **create_content_entry**: Create a new content entry
- **get_content_entry**: Get a specific content entry
- **get_model**: Get details of a specific content model
- **get_space**: Get details of a specific space
- **get_api_usage**: Retrieve API usage statistics
- **list_content**: List content entries for a specific model
- **list_models**: List all content models in the space
- **list_spaces**: List all spaces in your organization
- **list_symbols**: List all reusable symbols
- **update_content_entry**: Update an existing content entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Builder.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all content entries for the 'page' model."

**🤖 AI Agent:**
> I've retrieved your pages. You have 5 entries, including 'Home' (ID: page_1), 'About Us' (ID: page_2), and 'Contact' (ID: page_3).

---

**👤 You:**
> "Show the schema details for the 'blog-post' model."

**🤖 AI Agent:**
> Retrieving model details... The 'blog-post' model includes fields like 'title' (Text), 'content' (Rich Text), 'author' (Reference), and 'publishDate' (Date).

---

**👤 You:**
> "Create a new entry in 'announcement-bar' with name 'Promo Banner'."

**🤖 AI Agent:**
> Entry 'Promo Banner' has been successfully created in the 'announcement-bar' model with ID entry_99283.


## ❓ FAQ

**Q: Can I update a content entry using the agent?**
Yes! Use the `update_content_entry` tool with the Model name and Entry ID. You can provide a new `data` JSON string to modify the content fields directly from your workspace.

**Q: How do I list all the models defined in my space?**
Simply ask the agent to `list_models`. It will retrieve all the content models (like 'page', 'header', 'announcement-bar') configured in your Builder.io account.

**Q: Does the integration allow checking API usage limits?**
Yes. Use the `get_api_usage` tool. It will retrieve real-time statistics about your API requests, helping you monitor your performance and limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/builderio](https://vinkius.com/mcp/builderio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Builder.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `builderio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Builder.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "builderio": {
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
