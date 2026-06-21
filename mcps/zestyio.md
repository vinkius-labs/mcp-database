# Zesty.io MCP Server

Manage content models, items, and instances via the Zesty.io API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zestyio)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect your **Zesty.io** account to any AI agent to streamline your headless CMS operations. This MCP server enables your agent to interact with instances, content models, and data entries (items) directly from natural language.

### What you can do

- **Instance Oversight** — List all Zesty.io instances associated with your account and retrieve their metadata
- **Schema Management** — List content models to understand your data structures and identify Model ZUIDs
- **Content Operations** — List, retrieve, create, and update content items within specific models
- **Technical Auditing** — Access instance settings and technical metadata for any of your properties
- **Workflow Automation** — Delete content items and maintain your CMS hierarchy via natural language commands

### How it works

1. Subscribe to this server
2. Enter your Zesty API Token and Instance ZUID (starting with 8-)
3. Start managing your content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — Update website content and manage entries without logging into the Zesty interface
- **Developers** — Quickly query content models and test API data structures from your IDE
- **Growth Engineers** — Automate the creation of landing page items and marketing content entries


## Available Tools
- **create_content_item**: Requires a JSON object with field values.

Create a new content item
- **delete_content_item**: Delete a content item
- **get_content_item**: Get details for a specific content item
- **list_zesty_instances**: List all Zesty.io instances associated with the account
- **list_content_items**: List content items for a specific model
- **list_content_models**: Use this to identify Model ZUIDs.

List all content models for the current instance
- **get_instance_settings**: Get configuration settings for the instance
- **update_content_item**: Update an existing content item


## Installation & Usage

To install and use the **Zesty.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zestyio](https://vinkius.com/mcp/zestyio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
