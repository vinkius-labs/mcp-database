# Rows MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rows)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rows-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rows-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate spreadsheets via Rows.com — manage tables, data values, and folders with AI agents.

## Description
Connect your **Rows.com** account to any AI agent and take full control of your spreadsheet-based data orchestration and collaborative workflows through natural conversation. Rows provides a modern spreadsheet platform with built-in integrations, and this integration allows you to retrieve row metadata, update cell values, and perform complex data queries directly from your chat interface.

### What you can do

- **Spreadsheet & Table Orchestration** — List all managed spreadsheets and retrieve detailed metadata, including table structures programmatically.
- **Data Value Intelligence** — Access and monitor range values to retrieve real-time spreadsheet data directly from the AI interface.
- **Cell Lifecycle Management** — Update and append values to specific ranges to ensure your records are always synchronized via natural language.
- **Folder & Organization Control** — List and search through your folders to maintain a clear overview of your digital workspace.
- **Operational Monitoring** — Track system activity and manage spreadsheet metadata using simple AI commands to streamline your business workflows.

### How it works

1. Subscribe to this server
2. Enter your Rows.com API Key from your workspace settings
3. Start managing your collaborative spreadsheets from Claude, Cursor, or any MCP-compatible client

No more manual copy-pasting or complex VLOOKUP building. Your AI acts as a dedicated data analyst or spreadsheet coordinator.

### Who is this for?

- **Operations Managers** — quickly retrieve data summaries and update project trackers without switching browser tabs.
- **Data Analysts** — automate the ingestion of new records and track aggregate values via natural conversation.
- **Business Owners** — streamline the retrieval of spreadsheet metadata and monitor organizational health directly within the chat.


## Available Tools
- **create_spreadsheet**: Create a new spreadsheet
- **delete_spreadsheet**: Delete a spreadsheet
- **get_folder**: Get details for a specific folder
- **append_values_to_table**: Add new rows to a table
- **get_range_cells**: Get detailed cell objects
- **get_spreadsheet_details**: Get metadata for a spreadsheet
- **get_range_values**: g., A1:B5).

Get values from a specific range
- **get_workspace_info**: Get Rows workspace details
- **list_folders**: List workspace folders
- **list_spreadsheets**: List your Rows spreadsheets
- **update_range_values**: Overwrite values in a range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rows** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all spreadsheets in my Rows workspace."

**🤖 AI Agent:**
> I've retrieved your spreadsheets. You have 4 active documents including 'Sales Forecast 2024' and 'Project Tracker'. Which one would you like to retrieve values from?

---

**👤 You:**
> "Show me all spreadsheets in my workspace and pull the latest data from the Sales Dashboard."

**🤖 AI Agent:**
> 12 spreadsheets in your workspace. "Sales Dashboard" (last modified 2h ago): Q2 revenue at $1.2M (78% of target), 234 deals closed, pipeline value $3.4M. "Marketing Metrics" (modified today): 45,600 website visits this week (+12%). "Product Roadmap" (modified yesterday): 34 features tracked, 8 shipped this sprint. "HR Headcount" (modified 3 days ago): 127 employees. "Financial Model" (modified 1 week ago). 7 additional spreadsheets. Total cells with live data integrations: 2,340.

---

**👤 You:**
> "Create a new spreadsheet called Q3 Planning and populate it with department budget data."

**🤖 AI Agent:**
> Spreadsheet "Q3 Planning" created. 5 columns populated: Department, Q2 Actual, Q3 Budget, Variance, Status. Engineering: $890K actual / $950K budget. Marketing: $234K / $280K. Sales: $456K / $500K. Product: $178K / $200K. Operations: $123K / $140K. Total row: $1.88M actual / $2.07M budget (9.2% planned increase). Conditional formatting applied: green for under budget, yellow for within 5%, red for over. Chart widget added for visual comparison.


## Installation & Usage

To install and use the **Rows** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rows](https://vinkius.com/mcp/rows)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
