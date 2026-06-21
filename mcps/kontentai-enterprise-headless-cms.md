# Kontent.ai (Enterprise Headless CMS) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kontentai-enterprise-headless-cms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kontentai-enterprise-headless-cms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kontentai-enterprise-headless-cms-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage enterprise content via Kontent.ai — create items, publish language variants, and audit content types.

## Description
Connect your **Kontent.ai** project to any AI agent and take full control of your enterprise-grade headless CMS and content orchestration through natural conversation.

### What you can do

- **Item Orchestration** — List and retrieve content item containers, and create or update top-level item shells defining types and codenames directly from your agent
- **Variant Management** — Update actual content fields (`elements`) for specific languages (e.g., English, Portuguese), moving variants into Draft status securely
- **Publishing Workflow** — Transition specific language variants from Draft to Published status to make content immediately live via Delivery APIs
- **Schema Introspection** — Discover and inspect Content Type definitions to understand available fields, scalar parameters, and required element blocks
- **Taxonomy & Tags** — Manage hierarchical taxonomy groups used to classify and filter your content assets for better organizational structure
- **Media Audit** — List uploaded media assets and document files to retrieve precise identifiers and cloud URLs for frontend delivery

### How it works

1. Subscribe to this server
2. Enter your Kontent.ai Environment ID and Management API Key
3. Start managing your content lifecycle from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Content Editors** — update and publish content variants quickly through natural conversation without logging into the Kontent.ai UI
- **Content Architects** — audit taxonomy trees and verify content type schemas across multiple environments and projects efficiently
- **Frontend Developers** — introspect content types and verify asset identifiers to ensure accurate mapping in your downstream applications


## Available Tools
- **get_item**: Retrieve metadata for a specific Kontent.ai item by codename
- **get_taxonomy**: Get details and nested terms for a specific Taxonomy group
- **get_content_type**: Retrieve the exact structural fields of a specific Content Type
- **list_assets**: List uploaded Media Assets and Document files
- **list_items**: ai project space.

List all content items in the Kontent.ai environment
- **list_taxonomies**: List all hierarchical Taxonomies (tags/categories)
- **list_content_types**: List all Content Type schemas registered in the environment
- **publish_variant**: Publish a specific language variant of an item to Delivery APIs
- **upsert_item**: Note: this does not update the language variant fields (the actual content text)—use upsert_language_variant for that.

Create or update a top-level content item container
- **upsert_language_variant**: g. `default`). This places the variant into Draft status.

Update the actual content fields of an item for a specific language


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kontent.ai (Enterprise Headless CMS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all content items in our project"

**🤖 AI Agent:**
> I've retrieved your content items. Highlights include 'Homepage' (codename: homepage), 'About Us' (about_us), and 'Q4 Roadmap' (q4_roadmap). Would you like to check the language variants for any of these?

---

**👤 You:**
> "Publish the 'default' variant for item 'q4_roadmap'"

**🤖 AI Agent:**
> Publishing variant… Done. The 'default' language version of 'q4_roadmap' has been transitioned to the Published stage. It is now live and available via your delivery endpoints.

---

**👤 You:**
> "What are the structural fields for the 'Article' content type?"

**🤖 AI Agent:**
> The 'Article' content type (codename: article) contains 5 fields: 'title' (Text), 'slug' (URL slug), 'body' (Rich text), 'author' (Content relation), and 'hero_image' (Asset). I can help you create a new item implementing this schema.


## Installation & Usage

To install and use the **Kontent.ai (Enterprise Headless CMS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kontentai-enterprise-headless-cms](https://vinkius.com/mcp/kontentai-enterprise-headless-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
