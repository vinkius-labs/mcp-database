# Memo Meister MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/memo-meister)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Create and organize smart notes with AI-powered tagging, search, and knowledge connections that make your ideas retrievable.

## Description
Connect your **Memo Meister** account to any AI agent and manage field documentation and project files through natural conversation.

### What you can do

- **Project Management** — Create and manage project folders and workspaces
- **Memo Management** — Create, read, and organize documentation memos
- **File Handling** — Access images, PDFs, and field reports attached to memos
- **Task Tracking** — Monitor task statuses and comments within projects
- **Search** — Query projects and memos using GraphQL

### How it works

1. Subscribe to this server
2. Enter your Memo Meister API Key
3. Start managing field documentation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Construction & Trades** — document field work with photos and memos
- **Project Managers** — track progress and centralize project files
- **Field Service** — automate report generation and file organization


## Available Tools (11)
- **get_memo**: Get details of a specific memo
- **get_project**: Get details of a specific project
- **list_memo_comments**: List comments on a memo
- **list_memo_files**: List files attached to a memo
- **list_memos**: List memos (notes) in a project
- **list_projects**: List all projects (memosets) in MemoMeister
- **update_memo**: Update an existing memo
- **add_memo_comment**: Add a comment to a memo
- **create_memo**: Create a new memo in a project
- **delete_memo**: Delete a memo
- **get_me**: Get information about the current authenticated user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Memo Meister** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show recent memos in the 'Downtown Office Build' project."

**🤖 AI Agent:**
> Project 'Downtown Office Build': 3 recent memos. 1) 'HVAC Installation Update' (By Mike, Today 10:00 AM). 2) 'Safety Inspection Report' (By Sarah, Yesterday. 1 PDF attached). 3) 'Material Delivery Photos' (By John, Monday. 4 Images attached).

---

**👤 You:**
> "Create a new memo for the daily site report."

**🤖 AI Agent:**
> Memo created! ✅ Title: 'Daily Site Report - Apr 26'. Project: 'Downtown Office Build'. Content: 'Foundation pouring completed. Weather clear. No safety incidents.'. Tags: [daily-report, foundation, safety]. ID: memo_8901.

---

**👤 You:**
> "List all open tasks assigned to me across projects."

**🤖 AI Agent:**
> Open tasks (Assigned to you): 4. 1) 'Review Electrical Plan' (Project A, Due: Tomorrow). 2) 'Approve Material Invoice' (Project B, Due: Friday). 3) 'Schedule Crane Delivery' (Project A, Overdue ⚠️). 4) 'Sign off on Safety Audit' (Project C).


## ❓ FAQ

**Q: Can I read and create project memos?**
Yes. Create text memos, attach files, and organize them within specific project folders.

**Q: What API does Memo Meister use?**
Memo Meister uses a custom API Key header against a GraphQL endpoint at `api.memomeister.com/graphql`.

**Q: Can I search for specific field reports?**
Yes. Query the GraphQL API to search memos by tags, content, or project assignment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/memo-meister](https://vinkius.com/mcp/memo-meister)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Memo Meister** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `memo-meister` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Memo Meister** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "memo-meister": {
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
