# Shimo Docs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shimo-docs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Collaborative office suite and document management platform — manage Word, Excel, and PPT via AI.

## Description
Empower your AI agent to orchestrate your collaborative workflow with **Shimo Docs**, the leading professional office suite in China. By connecting Shimo Docs to your agent, you transform complex document management and team collaboration into a natural conversation. Your agent can instantly list your files, create new collaborative documents, import external content, and even export your work into multiple formats without you ever needing to navigate the web interface. Whether you are managing complex project documentation or financial spreadsheets, your agent acts as a real-time collaborative assistant, keeping your files organized and your team aligned.

### What you can do

- **Document Orchestration** — List all accessible documents, sheets, and presentations across your workspace.
- **File Management** — Create, retrieve, and delete files with full support for collaborative metadata.
- **Import & Export** — Seamlessly import external content and export Shimo documents into standard formats like docx and pdf.
- **Folder Organization** — Browse folder structures and manage file locations efficiently.
- **Administrative Insights** — List organization users and monitor audit logs for security and compliance.

### How it works

1. Subscribe to this server
2. Enter your Shimo App ID and App Secret
3. Start managing your collaborative documents through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — track documentation progress and manage project folders through natural language.
- **Knowledge Workers** — create and organize collaborative documents directly from your AI-powered workspace.
- **Administrative Teams** — manage user lists and monitor workspace activity through a unified AI interface.
- **Enterprise Leaders** — get real-time insights into organization-wide collaboration and document audit trails.


## Available Tools
- **create_file**: Create a new Shimo file
- **export_file**: Export a Shimo file
- **get_file**: Get file details
- **get_folder_content**: Get folder contents
- **get_org_info**: Get organization details
- **import_file**: Import a document into Shimo
- **list_audit_logs**: List audit logs
- **list_files**: List all Shimo files
- **list_folders**: List all Shimo folders
- **list_users**: List organization users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shimo Docs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my collaborative documents on Shimo."

**🤖 AI Agent:**
> I've retrieved your Shimo documents. You have 5 active files, including 'Marketing Strategy 2026' and 'Budget Planning'. Would you like to view the details of any of them?

---

**👤 You:**
> "Create a new spreadsheet titled 'Q2 Expenses' in folder 'Finance'."

**🤖 AI Agent:**
> Done! I've created the spreadsheet 'Q2 Expenses' inside the 'Finance' folder. You can now start collaborating on it. File ID: SH-8821.

---

**👤 You:**
> "Export the document 'Project Roadmap' to PDF."

**🤖 AI Agent:**
> I've processed the export for you. Your document 'Project Roadmap' is now ready in PDF format. You can download it here: [link].


## ❓ FAQ

**Q: How do I find my Shimo App ID and Secret?**
Log in to the [Shimo Open Platform](https://platform.shimo.im/), create a new application, and you will find your App ID and App Secret in the application credentials section.

**Q: Can I export documents to PDF through the agent?**
Yes. Use the `export_file` tool with the file ID and specify 'pdf' as the type. Your agent will provide the link to download the exported document.

**Q: Is multi-user editing supported?**
Yes, Shimo Docs is natively designed for real-time collaboration. Any file you manage or create via this server can be shared and edited by multiple users simultaneously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shimo-docs](https://vinkius.com/mcp/shimo-docs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shimo Docs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shimo-docs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shimo Docs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shimo-docs": {
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
