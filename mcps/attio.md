# Attio MCP Server

Manage your CRM data with Attio — track objects, records, and relationships via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/attio)

## Overview
**Category:** sales-automation
**Tools Count:** 9

## Description
The **Attio MCP Server** brings powerful CRM capabilities directly to your AI agent. Seamlessly manage your relationship data, from standard objects like People and Companies to custom entities and complex record attributes using simple natural language.

### Key Features

- **Object Oversight** — List all data objects (tables) in your workspace and retrieve detailed metadata for any specific entity.
- **Record Management** — Query, create, and update records for any object, including people, companies, and deals.
- **Smart Assert (Upsert)** — Use the `assert_record` tool to automatically create or update records based on unique matching attributes (e.g., email).
- **Attribute Intelligence** — Access available fields (attributes) for any object to understand your data structure.
- **Global Search** — Perform fuzzy searches across multiple objects simultaneously to find relevant records instantly.
- **Secure API Integration** — Uses secure Bearer Token authentication with your Attio Personal Access Token (PAT).

### Who is this for?

- **Sales Teams** — Quickly search for prospect details and update deal statuses during conversations.
- **Account Managers** — Retrieve company information and relationship history without manual dashboard navigation.
- **Growth Marketers** — Programmatically assert records from new leads and enrich CRM data using AI-assisted tools.


## Available Tools
- **assert_record**: Upsert a record (update if exists, create otherwise)
- **create_record**: Create a new record in an object
- **get_account_check**: Verify Attio account connection
- **get_object**: Get metadata for a specific object
- **get_record**: Retrieve a specific record by ID
- **list_attributes**: List all attributes (columns) for a specific object
- **list_objects**: List all objects (tables) in the Attio workspace
- **query_records**: Query and filter records for a specific object
- **search_records**: Global fuzzy search across all objects (Beta)


## Installation & Usage

To install and use the **Attio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/attio](https://vinkius.com/mcp/attio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
