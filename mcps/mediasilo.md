# MediaSilo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mediasilo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mediasilo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mediasilo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Video collaboration and asset management via MediaSilo — manage projects, assets, and Quicklinks.

## Description
Connect your **MediaSilo** (Shift) account to any AI agent and take full control of your media asset management and collaboration through natural conversation.

### What you can do

- **Asset Management** — List all media assets, search by term, and fetch detailed metadata for videos and images
- **Project Organization** — Enumerate active projects, list folders, and inspect specific project configurations
- **Collaboration** — Manage Quicklinks for secure media sharing and review with your team and clients
- **User Inventory** — List authorized users and manage access within your MediaSilo workspace

### How it works

1. Subscribe to this server
2. Enter your MediaSilo API Key and API Secret
3. Start managing your media workflows from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_asset**: Get details for a specific asset
- **get_project**: Get details for a specific project
- **get_project_assets**: List all assets within a project
- **get_quicklink**: Get details for a specific Quicklink
- **list_assets**: ) from MediaSilo.

List all media assets
- **list_folders**: List folders within a project
- **list_projects**: List all projects
- **list_quicklinks**: List all Quicklinks
- **list_users**: List all users
- **search_assets**: Search for assets by term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MediaSilo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent assets in MediaSilo."

**🤖 AI Agent:**
> Retrieving assets... I found several recently added files, including 'Commercial_V3.mp4' and 'Product_Hero_Shot.jpg'.

---

**👤 You:**
> "Show folders for project 'Fall Campaign'."

**🤖 AI Agent:**
> Querying project folders... The 'Fall Campaign' project contains 3 folders: 'Raw Footage', 'Drafts', and 'Approved Masters'.

---

**👤 You:**
> "Search for assets matching 'logo'."

**🤖 AI Agent:**
> Searching... I found 5 assets matching 'logo', including high-res PNGs and vector files.


## Installation & Usage

To install and use the **MediaSilo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mediasilo](https://vinkius.com/mcp/mediasilo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
