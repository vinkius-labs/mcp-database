# Builder MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/builder)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/builder-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/builder-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Automate Builder.io headless CMS workflows — generate content blocks, update models, and orchestrate visual components directly from any AI agent.

## Description
Connect your **Builder.io** space to any AI agent and take full programmatic control over your headless CMS architecture and visual pages through natural conversation.

### What you can do

- **Content Automation** — Create, update, or wipe specific content entries across any data model dynamically
- **Schema Navigation** — List your active Builder models and analyze exact field definitions and strict JSON bounds
- **Search & Retrieval** — Use query strings to pull matched content documents or count entities effortlessly
- **Media Fetching** — Inspect metadata and URLs of uploaded assets living on the Builder platform
- **Headless Maintenance** — Delete deprecated components or page sections instantly using targeted endpoints

### How it works

1. Subscribe to this server
2. Enter your Builder Public and Private API Key pair
3. Start fetching schemas and inserting web blocks from Claude, Cursor, or any MCP-compatible client

No need to leave the code editor to see how a model is defined. Read schema structures immediately inside your chat.

### Who is this for?

- **Frontend Developers** — retrieve the strict data schema of a Builder model before configuring your frontend fetch logic
- **Content Editors** — push 50 translated copies of a landing page section automatically via API automation
- **DevOps** — wipe orphaned elements or test environment components natively without touching the UI


## Available Tools
- **count_model_entities**: Quickly count the number of live items stored within a specific model
- **create_visual_block**: Create new content entries or visual blocks inside a Builder model
- **wipe_visual_block**: Permanently delete a specific content entry from Builder.io
- **get_single_content**: g. `query.data.title=Home`).

Retrieve a specific content document by query matching from Builder.io
- **get_media_file**: Retrieve details about an uploaded media asset within Builder.io
- **get_model_schema**: Get the exact field structure and schema definitions for a single model
- **list_model_content**: Useful for fetching dynamic content blocks or pages.

Retrieve a list of content entries for a specific Builder.io model
- **list_builder_models**: List all defined data models and schemas in the Builder space
- **search_active_models**: Find Builder models matching a specific criteria or substring
- **update_visual_block**: Update an existing Builder.io content block or document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Builder models in my workspace."

**🤖 AI Agent:**
> You have 4 models configured:
1. 'page' (Visual page content)
2. 'section' (Visual block/symbol)
3. 'blog-post' (Data model with text fields)
4. 'custom-hero' (Visual component)

Which of these models would you like me to inspect the schema for?

---

**👤 You:**
> "Fetch the schema for the 'custom-hero' model."

**🤖 AI Agent:**
> The 'custom-hero' model expects the following main fields:
- `title` (Text) — Required
- `subtitle` (Text) — Optional
- `cta_link` (URL) — Required
- `bg_image` (File/URL) — Optional

Would you like me to create a sample block using this exact formatting for you?

---

**👤 You:**
> "Find a page with the title "Home" on the 'page' model."

**🤖 AI Agent:**
> I queried `query.data.title=Home` on the 'page' model. Found 1 match: Document ID `d9e72a4...`. It is currently published and holds multiple visual layout blocks inside `data.blocks`. Do you want to receive the full JSON output of the structure?


## Installation & Usage

To install and use the **Builder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/builder](https://vinkius.com/mcp/builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
