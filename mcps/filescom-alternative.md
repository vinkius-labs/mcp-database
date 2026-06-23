# Files.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/filescom-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Securely manage Files.com storage, users, and permissions. List folders, move files, and automate workflows through natural language.

## Description
Connect your **Files.com** account to any AI agent to streamline enterprise file management and user administration through natural conversation.

### What you can do

- **File & Folder Control** — List directory contents, retrieve metadata, and perform file operations like move, copy, or delete.
- **User Management** — List, create, update, or delete users and manage group assignments directly.
- **Security & Permissions** — Audit folder permissions and grant access to specific users or groups programmatically.
- **Workflow Automation** — List active automations and create webhooks to integrate with your existing tech stack.

### How it works

1. Subscribe to this server
2. Enter your Files.com API Key
3. Start managing your enterprise storage from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **IT Administrators** — quickly manage user access, audit permissions, and organize directory structures without the web UI.
- **DevOps Engineers** — automate file movements and monitor webhooks/automations directly from the terminal or IDE.
- **Data Managers** — organize large datasets, move files between environments, and verify file metadata via chat.


## Available Tools (17)
- **add_user_to_group**: Add a user to a group
- **copy_file**: Copy a file or folder
- **create_group**: Create a new group
- **create_permission**: Create a new permission
- **create_user**: Create a new user
- **create_webhook**: Create a new webhook
- **delete_file**: Delete a file or folder
- **delete_permission**: Delete a permission
- **delete_user**: Delete a user
- **get_file_metadata**: Get metadata for a specific file
- **list_automations**: List all automations
- **list_folder**: List contents of a folder
- **list_groups**: List all groups
- **list_permissions**: List all permissions
- **list_users**: com site.

List all users
- **move_file**: Move a file or folder
- **update_user**: Update an existing user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Files.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files and folders inside the /marketing/2024 directory."

**🤖 AI Agent:**
> I've scanned the /marketing/2024 folder. It contains 3 subfolders (Campaigns, Assets, Reports) and 2 files: 'strategy_v1.pdf' and 'budget.xlsx'.

---

**👤 You:**
> "Create a new user with username 'dev_team_lead' and email 'lead@company.com'."

**🤖 AI Agent:**
> User 'dev_team_lead' has been successfully created with ID 88291. Would you like me to add them to any specific groups now?

---

**👤 You:**
> "Move 'invoice_99.pdf' from /uploads to /finance/invoices."

**🤖 AI Agent:**
> The file 'invoice_99.pdf' has been moved to /finance/invoices. The operation was successful.


## ❓ FAQ

**Q: Can I move or copy files between different folders using the AI?**
Yes. You can use the `move_file` and `copy_file` tools. Just provide the source path and the destination path, and the agent will handle the transfer within your Files.com site.

**Q: Is it possible to manage user permissions for specific folders?**
Absolutely. You can use `list_permissions` to audit current access and `create_permission` to grant new access levels to specific users or groups for any folder path.

**Q: Can I see a list of all active automations on my site?**
Yes, the `list_automations` tool allows your agent to retrieve all configured automations, helping you monitor scheduled tasks and sync processes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/filescom-alternative](https://vinkius.com/mcp/filescom-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Files.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `filescom-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Files.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "filescom-alternative": {
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
