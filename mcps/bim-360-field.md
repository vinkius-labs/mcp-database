# BIM 360 Field MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bim-360-field)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your construction projects via BIM 360 Field — list issues, checklists, and tasks directly from any AI agent.

## Description
Connect your **BIM 360 Field** account to any AI agent and orchestrate your construction management and site execution workflows through natural conversation.

### What you can do

- **Project Navigation** — List and access details for all your assigned construction projects.
- **Issue Tracking** — Query quality, safety, and punch list issues to monitor site progress.
- **Checklist Management** — Retrieve QA/QC checklists and safety inspections.
- **Equipment & Tasks** — Track equipment installation and commissioning tasks.
- **Directory Access** — List project companies, users, and specific site locations.

### How it works

1. Subscribe to this server
2. Enter your BIM 360 Field Username, Password, and Region (US or EU)
3. Start managing your construction site from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — quickly check open issues and checklist statuses without navigating the full portal.
- **Field Engineers** — retrieve equipment task lists and location data straight from their workflow tools.
- **Quality & Safety Managers** — audit safety issues and inspection logs using natural language.


## Available Tools
- **get_project**: Get details of a specific project
- **list_checklists**: List checklists for a project
- **list_companies**: List companies associated with a project
- **list_issue_types**: List configured issue types for a project
- **list_issues**: List issues for a project
- **list_locations**: List locations configured for a project
- **list_projects**: List all accessible BIM 360 Field projects
- **list_tasks**: List tasks/equipment for a project
- **list_users**: List users associated with a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BIM 360 Field** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my BIM 360 Field projects."

**🤖 AI Agent:**
> I've retrieved your projects. You are assigned to 'Downtown Tower' (ID: proj_1) and 'City Hospital Renovation' (ID: proj_2).

---

**👤 You:**
> "Show recent issues for project proj_1."

**🤖 AI Agent:**
> Retrieving issues... There are 5 open issues, including a safety hazard reported on Level 3 and a quality check pending for the HVAC installation.

---

**👤 You:**
> "List all companies working on the Downtown Tower project."

**🤖 AI Agent:**
> I've retrieved the company directory for Downtown Tower. There are 12 companies involved, including 'Apex Foundations', 'Skyline Glazing', and 'City Electrical'.


## ❓ FAQ

**Q: Can I see all open issues for my project?**
Yes! Use the `list_issues` tool with your Project ID. The agent will retrieve the latest issues recorded on the field.

**Q: How do I list the companies working on my site?**
Simply ask the agent to `list_companies` and provide the Project ID. It will retrieve the directory of all subcontractors and partners.

**Q: Can I retrieve the status of equipment installation tasks?**
Yes. Use the `list_tasks` tool with your Project ID to track commissioning and installation activities for all site equipment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bim-360-field](https://vinkius.com/mcp/bim-360-field)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BIM 360 Field** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bim-360-field` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BIM 360 Field** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bim-360-field": {
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
