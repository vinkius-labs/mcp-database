# Kontent.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kontentai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage content items, types, and taxonomies via Kontent.ai's Delivery and Management APIs directly from your AI agent.

## Description
Connect your **Kontent.ai** project to any AI agent to streamline your headless CMS workflows. This server provides comprehensive access to both Delivery and Management APIs, allowing for seamless content retrieval and manipulation.

### What you can do

- **Content Delivery** — List and fetch content items, types, and taxonomies using the high-performance Delivery API.
- **Content Management** — Create, update, and delete content items, and manage language variants through the Management API.
- **Schema Exploration** — Inspect content type definitions and taxonomy groups to understand your project structure.
- **Advanced Filtering** — Query items by type, collection, or depth to retrieve exactly the data your agent needs.

### How it works

1. Subscribe to this server
2. Enter your Kontent.ai Project ID and API keys (Delivery and Management)
3. Start managing your headless content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — Quickly update content variants or check taxonomy tags without leaving the chat interface.
- **Developers** — Fetch content schemas and item payloads directly into your IDE for faster integration.
- **Digital Marketers** — Audit content items across different collections and languages using natural language queries.


## Available Tools
- **delivery_get_item**: Get a single content item via Delivery API
- **delivery_list_items**: ai project. Supports filtering and depth.

List content items via Delivery API
- **delivery_list_taxonomies**: List taxonomies via Delivery API
- **delivery_list_types**: List content types via Delivery API
- **manage_list_assets**: List assets via Management API
- **manage_create_asset**: Create an asset via Management API
- **manage_create_item**: Create a content item via Management API
- **manage_create_taxonomy**: Create a taxonomy via Management API
- **manage_create_type**: Create a content type via Management API
- **manage_delete_asset**: Delete an asset via Management API
- **manage_delete_item**: Delete a content item via Management API
- **manage_delete_taxonomy**: Delete a taxonomy via Management API
- **manage_delete_type**: Delete a content type via Management API
- **manage_get_variant**: Get a language variant of a content item
- **manage_list_items**: List content items via Management API
- **manage_list_taxonomies**: List taxonomies via Management API
- **manage_list_types**: List content types via Management API
- **manage_update_asset**: Update an asset via Management API
- **manage_update_item**: Update a content item via Management API
- **manage_update_taxonomy**: Update a taxonomy via Management API
- **manage_update_type**: Update a content type via Management API
- **manage_update_variant**: Update a language variant of a content item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kontent.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all content items of type 'blog_post' from my Kontent.ai project."

**🤖 AI Agent:**
> I've retrieved the blog posts. I found 3 items: 'Welcome to our Blog', 'Tech Trends 2024', and 'Headless CMS Guide'. Would you like to see the details for any of these?

---

**👤 You:**
> "Get the content item with codename 'about_us_page'."

**🤖 AI Agent:**
> Fetching 'about_us_page'... I've found the item. It's a 'page' type item in the 'Main' collection. The title is 'About Our Company' and it was last updated on October 12th.

---

**👤 You:**
> "List all taxonomy groups in my project."

**🤖 AI Agent:**
> I've fetched the taxonomies. Your project contains 2 groups: 'Persona' (targeting different audience segments) and 'Product Category' (organizing your inventory).


## ❓ FAQ

**Q: Can I filter content items by their content type?**
Yes. Use the `delivery_list_items` tool and provide the `system_type` parameter with the codename of the content type you want to filter by.

**Q: Is it possible to create new content items using this server?**
Absolutely. The `manage_create_item` tool allows you to create new content items by providing a JSON payload according to the Kontent.ai Management API schema.

**Q: How do I retrieve a specific language variant of a content item?**
You can use the `manage_get_variant` tool, providing both the `item_id` and the `language_id` to fetch the specific version of the content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kontentai-alternative](https://vinkius.com/mcp/kontentai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kontent.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `kontentai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kontent.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kontentai-alternative": {
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
