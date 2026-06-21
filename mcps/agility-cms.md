# Agility CMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agility-cms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage and query your Agility CMS content through AI — navigate sitemaps, search lists, and fetch layouts.

## Description
Connect your **Agility CMS** instance to your AI agent and turn it into the ultimate Headless CMS assistant. Skip manual API queries and interact directly with your content architecture using natural language.

### What you can do

- **Sitemap & Routing** — Retrieve nested sitemap trees or flat router architectures to understand how your channels are structured
- **Content Lists** — Search, list, and count items across specific CMS references like articles, authors, or products
- **Page Layouts** — Fetch exact page modules, UI components mapping, and structural layout definitions using Page IDs
- **Content Operations** — Read full content payloads for individual items and synchronize granular CMS updates over time
- **Media Galleries** — Fetch specific media asset groups and tracking galleries for imagery

### How it works

1. Subscribe to this server
2. Provide your Agility GUID, target Locale, and API Key
3. Let your agent seamlessly query documents, pages, and components via Claude or Cursor

### Who is this for?

- **Frontend Developers** — get an instant breakdown of page modules and sitemaps while building frontends
- **Content Managers** — audit content lists, search for specific entries, and check page structures directly
- **SEO Specialists** — analyze the flat site router graph natively to map out content opportunities


## Available Tools
- **get_page_layout**: Retrieve the layout and structural modules of a single Page
- **get_site_flat_router**: Retrieve the exact flat list of all CMS routes/pages
- **count_reference_items**: Get the total size/count of items in a specific Reference List
- **get_media_gallery**: Retrieve a specific media gallery mapping containing photos
- **get_single_item**: g., an article body) knowing its numeric content ID.

Retrieve a single Agility CMS content item by its ID
- **get_site_tree**: Requires the target channel name.

Retrieve the nested sitemap architecture of a digital channel
- **list_content_items**: g. blog posts, articles, authors). The items are retrieved from the Headless CMS environment.

List content items from an Agility CMS Reference list
- **search_content_reference**: Search for specific keywords inside a Content Reference List
- **sync_incremental_items**: Start with 0 for full backup.

Get incrementally updated items since the last sync token
- **sync_incremental_pages**: Start with 0 for a full fetch.

Get incrementally updated pages since the last sync token


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agility CMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the flat sitemap for our website to see all registered routes."

**🤖 AI Agent:**
> I've fetched the flat router map. You currently run 42 routes on your primary 'website' channel. The latest pages registered are '/about/team' (Page ID 108) and '/products/new-launch' (Page ID 109).

---

**👤 You:**
> "Search the 'blog_posts' reference list for the keyword 'announcement'."

**🤖 AI Agent:**
> I found 3 matching items in 'blog_posts' containing 'announcement'. The most recent one is 'Q3 Product Announcement' (Item ID 4512). Would you like me to fetch the full content payload for this article?

---

**👤 You:**
> "Retrieve the full page layout and modules for page ID 12."

**🤖 AI Agent:**
> Here is the layout breakdown for Page ID 12 (Home Page). It uses the 'StandardTemplate'. There are 4 UI modules mapped in the 'MainContentZone': Hero Banner, Features Grid, Testimonials, and Call to Action.


## ❓ FAQ

**Q: Can my agent keep track of incremental updates to my CMS items?**
Yes. The agent has tools specifically designed to fetch incremental updates using a sync token. It can request only the CMS items or pages that have changed (created, updated, or deleted) since the last automated sync, optimizing fetch latency.

**Q: How do I find the correct Reference Name to query content?**
Reference Names match the identifiers predefined in your Agility CMS Models architecture (such as 'articles', 'authors', or 'posts'). If you are unsure, ask the agent to scan common variables based on your company's naming conventions.

**Q: Can my agent preview unpublished drafting content?**
That depends on the API Token you supply during the integration. If you provide a Preview API Key, the agent will have read-access to the staging and drafted documents. If you provide a Fetch API key, it will only see published items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agility-cms](https://vinkius.com/mcp/agility-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agility CMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `agility-cms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agility CMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agility-cms": {
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
