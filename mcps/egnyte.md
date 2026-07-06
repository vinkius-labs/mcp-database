# Egnyte MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/egnyte)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Store and govern enterprise content with intelligent file management, access controls, and compliance monitoring across teams.

## Description
Connect your **Egnyte** enterprise account to any AI agent and take full control of your corporate file sync and share (EFSS) workflows through natural conversation.

### What you can do

- **Content Orchestration** — List and manage files and folders programmatically, including creating new directories and retrieving detailed metadata
- **Secure Sharing** — Programmatically generate shared links with customizable accessibility (public, password, domain) directly from your agent
- **Deep Semantic Search** — Find relevant files and folders across your entire domain using advanced text queries and filters
- **User & Group Visibility** — Retrieve complete directories of users and groups to coordinate permissions and team collaboration
- **Compliance Monitoring** — Access security audit logs and monitor active webhooks to maintain high-fidelity oversight of your corporate data

### How it works

1. Subscribe to this server
2. Register an Internal Application in your Egnyte Developer Portal
3. Retrieve your **Access Token** and **Domain** (e.g., 'acme' from acme.egnyte.com)
4. Start managing your enterprise content from Claude, Cursor, or any MCP client

No more manual folder navigation or complex permission setting in the web UI. Your AI acts as your dedicated IT and content operations coordinator.

### Who is this for?

- **IT Administrators** — instantly retrieve audit logs and manage user groups using natural language commands
- **Operations Leads** — automate folder structures for new projects and monitor shared link usage without leaving your workspace
- **Compliance Officers** — search for sensitive documents and verify access levels through simple AI queries


## Available Tools (12)
- **list_folder**: List folder contents
- **list_groups**: List user groups
- **list_shared_links**: List all shared links
- **list_users**: List Egnyte users
- **list_webhooks**: List active webhooks
- **search_files**: Search for files
- **create_folder**: Create a new folder
- **create_shared_link**: Generate share link
- **delete_item**: Delete file or folder
- **get_account_info**: Get domain info
- **get_audit_logs**: List audit events
- **get_file_metadata**: Get file details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Egnyte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files in the folder '/Shared/Projects/MCP'."

**🤖 AI Agent:**
> I've retrieved the contents of '/Shared/Projects/MCP'. I found 3 files and 2 subfolders, including 'spec_v1.pdf' and 'assets/'. Would you like the metadata for any of these items?

---

**👤 You:**
> "Search for documents containing '2026 marketing budget'."

**🤖 AI Agent:**
> Searching domain... I've found 2 documents: 'Marketing_Budget_v2.xlsx' in /Shared/Finance and 'Q1_Strategy.docx'. Both mention your query. Shall I provide the share links for them?

---

**👤 You:**
> "Show me the last 5 security audit logs."

**🤖 AI Agent:**
> Fetching audit logs... The last 5 events include a password change for user 'John', two folder deletions in /Private, and two successful admin logins. Would you like the detailed timestamps for these?


## ❓ FAQ

**Q: How do I find my Egnyte domain?**
The domain is the first part of your URL. For example, if you access Egnyte at `acme.egnyte.com`, your domain is `acme`.

**Q: Can I search for files by content?**
Yes! The `search_files` tool performs a full-text search across your Egnyte domain to find relevant documents and folders.

**Q: How do I generate a shared link via AI?**
Use the `create_shared_link` tool and provide the full path to the item. You can also specify access levels like 'public' or 'domain'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/egnyte](https://vinkius.com/mcp/egnyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Egnyte** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `egnyte` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Egnyte** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "egnyte": {
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
