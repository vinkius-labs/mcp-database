# Builder.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/builderio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/builderio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/builderio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your visual CMS via Builder.io — track content entries, models, and symbols directly from any AI agent.

## Description
Connect your **Builder.io** account to any AI agent and orchestrate your visual CMS, content management, and digital experience workflows through natural conversation.

### What you can do

- **Content Oversight** — List and retrieve detailed metadata for all your content entries across different models (Pages, Blog Posts, etc.).
- **Model Management** — List all content models in your space and retrieve detailed schema metadata.
- **Visual Automation** — Create and update content entries programmatically using the Write API directly from your workspace.
- **Infrastructure Coordination** — Access and monitor your spaces, organization settings, and reusable symbols.
- **Performance Tracking** — Retrieve real-time API usage statistics to monitor your CMS performance.
- **Entry Deep Dives** — Get detailed data for specific content or model IDs straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Builder.io Public and Private API Keys
3. Start managing your digital experiences from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers & Engineers** — quickly check content structures or update entries without manual dashboard work.
- **Content Managers & Editors** — retrieve published content and monitor model schemas straight from their workflow tools.
- **Digital Teams** — orchestrate cross-space content and monitor usage using natural language.


## Available Tools
- **create_content_entry**: Create a new content entry
- **get_content_entry**: Get a specific content entry
- **get_model**: Get details of a specific content model
- **get_space**: Get details of a specific space
- **get_api_usage**: Retrieve API usage statistics
- **list_content**: List content entries for a specific model
- **list_models**: List all content models in the space
- **list_spaces**: List all spaces in your organization
- **list_symbols**: List all reusable symbols
- **update_content_entry**: Update an existing content entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Builder.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all content entries for the 'page' model."

**🤖 AI Agent:**
> I've retrieved your pages. You have 5 entries, including 'Home' (ID: page_1), 'About Us' (ID: page_2), and 'Contact' (ID: page_3).

---

**👤 You:**
> "Show the schema details for the 'blog-post' model."

**🤖 AI Agent:**
> Retrieving model details... The 'blog-post' model includes fields like 'title' (Text), 'content' (Rich Text), 'author' (Reference), and 'publishDate' (Date).

---

**👤 You:**
> "Create a new entry in 'announcement-bar' with name 'Promo Banner'."

**🤖 AI Agent:**
> Entry 'Promo Banner' has been successfully created in the 'announcement-bar' model with ID entry_99283.


## Installation & Usage

To install and use the **Builder.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/builderio](https://vinkius.com/mcp/builderio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
