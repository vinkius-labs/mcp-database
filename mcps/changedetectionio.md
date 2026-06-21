# ChangeDetection.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/changedetectionio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/changedetectionio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/changedetectionio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Monitor website changes automatically — track visual or text updates, manage watches, and receive alerts via any AI agent.

## Description
Connect your **ChangeDetection.io** instance to any AI agent to automate web monitoring and data extraction through natural conversation.

### What you can do

- **Watch Management** — Create, update, and delete monitors for any URL to track content changes
- **Snapshot Analysis** — Retrieve historical snapshots and compare differences (diffs) to see exactly what changed
- **Tagging & Organization** — Categorize your watches with tags to manage large-scale monitoring projects
- **Instant Rechecks** — Trigger immediate checks for specific watches to get the most up-to-date information
- **History Tracking** — Access the full history of a watch to analyze trends and previous versions of a page

### How it works

1. Subscribe to this server
2. Enter your ChangeDetection.io Instance URL and API Key
3. Start monitoring the web from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — track price changes, availability, or content updates across multiple competitors automatically
- **Developers** — monitor API documentation or website changes to stay ahead of breaking updates
- **SEO Specialists** — keep an eye on SERP changes or competitor landing page modifications


## Available Tools
- **create_tag**: Create a new tag
- **create_watch**: Create a new watch
- **delete_watch**: Delete a watch
- **get_snapshot_diff**: Use "previous" and "latest" as keywords.

Get snapshot difference (diff)
- **get_snapshot**: Use "latest" for the most recent check.

Get single snapshot
- **get_tag**: Get single tag
- **get_watch_favicon**: Get watch favicon
- **get_watch_history**: Get watch history
- **get_watch**: Get single watch
- **import_urls**: io.

Import API
- **list_tags**: List all tags
- **list_watches**: List all watches
- **search_watches**: Search API
- **update_watch**: Update an existing watch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChangeDetection.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active web watches."

**🤖 AI Agent:**
> I've retrieved your watches. You have 3 active monitors: 'Competitor Pricing' (UUID: 550e8400), 'API Docs' (UUID: 123e4567), and 'Stock Alert' (UUID: 890b1234).

---

**👤 You:**
> "Create a new watch for https://example.com with the title 'Example Monitor'."

**🤖 AI Agent:**
> Successfully created the watch for https://example.com. It has been assigned UUID: 771f9211. I will start tracking changes for you now.

---

**👤 You:**
> "Show me the difference between the last snapshots for watch 550e8400."

**🤖 AI Agent:**
> Comparing snapshots for 'Competitor Pricing'... I found that the price text changed from '$49.99' to '$39.99' and a new 'On Sale' badge was added to the header.


## Installation & Usage

To install and use the **ChangeDetection.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/changedetectionio](https://vinkius.com/mcp/changedetectionio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
