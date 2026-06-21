# Zoho WorkDrive MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-workdrive)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoho-workdrive-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoho-workdrive-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage files, folders, and team workspaces via Zoho WorkDrive directly from your AI agent.

## Description
Integrate your **Zoho WorkDrive** cloud storage into your AI workflows to streamline file management and team collaboration through natural conversation.

### What you can do

- **File & Folder Operations** — List, rename, and delete files or folders across your storage with simple commands.
- **Team Collaboration** — Access team folders (workspaces) and manage user permissions programmatically.
- **External Sharing** — Generate and track external share links for secure file distribution to clients or partners.
- **User Insights** — Retrieve profile details and monitor recently accessed or modified files to stay on top of team activity.

### How it works

1. Subscribe to this server
2. Enter your Zoho API Console Client ID and Client Secret
3. Connect your account via OAuth 2.0 flow
4. Start managing your cloud storage from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Teams** — organize project documents and manage shared workspaces through natural language without leaving the chat.
- **Content Managers** — quickly rename, move, or share assets across folders to maintain a clean digital workspace.
- **Business Administrators** — monitor team activity, manage file permissions, and ensure document security efficiently.


## Available Tools
- **create_folder**: Create a new folder
- **create_share_link**: Create a new share link
- **delete_file**: Delete a file or folder
- **get_file_metadata**: Get file or folder metadata
- **get_my_profile**: Get current user profile
- **list_files**: List files and folders
- **list_file_permissions**: List file permissions
- **list_recent_files**: List recently accessed files
- **list_share_links**: List external share links
- **list_team_folders**: List team folders (workspaces)
- **list_teams**: List all teams
- **rename_file**: Rename a file or folder


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho WorkDrive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new folder named 'Q4 Marketing Assets' inside the root directory and list the contents to confirm it was created."

**🤖 AI Agent:**
> I have successfully created the 'Q4 Marketing Assets' folder in your root directory. The directory now contains 4 items, including your new folder, 'Sales Reports', and 'Team Guidelines.pdf'.

---

**👤 You:**
> "Generate a new external share link for the 'Client Proposal v2.pdf' file so I can send it to the external vendor."

**🤖 AI Agent:**
> I have created a new public share link for 'Client Proposal v2.pdf' named 'Vendor Access'. You can copy the URL here: [Link]. The file now has 2 active external share links.

---

**👤 You:**
> "Show me the workspaces for the 'Engineering Team' and check who has access permissions to the 'Architecture Specs' folder."

**🤖 AI Agent:**
> I've retrieved the workspaces for the Engineering Team. For the 'Architecture Specs' folder, there are 3 users with access: Sarah (Admin), John (Editor), and the 'Guest Contractors' group (Viewer). Would you like to modify any of these permissions?


## Installation & Usage

To install and use the **Zoho WorkDrive** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-workdrive](https://vinkius.com/mcp/zoho-workdrive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
