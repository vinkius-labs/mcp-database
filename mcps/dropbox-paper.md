# Dropbox Paper MCP Server

Manage collaborative docs via Dropbox Paper — create documents, search content, handle shared links, and move files directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dropbox-paper)

## Overview
**Category:** collaboration
**Tools Count:** 12

## Description
Connect your **Dropbox Paper** account to any AI agent and take full control of your collaborative document creation and file organization through natural conversation.

### What you can do

- **Live Document Creation** — Create brand-new Dropbox Paper documents by parsing literal markdown boundaries directly into rendered `.paper` artifacts
- **Content Discovery** — Execute deep full-text indexing queries to search across all your Paper documents and retrieve content snippets natively
- **Directory Orchestration** — List all files and Paper documents in any specified Dropbox folder path to browse and discover your workspace
- **Metadata Auditing** — Retrieve detailed metadata for specific documents, extracting exact structural limits mapping hashes and file IDs directly
- **Atomic File Operations** — Move, rename, or permanently delete Paper documents and files by transmitting logical atomic routing operations
- **Shared Workspace Control** — List all folders shared with or by you, and manage exposed public or restricted routes for specific documents securely
- **Storage Monitoring** — Check current storage space usage and quotas to ensure physical volume safety across your account
- **Account Oversight** — Retrieve the authenticated profile identity bindings to verify permission limits and account contexts natively

### How it works

1. Subscribe to this server
2. Enter your Dropbox Generated Access Token (found in your Dropbox App Console > Settings > OAuth 2)
3. Start managing your collaborative docs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Writers** — create and organize Paper docs using natural language without opening the web interface
- **Project Teams** — search for project documentation and manage shared folder permissions through natural conversation
- **Product Managers** — audit document metadata and track team contributions using natural language
- **Developers** — test and debug collaborative document integrations and verify markdown rendering logic in real-time


## Available Tools
- **list_files**: Use to browse and discover documents.

List all files and Paper documents in a specified Dropbox folder path
- **list_files_continue**: Continue paginating through a large folder listing
- **search_files**: paper` file extensions mapping structural relevance.

Full-text search across all Dropbox Paper documents (*.paper files)
- **get_metadata**: Retrieve detailed metadata for a specific file or Paper document
- **create_document**: paper` artifact.

Create a brand-new Dropbox Paper document with Markdown content
- **move_file**: Move or rename a file/Paper document
- **delete_file**: Permanently delete a file or Paper document
- **create_folder**: Create a new folder at the specified Dropbox path
- **get_account**: Retrieve the authenticated Dropbox account profile
- **get_space_usage**: Check current Dropbox storage space usage and quota
- **list_shared_folders**: List all folders shared with or by the authenticated user
- **list_shared_links**: List all shared links created for files or folders


## Installation & Usage

To install and use the **Dropbox Paper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dropbox-paper](https://vinkius.com/mcp/dropbox-paper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
