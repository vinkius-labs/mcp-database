# ProcessOn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/processon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Online flowchart and mind mapping platform — manage diagrams, collaborations, and exports via AI.

## Description
Empower your AI agent to orchestrate your visual documentation with **ProcessOn**, the premier online platform for flowcharts, mind maps, and organizational charts. By connecting ProcessOn to your agent, you transform complex diagram management and project coordination into a natural conversation. Your agent can instantly list your files, create new diagrams, export your work into multiple formats, and even monitor collaborators without you ever needing to navigate the web interface. Whether you are designing a system architecture or a complex business process, your agent acts as a real-time visual documentation assistant, keeping your diagrams organized and your production moving.

### What you can do

- **Diagram Orchestration** — List all accessible flowcharts, mind maps, and diagrams across your ProcessOn workspace.
- **File Management** — Create, retrieve, and delete diagrams with full support for collaborative metadata.
- **Export Control** — Seamlessly export diagrams into standard formats like png, pdf, svg, and Visio.
- **Folder Organization** — Browse folder structures and manage diagram locations efficiently.
- **Collaboration Monitoring** — List file collaborators and manage access insights for your team.

### How it works

1. Subscribe to this server
2. Enter your ProcessOn API Key and API Secret
3. Start managing your diagrams through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Analysts** — automate process documentation and manage diagram folders through natural language.
- **Software Architects** — create and organize system architecture diagrams directly from your AI-powered workspace.
- **Project Coordinators** — track documentation progress and coordinate between different team members via a unified AI interface.
- **Operations Managers** — get real-time insights into organization-wide visual documentation and collaborative audit trails.


## Available Tools
- **create_file**: Create a new diagram
- **delete_file**: Delete a diagram
- **export_file**: Export a diagram
- **get_file**: Get diagram file details
- **get_folder_content**: Get folder contents
- **get_org_info**: Get organization details
- **get_recent_files**: Get recent files
- **list_collaborators**: List file collaborators
- **list_files**: List all ProcessOn files
- **list_folders**: List all folders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProcessOn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my flowcharts on ProcessOn."

**🤖 AI Agent:**
> I've retrieved your ProcessOn diagrams. You have 4 active flowcharts, including 'Customer Onboarding Flow' and 'System Architecture'. Which one would you like to view info for?

---

**👤 You:**
> "Create a new mind map titled 'Q4 Goals' in the 'Planning' folder."

**🤖 AI Agent:**
> Done! I've created the mind map 'Q4 Goals' inside the 'Planning' folder. You can now start brainstorming your objectives. File ID: PO-8821.

---

**👤 You:**
> "Export the diagram 'Architecture V2' to PNG format."

**🤖 AI Agent:**
> I've processed the export for you. Your diagram 'Architecture V2' is now ready in PNG format. You can download it here: [link].


## ❓ FAQ

**Q: How do I find my ProcessOn API Key and Secret?**
Log in to your ProcessOn account, navigate to the [API Developer Center](https://www.processon.com/api), and apply for developer credentials to receive your unique API Key and Secret.

**Q: Can I export my mind maps to PDF through the agent?**
Yes. Use the `export_file` tool with the diagram file ID and specify 'pdf' as the format. Your agent will provide the download link for the exported file.

**Q: Does ProcessOn support real-time collaboration?**
Yes, ProcessOn is natively built for visual collaboration. You can list existing collaborators for any diagram using the `list_collaborators` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/processon](https://vinkius.com/mcp/processon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ProcessOn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `processon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ProcessOn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "processon": {
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
