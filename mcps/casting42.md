# Casting42 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/casting42)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/casting42-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/casting42-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage talent databases and casting projects via Casting42 — track profiles, media, and custom attributes directly from any AI agent.

## Description
Connect your **Casting42** account to any AI agent and take full control of your talent database and casting workflows through natural conversation. Streamline talent discovery and project management.

### What you can do

- **Talent Discovery** — Search and list talent profiles with detailed metadata and categories natively
- **Deep-Dive Profiles** — Access complete talent information, including custom attributes and organizational tags flawlessly
- **Media Management** — Retrieve headshots, videos, and self-tapes associated with talent profiles securely
- **Project Oversight** — Monitor active casting projects and talent assignments in real-time
- **Custom Data Control** — Access the unique custom fields and attributes defined in your specific database
- **Classification Analysis** — List and filter talents by categories and tags to identify the right fit for your needs

### How it works

1. Subscribe to this server
2. Enter your Casting42 API Key (obtained from your account Settings)
3. Start managing your talent database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Casting Directors** — search talent profiles and review media using natural language
- **Talent Agents** — manage their internal talent database and project assignments without opening the dashboard
- **Production Teams** — quickly look up talent details and custom attributes straight from their chat interface
- **Recruiters** — identify and classify talents based on specific project needs and tags


## Available Tools
- **get_talent_details**: Get detailed information for a specific talent
- **list_talent_categories**: List configured talent categories
- **list_custom_attributes**: List custom data fields defined in the database
- **list_talent_media**: List headshots, videos, and media for a specific talent
- **list_casting_projects**: List casting projects
- **list_talent_tags**: List tags used for talent organization
- **list_talents**: List talents from the database
- **search_talents**: Search for talents by name or attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Casting42** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for talents named 'John' in my Casting42 database."

**🤖 AI Agent:**
> Searching for 'John'... I found 3 profiles: John Smith (Actors), John Doe (Models), and John Wayne (Stunt). Which one would you like to see details for?

---

**👤 You:**
> "Show me the media files for talent ID 12345."

**🤖 AI Agent:**
> Retrieving media for talent 12345... I found 2 headshots, 1 showreel video, and 3 self-tapes. You can access them via these links: [Links provided].

---

**👤 You:**
> "What are the active casting projects right now?"

**🤖 AI Agent:**
> Checking active projects... You have 2 active projects: 'Summer Commercial 2024' and 'Feature Film - Project X'. Both are currently in the 'Selection' phase.


## Installation & Usage

To install and use the **Casting42** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/casting42](https://vinkius.com/mcp/casting42)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
