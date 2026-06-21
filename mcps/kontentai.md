# Kontent.ai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kontentai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kontentai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kontentai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access headless content — list items, audit types, and query taxonomies.

## Description
Connect your AI agent to **Kontent.ai Delivery API** to fetch and analyze your modular content.

### Key Features

- **Content Item Retrieval** — Fetch the full modular content of any item by its codename
- **Schema Auditing** — List and examine content types to understand your project's data model
- **Taxonomy Access** — Query taxonomy groups and terms for content categorization
- **Asset Discovery** — Locate images and files stored in your content library
- **Smart Search** — Perform filtered searches across your entire delivery repository

### Simple Setup

1. Subscribe to this server
2. Get your **Project ID** from Kontent.ai (Project Settings > API keys)
3. (Optional) Enter your **Delivery API Key** if Secure Access is enabled
4. Start querying your content via natural language


## Available Tools
- **list_content_items**: Use this to find codenames for specific articles, products, or pages.

List all content items from Kontent.ai
- **get_content_item**: Get a specific content item by codename
- **list_content_types**: List all content types (schemas)
- **get_content_type**: Get details for a content type
- **list_taxonomies**: List taxonomy groups
- **get_taxonomy_group**: Get details for a taxonomy group
- **list_project_languages**: List supported languages
- **list_content_assets**: ai.

Query assets from the content library
- **search_kontent_ai**: Search for content using query parameters
- **get_content_type_element**: g., options for a multiple choice element).

Get metadata for a specific element in a type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kontent.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 10 content items in Kontent.ai"

**🤖 AI Agent:**
> I've retrieved the latest content items. Highlights include 'Homepage' (type: Page), 'Our Mission' (type: Article), and 'Product Catalog' (type: Catalog). Which one should I inspect for you?

---

**👤 You:**
> "Show the schema for content type 'article'"

**🤖 AI Agent:**
> The 'Article' content type consists of: Title (text), Body (rich text), Author (taxonomy), and Publication Date (date). I can fetch specific articles of this type if you'd like.

---

**👤 You:**
> "Search for items related to 'Winter Sale'"

**🤖 AI Agent:**
> Searching Delivery API… I found 2 items: 'Winter Sale Banner' and 'Promotion Rules'. I can retrieve the full content for either.


## Installation & Usage

To install and use the **Kontent.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kontentai](https://vinkius.com/mcp/kontentai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
