# Framer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/framer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/framer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/framer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Equip your AI agent with direct access to Framer — manage CMS collections, sync content, and publish site changes without opening the Framer editor.

## Description
Connect **Framer** to your AI agent and manage your website CMS content and publishing workflow conversationally.

### What you can do

- **CMS Collections** — List, create, update, and manage CMS collection items directly from natural language commands.
- **Content Sync** — Push content updates from external data sources into your Framer CMS collections programmatically.
- **Site Publishing** — Trigger site publishes to push your latest CMS changes live.
- **Collection Schema** — Query collection structures and field definitions to understand your content model.

### How it works

1. Subscribe to the Framer integration on the marketplace.
2. Generate a Server API key from your Framer project (Site Settings → General → generate API key).
3. Ask your AI agent to manage CMS content, sync data, or publish your site.

### Who is this for?

- **Design-Led Teams** — Update website content without touching the Framer canvas or disrupting design layouts.
- **Marketing Teams** — Publish landing pages, blog posts, and campaign content directly from conversations.
- **Developers** — Programmatically sync CMS data from headless APIs, databases, or spreadsheets into Framer.


## Available Tools
- **list_projects**: List all Framer projects
- **get_project**: Get project details
- **list_collections**: List CMS collections
- **list_collection_items**: List items in a CMS collection
- **create_collection_item**: Create a new CMS item
- **publish_site**: This makes changes visible to visitors.

Publish the website
- **list_pages**: List all site pages
- **get_site_info**: Get site configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Framer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all CMS collections in my Framer site."

**🤖 AI Agent:**
> Your Framer project has 3 CMS collections: 'Blog Posts' (18 items), 'Team Members' (12 items), and 'Case Studies' (7 items).

---

**👤 You:**
> "Add a new team member 'Ana Silva' to the Team Members collection."

**🤖 AI Agent:**
> Team member 'Ana Silva' added to the 'Team Members' collection. Fields set: Name, Role (empty). You can ask me to update additional fields like bio, photo URL, or social links.

---

**👤 You:**
> "Publish my Framer site with the latest CMS changes."

**🤖 AI Agent:**
> Site publish triggered. Your CMS changes are now live. Last updated: just now. All 37 collection items synced across 3 collections.


## Installation & Usage

To install and use the **Framer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/framer](https://vinkius.com/mcp/framer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
