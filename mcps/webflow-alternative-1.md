# Webflow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webflow-alternative-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/webflow-alternative-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/webflow-alternative-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Webflow sites, CMS collections, pages, and assets directly from your AI agent.

## Description
Connect your **Webflow** account to any AI agent to automate your web design and content management workflows. This server provides comprehensive access to the Webflow Data API v2.

### What you can do

- **Site Management** — List all accessible sites, fetch detailed metadata, and trigger site publishing to live domains.
- **CMS Operations** — Full control over Collections and Items. List, create, update, and delete CMS content programmatically.
- **Page & SEO** — Retrieve page lists and update metadata like SEO titles and descriptions without opening the Designer.
- **Asset Handling** — Manage your site's media library by listing, uploading, or deleting assets.
- **Forms & Webhooks** — Access form submissions and manage real-time event triggers via webhooks.

### How it works

1. Subscribe to this server
2. Enter your Webflow API Token (v2)
3. Start managing your sites from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers** — Update CMS items or check site status directly from your terminal or IDE.
- **Content Managers** — Bulk create or update blog posts and products using natural language.
- **SEO Specialists** — Audit and update page metadata across multiple sites efficiently.


## Available Tools
- **list_assets**: ) uploaded to a specific site.

List assets for a site
- **list_collections**: List CMS collections for a site
- **create_items**: Create items in a CMS collection
- **create_webhook**: Create a webhook for a site
- **delete_asset**: Delete an asset from a site
- **delete_items**: Delete items from a CMS collection
- **list_forms**: List forms for a site
- **get_collection**: Get details for a specific CMS collection
- **get_form**: Get schema for a specific form
- **get_page**: Get metadata for a specific page
- **get_site**: Get details for a specific Webflow site
- **list_items**: List items in a CMS collection
- **list_pages**: List pages for a site
- **publish_site**: Limited to 1 successful publish per minute.

Publish a Webflow site
- **list_sites**: List all Webflow sites
- **update_items**: Update items in a CMS collection
- **update_page**: Update metadata for a specific page
- **upload_asset**: Upload an asset to a site
- **list_webhooks**: List webhooks for a site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Webflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Webflow sites and their IDs."

**🤖 AI Agent:**
> I've retrieved your sites. You have access to: 'Portfolio 2024' (ID: site_abc123) and 'Company Blog' (ID: site_xyz789).

---

**👤 You:**
> "Show me the items in the 'Blog Posts' collection with ID 507f1f77bcf86cd799439011."

**🤖 AI Agent:**
> Fetching items... I found 3 items in that collection: 'How to use MCP', 'Webflow Tips', and 'AI Automation Guide'. Would you like the details for any of these?

---

**👤 You:**
> "Publish the site with ID site_abc123."

**🤖 AI Agent:**
> Initiating publish for 'Portfolio 2024' (site_abc123)... The site has been successfully queued for publishing to its configured domains.


## Installation & Usage

To install and use the **Webflow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webflow-alternative-1](https://vinkius.com/mcp/webflow-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
