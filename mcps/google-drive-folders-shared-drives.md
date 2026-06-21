# Google Drive: Folders & Shared Drives MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-drive-folders-shared-drives)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Drive hierarchy — organize folders, manage Shared Drives, and create shortcuts via AI.

## Description
Connect your **Google Drive** account to your AI agent and specialize in advanced folder management and organizational structures. Use natural language to coordinate Shared Drives (formerly Team Drives), maintain folder hierarchies, and manage shortcuts across your entire corporate storage.

### What you can do

- **Folder Organization** — Create deep folder structures and move files or folders between parents instantly
- **Shared Drive Management** — List and inspect all accessible Shared Drives to manage collaborative workspaces
- **Shortcut Creation** — Create shortcuts to critical documents within relevant project folders for easy access
- **Bulk Permissions** — Share entire folders with users or groups and audit existing access levels efficiently
- **Storage Insights** — Retrieve high-level quota and storage information to keep your organizational drive clean

### How it works

1. Subscribe to this server
2. Enter your Google OAuth Client ID and Secret
3. Complete the secure Google authorization flow
4. Start organizing your shared workspaces from Claude, Cursor, or any MCP-compatible client

This version is optimized for administrative organizational tasks and large-scale folder management. Your AI agent acts as your workspace architect.

### Who is this for?

- **IT Administrators** — manage Shared Drive structures and audit large-scale folder permissions via natural language
- **Operations Managers** — organize project hierarchies and ensure all team members have access to the correct folders
- **Workspace Architects** — maintain clean organizational structures and create intuitive shortcut paths across the company drive


## Available Tools
- **add_folder_permission**: Share a folder with a user or group
- **create_folder**: Create a new folder
- **create_shortcut**: Create a shortcut to a file or folder
- **get_drive_about**: Get Drive storage and quota info
- **get_folder_metadata**: Get detailed metadata for a folder
- **list_folder_contents**: List files and subfolders within a specific folder
- **list_shared_drives**: List accessible Shared Drives
- **list_shortcuts**: List all shortcuts within a folder
- **list_team_drives**: List legacy Team Drives
- **move_file_to_folder**: Move a file or folder to a different parent folder
- **remove_folder_permission**: Remove a specific permission from a folder
- **search_folders**: Search for folders by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Drive: Folders & Shared Drives** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all subfolders inside the 'Marketing 2024' folder."

**🤖 AI Agent:**
> Inspecting folder hierarchy... Inside 'Marketing 2024', I found 5 subfolders: 'Q1_Campaigns', 'Q2_Strategy', 'Brand_Assets', 'Social_Media_Backlog', and 'Archives'. Would you like the contents of 'Brand_Assets'?

---

**👤 You:**
> "Move the file 'Final_Report.pdf' to the 'Approved_Exports' folder."

**🤖 AI Agent:**
> Moving file... I've successfully transferred 'Final_Report.pdf' (ID: 839201) to the 'Approved_Exports' folder (ID: 93021). The file is no longer in its previous location.

---

**👤 You:**
> "Create a shortcut to 'Price_List_Global' in the 'Sales_Team_Quick_Access' folder."

**🤖 AI Agent:**
> Creating shortcut... Success! I've created a shortcut named 'Link to Price List' in the 'Sales_Team_Quick_Access' folder, pointing to the original 'Price_List_Global' document.


## ❓ FAQ

**Q: What is the difference between this and the regular Google Drive server?**
This version is specialized for folder management, hierarchical organization, and Shared Drives. It includes specific tools for moving files between folders, managing Shared Drive memberships, and creating shortcuts to maintain a clean workspace.

**Q: Can I move an entire folder structure to a Shared Drive?**
Yes! You can use the `move_file_to_folder` tool (which also works for folders) to transfer a root folder into a Shared Drive ID. The AI agent will handle the parent reassignment via the API.

**Q: How do I create a shortcut to a document in another folder?**
Use the `create_shortcut` tool. Provide the name for the shortcut, the ID of the target document, and the ID of the folder where you want the shortcut to appear.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-drive-folders-shared-drives](https://vinkius.com/mcp/google-drive-folders-shared-drives)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Drive: Folders & Shared Drives** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-drive-folders-shared-drives` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Drive: Folders & Shared Drives** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-drive-folders-shared-drives": {
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
