# Statuspage (Atlassian) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/statuspage-atlassian)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/statuspage-atlassian-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/statuspage-atlassian-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Atlassian Statuspage — list pages, update configurations, and handle user permissions or access controls via AI.

## Description
Connect your **Statuspage (Atlassian)** account to any AI agent to monitor and manage your incident communication infrastructure through natural conversation.

### What you can do

- **Page Management** — List all status pages and fetch detailed configurations for specific IDs using `list_pages` and `get_page`.
- **Configuration Updates** — Update page names, domains, and branding settings instantly with the `update_page` tool.
- **User Permissions** — Query and update user roles and permissions within your organization using `get_user_permissions` and `update_user_permissions`.
- **Embed Widgets** — Manage status embed configurations to control how status is displayed on your site via `get_status_embed_config`.
- **Access Control** — Manage audience-specific users for private status pages, including creation and updates with `list_page_access_users` and `create_page_access_user`.

### How it works

1. Subscribe to this server
2. Enter your Statuspage API Key
3. Start managing your status infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — quickly check and update status page configurations during incident response without leaving the terminal.
- **Support Teams** — manage private page access for specific customers directly through the AI assistant.
- **Product Owners** — ensure branding and domains are correctly configured across all status environments.


## Available Tools
- **create_page_access_user**: Add a page access user
- **delete_page_access_user_components**: Remove components for page access user
- **delete_page_access_user_metrics**: Delete metrics for page access user
- **delete_page_access_user**: Delete page access user
- **get_page_access_user_components**: Get components for page access user
- **get_page**: Get a specific page
- **get_status_embed_config**: Get status embed config settings
- **get_user_permissions**: Get a user's permissions
- **list_page_access_users**: Get a list of page access users
- **list_pages**: Get a list of pages
- **update_page_access_user_components**: Add/Replace components for page access user
- **update_page_access_user_metrics**: Add/Replace metrics for page access user
- **update_page_access_user**: Update page access user
- **update_page**: ).

Update a page
- **update_status_embed_config**: Update status embed config settings
- **update_user_permissions**: g., page_configuration, incident_manager, maintenance_manager).

Update a user's role permissions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Statuspage (Atlassian)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Statuspage pages."

**🤖 AI Agent:**
> I've retrieved your pages. You have access to: 'Main Production' (ID: abc123) and 'Internal Services' (ID: def456).

---

**👤 You:**
> "Show me the details for page ID abc123."

**🤖 AI Agent:**
> Fetching details for page abc123... The page is named 'Main Production', hosted at status.example.com, and currently has branding enabled.

---

**👤 You:**
> "Update the name of page abc123 to 'Global Operations Status'."

**🤖 AI Agent:**
> I have successfully updated the name of page abc123 to 'Global Operations Status'.


## Installation & Usage

To install and use the **Statuspage (Atlassian)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/statuspage-atlassian](https://vinkius.com/mcp/statuspage-atlassian)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
