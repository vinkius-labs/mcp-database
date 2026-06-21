# JSONBin.io MCP Server

Store, manage, and retrieve JSON data effortlessly. Create bins, manage collections, and handle large datasets directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jsonbinio)

## Overview
**Category:** developer-tools
**Tools Count:** 27

## Description
Connect **JSONBin.io** to your AI agent to turn it into a powerful data management assistant. Whether you are prototyping, storing configuration, or managing application state, this server provides full control over your cloud-based JSON storage.

### What you can do

- **Bin Management** — Create, read, update, and delete JSON bins (CRUD) with support for private or public visibility.
- **Versioning & Metadata** — Track changes with bin versioning and retrieve detailed metadata or specific versions of your records.
- **XL Bins** — Store large JSON files up to 10MB for complex datasets that exceed standard limits.
- **Collections** — Organize your bins into logical groups for better project structure and bulk management.
- **Advanced Querying** — Use JSON Path expressions to filter and retrieve only the specific data you need from a bin.

### How it works

1. Subscribe to this server
2. Enter your JSONBin.io Master Key and Access Key
3. Start storing and querying data from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — quickly store API mock data or app configurations without setting up a full database.
- **Data Analysts** — persist processed JSON results and query them using JSON Path directly from the chat.
- **Automation Engineers** — maintain state across different AI workflows and agent sessions.


## Available Tools
- **add_schema_to_collection**: Add a schema to a collection for validation
- **count_bin_versions**: Count versions of a JSON bin
- **create_access_key**: Create a restricted access key
- **create_bin**: Requires valid JSON data.

Create a new JSON bin
- **create_collection**: Create a new collection
- **create_schema**: Create a JSON schema document
- **create_xl_bin**: Requires Early Access and a paid plan.

Create an XL JSON bin (up to 10MB)
- **delete_access_key**: Delete an access key
- **delete_all_bin_versions**: Delete all versions of a JSON bin
- **delete_bin**: Delete a JSON bin
- **delete_xl_bin**: Delete an XL JSON bin
- **download_usage_logs**: Download usage logs for a specific date
- **fetch_collection_bins**: Fetch bins within a collection
- **fetch_uncategorized_bins**: Fetch all uncategorized bins
- **list_access_keys**: List all access keys
- **list_collections**: List all collections
- **list_usage_log_dates**: List available dates for usage logs
- **read_bin**: Can optionally fetch a specific version or filter via JSON Path.

Read a JSON bin
- **read_schema**: Read a JSON schema document
- **read_xl_bin**: Read an XL JSON bin
- **remove_schema_from_collection**: Remove a schema from a collection
- **update_bin_name**: Update the name of a JSON bin
- **update_bin_privacy**: Update the privacy setting of a JSON bin
- **update_bin**: Update an existing JSON bin
- **update_collection_name**: Update the name of a collection
- **update_schema_name**: Update the name of a JSON schema document
- **update_schema**: Update a JSON schema document


## Installation & Usage

To install and use the **JSONBin.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jsonbinio](https://vinkius.com/mcp/jsonbinio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
