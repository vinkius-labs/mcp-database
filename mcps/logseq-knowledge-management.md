# Logseq (Knowledge Management) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/logseq-knowledge-management)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/logseq-knowledge-management-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/logseq-knowledge-management-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your knowledge base via Logseq — create pages, insert outliner blocks, and search across your local graph.

## Description
Connect your **Logseq** instance to any AI agent and take full control of your privacy-first knowledge graph and personal documentation through natural conversation.

### What you can do

- **Graph Orchestration** — List all pages and retrieve detailed hierarchical block trees representing your local outliner data directly from your agent
- **Page Management** — Create new organized pages or journal entries and manage their lifecycle including irreversible deletion of metadata loops securely
- **Block Operations** — Append, update, or delete individual outliner blocks, preserving precise UUID bounds and linking indices within your graph
- **Deep Content Search** — Execute local queries to extract explicitly bound text targets across your entire knowledge base, including titles and namespaces
- **Hierarchical Inspection** — Extract deeply nested outliner hierarchies to understand the complex structural relationships between your ideas and projects
- **Environment Audit** — Identify current active graph paths and local database directories to verify your agent is targeting the correct knowledge store

### How it works

1. Subscribe to this server
2. Enable the HTTP API in your Logseq Settings
3. Enter your Logseq API Token and Host URL (e.g., http://localhost:12315)
4. Start managing your local graph from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — organize research and meeting notes through natural conversation without manually navigating the Logseq outliner
- **Software Developers** — manage technical documentation and project logs directly from your IDE or workspace terminal
- **PKM Enthusiasts** — audit complex graph structures and perform bulk block updates to maintain a clean and optimized personal knowledge base


## Available Tools
- **list_pages**: List all pages in the current Logseq graph
- **get_page**: Retrieve metadata for a specific Logseq page by mapping name or UUID limits
- **create_page**: Editor.createPage` deploying new pages including native markdown contents inside the local map.

Create explicitly a new organized page in the Logseq target Graph
- **delete_page**: Editor.deletePage` removing content arrays destroying metadata loops.

Delete an entire explicit active Logseq page irreversibly
- **get_page_blocks**: Extract the hierarchical explicit native tree limit array block from a page map
- **insert_block**: Editor.insertBlock` natively adding outliner chunks executing explicit properties updating nodes immediately.

Append an explicitly managed Block limit tracking inside the specific Logseq map
- **update_block**: Editor.updateBlock` safely preserving UUID bounds retaining linking indices natively.

Modify raw properties explicitly bound inside a given Logseq tracked block
- **delete_block**: Editor.removeBlock` erasing specific limit bounds dropping child dependencies explicitly.

Delete an explicit active Block target removing explicit nodes safely
- **search_content**: Execute local queries extracting explicitly bound text targets crossing Graph indices
- **get_current_graph**: Validate environment limits identifying explicit current graph arrays parsed natively


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Logseq (Knowledge Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Logseq graph for 'smart building research'"

**🤖 AI Agent:**
> I've scanned your graph and found 3 relevant matches: 1) Page 'Smart-Buildings-Project', 2) Block in 'Journal 2026-03-27' mentioning sensor setups, 3) Tag '#research' in multiple blocks. Would you like to see the blocks from the project page?

---

**👤 You:**
> "Create a new page called 'Meeting Notes' with content '# Meetings 2026'"

**🤖 AI Agent:**
> Page 'Meeting Notes' created successfully in your graph. I've added the initial markdown header. You can now use the `insert_block` tool to add specific meeting items or agenda points.

---

**👤 You:**
> "Add a block to the 'Project Alpha' page: 'Verify API endpoints for production'"

**🤖 AI Agent:**
> Block added successfully to 'Project Alpha'. It is now part of the outliner tree for that page. Would you like me to add any specific child blocks or sub-tasks under this point?


## Installation & Usage

To install and use the **Logseq (Knowledge Management)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/logseq-knowledge-management](https://vinkius.com/mcp/logseq-knowledge-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
