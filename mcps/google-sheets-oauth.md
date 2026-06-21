# Google Sheets (OAuth) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-sheets-oauth)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Power up spreadsheets via Google Sheets — create, read, write, and append data, handle batch operations, and audit sheet info directly from any AI agent.

## Description
Connect your **Google Sheets** via OAuth2 to any AI agent and take full control of your spreadsheet creation, data manipulation, and batch processing through natural conversation.

### What you can do

- **Live Spreadsheet Creation** — Create brand-new Google Spreadsheets by commanding specific titles and optionally including initial sheet names natively within your workspace
- **Advanced Data Retrieval** — Extracts structured cell arrays by evaluating physical spreadsheet coordinates utilizing A1 notation to retrieve read-only content flawlessly
- **High-Throughput Batch Reading** — Retrieve data from multiple ranges simultaneously, allowing your agent to analyze complex cross-sheet dependencies synchronously
- **Cell & Range Orchestration** — Injects discrete structural nodes executing precise write operations to overwrite existing values or append new rows while maintaining native formats
- **Range Invalidation & Clearing** — Irreversibly vaporizes cell target values within specific A1 boundaries to manage your workspace volume and data integrity securely
- **Spreadsheet Metadata Auditing** — Fetch detailed info about your spreadsheet including titles, locale, timezone, and individual sheet attributes flawlessly
- **Automation & Logging Discovery** — Identify bounded spreadsheet IDs from URLs and analyze specific cell ranges to extract precise textual strings for RAG or reporting

### How it works

1. Subscribe to this server
2. Enter your Google OAuth2 Access Token (can be obtained via Google OAuth Playground or `gcloud auth print-access-token`)
3. Start managing your spreadsheets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts & Scientists** — create and populate spreadsheets for analysis using natural language without opening the Google Sheets UI
- **Operations & Finance Teams** — automate reporting and log data across multiple sheet ranges in real-time
- **Product Managers** — audit project trackers and verify spreadsheet metadata through natural conversation
- **Developers** — test and debug complex spreadsheet batch operations and verify A1 notation logic through the chat interface


## Available Tools
- **sheets.info**: Accepts full Google Sheets URL or just the spreadsheet ID. For reading cell values, use sheets.read.

Get Google Sheets spreadsheet metadata: title, timezone, locale, and list of all sheet tabs with row/column dimensions
- **sheets.read**: Range uses A1 notation: "SheetName!A1:D10". If no sheet name, defaults to first sheet. To read multiple ranges in one call, use sheets.batch_read. To discover sheet names and dimensions first, use sheets.info. Present results as a Markdown table with the first row as headers.

Read cell values from a Google Sheets range in A1 notation (e.g. "Sheet1!A1:D10" or "A:Z")
- **sheets.batch_read**: Provide ranges as comma-separated A1 notation strings (e.g. "Sheet1!A1:D10, Summary!A:B"). For a single range, use sheets.read instead.

Read multiple cell ranges from a Google Sheet in a single API call — more efficient than calling sheets.read multiple times
- **sheets.write**: Provide values as a 2D JSON array: [["row1col1","row1col2"],["row2col1","row2col2"]]. Uses USER_ENTERED input — formulas (starting with =) will be evaluated. WARNING: This overwrites existing data in the range. To add rows without overwriting, use sheets.append instead. Always confirm with the user before writing to production spreadsheets.

Write data to a Google Sheets range — overwrites existing values. Accepts 2D array of rows and columns
- **sheets.append**: Rows are inserted after the last row of existing data in the table range. Provide values as a 2D JSON array: [["val1","val2"],["val3","val4"]]. For overwriting a specific range, use sheets.write instead.

Append new rows to the end of a Google Sheet table — does not overwrite existing data
- **sheets.clear**: Note: formatting (colors, borders, fonts) is preserved — only values are removed. WARNING: This is destructive. Always confirm with the user before clearing. To clear a whole sheet, use the sheet name with no range: "Sheet1".

Clear all values in a Google Sheets range — removes cell content but preserves formatting and formulas structure
- **sheets.create**: Returns the spreadsheet ID and a direct edit URL. After creating, use sheets.write or sheets.append to add data.

Create a new blank Google Sheets spreadsheet with a given title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Sheets (OAuth)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new spreadsheet titled 'Sales Forecast Q2'"

**🤖 AI Agent:**
> Spreadsheet created! I've successfully initialized 'Sales Forecast Q2' in your Google Drive. The spreadsheet ID is 'spreadsheet_abc123'. Would you like me to add headers to the first sheet?

---

**👤 You:**
> "Write these values to 'Sheet1!A1': [['Date', 'Amount'], ['2026-03-30', 500]]"

**🤖 AI Agent:**
> Data written! I've successfully populated Sheet1!A1:B2 with your provided values. The spreadsheet is now updated with the correct date and amount information.

---

**👤 You:**
> "Get info for spreadsheet 'abc-123'"

**🤖 AI Agent:**
> Retrieving spreadsheet info... Title: 'Budget 2026'. Sheets: 'Jan-March', 'April-June'. Locale: en_US. Timezone: UTC. I can also retrieve the grid properties or specific range data for you.


## ❓ FAQ

**Q: How do I get a Google OAuth2 access token for this server?**
You can use the Google OAuth Playground (select Sheets API v4 and authorize) or run 'gcloud auth print-access-token' in your terminal. Note that these tokens are typically valid for 1 hour.

**Q: Can my agent create a new spreadsheet and add data to it in one go?**
Yes. The agent can orchestrate multiple operations. First, use 'create_spreadsheet' to get the new ID, and then use 'write_data' or 'append_data' to populate it with your JSON arrays natively.

**Q: What is the benefit of batch reading through the agent?**
Batch reading allowing your agent to retrieve data from multiple non-contiguous ranges (e.g., 'Sheet1!A1:B10' and 'Sheet2!C5:D15') in a single request, improving context efficiency and reasoning accuracy flawlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-sheets-oauth](https://vinkius.com/mcp/google-sheets-oauth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Sheets (OAuth)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-sheets-oauth` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Sheets (OAuth)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-sheets-oauth": {
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
