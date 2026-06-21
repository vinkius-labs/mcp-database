# Google Drive MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-drive)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your files — search, create, share, and organize your Google Drive via AI.

## Description
Connect your **Google Drive** to your AI agent and transform how you interact with your cloud storage. Use natural language to find documents, manage sharing permissions, organize folders, and audit your file history across your entire drive.

### What you can do

- **Deep Search** — Find files instantly using natural language queries (e.g., 'Find all PDFs from last week')
- **File & Folder Management** — Create, update, copy, and delete files or folders directly through the chat
- **Sharing & Permissions** — Audit who has access to your sensitive documents and add or remove permissions securely
- **Content Conversion** — Export Google Docs, Sheets, and Slides to formats like PDF or CSV with simple commands
- **Version Control** — List file revisions to track changes and see the evolution of your documents over time

### How it works

1. Subscribe to this server
2. Enter your Google OAuth Client ID and Secret
3. Complete the secure Google authorization flow
4. Start managing your files from Claude, Cursor, or any MCP-compatible client

Stop digging through nested folders. Your AI agent acts as your personal file librarian, keeping your cloud storage clean and accessible.

### Who is this for?

- **Productivity Experts** — organize messy drives and find misplaced documents using conversational search
- **Project Managers** — share project folders with new team members and audit document access levels efficiently
- **Content Teams** — manage document lifecycles and export files to different formats for external distribution


## Available Tools (15)
- **copy_file**: Create a copy of a file
- **update_file**: Update file metadata or content
- **create_file_comment**: Add a comment to a file
- **list_file_comments**: List all comments on a file
- **create_file**: Create a new file (metadata only, or folder)
- **create_permission**: Share a file with an email or group
- **delete_file**: Move a file to trash
- **empty_trash**: Permanently delete all files in the trash
- **export_file**: Export a Google Doc/Sheet to a specific format (e.g. application/pdf)
- **get_drive_about**: Get info about the user Drive (quota, usage)
- **get_file_metadata**: Get detailed info for a specific file
- **list_files**: List or search for files in Google Drive
- **list_permissions**: Check who has access to a file
- **list_revisions**: View file history/revisions
- **search_files**: g. "name contains 'report' and mimeType='application/pdf'"

Search for files using Google Drive query syntax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Drive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all spreadsheets I created in the last 30 days."

**🤖 AI Agent:**
> Searching files... I found 4 spreadsheets created last month: 'Budget_Q2.xlsx', 'User_Feedback_Raw', 'Inventory_April', and 'Campaign_Results'. Would you like the metadata for any of these?

---

**👤 You:**
> "Who has access to the file 'Confidential_Roadmap'?"

**🤖 AI Agent:**
> Checking permissions... The file 'Confidential_Roadmap' is shared with 3 people: Marcus R. (Owner), Sarah P. (Editor), and Mike T. (Viewer). It is NOT shared publicly.

---

**👤 You:**
> "Create a new folder named 'Project Apollo Assets'."

**🤖 AI Agent:**
> Creating folder... Success! I've created the folder 'Project Apollo Assets' in your root directory. The folder ID is FOLDER-93021.


## ❓ FAQ

**Q: Can I search for files by their content, not just their name?**
Yes! The `list_files` tool uses Google Drive's powerful search engine. You can use queries like 'fullText contains "marketing plan"' to find files based on the text inside them.

**Q: How do I share a file with someone using the AI agent?**
Use the `create_permission` tool. You just need to provide the File ID, the person's email address, and the role you want to grant (e.g., 'reader', 'commenter', or 'writer').

**Q: Can I export a Google Sheet to a PDF through the chat?**
Yes. The `export_file` tool allows you to specify a Google Doc/Sheet/Slide ID and a target MIME type like `application/pdf`. The agent will initiate the export for you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-drive](https://vinkius.com/mcp/google-drive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Drive** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-drive` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Drive** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-drive": {
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
