# Wolai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wolai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wolai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wolai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

All-in-one information organization and collaboration platform — manage pages, databases, and blocks via AI.

## Description
Empower your AI agent to orchestrate your knowledge base with **Wolai**, the versatile information organization platform. By connecting Wolai to your agent, you transform complex page organization and database management into a natural conversation. Your agent can instantly list your pages, retrieve block-level content, manage multi-dimensional databases, and even create new entries without you needing to navigate the complex web interface. Whether you are managing personal notes, project documentation, or shared team databases, your agent acts as a real-time knowledge assistant, keeping your workspace organized and your information accessible.

### What you can do

- **Page Orchestration** — List all accessible pages and retrieve detailed metadata about your workspace structure.
- **Block Management** — Browse content blocks within pages to access text and media information instantly.
- **Database Control** — Manage multi-dimensional tables (databases) with full support for querying and creating new rows.
- **Workspace Organization** — Create and update pages to maintain a clean and structured knowledge base.
- **Team Coordination** — Access workspace user lists to manage participation and collaboration effectively.

### How it works

1. Subscribe to this server
2. Enter your Wolai App ID and App Secret
3. Start managing your knowledge base through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — automate note-taking and organize project documentation through natural language.
- **Product Managers** — track feature requirements and manage product roadmaps directly from your AI-powered workspace.
- **Operations Teams** — oversee shared databases and team wikis through a unified AI interface.
- **Alibaba Ecosystem Users** — integrate your Wolai workflow into your AI-driven daily routines.


## Available Tools
- **create_database_row**: Add row to database
- **create_page**: Create a new Wolai page
- **get_database**: Get database schema
- **get_page**: Get page details
- **get_workspace_info**: Get workspace details
- **list_blocks**: ) within a specific page.

List page blocks
- **list_databases**: List all Wolai databases
- **list_pages**: List all Wolai pages
- **list_users**: List workspace users
- **query_database**: Query database rows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wolai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pages in my Wolai workspace."

**🤖 AI Agent:**
> I've retrieved your Wolai pages. You have 6 active pages, including 'Project Roadmap' and 'Meeting Notes'. Which one would you like to view the content for?

---

**👤 You:**
> "Query the 'Product Backlog' database for items with 'High' priority."

**🤖 AI Agent:**
> I've queried the 'Product Backlog' database. I found 3 items with high priority: 'Refactor Auth Engine', 'Implement PDF Export', and 'API Documentation'. Would you like more details on any of them?

---

**👤 You:**
> "Create a new page in Wolai titled 'Weekly Sprint Notes'."

**🤖 AI Agent:**
> Done! I've created the page 'Weekly Sprint Notes' in your workspace. You can now start adding content blocks to it. Page ID: WL-8821.


## Installation & Usage

To install and use the **Wolai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wolai](https://vinkius.com/mcp/wolai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
