# Dropbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dropbox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage cloud storage via Dropbox — list folders, search files, handle shared links, and monitor space usage directly from any AI agent.

## Description
Connect your **Dropbox** account to any AI agent and take full control of your cloud storage and file management through natural conversation.

### What you can do

- **Directory Orchestration** — Iterate through explicitly nested directory items mapping native paths and analyzing contents returning names, tags, and server-modified times
- **Metadata Inspection** — Fetch absolute precise metadata bindings for exact native objects isolating unique IDs, hashes, and byte sizes natively
- **File Discovery** — Execute structural query matches leveraging V2 search boundaries to find files by name securely against indexed representations
- **Shared Link Management** — Extract exposed URLs explicitly tracking active public or restricted boundaries granting file downloads over sharing APIs
- **Shared Folder Auditing** — Isolate specifically nested directories governed under explicit organizational or cross-tenant permissions mapped internally
- **Space & Usage Monitoring** — Validate physical allocation blocks returning byte usage (used vs total) bounding physical server storage capacity
- **Namespace Management** — Reveal inbound shared spaces unmounted preventing synchronization and retrieve unmounted namespace IDs securely
- **Account Oversight** — Interrogate underlying tokens resolving precise user contexts including name, email, and account type bound natively

### How it works

1. Subscribe to this server
2. Enter your Dropbox Generated Access Token (found in your Dropbox App Console > Settings > OAuth 2)
3. Start managing your files from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — search for documents and manage shared links without leaving the chat interface
- **Developers** — test and debug file storage integrations and verify metadata schemas through natural conversation
- **Project Managers** — audit shared folders and monitor team storage usage using natural language
- **Ops Teams** — verify account details and manage unmounted shared spaces in real-time


## Available Tools (12)
- **get_space_usage**: Get storage space usage
- **get_metadata**: Get file/folder metadata
- **list_folder**: Analyzes contents returning names, tags (`folder`/`file`), sizes, and server-modified times.

List files and folders in a directory
- **search_files**: Search files by name
- **list_shared_links**: List all shared links
- **list_shared_folders**: List all shared folders
- **get_account**: Get current account info
- **list_mountable_folders**: List mountable shared folders
- **create_folder**: Use full path like /my-project/assets.

Create a new folder in Dropbox
- **move_file**: Can be used for renaming.

Move or rename a file/folder
- **copy_file**: Copy a file or folder
- **create_shared_link**: Create a public shared link for a file or folder


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dropbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List files in my '/Projects/2024' folder"

**🤖 AI Agent:**
> Retrieving items from '/Projects/2024'... I found 5 files: 'Plan.pdf', 'Budget.xlsx', and 3 images. Would you like to see the metadata for the planning document?

---

**👤 You:**
> "Search for any files containing 'invoice' in their name"

**🤖 AI Agent:**
> Searching for 'invoice'... I found 3 matches: 'Invoice_Jan.pdf', 'Invoice_Feb.pdf', and 'Old_Invoices.zip'. Which one would you like more details on?

---

**👤 You:**
> "Show me my Dropbox storage usage"

**🤖 AI Agent:**
> Retrieving storage info... You are using 1.2 GB of your 2.0 GB total capacity (60% used). You have approximately 800 MB of space remaining.


## ❓ FAQ

**Q: Can my agent list files in a specific Dropbox folder?**
Yes. Use the 'list_folder' tool. Provide the folder path (use an empty string for the root). The agent will return an array of items including names, types, and modification dates.

**Q: How do I find a file by its name through natural conversation?**
Use the 'search_files' tool. Provide your query string, and the agent will execute a structural match against your indexed Dropbox files, returning the most relevant results.

**Q: Can I check how much storage space I have left via the agent?**
Absolutely. The 'get_space_usage' tool retrieves your physical allocation blocks. It will show you exactly how many bytes are used versus your total account capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dropbox](https://vinkius.com/mcp/dropbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dropbox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dropbox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dropbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dropbox": {
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
