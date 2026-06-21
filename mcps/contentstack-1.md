# Contentstack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contentstack-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/contentstack-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/contentstack-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Manage headless CMS via Contentstack — list and create entries, audit content types, handle media assets, and publish to environments directly from any AI agent.

## Description
Connect your **Contentstack** account to any AI agent and take full control of your agentic experience platform and headless CMS through natural conversation.

### What you can do

- **Entry Orchestration** — List and retrieve document rows bound to specific content types and create new drafts using purely formatted JSON attributes
- **Content Mutation** — Safely update existing entries by overwriting schema blocks and substituting draft values through the Management API
- **Live Publishing** — Trigger the exact publication sequence to push CMS data to specific environments (e.g., development, production, staging)
- **Schema Inspection** — Enumerate global schemas and decode native boundaries to identify exactly what fields and validation rules the database expects
- **Media Management** — Access global files and retrieve explicit media metadata, including original Contentstack URLs, to mitigate manual CDN scraping
- **Repository Cleanup** — Irreversibly remove app nodes and delete live document rows to manage internal database allocations and clear quotas

### How it works

1. Subscribe to this server
2. Enter your Contentstack Stack API Key and Management Token
3. Start managing your composable content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — create, update, and publish entries across environments without leaving the chat
- **Front-end Developers** — inspect content type schemas and retrieve asset URLs directly during development
- **Product Teams** — monitor content models and audit available field types for new digital experiences
- **Digital Ops** — manage stack environments and verify publication statuses using natural language


## Available Tools
- **create_cms_entry**: Provision a highly-available JSON Payload generating new Contentstack Drafts
- **wipe_cms_entry**: Irreversibly vaporize explicit App nodes dropping live Document rows
- **get_media_asset**: Retrieve the exact structural matching verifying explicit Media IDs
- **get_schema_details**: Perform structural extraction of properties driving active Fields
- **get_single_entry**: Retrieve explicit Cloud logging tracing explicit Entry UUIDs limitlessly
- **list_media_assets**: Inspect deep internal arrays mitigating specific Picture limits
- **list_global_schemas**: Enumerate explicitly attached structured rules exporting active Types
- **list_type_entries**: Identify bounded routing spaces inside the Headless Contentstack CMS schemas
- **publish_to_environment**: g., development, production).

Dispatch an automated validation check routing CMS Data Live
- **update_cms_entry**: Mutate global Web CRM boundaries substituting Draft values safely


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contentstack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all entries for content type 'homepage'"

**🤖 AI Agent:**
> I found 3 entries for 'homepage'. The latest is 'Main Homepage v2' (UID: entry_123). Would you like to see the draft values for this entry?

---

**👤 You:**
> "Publish entry 'entry_456' of type 'blog_post' to production"

**🤖 AI Agent:**
> Publishing request sent! 'entry_456' is now being pushed to the 'production' environment. I will notify you once the sequence is complete.

---

**👤 You:**
> "Show me the details for content model 'product_schema'"

**🤖 AI Agent:**
> Retrieving schema for 'product_schema'... This model includes fields like 'product_name' (Text), 'sku' (Symbol), 'price' (Number), and 'gallery' (File Reference). I can decode the specific validation rules for you.


## Installation & Usage

To install and use the **Contentstack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentstack-1](https://vinkius.com/mcp/contentstack-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
