# Dropbox MCP Server

Manage cloud storage via Dropbox — list folders, search files, handle shared links, and monitor space usage directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dropbox)

## Overview
**Category:** industry-titans
**Tools Count:** 12

## Description
Connect your **Dropbox** account to any AI agent and take full control of your cloud storage and file management through natural conversation.

### What you can do

- **Directory Orchestration** — Iterate through explicitly nested directory items mapping native paths and analyzing contents returning names, tags, and server-modified times
- **Metadata Inspection** — Fetch absolute precise metadata bindings for exact native objects isolating unique IDs, hashes, and byte sizes natively
- **File Discovery** — Execute structural query matches leveraging V2 search boundaries to find files by name securely against indexed representations
- **Shared Link Management** — Extract exposed URLs explicitly tracking active public or restricted boundaries granting file downloads over sharing APIs
- **Shared Folder Auditing** — Isolate specifically nested directories governed under explicit organizational or cross-tenant permissions mapped internally
- **Space & Usage Monitoring** — Validate physical allocation blocks returning byte usage (used vs total) bounding physical server storage capacity
- **Namespace Management** — Reveal inbound shared spaces unmounted preventing synchronization and retrieve unmounted namespace IDs securely
- **Account Oversight** — Interrogate underlying tokens resolving precise user contexts including name, email, and account type bound natively

### How it works

1. Subscribe to this server
2. Enter your Dropbox Generated Access Token (found in your Dropbox App Console > Settings > OAuth 2)
3. Start managing your files from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — search for documents and manage shared links without leaving the chat interface
- **Developers** — test and debug file storage integrations and verify metadata schemas through natural conversation
- **Project Managers** — audit shared folders and monitor team storage usage using natural language
- **Ops Teams** — verify account details and manage unmounted shared spaces in real-time


## Available Tools
- **get_space_usage**: Get storage space usage
- **get_metadata**: Get file/folder metadata
- **list_folder**: Analyzes contents returning names, tags (`folder`/`file`), sizes, and server-modified times.

List files and folders in a directory
- **search_files**: Search files by name
- **list_shared_links**: List all shared links
- **list_shared_folders**: List all shared folders
- **get_account**: Get current account info
- **list_mountable_folders**: List mountable shared folders
- **create_folder**: Use full path like /my-project/assets.

Create a new folder in Dropbox
- **move_file**: Can be used for renaming.

Move or rename a file/folder
- **copy_file**: Copy a file or folder
- **create_shared_link**: Create a public shared link for a file or folder


## Installation & Usage

To install and use the **Dropbox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dropbox](https://vinkius.com/mcp/dropbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
