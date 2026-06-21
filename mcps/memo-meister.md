# Memo Meister MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/memo-meister)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/memo-meister-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/memo-meister-mcp)
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


## Available Tools
- **add_memo_comment**: Add a comment to a memo
- **create_memo**: Create a new memo in a project
- **delete_memo**: Delete a memo
- **get_me**: Get information about the current authenticated user
- **get_memo**: Get details of a specific memo
- **get_project**: Get details of a specific project
- **list_memo_comments**: List comments on a memo
- **list_memo_files**: List files attached to a memo
- **list_memos**: List memos (notes) in a project
- **list_projects**: List all projects (memosets) in MemoMeister
- **update_memo**: Update an existing memo


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


## Installation & Usage

To install and use the **Memo Meister** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/memo-meister](https://vinkius.com/mcp/memo-meister)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
