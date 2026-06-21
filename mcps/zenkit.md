# Zenkit MCP Server

Manage workspaces, lists, and entries via the Zenkit API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zenkit)

## Overview
**Category:** productivity
**Tools Count:** 8

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


## Installation & Usage

To install and use the **Zenkit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenkit](https://vinkius.com/mcp/zenkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
