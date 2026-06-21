# Box MCP Server

Store, share, and collaborate on files securely with enterprise-grade cloud content management and governance controls.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/box-alternative)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **Box** account to any AI agent and take full control of your cloud content management and enterprise collaboration workflows through natural conversation.

### What you can do

- **Folder Orchestration** — Navigate through your entire Box directory structure programmatically, listing folder items and retrieving high-fidelity metadata in real-time
- **File Lifecycle Management** — Access detailed information about individual files, including version history, size, and high-fidelity descriptions directly through your agent
- **Collaboration Intelligence** — Programmatically manage folder collaborations by inviting team members with specific roles (editor, viewer) to ensure perfectly coordinated access
- **Search & Discovery** — Use semantic keywords to search for specific files and folders across your entire Box account to maintain a perfectly coordinated digital library
- **User Visibility** — Retrieve complete profile information for the authenticated user and manage account-level metadata for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Developer Token** (for testing) or **Access Token** (OAuth) from the Box Developer Console
3. Start managing your enterprise content from Claude, Cursor, or any MCP client

No more manual searching through browser tabs to find specific documents or check permissions. Your AI acts as your dedicated cloud content manager and digital librarian.

### Who is this for?

- **Project Managers** — instantly retrieve project files and manage team access using natural language commands
- **Knowledge Workers** — verify document versions and search for internal resources without leaving your workspace
- **IT & Admin Leads** — automate organizational file auditing and collaboration oversight through simple AI queries


## Available Tools
- **create_collaboration**: Requires the folder ID, the user's email (login), and an assigned role (e.g., "editor", "viewer", "previewer").

Share a folder with a collaborator
- **create_folder**: Use parent ID "0" for the root folder.

Create a new folder in Box
- **get_current_user**: Use this to verify the current identity.

Retrieve current Box user details
- **delete_file**: Delete a file from Box
- **delete_folder**: If the folder is not empty, you must set the recursive flag to true to delete all its contents.

Delete a folder from Box
- **get_file_info**: Includes size, SHA1 hash, version information, and parent folder details.

Get details and metadata for a file
- **get_folder_info**: Includes information about the parent folder, creator, and modified dates.

Get details and metadata for a folder
- **list_folder_items**: Note: Use ID "0" for the root folder.

List all items within a folder
- **search_content**: Useful for discovering items when the IDs are unknown.

Search for files and folders
- **update_file**: Can be used to rename the file or update its description.

Update file attributes and metadata


## Installation & Usage

To install and use the **Box** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/box-alternative](https://vinkius.com/mcp/box-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
