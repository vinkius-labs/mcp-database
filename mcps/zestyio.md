# Zesty.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zestyio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zestyio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zestyio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage content models, items, and instances via the Zesty.io API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zesty.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Zesty instances I have access to."

**🤖 AI Agent:**
> I've retrieved your instances. You have access to 3 properties: 'Corporate Blog' (ZUID: 8-abc-123), 'Product Showcase' (ZUID: 8-xyz-456), and 'Marketing Landing Pages' (ZUID: 8-def-789).

---

**👤 You:**
> "Show me the content items for the 'Press Releases' model (ZUID: '6-ghi-987')."

**🤖 AI Agent:**
> I found 5 items in the 'Press Releases' model. Recent titles include 'Q3 Earnings Report' and 'New Partnership Announcement'. Would you like to see the details for any of them?

---

**👤 You:**
> "Update the title of content item '7-jkl-654' in model '6-ghi-987' to '2024 Product Roadmap'."

**🤖 AI Agent:**
> Successfully updated content item '7-jkl-654'. The new title is now '2024 Product Roadmap' in your Zesty instance.


## Installation & Usage

To install and use the **Zesty.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zestyio](https://vinkius.com/mcp/zestyio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
