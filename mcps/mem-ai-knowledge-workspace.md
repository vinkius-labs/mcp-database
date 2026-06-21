# Mem AI (Knowledge Workspace) MCP Server

Manage your knowledge base via Mem.ai — create notes, run AI semantic search, and organize collections.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mem-ai-knowledge-workspace)

## Overview
**Category:** productivity
**Tools Count:** 12

## Description
Connect your **Mem.ai** workspace to any AI agent and take full control of your personal and team knowledge through natural conversation.

### What you can do

- **Knowledge Orchestration** — Create new mems (notes) using Markdown directly from your agent, instantly transforming textual ideas into indexed knowledge vectors
- **AI Semantic Search** — Leverage dense semantic similarity to find notes across your entire workspace, identifying relevant information based on meaning rather than explicit keywords
- **Deep Content Retrieval** — Extract the full scalar text body and context metadata for specific mems to retrieve precise project details securely
- **Collection Management** — Establish thematic groupings (Collections) and attach live mems structurally to maintain organized project boundaries natively
- **Quick Capture (Mem It)** — Trigger rapid capture blocks for links, snippets, or raw thoughts, allowing your agent to log ideas without manual dashboard navigation
- **Contextual Updates** — Mutate existing mem content to keep project logs and meeting notes up-to-date while preserving historical knowledge mappings
- **Resource Inventory** — List all available mems or explore specific collections to understand your knowledge distribution and team documentation footprint

### How it works

1. Subscribe to this server
2. Enter your Mem.ai API Key
3. Start managing your workspace from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — organize research and meeting notes through natural conversation without manual outliner management
- **Project Teams** — sync project documentation and manage shared knowledge collections directly from your workspace
- **Researchers** — leverage AI semantic search to bridge ideas and retrieve relevant context across massive personal knowledge bases efficiently


## Available Tools
- **create_mem**: ai. Converts plain textual knowledge to indexed vectors immediately mapped implicitly via AI.

Create a new mem (note) in Mem.ai using Markdown
- **list_mems**: Returns identifiers and raw bodies. Careful, this returns heavy payloads.

List all raw mems across the global workspace
- **get_mem**: Retrieve explicit full context metadata by target Mem ID
- **update_mem**: Replaces absolute text values so ensure `get_mem` was run to append rather than destroy inadvertently.

Update pre-existing mem content natively swapping strings
- **delete_mem**: No recovery is possible via API.

Irreversibly vaporize a mem document globally
- **search_mems**: AI semantic search looking into all indexed knowledge
- **mem_it**: Quick capture shortcut generating automated blocks
- **list_collections**: Query explicitly tracked thematic Collections arrays
- **create_collection**: Establish new logical thematic groupings mapping notes
- **get_collection**: Inspect specific Collection metadata elements
- **add_mem_to_collection**: Attach live Mems structurally inside explicitly mapped Collections
- **list_collection_mems**: Query ALL explicit Mem bodies inside specific Collections


## Installation & Usage

To install and use the **Mem AI (Knowledge Workspace)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mem-ai-knowledge-workspace](https://vinkius.com/mcp/mem-ai-knowledge-workspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
