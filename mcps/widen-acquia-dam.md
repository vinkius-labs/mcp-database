# Widen (Acquia DAM) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/widen-acquia-dam)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/widen-acquia-dam-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/widen-acquia-dam-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search and manage digital assets, metadata, and CDN embed links on Widen (Acquia DAM) — the leading enterprise DAM solution.

## Description
Connect your **Widen (Acquia DAM)** account to any AI agent and take control of your enterprise digital assets through natural conversation.

### What you can do

- **Asset Search** — Find files instantly using Widen's internal search syntax (e.g., search by filename, category, or metadata)
- **Metadata Management** — Retrieve comprehensive technical properties and update metadata fields directly from your agent
- **Folder Navigation** — Browse top-level categories and explore contents within specific category nodes to understand your DAM hierarchy
- **Collection Access** — List user-defined asset collections and retrieve all files grouped within a specific collection ID
- **CDN Integration** — Retrieve active CDN embed links and HTML snippets for any asset to facilitate high-availability content delivery
- **User Auditing** — List authorized users and their account roles to monitor team access across the DAM instance
- **Data Integrity** — Safely delete obsolete media assets to manage storage and keep your content library clean

### How it works

1. Subscribe to this server
2. Enter your Widen Access Token
3. Start managing your digital assets through Claude, Cursor, or any MCP-compatible client

No more manual browsing through massive asset libraries. Your AI agent becomes your digital asset librarian.

### Who is this for?

- **Marketing Teams** — quickly find approved brand assets and retrieve CDN embed links for web distribution
- **Content Creators** — update asset metadata and manage file collections through simple chat commands
- **DAM Administrators** — audit user lists and monitor category structures to ensure asset organization
- **Creative Operations** — find specific media files by technical metadata and manage asset lifecycles efficiently


## Available Tools
- **delete_media_asset**: This action is irreversible and removes the asset from all collections.

Permanently removes an asset from the Acquia DAM
- **get_asset_details**: Retrieves comprehensive metadata and technical properties for a specific asset
- **get_category_contents**: Retrieves the assets and sub-nodes within a specific category
- **list_collection_assets**: Lists all assets contained within a specific user collection
- **list_global_categories**: Lists all top-level categories (folders) in the DAM hierarchy
- **list_saved_collections**: Lists all user-defined asset collections
- **list_cdn_embed_links**: Retrieves all active CDN embed links and HTML snippets for a specific asset
- **list_account_users**: Lists all authorized users in the Acquia DAM instance
- **search_widen_assets**: Provide a search query string.

Search for assets in Acquia DAM (Widen) using the internal search syntax
- **update_asset_metadata**: Provide the asset ID and a JSON object mapping field keys to values.

Updates the metadata fields of an existing asset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Widen (Acquia DAM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for assets with 'marketing' in the category and 'banner' in the filename."

**🤖 AI Agent:**
> I found 3 assets matching your query: 1. 'summer_banner_v1.jpg' (ID: wid-101), 2. 'winter_sale_banner.png' (ID: wid-102), and 3. 'logo_banner_final.ai' (ID: wid-103). Would you like to see the details or embed links for any of these?

---

**👤 You:**
> "Get the CDN embed links for asset ID 'wid-101'."

**🤖 AI Agent:**
> Here are the active CDN links for asset wid-101: 1. Public Image URL: https://embed.widen.net/img/..., 2. Responsive Snippet: <img src='...' />, 3. Original File: https://embed.widen.net/file/... Would you like the HTML code for a specific size?

---

**👤 You:**
> "List all global categories in our Widen DAM."

**🤖 AI Agent:**
> I found 5 top-level categories: 'Brand Guidelines', 'Product Photos', 'Marketing Campaigns', 'Internal Documentation', and 'Legacy Archive'. Which category would you like to explore?


## Installation & Usage

To install and use the **Widen (Acquia DAM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/widen-acquia-dam](https://vinkius.com/mcp/widen-acquia-dam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
