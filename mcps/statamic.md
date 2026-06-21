# Statamic MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/statamic)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/statamic-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/statamic-mcp)
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


## Installation & Usage

To install and use the **Statamic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/statamic](https://vinkius.com/mcp/statamic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
