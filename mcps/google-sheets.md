# Google Sheets MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-sheets)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Interact with Google Sheets to read, write, and manipulate data via AI.

## Description
Connect **Google Sheets** to your AI agent and turn conversational commands into complex spreadsheet operations. Read data from specific ranges, append new rows, and update existing values across all your Google Sheets without writing a single formula.

### What you can do

- **Data Extraction** — Read values from specific ranges (e.g., 'Sheet1!A1:D10') or fetch multiple ranges simultaneously for instant analysis
- **Data Entry & Updates** — Append new rows to existing tables or update specific cells directly from the chat
- **Sheet Management** — Create new spreadsheets, add new tabs (sheets) to existing files, and delete unwanted tabs
- **Formatting & Structure** — Execute batch update requests to manipulate the spreadsheet structure programmatically

### How it works

1. Subscribe to this server
2. Enter your Google OAuth Client ID and Secret
3. Complete the secure Google authorization flow
4. Start manipulating data from Claude, Cursor, or any MCP-compatible client

Your AI agent acts as a virtual data entry clerk and spreadsheet analyst, capable of translating natural language requests into structured API calls.

### Who is this for?

- **Financial Analysts** — quickly pull specific KPIs from massive financial models without opening the spreadsheet
- **Project Managers** — log updates, append new tasks, or extract project timelines from shared trackers seamlessly
- **Marketing Teams** — add new leads or campaign metrics to tracking sheets via conversational commands


## Available Tools
- **update_sheet_values**: Update values in a specific range
- **delete_sheet**: Delete a sheet from a spreadsheet
- **get_sheet_values**: Read values from a specific range
- **get_spreadsheet**: Get spreadsheet metadata and sheets
- **add_sheet**: Add a new sheet to a spreadsheet
- **append_sheet_values**: Append rows of data to a table
- **batch_get_values**: Read multiple ranges of values
- **batch_update_spreadsheet**: Apply multiple updates to a spreadsheet structure/formatting
- **clear_sheet_values**: Clear values from a range
- **create_spreadsheet**: Create a new Google Spreadsheet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Sheets** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read the data in range A1:C10 from spreadsheet ID '1abcxyz'."

**🤖 AI Agent:**
> Fetching data... Here are the values from A1:C10:
- [ Name | Department | Q1 Sales ]
- [ John Doe | Marketing | $45,000 ]
- [ Jane Smith | Sales | $82,000 ]...

---

**👤 You:**
> "Append a new row to the 'Q1 Sales' sheet with the values: 'Mike T', 'Engineering', '$12,000'."

**🤖 AI Agent:**
> Appending data... Success! I've appended the row ['Mike T', 'Engineering', '$12,000'] to the next available line.

---

**👤 You:**
> "Create a new sheet called 'Finances 2026' and populate the headers."

**🤖 AI Agent:**
> Tab successfully instantiated in spreadsheet ID '1abcxyz'. The empty array logic has been set.


## ❓ FAQ

**Q: How do I specify which cells to read or update?**
You use 'A1 notation'. For example, 'Sheet1!A1:B5' refers to the first two columns and first five rows of the tab named 'Sheet1'. If you just say 'Sheet1', it attempts to read the active data range.

**Q: Can I add a new row of data without knowing the exact empty row number?**
Yes! Use the `append_sheet_values` tool. You simply provide the range of the table (e.g., 'Sheet1!A:C') and the data you want to add. It automatically appends to the next empty row.

**Q: Can it delete sheets completely?**
The tool endpoints are restricted to inside-sheet operations. It cannot delete the root spreadsheet itself from your Drive to prevent catastrophic destructive commands.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-sheets](https://vinkius.com/mcp/google-sheets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Sheets** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-sheets` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Sheets** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-sheets": {
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
