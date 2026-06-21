# Statamic MCP Server

Manage your Statamic CMS content—list entries, fetch taxonomy terms, inspect global sets, and explore site navigation directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/statamic)

## Overview
**Category:** developer-tools
**Tools Count:** 14

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


## Installation & Usage

To install and use the **Statamic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/statamic](https://vinkius.com/mcp/statamic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
