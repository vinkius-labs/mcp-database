# Box MCP Server

Manage files, folders, collaborations, and metadata on Box — the enterprise cloud content management platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/box)

## Overview
**Category:** industry-titans
**Tools Count:** 7

## Description
Connect your **Box** enterprise account to any AI agent and manage cloud content through natural conversation.

### What you can do

- **Files** — Upload, download, search, and manage file metadata and permissions
- **Folders** — Navigate, create, and list folder contents with recursive traversal
- **Search** — Full-text search across all content with metadata filters
- **Collaborations** — Manage shared access, invitations, and permission levels
- **Metadata** — Apply and query custom metadata templates on files and folders
- **Users** — List enterprise users and manage group memberships

### Who is this for?

- **Operations** — organize and search enterprise documents through chat
- **Legal & Compliance** — query files with retention policies and metadata
- **IT Admins** — manage user access and collaboration permissions
- **Knowledge Workers** — find and share content without navigating the Box UI


## Available Tools
- **list_folder_items**: Use folder ID "0" for the root. Returns names, sizes, types, and modified dates.

List items in a Box folder
- **get_folder_info**: Get folder details
- **create_folder**: Default parent is root (ID "0").

Create a new folder
- **get_file_info**: Get file details
- **search_content**: Filter by file extensions (pdf,docx,xlsx) or ancestor folder. Searches inside documents.

Search files and folders
- **get_folder_collaborations**: List collaborators on a folder
- **list_users**: List enterprise users


## Installation & Usage

To install and use the **Box** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/box](https://vinkius.com/mcp/box)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
