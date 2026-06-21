# DeveloperHub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/developerhub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/developerhub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/developerhub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to manage documentation projects, track pages, and monitor changelogs via the DeveloperHub API.

## Description
Integrate **DeveloperHub**, the specialized platform for developer documentation, directly into your AI workflow. Manage your documentation portals, monitor page updates and versions, and track product changelogs using natural language.

### What you can do

- **Project Oversight** — List and retrieve technical metadata for all your documentation projects and portals.
- **Page Management** — Access the full page hierarchy, retrieve Markdown content, and track recent updates.
- **Version Control** — Monitor available documentation versions and identify which one is currently active.
- **Changelog Tracking** — List product release notes and updates associated with your documentation projects.

### How it works

1. Connect the DeveloperHub integration to your AI assistant.
2. Authorize using your DeveloperHub API Key (found in your account settings).
3. Orchestrate your developer experience and documentation through intuitive conversation.

### Who is this for?

- **Technical Writers** — Quickly check page statuses and recent modifications on the go.
- **Product Managers** — Monitor changelog entries and documentation readiness during releases.
- **Developer Advocates** — Search for specific documentation snippets and technical details via chat.


## Available Tools
- **get_account_metadata**: Retrieve metadata and usage limits for your DeveloperHub account
- **get_documentation_page_content**: Get the full content and metadata for a specific documentation page
- **get_documentation_sitemap**: Retrieve a structural map of all pages in a project
- **get_documentation_project_details**: Get detailed information for a specific documentation project
- **list_product_changelogs**: List all changelog entries associated with a documentation project
- **list_documentation_pages**: List all pages and sub-pages within a specific project
- **list_documentation_projects**: List all documentation projects in your DeveloperHub account
- **list_recently_updated_pages**: Identify documentation pages that have been recently modified
- **list_documentation_versions**: List all versions (e.g. v1.0, v2.0) available for a project
- **search_documentation_portal**: Search for specific keywords across all pages in a documentation project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeveloperHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all documentation pages in the 'API-Reference' project."

**🤖 AI Agent:**
> I've found 15 pages in 'API-Reference', including 'Authentication', 'Endpoints Overview', and 'Error Codes'. Would you like to see the sub-pages for any of these sections?

---

**👤 You:**
> "What were the latest updates in our project changelog?"

**🤖 AI Agent:**
> The latest changelog entries for your project are: 'v2.1.0 - Added GraphQL support', 'v2.0.5 - Improved search performance', and 'v2.0.4 - Bug fixes in SDK'. Should I retrieve the full details for the v2.1.0 update?

---

**👤 You:**
> "Search for 'webhooks' in our documentation portal."

**🤖 AI Agent:**
> I've found 3 pages matching 'webhooks': 'Webhooks Guide', 'Configuring Webhooks', and 'Webhook Events Reference'. Which one would you like to explore?


## Installation & Usage

To install and use the **DeveloperHub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/developerhub](https://vinkius.com/mcp/developerhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
