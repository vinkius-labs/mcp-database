# Autodesk Construction Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/autodesk-construction-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage projects, files, issues, and assets in Autodesk Construction Cloud natively via AI.

## Description
Connect your **Autodesk Construction Cloud (ACC)** environment to any AI agent and manage your construction projects through natural conversation.

### What you can do

- **Project Coordination** — List and audit accessible hubs and projects across your organization
- **Data Exploration** — Navigate complex folder structures and inspect file metadata and contents directly
- **Issue Tracking** — Create, monitor, and update construction issues to ensure project timelines are met
- **Asset Management** — Audit and track construction assets within your projects for better resource allocation

### How it works

1. Subscribe to this server
2. Enter your Autodesk APS Client ID and Client Secret
3. Start managing your construction workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — instantly retrieve project statuses, list open issues, and audit sprint progress
- **VDC & BIM Leads** — explore project data and file structures straight from your workspace without opening ACC
- **Field Engineers** — quickly check asset details and update issue statuses from any device


## Available Tools
- **create_issue**: Create a new issue in a project
- **get_asset_details**: Get details for a specific asset
- **get_issue_details**: Get complete details for a specific issue
- **get_project_details**: Get details for a specific project
- **list_assets**: List construction assets in a project
- **list_folder_contents**: List files and subfolders within a folder
- **list_hubs**: List all accessible Autodesk hubs
- **list_issues**: List issues in a specific project
- **list_projects**: List projects in a specific hub
- **list_top_folders**: List the top-level folders in a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Autodesk Construction Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my Autodesk hub."

**🤖 AI Agent:**
> I've accessed your hub. I found 4 active projects, including 'High-Rise Phase 1', 'Subdivision Infrastructure', and 'Hospital Renovation'. Which one would you like to inspect?

---

**👤 You:**
> "Show me the open issues for project 'High-Rise Phase 1'."

**🤖 AI Agent:**
> I've retrieved the issues for 'High-Rise Phase 1'. There are currently 5 open issues, including 'HVAC Ducting Conflict' and 'Safety Railing Missing'. Would you like the full details for the HVAC conflict?

---

**👤 You:**
> "List the files in the 'Structural Designs' folder."

**🤖 AI Agent:**
> Scanning 'Structural Designs'... I found 3 files: 'Foundation_Plan.rvt', 'Steel_Framing_Detail.dwg', and 'Load_Calculations.pdf'. Would you like to see the metadata for the Revit model?


## ❓ FAQ

**Q: How do I get my Autodesk APS Client ID and Secret?**
You need to register an application at [**Autodesk Platform Services**](https://aps.autodesk.com/myapps/). Create a 'Web App' to receive your unique Client ID and Client Secret credentials.

**Q: Does my account administrator need to authorize this integration?**
Yes. An Account Admin must add your Client ID under Account Admin > Settings > Custom Integrations within the Autodesk Construction Cloud dashboard for the server to access your data.

**Q: Can the AI help me find specific files or issues by name?**
Yes! You can ask the agent to search through your project's folders or issue lists. It will use the `get_folder_contents` and `get_issues` tools to filter and find the exact item you need in seconds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/autodesk-construction-cloud](https://vinkius.com/mcp/autodesk-construction-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Autodesk Construction Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `autodesk-construction-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Autodesk Construction Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "autodesk-construction-cloud": {
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
