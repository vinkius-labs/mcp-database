# Box MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/box)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage files, folders, collaborations, and metadata on Box — the enterprise cloud content management platform.

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


## Available Tools (7)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Box** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all contracts expiring in Q2 2026."

**🤖 AI Agent:**
> Found 14 files matching 'contract': 1. 'MSA-ClientAlpha-2024.pdf' (Legal/Contracts, 2.3 MB, metadata: expires=2026-06-30). 2. 'SaaS-License-BetaCorp.docx' (Procurement, 890 KB, expires=2026-04-15). Showing top 5 of 14.

---

**👤 You:**
> "Who has access to the Board Reports folder?"

**🤖 AI Agent:**
> 'Board Reports' folder collaborators: 1. CEO Jane Smith (Co-owner). 2. CFO Mike Chen (Editor). 3. Legal Team (Viewer, 5 members). 4. External Auditor Group (Viewer, 2 members, link expires Dec 2026). Total: 10 unique users.

---

**👤 You:**
> "List the 10 largest files in the Engineering folder."

**🤖 AI Agent:**
> Top 10 files by size in 'Engineering': 1. 'architecture-diagram-v12.fig' (245 MB). 2. 'load-test-results-march.zip' (189 MB). 3. 'database-backup-staging.sql' (156 MB). Total folder size: 2.1 GB across 847 files.


## ❓ FAQ

**Q: What authentication does Box use?**
Box supports Client Credentials Grant (CCG) for server-to-server auth. Create a Custom App in the Box Developer Console, select 'Server Authentication (Client Credentials Grant)', and get the Client ID and Client Secret.

**Q: Can I search file contents?**
Yes. The search_content tool uses Box's full-text search engine. It searches inside documents, presentations, spreadsheets, and PDFs.

**Q: Does it support metadata queries?**
Yes. The query_metadata tool supports Box metadata queries using SQL-like syntax against metadata templates applied to files and folders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/box](https://vinkius.com/mcp/box)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Box** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `box` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Box** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "box": {
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
