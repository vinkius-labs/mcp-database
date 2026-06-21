# Wiki.js MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wikijs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wikijs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wikijs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Wiki.js instance—create, search, and update documentation pages directly from your AI agent.

## Description
Connect your **Wiki.js** instance to any AI agent and take full control of your internal knowledge base through natural conversation. This server allows you to interact with your documentation without leaving your chat interface.

### What you can do

- **Page Management** — Create new pages with full metadata, update existing content by ID, or delete outdated documentation.
- **Search & Discovery** — Search across your entire wiki for specific keywords or list all available pages to understand your knowledge structure.
- **Content Retrieval** — Fetch the raw content and metadata of any page using its URL path and locale.
- **Flexible Editing** — Support for different editor types and publishing statuses (published/private) directly via the API.

### How it works

1. Subscribe to this server
2. Enter your Wiki.js API URL and API Key
3. Start managing your documentation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — quickly update technical docs or search for internal guides while coding.
- **Knowledge Managers** — organize and prune wiki content through simple natural language commands.
- **Support Teams** — find relevant internal documentation to answer customer queries faster.


## Available Tools
- **create_page**: Create a new Wiki.js page
- **delete_page**: Delete a Wiki.js page
- **get_page**: Fetch a Wiki.js page by path
- **list_pages**: List all Wiki.js pages
- **search_pages**: Search for content in Wiki.js
- **update_page**: Update an existing Wiki.js page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wiki.js** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'deployment guide' in our Wiki.js."

**🤖 AI Agent:**
> I found 2 pages matching 'deployment guide': 'Infrastructure/Deployment' (path: infra/deploy) and 'CI-CD/Production-Guide' (path: cicd/prod). Would you like me to fetch the content of one of them?

---

**👤 You:**
> "Create a new markdown page at 'docs/api-v2' titled 'API v2 Reference'."

**🤖 AI Agent:**
> I've created the page 'API v2 Reference' at the path 'docs/api-v2'. It is currently published and set to markdown format. You can now add content to it using the update tool.

---

**👤 You:**
> "List all the pages available in our wiki."

**🤖 AI Agent:**
> I've retrieved the list of pages. You have 15 pages in total, including 'Home', 'Onboarding', 'API-Docs', and 'Security-Policy'. Which one would you like to inspect?


## Installation & Usage

To install and use the **Wiki.js** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wikijs](https://vinkius.com/mcp/wikijs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
