# Contentstack MCP Server

Equip your AI agent to instantly retrieve digital content and schemas using the Contentstack Delivery API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/contentstack)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Empower your conversational AI with secure and instant read access to your **Contentstack** headless CMS. Utilizing the Contentstack Delivery API, your agent can efficiently fetch published entries, retrieve asset URLs, and audit content type schema structures in real-time.

### What you can do

- **Entry Retrieval** — Instruct the agent to query and read live content entries by searching for specific title tags or matching query filters.
- **Asset Discovery** — Request exact URLs from the media library to find specific images, PDFs, or files needed in your conversational context.
- **Schema Inspections** — Ask for a detailed structural breakdown of any Content Type before utilizing it in an external application.

### How it works

1. Enable the MCP integration linked to your workspace.
2. Secure the connection using a read-only Delivery Token, your Stack API Key, and the targeted Environment Name.
3. Chat seamlessly via natural text to retrieve whatever validated content exists within the targeted publishing environment.

### Who is this for?

- **Developers** — Check live payload structures instantly without leaving your ideation environment to verify frontend rendering code.
- **Content Managers** — Audit what content variants are currently available in the 'production' or 'staging' environments quickly.
- **Marketing Integrators** — Read copy text snippets and locate public URLs of campaign assets efficiently for cross-platform distribution.


## Available Tools
- **get_asset_details**: Get details for a specific asset
- **get_content_type_details**: Get the schema for a specific content type
- **get_entry**: Get detailed content for a specific entry
- **get_stack_summary**: Get high-level metadata about the current stack
- **list_assets**: List all published assets
- **list_content_types**: List all content types in the stack
- **list_entries**: List published entries for a specific content type
- **search_entries**: Search for entries using a JSON query
- **sync_content**: Retrieve delta of changes since last sync


## Installation & Usage

To install and use the **Contentstack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentstack](https://vinkius.com/mcp/contentstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
