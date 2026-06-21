# Statamic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/statamic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Statamic CMS content—list entries, fetch taxonomy terms, inspect global sets, and explore site navigation directly from your AI agent.

## Description
Connect your **Statamic** site to any AI agent and take full control of your flat-file or database-driven content through natural conversation.

### What you can do

- **Entries & Collections** — List entries from any collection with support for pagination, sorting, and field filtering.
- **Navigation & Structure** — Retrieve hierarchical tree structures for your site menus and structured collections to understand site architecture.
- **Taxonomy Management** — Query taxonomies and specific terms to organize content or check categorization.
- **Global Sets** — Fetch site-wide variables, settings, and configuration data stored in Statamic Globals.
- **Forms & Users** — List available forms and user profiles to manage site interactions and administrative data.

### How it works

1. Subscribe to this server
2. Ensure the Statamic REST API is enabled in your site's configuration
3. Enter your Statamic Base URL and API Token
4. Start querying your CMS content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — quickly find entries, check publication status, or verify global site settings without logging into the CP.
- **Developers** — inspect API responses and content structures directly from your IDE while building frontends.
- **SEO Specialists** — audit collection entries and taxonomy terms to ensure consistent metadata and categorization.


## Available Tools
- **get_asset**: Get a single asset
- **get_collection_tree**: Get entry tree for structured collections
- **get_entry**: Get a single Statamic entry
- **get_form**: Get a single form
- **get_global**: Get variables for a global set
- **get_nav_tree**: Get navigation structure tree
- **get_term**: Get a single taxonomy term
- **get_user**: Get a single user
- **list_assets**: List assets in a container
- **list_entries**: List entries in a Statamic collection
- **list_forms**: List all forms
- **list_globals**: List all global sets
- **list_terms**: List terms in a Statamic taxonomy
- **list_users**: List users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Statamic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent 5 entries from the 'blog' collection."

**🤖 AI Agent:**
> I've retrieved the latest 5 blog entries. The most recent is 'New Features in v5' followed by 'Getting Started with MCP'. Would you like the full content of any of these?

---

**👤 You:**
> "Show me the navigation structure for the 'footer' menu."

**🤖 AI Agent:**
> The 'footer' navigation tree contains 3 main items: 'Privacy Policy', 'Terms of Service', and 'Contact Us'. Each points to its respective entry ID.

---

**👤 You:**
> "Get the details for the term 'tutorials' in the 'categories' taxonomy."

**🤖 AI Agent:**
> The term 'tutorials' (slug: tutorials) in the 'categories' taxonomy has been found. It is currently associated with 12 entries in your collections.


## ❓ FAQ

**Q: Can I see the hierarchical structure of my site navigation?**
Yes. Use the `get_nav_tree` tool with the handle of your navigation (e.g., 'main'). The agent will return the full nested structure of your menu items.

**Q: How do I fetch specific variables like the site name or social media links?**
You can use `list_globals` to see all available sets, then use `get_global` with the specific handle to retrieve all variables stored within that global set.

**Q: Is it possible to filter entries when listing a collection?**
The `list_entries` tool supports `limit`, `sort`, and `fields` parameters, allowing you to paginate results and choose exactly which data fields the agent should process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/statamic](https://vinkius.com/mcp/statamic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Statamic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `statamic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Statamic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "statamic": {
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
