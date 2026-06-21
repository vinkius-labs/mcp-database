# CrafterCMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/craftercms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage and query content from CrafterCMS — fetch pages, components, and trees, execute GraphQL/OpenSearch queries, and manage engine cache directly from your AI agent.

## Description
Connect your **CrafterCMS** instance to any AI agent to streamline your content management and delivery workflows. This server provides deep integration with Crafter Engine, allowing you to inspect content structures, perform advanced searches, and manage site contexts through natural language.

### What you can do

- **Content Retrieval** — Fetch specific items, components, or entire folder hierarchies using `get_item`, `get_component`, and `get_tree`.
- **Navigation & Structure** — Explore site architecture with `get_navigation_tree`, `get_breadcrumb`, and `get_children` to understand content relationships.
- **Advanced Querying** — Execute complex `graphql` queries against your content schema or perform raw `search` operations using OpenSearch JSON syntax.
- **URL Transformation** — Use `transform_url` to apply specific logic to content paths for different delivery environments.
- **Engine Management** — Monitor system health with `get_status` and perform administrative actions like `clear_cache` or `rebuild_context`.

### How it works

1. Subscribe to this server
2. Provide your CrafterCMS Base URL and Site ID
3. Enter your Access and Management tokens
4. Start querying your headless content directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Query content schemas and test GraphQL queries directly from the IDE without switching to the Crafter Studio.
- **Content Managers** — Quickly verify content status, hierarchy, and metadata across different site environments.
- **DevOps & Admins** — Monitor engine status and trigger cache invalidations or context rebuilds via simple commands.


## Available Tools
- **clear_cache**: Requires management token.

Clear the Crafter Engine cache
- **get_breadcrumb**: Get breadcrumb navigation for a URL
- **get_children**: List children of a folder in CrafterCMS
- **get_component**: Render and retrieve a specific component
- **get_item**: Get a single item from CrafterCMS content store
- **get_navigation_tree**: Get navigation tree
- **get_status**: Get Crafter Engine monitoring status
- **get_tree**: Get complete hierarchy under a folder
- **graphql**: Execute a GraphQL query
- **rebuild_context**: Requires management token.

Rebuild the Crafter Engine context
- **search**: Execute an OpenSearch JSON query
- **transform_url**: Transform a URL using a specific transformer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrafterCMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the content for the item at path '/site/website/index.xml'."

**🤖 AI Agent:**
> I've retrieved the item. It's a page titled 'Home' with several components attached. Would you like me to list the components or show the full metadata?

---

**👤 You:**
> "Show me the navigation tree for the root folder with a depth of 2."

**🤖 AI Agent:**
> Generating the navigation tree... I've found the main sections: 'Products', 'Services', and 'About Us', each with their primary sub-pages. Which section should we explore further?

---

**👤 You:**
> "Run a GraphQL query to fetch all articles with their titles and dates."

**🤖 AI Agent:**
> Executing GraphQL query... I've retrieved 10 articles. The latest is 'New Features in v4' dated 2023-10-27. Would you like the content of a specific article?


## ❓ FAQ

**Q: Can I execute complex GraphQL queries against my content?**
Yes! Use the `graphql` tool to send query strings and optional variables. The agent will return the data according to your site's auto-generated schema.

**Q: How do I clear the delivery cache for my site?**
You can use the `clear_cache` action. Note that this requires a valid `CRAFTERCMS_MANAGEMENT_TOKEN` to be configured in your credentials.

**Q: Is it possible to search for content using OpenSearch syntax?**
Absolutely. The `search` tool allows you to pass a raw OpenSearch JSON query object to find exactly what you need within your CrafterCMS index.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/craftercms](https://vinkius.com/mcp/craftercms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CrafterCMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `craftercms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CrafterCMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "craftercms": {
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
