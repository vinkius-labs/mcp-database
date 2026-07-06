# Zoho Sheet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-sheet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI agents to Zoho Sheet for spreadsheet management: workbooks, worksheets, cell data, rows, and sharing.

## Description
Give your AI agents programmatic control over your cloud data arrays by connecting to the Zoho Sheet API. With 13 powerful tools, your AI can dynamically manipulate cell ranges, manage workbook structures, automate row data insertion, and audit sharing permissions directly through natural language.

### What you can do
- Read and write specific cell ranges programmatically
- Append and list large row datasets automatically
- Create, search, and manage complete workbooks
- Add, delete, and configure worksheet tabs
- View and audit document sharing permissions
- Format cells and manipulate cloud-based formulas

### How it works
1. Subscribe to this server
2. Enter your Zoho API Credentials (found in your Zoho Developer Console)
3. Let your AI agents seamlessly manipulate spreadsheets via Vinkius

### Who is it for?
Essential for data analysts, operations teams, and administrative staff who require intelligent automation for spreadsheet data entry and reporting.


## Available Tools (13)
- **delete_worksheet**: Delete a worksheet
- **get_cells**: g. A1:D10).

Get cell contents
- **get_workbook**: Get workbook details
- **get_worksheet**: Get worksheet details
- **list_rows**: List data rows
- **list_shared_users**: List shared users
- **list_workbooks**: List workbooks
- **list_worksheets**: List worksheets
- **search_workbooks**: Search workbooks
- **update_cells**: Update cells
- **add_row**: Add a data row
- **create_workbook**: Create a workbook
- **create_worksheet**: Create a worksheet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Sheet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the 'Q3 Financials' workbook and read the data in cells A1 to D20 from the first worksheet."

**🤖 AI Agent:**
> I found the 'Q3 Financials' workbook. The data in range A1:D20 shows your quarterly revenue at $1.2M and expenses at $850K. Would you like me to analyze these figures further?

---

**👤 You:**
> "Create a new workbook called 'Event Attendees' and add a new row with name 'Sarah Connor' and email 'sarah.c@example.com'."

**🤖 AI Agent:**
> I have successfully created the 'Event Attendees' workbook. The first worksheet has been set up, and I've added the new data row for 'Sarah Connor' (sarah.c@example.com). You can now access it in your Zoho console.

---

**👤 You:**
> "List all my workbooks and tell me who has shared access to the 'Master Inventory' spreadsheet."

**🤖 AI Agent:**
> You have 5 active workbooks. For the 'Master Inventory' spreadsheet, the shared users are Alex (Editor) and Taylor (Viewer). Would you like to update any permissions?


## ❓ FAQ

**Q: Can I read and write cells?**
Yes, read cell contents from any range (e.g. A1:D10) and write new values to specific cell ranges.

**Q: Can I manage sharing?**
Yes, view all users with access to a workbook and their permission levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-sheet](https://vinkius.com/mcp/zoho-sheet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Sheet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-sheet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Sheet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-sheet": {
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
