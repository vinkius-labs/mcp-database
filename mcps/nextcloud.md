# Nextcloud MCP Server

Manage your Nextcloud instance — handle files, shares, user statuses, and server capabilities directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nextcloud)

## Overview
**Category:** productivity
**Tools Count:** 16

## Description
Connect your **Nextcloud** instance to any AI agent and take full control of your self-hosted productivity suite through natural conversation.

### What you can do

- **File & Folder Management** — List, create, and delete files or folders within your Nextcloud storage directly from the chat.
- **Advanced Sharing** — Create and manage shares for users, groups, or public links with custom permissions and passwords.
- **User & Admin Tools** — List users (admin only), fetch detailed user profiles, and inspect server capabilities and enabled apps.
- **Presence & Status** — Get or set your online status and custom status messages with emojis to keep your team informed.
- **Activity Tracking** — Monitor recent activities and changes within your Nextcloud environment.

### How it works

1. Subscribe to this server
2. Enter your Nextcloud URL, Username, and App Password
3. Start managing your cloud storage and collaboration tools from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Self-Hosters** — Manage your personal cloud infrastructure without leaving your AI workspace.
- **Teams & Organizations** — Quickly share documents and update statuses during collaborative sessions.
- **Developers** — Inspect server capabilities and manage app passwords directly from your coding environment.


## Available Tools
- **get_capabilities**: Get Nextcloud server capabilities
- **create_folder**: Create a new folder in Nextcloud (WebDAV)
- **create_share**: Share Types: 0=User, 1=Group, 3=Public Link, 4=Email, 6=Federated, 7=Circle, 10=Talk.

Create a new Nextcloud share
- **delete_app_password**: Delete the current app password
- **delete_file**: Delete a file or folder in Nextcloud (WebDAV)
- **delete_share**: Delete a Nextcloud share
- **get_app_password**: Requires authenticating with the real user password.

Generate a new app password
- **get_user_status**: Get current user status
- **get_user**: Get details for a specific Nextcloud user
- **list_activities**: List Nextcloud activity stream
- **list_files**: Path is relative to the user root.

List files in a Nextcloud directory (WebDAV)
- **list_shares**: List all Nextcloud shares
- **list_users**: Requires admin privileges.

List Nextcloud users (Admin only)
- **set_user_status_message**: Set custom user status message
- **set_user_status**: Set user online status
- **update_share**: Update an existing Nextcloud share


## Installation & Usage

To install and use the **Nextcloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nextcloud](https://vinkius.com/mcp/nextcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
