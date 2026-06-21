# Cockpit (Self-hosted Headless CMS API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cockpit-self-hosted-headless-cms-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your self-hosted Cockpit CMS content, assets, and menus directly from any AI agent.

## Description
Connect your **Cockpit CMS** instance to any AI agent and take full control of your headless content infrastructure through natural conversation.

### What you can do

- **Content Management** — List, fetch, create, update, and delete items from any content collection using Mongo-style filters.
- **Asset Handling** — Retrieve file metadata and generate processed thumbnails or resized images on the fly.
- **Navigation & Menus** — Access and manage menus and page structures via the Pages addon integration.
- **Batch Operations** — Fetch data from multiple content models in a single request for high-performance workflows.
- **Localization** — Support for multi-language content retrieval and localized project management.

### How it works

1. Subscribe to this server
2. Enter your Cockpit Instance URL and API Key
3. Start managing your CMS content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — Update blog posts, products, or FAQs without logging into the CMS dashboard.
- **Developers** — Query content structures and asset metadata directly from your IDE while coding.
- **Marketing Teams** — Quickly retrieve localized content and assets for multi-channel campaigns.


## Available Tools
- **batch_content_items**: Batch request content from multiple models
- **create_or_update_content_item**: If an _id is provided in the data, it updates the existing item.

Create or update a content item
- **delete_content_item**: Delete a content item by ID
- **get_asset_image**: Generate thumbnails or resized images
- **get_asset**: Get asset metadata by ID
- **get_content_item**: Fetch a single content item by ID
- **get_lokalize_project_locale**: Get translations for a specific locale in a Lokalize project
- **get_lokalize_project**: Get all translations for a Lokalize project
- **get_menu**: Get a specific menu by name
- **get_page_by_route**: Fetch a page by its route
- **get_sitemap**: Get the complete sitemap
- **list_content_items**: Supports filtering, sorting, and pagination.

Fetch a list of items from a Cockpit content collection
- **list_menus**: List all menus
- **list_pages**: List all pages
- **list_routes**: Get a lightweight list of all routes and slugs
- **search_detektivo**: Search within a specific Detektivo index
- **submit_inbox**: Submit form data to an Inbox


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cockpit (Self-hosted Headless CMS API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest 5 articles from the 'blog' collection."

**🤖 AI Agent:**
> I've retrieved the 5 most recent articles from your 'blog' collection. They include 'New Product Launch', 'Summer Trends', and three others. Would you like to see the full content of any specific post?

---

**👤 You:**
> "Get the metadata for asset ID 12345."

**🤖 AI Agent:**
> Inspecting asset 12345... It's a JPEG image named 'hero-banner.jpg', size 1.2MB, with dimensions 1920x1080. It was uploaded on June 12th. Do you need a resized version of this image?

---

**👤 You:**
> "Update the content item in 'products' with ID 98765 to change the price to 49.99."

**🤖 AI Agent:**
> I've updated the product (ID: 98765). The price field has been successfully set to 49.99. All other fields remain unchanged. Is there anything else you'd like to modify?


## ❓ FAQ

**Q: Can I filter content items using Mongo-style queries?**
Yes! The `list_content_items` tool supports a `filter` parameter where you can pass a JSON object with Mongo-style query operators to precisely target your data.

**Q: Is it possible to resize images directly through the agent?**
Absolutely. Use the `get_asset_image` tool with parameters like `w` (width), `h` (height), and `m` (mode) to request processed versions of your stored image assets.

**Q: Can I fetch data from multiple collections at once?**
Yes, the `batch_content_items` tool allows you to define multiple models and their respective query parameters in a single JSON object to retrieve all required data in one go.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cockpit-self-hosted-headless-cms-api](https://vinkius.com/mcp/cockpit-self-hosted-headless-cms-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cockpit (Self-hosted Headless CMS API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cockpit-self-hosted-headless-cms-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cockpit (Self-hosted Headless CMS API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cockpit-self-hosted-headless-cms-api": {
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
