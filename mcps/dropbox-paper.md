# Dropbox Paper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dropbox-paper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage collaborative docs via Dropbox Paper — create documents, search content, handle shared links, and move files directly from any AI agent.

## Description
Connect your **Dropbox Paper** account to any AI agent and take full control of your collaborative document creation and file organization through natural conversation.

### What you can do

- **Live Document Creation** — Create brand-new Dropbox Paper documents by parsing literal markdown boundaries directly into rendered `.paper` artifacts
- **Content Discovery** — Execute deep full-text indexing queries to search across all your Paper documents and retrieve content snippets natively
- **Directory Orchestration** — List all files and Paper documents in any specified Dropbox folder path to browse and discover your workspace
- **Metadata Auditing** — Retrieve detailed metadata for specific documents, extracting exact structural limits mapping hashes and file IDs directly
- **Atomic File Operations** — Move, rename, or permanently delete Paper documents and files by transmitting logical atomic routing operations
- **Shared Workspace Control** — List all folders shared with or by you, and manage exposed public or restricted routes for specific documents securely
- **Storage Monitoring** — Check current storage space usage and quotas to ensure physical volume safety across your account
- **Account Oversight** — Retrieve the authenticated profile identity bindings to verify permission limits and account contexts natively

### How it works

1. Subscribe to this server
2. Enter your Dropbox Generated Access Token (found in your Dropbox App Console > Settings > OAuth 2)
3. Start managing your collaborative docs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Writers** — create and organize Paper docs using natural language without opening the web interface
- **Project Teams** — search for project documentation and manage shared folder permissions through natural conversation
- **Product Managers** — audit document metadata and track team contributions using natural language
- **Developers** — test and debug collaborative document integrations and verify markdown rendering logic in real-time


## Available Tools
- **list_files**: Use to browse and discover documents.

List all files and Paper documents in a specified Dropbox folder path
- **list_files_continue**: Continue paginating through a large folder listing
- **search_files**: paper` file extensions mapping structural relevance.

Full-text search across all Dropbox Paper documents (*.paper files)
- **get_metadata**: Retrieve detailed metadata for a specific file or Paper document
- **create_document**: paper` artifact.

Create a brand-new Dropbox Paper document with Markdown content
- **move_file**: Move or rename a file/Paper document
- **delete_file**: Permanently delete a file or Paper document
- **create_folder**: Create a new folder at the specified Dropbox path
- **get_account**: Retrieve the authenticated Dropbox account profile
- **get_space_usage**: Check current Dropbox storage space usage and quota
- **list_shared_folders**: List all folders shared with or by the authenticated user
- **list_shared_links**: List all shared links created for files or folders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dropbox Paper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Paper doc at '/Notes/Draft.paper' with content: '# Meeting Notes\n- Item 1'"

**🤖 AI Agent:**
> Document created! I've generated '/Notes/Draft.paper' with your Markdown content. You can now access it in Dropbox Paper for further collaboration.

---

**👤 You:**
> "Search my Paper documents for 'marketing strategy'"

**🤖 AI Agent:**
> Searching Paper docs... I found 2 matches: 'Q4 Marketing Plan.paper' and 'Brand Guidelines.paper'. Would you like to see the full path or metadata for either document?

---

**👤 You:**
> "Move '/Documents/Old_Report.paper' to '/Archive/2023/'"

**🤖 AI Agent:**
> File moved successfully! '/Documents/Old_Report.paper' is now located at '/Archive/2023/Old_Report.paper'. The document's ID and sharing links remain unchanged.


## ❓ FAQ

**Q: Can my agent create a new Paper document with Markdown content?**
Yes. Use the 'create_document' tool. Provide the destination path and your Markdown text. The agent will parse the boundaries and generate a rendered '.paper' artifact in your Dropbox account.

**Q: How do I search across all my Paper documents via chat?**
Use the 'search_files' tool. It executes deep full-text indexing queries specifically filtering for '.paper' files, allowing you to find content across your entire workspace through natural language.

**Q: Can I move a Paper document to a different folder through the agent?**
Absolutely. Use the 'move_file' tool. Provide the current 'from_path' and the new 'to_path'. The agent will transmit a logical atomic operation to relocate the document safely while maintaining its unique ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dropbox-paper](https://vinkius.com/mcp/dropbox-paper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dropbox Paper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dropbox-paper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dropbox Paper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dropbox-paper": {
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
