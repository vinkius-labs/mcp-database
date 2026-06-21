# Contentstack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contentstack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/contentstack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/contentstack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to instantly retrieve digital content and schemas using the Contentstack Delivery API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contentstack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the published blog post entry with the title 'Future Trends in AI' from our primary environment."

**🤖 AI Agent:**
> I've successfully queried your Contentstack instance. The entry 'Future Trends in AI' was found in your defined environment. It contains a rich-text body, a featured asset identifier, and an author reference currently set to 'Jane Smith'. The main text emphasizes large language model advancements mapped over the next 5 years.

---

**👤 You:**
> "Describe the content model schema required for 'Hero Banner' items in my stack."

**🤖 AI Agent:**
> The 'Hero Banner' model in your target stack requires three main fields: 1) A 'heading' (Short text, mandatory). 2) A 'subText' (Long text, optional). 3) A 'backgroundAsset' (File reference, mandatory). This ensures all deployed hero sections have enough styling definitions to render without encountering frontend errors.

---

**👤 You:**
> "List the most recent image assets uploaded to our Contentstack library."

**🤖 AI Agent:**
> I've retrieved the latest assets from your stack. You have several new items, including 'Banner-Spring-2024.png' and 'Product-Logo-v2.svg'. Would you like the direct CDN URLs for any of these?


## Installation & Usage

To install and use the **Contentstack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentstack](https://vinkius.com/mcp/contentstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
