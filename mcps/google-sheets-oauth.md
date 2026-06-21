# Google Sheets (OAuth) MCP Server

Power up spreadsheets via Google Sheets — create, read, write, and append data, handle batch operations, and audit sheet info directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/google-sheets-oauth)

## Overview
**Category:** industry-titans
**Tools Count:** 7

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


## Installation & Usage

To install and use the **Google Sheets (OAuth)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-sheets-oauth](https://vinkius.com/mcp/google-sheets-oauth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
