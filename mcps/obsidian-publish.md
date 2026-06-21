# Obsidian Publish MCP Server

Empower your AI to read your public or private Obsidian Publish sites. Index files, crawl navigation trees, and retrieve deep markdown knowledge.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/obsidian-publish)

## Overview
**Category:** productivity
**Tools Count:** 5

## Description
Connect your **Obsidian Publish** environment to your AI agent and construct an intelligent oracle that reads smoothly from your personal or corporate markdown knowledge base.

### What you can do

- **Vault Crawling** — Programmatically fetch your entire published vault structure utilizing `list_files` and `list_navigation` to build contextual trees.
- **Direct Note Access** — Execute `get_file` to stream the complete raw markdown contents of any note directly into your chat workflow for fast summarization.
- **Metadata Operations** — Use `get_metadata` to retrieve frontmatter properties, tags, and internal link logic mapped by Obsidian.
- **Site Auditing** — Easily ping `site_info` to ensure connectivity and verify the deployment status of your target Obsidian publish endpoint.

### How it works

1. Subscribe to this server
2. Enter your Obsidian Publish Site ID (and optional access token for private vaults)
3. Start fetching and analyzing your personal notes directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Writers** — seamlessly command an AI to read past chapters, cross-reference characters, or verify published assertions without opening Obsidian.
- **Corporate Teams** — build a highly accessible chatbot that rapidly reads and summarizes your team's documented standard operating procedures (SOPs).
- **Developers** — fetch specific code snippets and technical architectures housed in your digital garden natively within the IDE.


## Available Tools
- **list_files**: List all explicitly published raw file paths across the Obsidian workspace
- **get_file**: Retrieve exact textual file content and binary assets
- **site_info**: Identify global configuration and styling mapping the site
- **list_navigation**: Visualize structurally formatted Markdown navigation trees
- **get_metadata**: Extract internal creation hashes mapping a specific Markdown page


## Installation & Usage

To install and use the **Obsidian Publish** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/obsidian-publish](https://vinkius.com/mcp/obsidian-publish)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
