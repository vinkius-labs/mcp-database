# Smartsheet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smartsheet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Empower your AI to read Smartsheet rows, list workspaces, and manage your spreadsheets effortlessly from your code editor.

## Description
Connect your **Smartsheet** account to any AI agent and empower your team to query project configurations, internal spreadsheets, and custom reports seamlessly. Interact with your organization's grids through natural language without ever switching tabs.

### What you can do

- **Project Navigation** — Easily map out your hierarchical structures calling `list_workspaces` and `list_folders` to find correct document locations
- **Sheet Deep-Dives** — Browse all your active spreadsheets using `list_sheets` and extract raw rows/columns instantly via `get_sheet_details`
- **Reporting Overviews** — Retrieve saved tabular aggregations automatically calling `list_reports` across all configured company sheets
- **Identity Profiling** — Test the connectivity and query authorized scopes by requesting the internal `get_current_user` tool

### How it works

1. Subscribe to this server
2. Enter your Personal Smartsheet Access Token
3. Start using Claude, Cursor, or any MCP-compatible client to query the state of your tabular data

Stop manually hunting down the ID of a specific project table just to wire up your Python scripts. Let your AI agent read the workspace layout automatically.

### Who is this for?

- **Project Managers** — rapidly audit how many tasks are active across cross-functional sheets or pull report overviews without exporting CSVs
- **Data Engineers** — query the actual sheet layout and row metadata directly from the code editor to build sturdy ETL scripts
- **Team Leaders** — have the bot read specific spreadsheets to generate weekly summary drafts completely autonomously


## Available Tools
- **list_sheets**: Lists all sheets available in Smartsheet
- **get_sheet_details**: Retrieves details for a specific sheet
- **list_workspaces**: Lists all workspaces in Smartsheet
- **list_folders**: Lists all folders
- **list_reports**: Lists all reports
- **get_current_user**: Retrieves information about the current Smartsheet user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smartsheet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all sheets available in my Smartsheet account."

**🤖 AI Agent:**
> I've invoked the listing call. Your account currently has access to the following 3 sheets:
- Q1 Marketing Budget (ID: `10023`)
- Employee Resource Registry (ID: `82910`)
- Bug Triage Queue (ID: `15523`)

Which sheet would you like me to inspect in more detail?

---

**👤 You:**
> "Retrieve the details and rows for the 'Release Candidate Tracker' sheet."

**🤖 AI Agent:**
> I matched 'Release Candidate Tracker' to ID `85739`.
**Columns Detected**:
1. Status (Dropdown)
2. Task Name (Text/Number)
3. Assigned To (Contact List)

**Rows retrieved**:
- Row 1: Status: In Progress | Task: Implement API Docs | Assigned To: J. Doe
- Row 2: Status: Complete | Task: Docker Upgrade | Assigned To: S. Smith

---

**👤 You:**
> "Summarize all our workspaces in a markdown table."

**🤖 AI Agent:**
> Sure. Using `list_workspaces`, I've compiled this table:

| Workspace Name | ID | Permission Level |
| --- | --- | --- |
| External Consultants | `W-2391` | Admin |
| Core Engineering Team | `W-8472` | Owner |
| Q3 Marketing Rollouts | `W-1102` | Viewer |


## ❓ FAQ

**Q: Can the AI understand the raw tabular data of my spreadsheet?**
Yes. When you call the `get_sheet_details` tool, the server returns the spreadsheet's metadata, including all column names, types (e.g., date, dropdown), and rows. The AI maps the internal IDs together to form a highly accurate contextual grid of your project.

**Q: Does my agent need to use a sheet ID?**
No manual hunting needed! While the underlying tool does require a sheet ID, you can just tell your bot, 'Find our Onboarding Spreadsheet and read the rows'. The AI will first scan via `list_sheets`, match the textual name to the ID, and then naturally pull the targeted entity.

**Q: How do I list folders within a workspace?**
Your AI agent will act autonomously. Ask it to 'check our Engineering workspace' and it will first fetch its workspace ID and intelligently map the nested sub-folders and sheets stored inside. You can instruct it to keep going deeper as needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smartsheet](https://vinkius.com/mcp/smartsheet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smartsheet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `smartsheet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smartsheet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smartsheet": {
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
