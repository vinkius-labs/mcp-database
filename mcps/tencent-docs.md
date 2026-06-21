# Tencent Docs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-docs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Collaborative office workspace by Tencent — manage documents, sheets, and slides via AI.

## Description
Empower your AI agent to orchestrate your collaborative production with **Tencent Docs**, the premier office workspace for real-time collaboration. By connecting Tencent Docs to your agent, you transform complex file operations and spreadsheet management into a natural conversation. Your agent can instantly list your documents, create new files, retrieve spreadsheet data, and even monitor collaborators without you ever needing to navigate the web interface. Whether you are managing team reports or complex financial models, your agent acts as a real-time productivity assistant, keeping your workspace organized and your data accessible.

### What you can do

- **File Orchestration** — List all accessible documents, sheets, and slides across your Tencent Docs account.
- **Spreadsheet Control** — Retrieve and update values in specific ranges within your sheets with ease.
- **Content Access** — Retrieve the full text content of your documents for analysis and summarization.
- **Collaboration Monitoring** — List file collaborators and manage access insights for your team.
- **Organization Overview** — Access member lists to ensure effective coordination within your organization.

### How it works

1. Subscribe to this server
2. Enter your Tencent Docs Access Token
3. Start managing your collaborative workspace through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Team Leads** — monitor document progress and update spreadsheet data through natural language.
- **Project Coordinators** — manage project files and collaborators directly from your AI-powered workspace.
- **Data Analysts** — retrieve and update sheet values for analysis through a unified AI interface.
- **Enterprise Users** — integrate your Tencent Docs workflow into your AI-driven daily production.


## Available Tools (10)
- **create_file**: Create a new document
- **delete_file**: Delete a document
- **get_doc_content**: Get document content
- **get_file_info**: Get file metadata
- **get_org_members**: List organization members
- **get_sheet_data**: Read spreadsheet data
- **list_collaborators**: List file collaborators
- **list_files**: List all Tencent Docs files
- **list_folders**: List all folders
- **update_sheet_data**: Update spreadsheet data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent Docs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my documents on Tencent Docs."

**🤖 AI Agent:**
> I've retrieved your Tencent Docs files. You have 4 active documents, including 'Q3 Sales Plan' and 'Technical Specs'. Which one would you like to view info for?

---

**👤 You:**
> "Read the values from 'Inventory!A1:B10' in spreadsheet 'doc-8821'."

**🤖 AI Agent:**
> I've retrieved the data from the specified range in 'doc-8821'. It contains a list of 10 items with their current stock levels. Would you like me to summarize the low-stock items?

---

**👤 You:**
> "Create a new document titled 'Project Kickoff Notes'."

**🤖 AI Agent:**
> Done! I've created the new document 'Project Kickoff Notes' for you. You can now access it and start adding your meeting notes. File ID: TD-9920.


## ❓ FAQ

**Q: How do I obtain a Tencent Docs Access Token?**
Log in to the [Tencent Docs Open Platform](https://docs.qq.com/open), create an application, and generate an access token in the API console.

**Q: Can I read data from a specific sheet range?**
Yes. Use the `get_sheet_data` tool with the file ID and the range (e.g., 'Sheet1!A1:C5'). Your agent will retrieve the values for you.

**Q: Does this server support multi-user collaboration?**
Yes, Tencent Docs is built for real-time collaboration. You can list existing collaborators using the `list_collaborators` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-docs](https://vinkius.com/mcp/tencent-docs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tencent Docs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tencent-docs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tencent Docs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tencent-docs": {
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
