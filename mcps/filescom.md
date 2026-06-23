# Files.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/filescom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Sync, share, and automate file workflows across teams with secure cloud storage that integrates with your existing tools.

## Description
Connect your **Files.com** secure storage account to any AI agent and simplify how you manage your enterprise files, coordinate folder structures, and monitor audit logs through natural conversation.

### What you can do

- **Folder Oversight** — List files and directories at any path and coordinate your organizational storage hierarchy.
- **File Intelligence** — Retrieve detailed metadata and direct download links for specific files using their unique paths.
- **Access Control** — List account users, groups, and detailed permissions to ensure your data security is ready.
- **Audit Monitoring** — Query real-time and historical activity logs to track file uploads, downloads, and deletions.
- **Operational Utility** — Create new folders and remove outdated assets programmatically via simple AI commands.
- **Data Insights** — Fetch complete file metadata and permission distributions directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Files.com API Key and Subdomain (e.g., yourcompany.files.com)
3. Start managing your secure ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **IT Administrators** — quickly check folder permissions and verify user access via simple AI queries.
- **Operations Teams** — monitor file activity history and coordinate folder creation directly from the workspace.
- **Compliance Officers** — verify audit logs and track file lifecycle changes via the AI assistant.


## Available Tools (8)
- **create_folder**: Create a new folder
- **delete_file**: Delete a file or folder
- **get_file_details**: Get details for a specific file
- **list_folders**: List Files.com folders
- **list_user_groups**: List organizational groups
- **list_activity_history**: List file activity history
- **list_permissions**: List file permissions
- **list_users**: List Files.com users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Files.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files in the '/Client-Projects' folder."

**🤖 AI Agent:**
> I've retrieved the folder contents. Inside '/Client-Projects' you have: 'Contract_v1.pdf', 'Design_Mockup.png', and 'Project_Brief.docx'. Which one would you like more details on?

---

**👤 You:**
> "Show me the activity history for the last 24 hours."

**🤖 AI Agent:**
> Fetching audit logs... In the last 24 hours, there were 15 activities: 10 uploads, 3 downloads by Mike Ross, and 2 folder deletions. Would you like a detailed report on the deletions?

---

**👤 You:**
> "Create a new folder called '/Archive-2023'."

**🤖 AI Agent:**
> Success! The folder '/Archive-2023' has been created in your Files.com account. You can now start moving your legacy assets into this directory.


## ❓ FAQ

**Q: Can I see who downloaded a specific file via AI?**
Yes! Use the `list_activity_history` tool. Your agent will retrieve the audit logs, which you can filter to find download events for a particular file or user.

**Q: How do I create a new folder in my secure storage?**
Use the `create_folder` action. Provide the path where you want the new directory to be created (e.g., '/projects/2024') and the agent will register it in Files.com instantly.

**Q: Is it possible to list all users in my Files.com instance via AI?**
Absolutely. Use the `list_users` query. The agent will retrieve the complete directory of users configured for your company's instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/filescom](https://vinkius.com/mcp/filescom)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `filescom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Files.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "filescom": {
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
