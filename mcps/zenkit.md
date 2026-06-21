# Zenkit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenkit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zenkit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zenkit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage workspaces, lists, and entries via the Zenkit API.

## Description
Connect your **Zenkit** account to any AI agent to streamline your productivity and project management. This MCP server enables your agent to interact with workspaces, lists (collections), and data entries directly from natural language.

### What you can do

- **Workspace Oversight** — List all workspaces and retrieve their constituent lists and metadata
- **List Management** — Query detailed configurations and field elements for any Zenkit list
- **Data Operations** — List, retrieve, create, and update entries (items) within your collections
- **Field Discovery** — Inspect list elements to understand the data structure and field types
- **Content Cleanup** — Delete entries and maintain your lists directly via natural language commands

### How it works

1. Subscribe to this server
2. Enter your Zenkit API Key
3. Start managing your productivity data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — Monitor task lists and update entry statuses across multiple workspaces
- **Operations Teams** — Automate data entry and record maintenance via simple commands
- **Knowledge Workers** — Quickly retrieve and organize information stored in Zenkit collections


## Available Tools
- **create_entry**: Requires a JSON object with field values.

Create a new entry in a list
- **delete_entry**: Delete an entry from a list
- **list_elements**: List all elements (fields) defined in a list
- **list_entries**: List all entries (items) in a list
- **get_list_details**: Get details for a specific list
- **get_workspace_details**: Get details for a specific workspace
- **update_entry**: Update an existing entry
- **list_workspaces**: List all workspaces and their lists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zenkit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Zenkit workspaces and their collections."

**🤖 AI Agent:**
> I've retrieved your workspaces. You have 3 workspaces: 'Marketing', 'Product Development', and 'Personal'. The 'Marketing' workspace contains 2 lists: 'Social Media Calendar' and 'Asset Library'.

---

**👤 You:**
> "Show me all entries in the list with ID '98765'."

**🤖 AI Agent:**
> I found 15 entries in list 98765. Notable items include 'Review Q2 Budget', 'Update Brand Guidelines', and 'Onboard New Intern'. Would you like to see the details for any of them?

---

**👤 You:**
> "Create a new entry in list '98765' with name 'Finish API documentation'."

**🤖 AI Agent:**
> Successfully created the entry 'Finish API documentation' in your Zenkit list. The new entry ID is '12345'.


## Installation & Usage

To install and use the **Zenkit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenkit](https://vinkius.com/mcp/zenkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
