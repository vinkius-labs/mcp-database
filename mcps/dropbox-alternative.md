# DropBox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dropbox-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your DropBox files and folders — audit storage and sharing via AI.

## Description
Empower your AI agent to orchestrate your entire cloud storage ecosystem with **DropBox**, the world's leading file hosting service. By connecting DropBox to your agent, you transform complex file management into a natural conversation. Your agent can instantly list folder contents, audit file metadata, and search across your entire account without you ever touching a dashboard. Whether you are organizing team assets or managing personal backups, your agent acts as a real-time file operator, ensuring your data is always accessible and well-structured.

### What you can do

- **Folder Auditing** — List all files and folders in any directory and retrieve detailed metadata, including sizes and paths.
- **File Lifecycle** — Create folders, move, copy, and delete items through natural language to keep your storage organized.
- **Powerful Search** — Query your entire DropBox account for specific files or folders using real-time search indexing.
- **Sharing Governance** — List existing shared links and autonomously create new ones to facilitate collaboration.
- **Account Auditing** — Quickly retrieve account details and usage info to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your DropBox Access Token
3. Start managing your files through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Asset Managers** — monitor project folders and update file structures straight from your workflow.
- **Operations Leads** — verify if team documents are being correctly uploaded and shared in specific directories.
- **Content Creators** — perform rapid audits of media libraries and generate shared links without manual logins.
- **Business Owners** — automate storage querying to orchestrate your data-driven growth smoothly.


## Available Tools
- **copy_item**: Copy a file or folder
- **create_folder**: Create a new folder in DropBox
- **create_shared_link**: Create a shared link for a path
- **delete_item**: Delete a file or folder
- **get_current_user**: Get current DropBox account details
- **get_metadata**: Get metadata for a file or folder
- **list_folder**: Use an empty string for the root.

List contents of a DropBox folder
- **list_shared_links**: List shared links
- **move_item**: Move a file or folder
- **search_files**: Search for files or folders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DropBox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the files in my root DropBox folder."

**🤖 AI Agent:**
> I've retrieved your root directory. You have 10 items, including folders like 'Photos' and 'Documents', and 3 files. Which directory would you like to explore next?

---

**👤 You:**
> "Search for a file named 'Project Specs'."

**🤖 AI Agent:**
> I've found 2 matches for 'Project Specs'. One is in '/Work/2024/' and another in '/Archive/'. Would you like the full metadata for either of them?

---

**👤 You:**
> "Create a shared link for '/Public/Presentation.pdf'."

**🤖 AI Agent:**
> Shared link generated! You can access the presentation at https://www.dropbox.com/s/xxxxxxxx. The link is currently set to public access.


## ❓ FAQ

**Q: How do I find my DropBox Access Token?**
Create a new app in the [**DropBox App Console**](https://www.dropbox.com/developers/apps) and click 'Generate' under the 'Generated access token' section. Copy and paste it below.

**Q: Can the agent search for specific files?**
Yes. Use the `search_files` tool providing a query string. Your agent will return all matching files and folders from your entire account instantly.

**Q: Is it possible to generate a shared link via the agent?**
Yes. The `create_shared_link` tool allows your agent to generate a public URL for any file or folder by providing its path.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dropbox-alternative](https://vinkius.com/mcp/dropbox-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DropBox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dropbox-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DropBox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dropbox-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
