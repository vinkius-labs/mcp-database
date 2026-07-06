# Joomla (Open-Source CMS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/joomla-open-source-cms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage content via Joomla — list and create articles, manage categories and tags, and audit site menus.

## Description
Connect your **Joomla** site to any AI agent and take full control of your content management and digital publication lifecycle through natural conversation.

### What you can do

- **Article Orchestration** — List, retrieve, and create new content articles directly from your agent, including support for custom titles, aliases, and HTML introtext
- **Categorization & Taxonomy** — Manage global content categories and system tags to ensure your articles are accurately mapped and organized
- **Structural Audit** — Extract detailed information about site menus and menu items to understand your website's navigation hierarchy and layout
- **User Management** — List registered platform users and monitor roles to understand team distribution across your Joomla instance
- **Marketing & Banners** — Enumerate active advertising banners and tracking modules to monitor your site's promotional performance
- **Content Lifecycle** — Update or irreversibly delete specific CMS articles to maintain a fresh and optimized digital storefront

### How it works

1. Subscribe to this server
2. Enter your Joomla Base URL and API Token
3. Start managing your CMS from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Content Editors** — publish and update articles quickly through natural conversation without logging into the Joomla administrator backend
- **Web Developers** — test API results and audit site structures through real-time REST queries directly from your workspace
- **Site Administrators** — monitor user activity, categories, and menu configurations across multiple Joomla projects efficiently


## Available Tools (10)
- **create_cms_article**: Requires title, alias, category ID, and HTML introtext.

Create a new Joomla article
- **delete_cms_article**: Delete a Joomla article
- **get_article_details**: Get details for a specific Joomla article
- **list_platform_users**: List Joomla users
- **list_site_articles**: You can optional pass query parameters like filter[state]=1.

List Joomla articles
- **list_active_banners**: List Joomla banners
- **list_global_categories**: List Joomla categories
- **list_site_menus**: List Joomla site menus
- **list_system_tags**: List Joomla tags
- **patch_cms_article**: Update an existing Joomla article


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Joomla (Open-Source CMS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 articles from my Joomla site"

**🤖 AI Agent:**
> I've retrieved the latest 5 articles. Highlights include 'Getting Started with Joomla 5' (ID: 101), '2024 Tech Trends' (ID: 105), and 'Product Launch Update' (ID: 108). All are currently published. Would you like the full text for any of these?

---

**👤 You:**
> "Create a new article titled 'AI in CMS' in the 'Technology' category (ID: 5)"

**🤖 AI Agent:**
> Article 'AI in CMS' created successfully in the Technology category. Alias: ai-in-cms. I've added the placeholder introtext you provided. You can now use the `patch_cms_article` tool to finalize the full HTML content.

---

**👤 You:**
> "What are the active categories on our site?"

**🤖 AI Agent:**
> I've identified 4 active categories: 'Uncategorised' (ID: 1), 'News' (ID: 2), 'Blog' (ID: 3), and 'Technology' (ID: 5). I can provide the description and parent mapping for any of these if needed.


## ❓ FAQ

**Q: Can I create a new article draft using my agent?**
Yes. Use the `create_cms_article` tool by providing a title, alias, category ID, and the HTML content. Your agent will generate the article in Joomla, allowing you to publish content without opening the admin panel.

**Q: How do I find the correct Category ID for a new article?**
Ask your agent to `list_global_categories`. It will return a list of all available categories on your Joomla site along with their unique numerical IDs, making it easy to map your new content accurately.

**Q: Can my agent check the site's menu structure?**
Absolutely. Use the `list_site_menus` tool to retrieve all configured menus and menu items. This is useful for auditing navigation links and ensuring your site layout is consistent with your content hierarchy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/joomla-open-source-cms](https://vinkius.com/mcp/joomla-open-source-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Joomla (Open-Source CMS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `joomla-open-source-cms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Joomla (Open-Source CMS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "joomla-open-source-cms": {
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
