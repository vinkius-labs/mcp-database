# Obsidian Publish MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/obsidian-publish)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/obsidian-publish-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/obsidian-publish-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Empower your AI to read your public or private Obsidian Publish sites. Index files, crawl navigation trees, and retrieve deep markdown knowledge.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Obsidian Publish** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the vault and list all the files currently publicly available."

**🤖 AI Agent:**
> According to the navigation tree, you have 14 distinct markdown entries published. Key documents include 'Index', 'Machine Learning Setup', and 'Project Specs'.

---

**👤 You:**
> "Read the contents of 'System Requirements 2026.md'."

**🤖 AI Agent:**
> I've pulled the content of 'System Requirements 2026.md'. The document includes heavy focus on horizontal scaling algorithms and Python-centric deployments. Would you like a condensed executive summary?

---

**👤 You:**
> "Fetch the metadata and tags applied to my 'Inbox' note."

**🤖 AI Agent:**
> The 'Inbox' note has the following metadata: generated on May 5th, tagged with `#todo` and `#ideas`, and links heavily to `Projects.md` and `Archived Content.md`.


## Installation & Usage

To install and use the **Obsidian Publish** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/obsidian-publish](https://vinkius.com/mcp/obsidian-publish)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
